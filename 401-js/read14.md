# Read 13:Access Control (ACL)

[README](/README.md)

## Review, Research, and Discussion

1. When is Basic Authorization used vs. Bearer Authorization?

- [Basic Auth](https://developer.mozilla.org/en-US/docs/Web/HTTP/Authentication) transmits credential as user ID/password pairs. They are
  encoded using base64. Basic auth is used to send the user information in
  a nice package in non plain text.

- [Bearer Auth](https://tools.ietf.org/html/rfc6750) involves OAuth na d lets clients access protected resources by obtaining an access token. This token is a string that represents access authorization issued to the client. This allows the transfer of that data without using the users actual credentials. It keeps their info secure

2. What does the JSON Web Token package do?

- [The JSON Web Token (JWT)](https://jwt.io/introduction/) securely transmits info between parties as aJSON obj on a compact and self contained way. There are both encrypted tokens ( which additionally provide secrecy between parties), and signed tokens. Signed tokens check to see if the person trying to access the data has the correct credentials.

3. What considerations should we make when creating and storing a SECRETS [Best Practices](https://blog.gitguardian.com/secrets-api-management/)

- We need to keep them in the dotenv or the secret is useless. Never store unencrypted secrets in .git repositories. add sensitive files in .gitignore

- Don't share unencrypted secrets via messenger like slack.

- Restrict API access and permissions

Vocabulary Terms

1. encryption - Encryption is used to keep data secret. In its simplest form, a file or data transmission is garbled so that only authorized people with a secret key can unlock the original text.

2. token

- Bearer Token A security token with the property that any party in possession of the token (a "bearer") can use the token in any way that any other party in possession of it can. Using a bearer token does not require a bearer to prove possession of cryptographic key material (proof-of-possession).

3. bearer

- a passport to get you into secure places

4. secret

- Also allows you get places

5. JSON Web Token

- JSON Web Token combines header, payload, signature into one encrypted string.

## Preparation material

[RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)

- Role-Based Access Control (RBAC) -- system to restrict access to authorized users

- Provides access depending on the role of the individual of that is asking for entry

access may be based on job function or role of a user
users authenticate themselves to the system
users then can activate one or more roles for themselves

Benefits
Policy does not need to be updated when certain person leaves the org
New employee is automatically able to access their role.
Roles give the ability to protect resources that people do not need access to.

5 steps to RBAC

[wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control) is a system to restrict access to authorized users

## Side Notes:

[Base64]() encodes binary strings into text representations using the base64 encoding format. Base64 encoding is often used in LDIF files to represent non-ASCII character strings. It is also frequently used to encode certificate contents or the output of message digests such as MD5 or SHA.

- Also decodes. This is not a secure method of password security
