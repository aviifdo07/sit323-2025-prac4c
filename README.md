

# Enhanced Calculator Microservice

## Introduction
This README provides comprehensive documentation for the Enhanced Calculator Microservice, which now includes advanced arithmetic operations such as exponentiation, square root, and modulo calculations. Built using Node.js and Express, this service extends the basic functionality previously established in task 4.1P.

## Prerequisites
To run this project, you will need:
- Node.js - Download and install from [https://nodejs.org/en/download/](https://nodejs.org/en/download/)
- npm (Node Package Manager), which comes with Node.js

## Project Setup

### Step 1: Clone the Repository
Begin by cloning the repository to your local machine:
```bash
git clone <repository-url>
cd calculator-service-enhanced
```

### Step 2: Install Dependencies
Within the project directory, install the necessary Node modules:
```bash
npm install
```

### Step 3: Start the Server
Launch the microservice by running:
```bash
node app.js
```
You should see an output indicating that the server is running on port 3000.

## API Endpoints
The microservice supports several endpoints, including:
- **POST /add, /subtract, /multiply, /divide** - Basic arithmetic operations.
- **POST /power** - Returns the result of raising a base to an exponent.
- **POST /sqrt** - Calculates the square root of a number.
- **POST /modulo** - Computes the modulo of two numbers.

### Using the Endpoints
Send POST requests with appropriate JSON payloads to each endpoint. For example, to use the power endpoint:
```json
{
  "base": 2,
  "exponent": 3
}
```

## Testing the Microservice
Use tools like Postman or curl commands to test the functionality of each endpoint. Example curl command for the exponentiation endpoint:
```bash
curl -X POST http://localhost:3000/power -H "Content-Type: application/json" -d '{"base": 2, "exponent": 3}'
```

## Error Handling
The microservice features enhanced error handling to provide clear and informative feedback for invalid inputs or computation errors. This includes checks for non-numerical inputs and handling edge cases like division by zero.

## Documentation
Detailed comments within the source code describe the purpose and function of each endpoint and the error handling mechanisms in place. This aids in understanding and maintaining the code.

## Conclusion
This README outlines the necessary steps to set up and interact with the Enhanced Calculator Microservice. The addition of advanced arithmetic operations greatly increases its utility and demonstrates the capability to extend its features seamlessly.

---

### Additional Notes:
- **Customization**: Make sure that the repository URL and specific project details in the README are correct as per your project setup.
- **Code Comments**: Include comprehensive comments in the `app.js` and other relevant files to aid future users and developers.
- **Testing Instructions**: Provide clear instructions on how to test each new endpoint, including potential edge cases or unusual input scenarios.

