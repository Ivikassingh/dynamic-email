

# Dynamic Email Templates

This Node.js application dynamically fetches email templates stored in an AWS S3 bucket, populates them with provided data, and sends emails using these templates. This setup allows for easy management of email templates without needing to redeploy the application for changes in email content.

## Features

- **Dynamic Email Template Retrieval**: Fetches email templates directly from an AWS S3 bucket.
- **Flexible Template Data**: Populates templates with dynamic data for personalized emails.
- **Email Sending**: Utilizes NodeMailer to send out the constructed emails.

## Prerequisites

Before you begin, ensure you have the following:

- Node.js installed (v10.x or later)
- An AWS account with access to S3 and IAM for credentials
- An S3 bucket with email templates stored in it
- Access credentials for AWS with permissions to access S3

## Installation

1. **Clone the repository**



2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Set up environment variables**

   Create a `.env` file in the root of your project and add the following:

   ```plaintext
   AWS_ACCESS_KEY_ID=your_access_key
   AWS_SECRET_ACCESS_KEY=your_secret_key
   AWS_REGION=your_region
   EMAIL_USER=your-email@example.com
   EMAIL_PASS=your-email-password
   ```
