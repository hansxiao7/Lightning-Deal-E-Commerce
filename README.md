# Lightning-Deal-E-Commerce

# Development Log

- 9/28/2021
  - Finish configuring the project;
  - Finish the Log-In module:
    - Two layers of MD5 encryptions are used for safety: MD5(MD5(password + salt) + salt);
    - Spring Boot Starter Validation is used to valid the form inputs for login, and @ControllerAdvice + ExceptionHandler to handle login validation error;
    - Cookie-session is used to check whether it is logged in or out.
  - Configure the Redis:
    - Instead of using SpringSession, user information is stored directly in Redis.
    - RedisTemplate + RedisConnectionFactory are used;
- 9/29/2021
  - Use WebMvcConfigurer to customerize the handler for cookie session to get user info;
  - Finished the front pages and order services;
  - Run load test wit JMeter;
