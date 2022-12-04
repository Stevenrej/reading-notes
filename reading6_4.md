## Reading 6

## Securing Passwords

Explain to a non-technical friend how you would safely hash and store a password.

- When a password is taken in it is changed and stored as something else that the database knows about. So when extracted and the user is trying to sign in the database can put out the correct response the user intialy put in.

What is Bcrypt?

- Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.

Why might you use something like Bcrypt?

- This work factor value determines how slow the hash function will be, means different work factor will generate different hash values in different time span, which makes it extremely resistant to brute force attacks. When computers become faster next year we can increase the work factor to balance it out i.e. to make the attack slower.

## Basic Auth

What is Basic Authentication?

-  basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon :.

What properties are necessary in the header of a Basic Auth request?

- Authorization: Basic <credentials>

How are username:password in Basic Auth encoded?

- They are merely encoded with Base64 in transit and not encrypted or hashed in any way. Therefore, basic authentication is typically used in conjunction with HTTPS to provide confidentiality.

## OWASP auth cheatsheet

Define the authentication process to a non-technical recruiter.

- Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

How should your error messaging respond (both HTTP and HTML)? Why?

- The problem with returning a generic error message for the user is a User Experience (UX) matter. A legitimate user might feel confused with the generic messages, thus making it hard for them to use the application, and might after several retries, leave the application because of its complexity. The decision to return a generic error message can be determined based on the criticality of the application and its data. For example, for critical applications, the team can decide that under the failure scenario, a user will always be redirected to the support page and a generic error message will be returned.

Regarding the user enumeration itself, protection against brute-force attack is also effective because they prevent an attacker from applying the enumeration at scale. Usage of CAPTCHA can be applied on a feature for which a generic error message cannot be returned because the user experience must be preserved.
