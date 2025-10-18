# Example sanitized findings (do not publish as-is; use as guidance)


## Example: Unsafe file upload acceptance (High)
**Summary:** The application accepts unvalidated file uploads and stores them in a web-accessible directory, enabling potential remote code execution in poorly configured servers.


**Evidence:** "Screenshot shows a successful upload confirmation. Filenames and IPs redacted."


**Recommendation:** Enforce server-side type checks, scan uploads in a sandbox, and avoid storing uploads in web root.


---


## Example: Weak password storage (Medium)
**Summary:** Passwords stored using weak hashing or without salts.
**Recommendation:** Migrate to strong password hashing (e.g., bcrypt/argon2) and enforce password policy.
