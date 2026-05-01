## usecase login new

1. Test Objective
The goal was to verify the system's behavior when an unregistered user attempts to log in or reset a password.

2. Steps Performed

    Login Attempt: Entered the username munguakonkwa kabidu and the email address munguakonkwakabidudu@gmail.com.

    Recovery Attempt: Accessed the "Lost your password?" link and submitted the same email address.

3. Observations and Error Messages

    During Login: The system triggered the following alert: "Error: The username is not registered on this site".

    During Reset: The system triggered the following alert: "Error: There is no account with that username or email address".

4. Test Conclusion
The Use Case is successfully validated. The system correctly enforces security protocols:

    Access is strictly restricted to users verified within the database.

    Error handling is accurate, providing clear feedback to the user.

    System integrity is maintained by preventing any unauthorized actions from non-existent accounts.

## Registration Interface: Test and Compliance Analysis Report



### Problem Description: Use Case Deviation

When accessing the registration page for a student profile, the interface currently only displays two fields: Username and Email Address.

### Observation: 

The use case is not being followed. According to the functional specifications, the user should be able to select their academic level and their preferred programming language at the time of registration. These elements are missing from the current interface.
### Details of Performed Tests

A. Mandatory Field Validation

    Empty Field Test: By leaving all fields empty and clicking the "Register" button, the system blocks the action and displays the following error messages:

        "Error: Please enter a username."

        "Error: Please type your email address."

    Partial Entry Test: If the username is provided but the email address is missing, the system also blocks the registration and requires the missing address to be entered.

B. Data Uniqueness Validation

    Username Duplicate Test: An attempt to register with a username that already exists in the database (but with a different email address) was blocked by the system with the following message:

        "Error: This username is already registered. Please choose another one."

C. Success Test and Mail Server Performance

Two accounts were successfully created to validate the complete workflow:

    User: kabidu sage | Address: abidusaagemg@mail.com

    User: sage kabidu | Address: abidusage@gmail.com


![alt text](../login%20new%20student%20path/img/email.png)


Result: For both accounts, the confirmation email was received within seven seconds, confirming the speed and reliability of the electronic mail delivery service.

### Conclusion

While the system is technically sound (excellent error management, duplicate validation, and fast email delivery), there is a major compliance gap regarding the business requirements.

 



## Validation of Security Protocols and Password Update Workflow.

1. Analysis of the Reset Interface
Upon accessing the recovery link, the system suggests a highly secure default password (e.g., E2Q6zDd(Hm%%%%Fd). This feature demonstrates a proactive approach to guiding users toward maximum security.

2. Password Strength Meter Testing
The system dynamically evaluates input complexity to ensure robust account protection:

    Medium Level: The password Toujours# was identified as having medium security.

    Strong Level: The password Toujours#toucher*123 was validated as "Strong" by the security algorithm.

3. Results and Confirmation
Once the password was saved, the system confirmed the update with the message: "Your password has been reset. Log in". The redirection link to the dashboard is immediately functional.

![alt text](../login%20new%20student%20path/img/password_reset.png)

4. Test Conclusion
The use case is fully validated. The application demonstrates high security standards by preventing the use of weak passwords or empty fields. The workflow now allows for a secure login to the dashboard using the new credentials.



# Validation of Error Handling during Login (Use Case: Login) 



1. Test Objective
The goal was to ensure that the system denies access and correctly informs the user when a non-existent account or incorrect credentials are provided.

2. Test Procedure

    Attempted to log in using the unregistered username: sage kabidus.

    Tested various combinations of usernames and passwords that are not stored in the database.

3. Observations and Error Messages
The system consistently blocked access and triggered the following error message:

    "Error: The username is not registered on this site. If you are unsure of your username, try your email address instead."

![alt text](../login%20new%20student%20path/img/wrong_crdl.png)    

4. Test Conclusion
The Use Case is fully validated. The security system operates according to the technical specifications:

    Any login attempt involving data not found in the database triggers an appropriate warning.

    Protection against unauthorized access is fully enforced, ensuring that only registered users can access the platform.