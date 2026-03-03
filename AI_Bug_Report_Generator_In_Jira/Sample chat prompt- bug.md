Create a bug in JIRA with proper steps to reproduce for below log 
[2026-03-03 10:42:17 UTC] ERROR

Application: VWO Web App Version: 3.14.2 Environment: Production OS: Windows 11 Browser: Chrome 122.0.0.0

Service: Authentication Service Module: Login API Endpoint: POST /api/v1/login

Error Code: AUTH-5001 HTTP Status: 500 Internal Server Error

Error Message: NullReferenceException: Object reference not set to an instance of an object.

Stack Trace: at AuthService.ValidateUserCredentials(UserRequest request) at AuthController.Login(UserRequest request) at lambda_method(Closure , Object , Object[] )

User Action: User attempted to log in using valid registered email and password.

Observed Behavior: Login request failed and user received "Something went wrong. Please try again later."

Additional Info:

Issue reproduced 4 times between 10:38–10:42 UTC Other APIs are functioning normally No recent deployment in last 24 hours