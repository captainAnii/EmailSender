# Email Sender

This is a Java Maven project for sending emails using JavaMail.

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- Maven 3.x or higher
- Gmail account with app password (see [How to generate app passwords](#how-to-generate-app-passwords))

## Setup

1. Clone the repository or download the project ZIP file.
2. Import the project into your Java IDE as a Maven project.
3. Update the `src/main/resources/config.properties` file with your Gmail account credentials, including the sender's email address, app password, recipient's email address, and other email details (e.g., subject, body).
4. Build the project using Maven by running `mvn clean install` in the project root directory.

## How to Generate App Passwords

To generate an app password for your Gmail account, follow these steps:

1. Go to the Google Account security page by visiting https://myaccount.google.com/security and sign in to your Google account.
2. In the "Signing in to Google" section, click on "App passwords" or navigate directly to https://myaccount.google.com/security/app-passwords.
3. If prompted, verify your Google account password.
4. Under the "Select app" drop-down menu, choose "Mail" or "Other (Custom name)".
5. If you chose "Mail", select the email app or device you will be using to send emails (e.g., "Mail on Mac" or "Outlook" if applicable). If you chose "Other (Custom name)", enter a custom name for the app or device.
6. Click on the "Generate" button.
7. Google will generate a unique app password for the selected app or device.
8. Copy the generated app password, as you will not be able to see it again.
9. Update the `config.properties` file in the project with the generated app password as the password for authentication.

## Usage

1. Run the Java program by executing the generated JAR file using `java -jar target/email-sender-1.0-SNAPSHOT.jar` command in the project root directory.
2. The program will send an email using the JavaMail library, and you will see the "Email sent successfully!" message printed in the console upon successful email sending.

## License

This project is licensed under the [MIT License](LICENSE).

## Contributions

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for more details.
