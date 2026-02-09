# AWS CDK Practice Ground

This repository serves as a testing ground and sandbox for exploring the fundamentals of the **AWS Cloud Development Kit (CDK)**.

The goal of this project is to experiment with CDK constructs, understand the synthesis process, and practice deploying infrastructure as code (IaC) in a safe, isolated environment.

## 🎯 Objectives
* Understand the core CDK concepts (App, Stack, Construct).
* Experiment with L1, L2, and L3 constructs.
* Practice cross-stack references and context management.
* Test deployment workflows and resource cleanup.

## 🛠 Prerequisites

Before running this project, ensure you have the following installed:

* **Node.js** (LTS version recommended)
* **AWS CLI** (configured with `aws configure`)
* **AWS CDK Toolkit** (installed globally: `npm install -g aws-cdk`)

## 🚀 Getting Started

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
    cd YOUR_REPO_NAME
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Bootstrap your AWS environment (if not already done):**
    *This creates the necessary S3 bucket and roles for CDK deployments.*
    ```bash
    cdk bootstrap aws://ACCOUNT-ID/REGION
    ```

## 💻 Useful Commands

Here are the most common commands used during development:

* `npm run build`   - Compile the TypeScript code to JavaScript.
* `npm run watch`   - Watch for changes and compile in the background.
* `npm run test`    - Run the Jest unit tests.
* `cdk synth`       - Synthesize the CloudFormation template from your code.
* `cdk diff`        - Compare your local stack with the deployed stack to see changes.
* `cdk deploy`      - Deploy the stack(s) to your default AWS account/region.
* `cdk destroy`     - Tear down the deployed stack(s) to avoid unwanted costs.

## 📂 Project Structure

* `bin/` - Contains the entry point for the CDK application.
* `lib/` - Contains the stack definitions and custom constructs.
* `test/` - Contains unit tests for your infrastructure code.
* `cdk.json` - Configuration file for the CDK Toolkit.

## ⚠️ Disclaimer
This is a practice repository. **Do not commit sensitive information** (such as hardcoded API keys or credentials) to this repo, especially if it is public. Always use environment variables or AWS Secrets Manager.