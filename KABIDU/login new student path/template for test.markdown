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