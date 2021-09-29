# Lightning-Deal-E-Commerce

# Development Log

- 9/28/2021
  - Finish configuring the project;
  - Finish the Log-In module:
    - Two layers of MD5 encryptions are used for safety: MD5(MD5(password + salt) + salt);
    - Use @ControllerAdvice + ExceptionHandler to handle login error;
