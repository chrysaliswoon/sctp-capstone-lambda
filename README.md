# CLOUDSCALE: AUTOMATED REPORT GENERATION USING AWS CLOUD SERVICES

This repository is dedicated to the creation and management of the AWS Lambda functions, as part of our SCTP capstone project. The Lambda functions are deployed using AWS infrastructure, including API Gateway and DynamoDB, and this repository contains the necessary files for configuring and managing these functions.

---

## What is AWS Lambda?

![AWS Lambda](https://d2908q01vomqb2.cloudfront.net/1b6453892473a467d07372d45eb05abc2031647a/2019/02/04/sam-layers-diag.png)

[AWS Lambda](https://aws.amazon.com/lambda/) is a serverless computing service that allows you to run code without provisioning or managing servers. You can trigger Lambda functions in response to various events, making it a flexible solution for building scalable applications.

![Architecture Diagram](https://github.com/chrysaliswoon/sctp-capstone-aws-insfrastructure/blob/main/assets/diagram.jpeg)

### Key Features of AWS Lambda:
- **Serverless Execution:** Automatically runs your code in response to events without requiring server management.
- **Automatic Scaling:** Scales automatically based on the number of incoming requests, providing a cost-effective solution.
- **Multiple Triggers:** Supports various event sources, including API Gateway, S3, DynamoDB, and more.
- **Flexible Language Support:** Supports multiple programming languages, including Python, Node.js, Java, and Go.
- **Integrated Monitoring:** Works with Amazon CloudWatch for logging and monitoring performance metrics.

### Why Use AWS Lambda?
AWS Lambda allows developers to focus on writing code rather than managing infrastructure. Its serverless model reduces costs by only charging for compute time used, making it an ideal choice for event-driven applications and microservices.

## Architecture Overview

The Lambda functions are deployed in a serverless architecture:
- **API Gateway**: Acts as a front door to trigger Lambda functions through HTTP requests.
- **DynamoDB**: A NoSQL database service used to store and manage application data.

![Architecture Diagram](https://github.com/chrysaliswoon/sctp-capstone-aws-insfrastructure/blob/main/assets/diagram.jpeg)

## Key Components

1. **AWS Lambda**  
   The core service for running serverless functions in response to events.

2. **Amazon API Gateway**  
   Manages the API endpoints and routes requests to the appropriate Lambda functions.

3. **Amazon DynamoDB**  
   A fully managed NoSQL database for storing application data efficiently.

4. **IAM and Security**  
   Access control and permissions are managed through IAM policies, ensuring secure and controlled access to the functions and resources.

## Getting Started

### Prerequisites
- AWS CLI configured with appropriate IAM permissions.
- Serverless Framework installed (optional but recommended for deployment).

### Deployment

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/chrysaliswoon/sctp-capstone-lambda.git
   cd sctp-capstone-lambda
   ```

2. **Deploy the Lambda Functions:**

   If using the Serverless Framework, run:
   ```bash
   serverless deploy
   ```

   Otherwise, use the AWS CLI to create and deploy the Lambda functions defined in the `template.yaml`.

### Management

You can manage your Lambda functions through the AWS Lambda console, including updating configurations or monitoring performance through Amazon CloudWatch.

## Troubleshooting

- Ensure that all environment variables are set correctly in the Lambda configuration.
- Verify that the API Gateway is properly configured to trigger the Lambda functions.
- Check IAM roles for appropriate permissions.
- Use CloudWatch logs to monitor function executions and troubleshoot errors.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```
