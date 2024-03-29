# Reading Notes Class 15

## What is OAuth

1. What is OAuth?

    * OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

2. Give an example of what using OAuth would look like.

    * The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

3. How does OAuth work? What are the steps that it takes to authenticate the user?

    * Let’s assume a user has already signed into one website or service (OAuth only works using HTTPS). The user then initiates a feature/transaction that needs to access another unrelated site or service. The following happens (greatly simplified):

    * The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
    * The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
    * The first site gives this token and secret to the initiating user’s client software.
    * The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
    * If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
    * The user approves (or their software silently approves) a particular transaction type at the first website.
    * The user is given an approved access token (notice it’s no longer a request token).
    * The user gives the approved access token to the first website.
    * The first website gives the access token to the second website as proof of authentication on behalf of the user.
    * The second website lets the first website access their site on behalf of the user.
    * The user sees a successfully completed transaction occurring.
    * OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

4. What is OpenID?

    * OpenID is about authentication: as a commenter on StackOverflow pithily put it: “OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.”

## Authorization and Authentication flows

1. What is the difference between authorization and authentication?

    * Authentication is the process of verifying the identity of a user or entity. In simple terms, it answers the question, "Are you who you claim to be?"

    * Authorization occurs after authentication and determines what resources a user has access to and what they are allowed to do with those resources. It addresses the question, "What are you allowed to do?"

2. What is Authorization Code Flow?

    * The Authorization Code Flow involves exchanging an authorization code for a token.

    This flow can only be used for confidential applications (such as Regular Web Applications) because the application's authentication methods are included in the exchange and must be kept secure.

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

    * Authorization Code Flow with Proof Key for Code Exchange (PKCE, pronounced "pixie") is an enhancement to the standard OAuth 2.0 authorization process. It was originally designed to provide enhanced security for mobile and public clients, which cannot securely store client secrets. However, its utility has extended to web and other applications due to its robustness.

4. What is Implicit Flow with Form Post?

    * As an alternative to the Authorization Code Flow, OAuth 2.0 provides the Implicit Flow, which is intended for Public Clients, or applications which are unable to securely store Client Secrets. While this is no longer considered a best practice for requesting Access Tokens, when used with Form Post response mode, it does offer a streamlined workflow if the application needs only an ID token to perform user authentication.

5. What is Client Credentials Flow?

    * With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. For this scenario, typical authentication schemes like username + password or social logins don't make sense. Instead, M2M apps use the Client Credentials Flow (defined in OAuth 2.0 RFC 6749, section 4.4).

6. What is Device Authorization Flow?

    * With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text. To do this, device apps use the Device Authorization Flow (drafted in OAuth 2.0). For use with mobile/native applications.

7. What is Resource Owner Password Flow?

    * Applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form. The Resource Owner Password Flow should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used.