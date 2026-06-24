# Portswigger Lab (Authentication)
## Description
An authentication vulnerability is a security weakness that allows an attacker to bypass, weaken, or abuse the authentication process and gain access to an account or system without properly proving their identity. These can arise from poor password management, insecure session handling, weak multi-factor authentication implementations, credential stuffing attacks, brute-force attacks, or improper validation of authentication tokens and credentials. 
## Impact:
* Unauthorized access to user accounts by exploiting weak or compromised credentials.
* Account takeover through brute-force attacks, credential stuffing, password spraying, or session hijacking.
* Privilege escalation when attackers gain access to administrative or high-privilege accounts.
* Exposure of sensitive information, including personal data, financial records, and confidential business information.
* Unauthorized actions performed on behalf of legitimate users, potentially leading to financial loss, data breaches, or reputational damage.
* Compromise of multiple systems when authentication mechanisms are shared across applications (Single Sign-On environments).
## Mitigation:
* Enforce strong password policies, including minimum length, complexity requirements, and password expiration where appropriate.
* Implement Multi-Factor Authentication (MFA) for all sensitive accounts and administrative access.
* Protect against brute-force attacks using account lockout mechanisms, rate limiting, CAPTCHA, and monitoring for suspicious login attempts.
* Store passwords securely using strong hashing algorithms such as bcrypt, Argon2, or PBKDF2 with unique salts.
* Use secure session management practices, including secure cookies, session expiration, and session invalidation after logout.
* Implement proper authentication token validation and ensure tokens are securely generated, transmitted, and stored.
## Lab: Broken brute-force protection, multiple credentials per request
* Open the URL in portswigger proxy tab to intercept the request.
![request intercepted](Screenshots/SS1.png)
