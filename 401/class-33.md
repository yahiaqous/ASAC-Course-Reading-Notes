# Authentication & Production Server

## JSON Web Tokens

JSON Web Token (JWT) is an **open standard** that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

### **When should you use JSON Web Tokens?**

- **Authorization** - Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token

- **Information Exchange** - JSON Web Tokens are a good way of securely transmitting information between parties

JSON Web Tokens consist of three parts separated by dots (.), which are:

- **Header**
- **Payload**
- **Signature**

Therefore, a JWT typically looks like **_xxxxx.yyyyy.zzzzz_**

&nbsp;

![client-credentials-grant](../Pictures/client-credentials-grant.png)

1. The application or client requests authorization to the authorization server. This is performed through one of the different authorization flows
2. When the authorization is granted, the authorization server returns an access token to the application
3. The application uses the access token to access a protected resource (like an API)

### **Benefits of JSON Web Tokens (JWT)**

- **JSON is less verbose than XML**, when it is encoded its size is also smaller

- Security-wise, SWT can only be symmetrically signed by a shared secret using the HMAC algorithm. However, **JWT and SAML tokens can use a public/private key** pair in the form of an X.509 certificate for signing

- JSON parsers are common in most programming languages because they **map directly to objects**

&nbsp;

## DRF JWT Authentication

The **refresh token** is necessary to make sure the user still has the correct permissions. If your access token has a long expire time, it may take longer to update the information associated with the token. That’s because the authentication check is done by cryptographic means, instead of querying the database and verifying the data. So some information is sort of cached.

&nbsp;

## Django Migrations Primer

Working directly with SQL can be quite cumbersome, so to make your life easier, Django comes with an object-relational mapper or ORM for short. The ORM maps the relational database to the world of object-oriented programming. Instead of defining database tables in SQL, you write Django models in Python. Your models define database fields, which correspond to the columns in their database tables.

Creating the database tables to store your Django models is the job of a database migration

### **Benefits of Django migrations**

- Making Database Changes Without SQL
- Avoiding Repetition
- Ensuring Model Definitions and the Database Schema in Sync
- Tracking Database Schema Change in Version Control
