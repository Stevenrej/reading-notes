## What is OAuth

1. What is OAuth? - OAuth is an open-standard authorization protocol or framework that provides applications the ability for “secure designated access.” For example, you can tell Facebook that it’s OK for ESPN.com to access your profile or post updates to your timeline without having to give ESPN your Facebook password. This minimizes risk in a major way: In the event ESPN suffers a breach, your Facebook password remains safe.
2. Give an example of what using OAuth would look like. -  example, Joe is the user, Bitly is the consumer, and Twitter is the service provided who controls Joe’s secure resource (his Twitter stream).  Joe would like Bitly to be able to post shortened links to his stream.
3. How does OAuth work? What are the steps that it takes to authenticate the user? - Step 1 – The User Shows Intent
Step 2 – The Consumer Gets Permission
Step 3 – The User Is Redirected to the Service Provider
Step 4 – The User Gives Permission
Step 5 – The Consumer Obtains an Access Token
Step 6 – The Consumer Accesses the Protected Resource

4. What is OpenID? OpenID allows you to use an existing account to sign in to multiple websites, without needing to create new passwords.

## Authorization and Authentication flows

1. What is the difference between authorization and authentication? - Authentication verifies the identity of a user or service, and authorization determines their access rights.
2. What is Authorization Code Flow? - authorization code grant type, or auth code flow, enables a client application to obtain authorized access to protected resources like web APIs.
3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)? - The user clicks Login within the application.

Auth0's SDK creates a cryptographically-random code_verifier and from this generates a code_challenge.

Auth0's SDK redirects the user to the Auth0 Authorization Server (
/authorize
endpoint) along with the code_challenge.

Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the application.

Your Auth0 Authorization Server stores the code_challenge and redirects the user back to the application with an authorization code, which is good for one use.

Auth0's SDK sends this code and the code_verifier (created in step 2) to the Auth0 Authorization Server (
/oauth/token
endpoint).

Your Auth0 Authorization Server verifies the code_challenge and code_verifier.

Your Auth0 Authorization Server responds with an ID token and access token (and optionally, a refresh token).

Your application can use the access token to call an API to access information about the user.

The API responds with requested data.

4. What is Implicit Flow with Form Post? Implicit Flow with Form Post flow uses OIDC to implement web sign-in
6. What is Device Authorization Flow? - With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text.
7. What is Resource Owner Password Flow? - The Resource Owner Password Credentials flow allows exchanging the username and password of a user for an access token and, optionally, a refresh token.

[Back To 301 Notes](https://stevenrej.github.io/reading-notes/readingnotes301main)