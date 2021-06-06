# working-with-<img src="Reddit_VerticalLockup_OnDark.png" alt="reddit" width="80px" height="auto"/>-api-using-dotnet

This repo records all my learnings while exploring reddit API.

## Getting Started
### Registering the application
To be able to use reddit API, one must first register the application [here](https://www.reddit.com/prefs/apps).

### Saving the client id and client password
1. Save the client id and password somewhere.
2. This should be then saved in any of the secrets management provider. Eg: Azure Key Vault in case of Azure.

### Handling authorization and security
1. [This](https://github.com/reddit-archive/reddit/wiki/OAuth2) article explains in details the steps and process to handle different aspects of security.
2. To get authorization from a user to view its accout details use the below url:-

```https://www.reddit.com/api/v1/authorize?client_id=YOURCLIENT-ID&response_type=code&state=UserNumber1&redirect_uri=https://commonstoragesa.z29.web.core.windows.net/&duration=temporary&scope=identity%20edit%20flair%20history%20modconfig%20modflair%20modlog%20modposts%20modwiki%20mysubreddits%20privatemessages%20read%20report%20save%20submit%20subscribe%20vote%20wikiedit%20wikiread```

## References
1. https://github.com/reddit-archive/reddit/wiki/API
