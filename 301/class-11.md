# Authentication


## **What is OAuth**


* What is OAuth?

    **An open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential**

* Give an example of what using OAuth would look like.

    **When logging onto a website and it offers one or more opportunities to log on using another website’s/service’s logon**

* How does OAuth work? What are the steps that it takes to authenticate the user?

1. **The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.**

2. **The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.**
3. **The first site gives this token and secret to the initiating user’s client software.**
4. **The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).**
5. **If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.**
6. **The user approves (or their software silently approves) a particular transaction type at the first website.**
7. **The user is given an approved access token (notice it’s no longer a request token).**
8. **The user gives the approved access token to the first website.**
9. **The first website gives the access token to the second website as proof of authentication on behalf of the user.**
10. **The second website lets the first website access their site on behalf of the user.**
11. **The user sees a successfully completed transaction occurring.**

* What is OpenID?

    **Authentication security technology, rather than having multiple logins for multiple websites, OpenID would serve as a single sign-in, vouching for the identities of users**



## **Authorization and Authentication flows**


* What is the difference between authorization and authentication?

    **Authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to.**

* What is Authorization Code Flow?

    **Exchanging an Authorization Code for a token**

* What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

    **Version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange, enhanced Authorization Code Flow introduces a secret created by the calling application that can be verified by the authorization server**

* What is Implicit Flow with Form Post?

    **Alternative to the Authorization Code Flow intended for Public Clients, or applications which are unable to securely store Client Secrets.**

* What is Client Credentials Flow?

    **Alternative for authenticates for machine-to-machine (M2M) applications**

* What is Device Authorization Flow?

    **Alternative for authenticate, where the device asks the user to go to a link on their computer or smartphone and authorize the device, in which they pass along their Client ID to initiate the authorization process and get a token.**

* What is Resource Owner Password Flow?

    **Used by highly-trusted applications, which requests that users provide credentials (username and password), typically using an interactive form**