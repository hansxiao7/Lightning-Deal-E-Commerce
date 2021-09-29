# Lightning-Deal-E-Commerce

# Development Log

- 9/28/2021
  - Finish configuring the project;
  - Finish the Log-In module:
    - Two layers of MD5 encryptions are used for safety: MD5(MD5(password + salt) + salt);
    - Use @ControllerAdvice + ExceptionHandler to handle login error;
    - Spring Boot Starter Validation is used to valid the form inputs for login.
    - Cookie-session is used to check whether it is logged in or out.
  - Configure the Redis:
    - Instead of using SpringSession, user information is stored directly in Redis.
    - RedisTemplate + RedisConnectionFactory are used;
