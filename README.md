# Rider Shield

Welcome to the Rider Shield project repository! This is a React-based website aimed at providing accessible and personalized bike rider insurance services to users. The website allows users to connect with insurance experts, apply insurance, and claim insurance in real time.

## Project Overview

- **Website**: [Rider Shield](https://engeniusam.github.io/rider-shield/ "Rider Shield")
- **Framework**: React.js
- **Deployment**: GitHub Pages
- **Libraries**: React-Toastify, React Router DOM, FontAwesomeIcon, tawk.to
- **AWS Security & Compliance**: Demonstrates use of AWS Audit Manager, AWS Config, and AWS Security Hub for monitoring, compliance, and security best practices.

## Features

- Easily apply for Insurance.
- Engage in real-time consultations to receive expert insurance advice.
- Responsive UI design for seamless user experience across devices.
- Utilizes React-Toastify for notifications, React Router DOM for page routing, and FontAwesomeIcon for icons.
- Deployed using GitHub Pages for easy access and sharing.

## Screenshots

### Home Page
![home page](https://github.com/user-attachments/assets/48d37a8a-c3e3-48e7-a59f-5bd745ff22d1)

### About Section

![About Us](https://github.com/user-attachments/assets/d620c2ed-1664-4d9d-b1d7-1474307d8d86)


### Services Section

![Services](https://github.com/user-attachments/assets/17551e57-13d3-4d87-994c-c377be500b2c)


### Why Choose Rider Shield ?

![Why Choose Us 4](https://github.com/user-attachments/assets/b688790b-1aa9-4492-9a52-ad9a0a799191)


### Reviews Section

![Reviews](https://github.com/user-attachments/assets/49070910-df9c-45b4-a8c4-82ba6a0b08b6)

### Partners Section

![partners](https://github.com/user-attachments/assets/705f3742-b12a-48b9-9997-ac97f895fd0e)

### Footer Section

![Footer](https://github.com/user-attachments/assets/b8659e81-8551-466f-a39b-08343213eba9)

## Deployment

The website is deployed using GitHub Pages and can be accessed at [https://engeniusam.github.io/rider-shield/](https://engeniusam.github.io/rider-shield/).

## Showcasing AWS Security Hub, Audit Manager, and Config

To demonstrate AWS security and compliance services with this insurance app for bikeriders, the following steps were taken:

1. **Pushing the App to AWS**
   After deploying the app on GitHub Pages, the static build was also pushed to AWS by:
   - Building the React app using `npm run build`.
   - Uploading the build output to an S3 bucket configured for static website hosting.
   - Setting up an AWS CloudFront distribution for secure and performant content delivery.
   - Optionally, using AWS Amplify Console for CI/CD integration with the GitHub repository.

2. **Integrating with AWS Security Hub**
   - Enabled AWS Security Hub in the AWS account.
   - Connected Security Hub to monitor the S3 bucket, CloudFront, and related AWS resources for security best practices and compliance findings.
   - Reviewed findings and recommendations directly in the Security Hub dashboard.

3. **Using AWS Audit Manager**
   - Created an assessment in AWS Audit Manager to track compliance requirements for the app's AWS resources.
   - Mapped controls to the S3 bucket, CloudFront, and IAM roles used by the app.
   - Generated audit-ready reports to demonstrate compliance posture.
![alt text](<aws audit manager-1.png>)

4. **Enabling AWS Config**
   - Enabled AWS Config to continuously record and evaluate the configuration of AWS resources used by the app.
   - Set up AWS Config rules to monitor changes and ensure resources remain compliant with organizational policies.
   - Used AWS Config timelines to review historical changes and support audit investigations.

### Example: How AWS Security Hub and AWS Config Identify Issues

Suppose a developer accidentally makes the S3 bucket (hosting the insurance app's static files) publicly accessible. Here's how AWS services help:

- **AWS Config** detects the configuration change and triggers a rule violation (e.g., "S3 bucket should not allow public read access").
- **AWS Security Hub** aggregates this finding and highlights it as a security issue in its dashboard, providing details and remediation steps.
- The team receives an alert, allowing them to quickly revoke public access and restore compliance.

This integration ensures that misconfigurations are identified and addressed promptly, protecting sensitive user and insurance data.

## Getting Started

To run the project locally:

1. Clone this repository: `git clone https://github.com/Engeniusam/rider-shield.git`
2. Navigate to the project directory: `cd Rider-shield`
3. Install dependencies: `npm install`
4. Start the development server: `npm start`
5. Open your browser and visit: `http://localhost:3000/Rider-Shield`

## Contributing

Contributions are welcome! If you find a bug or have a feature request, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](./LICENSE "Project LICENSE").
