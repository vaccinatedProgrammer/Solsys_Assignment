# Solsys_Assignment

## Solsys - API Reference

The Solsys API is organized around REST. Solsys API has predictable resource-oriented URLs, accepts form-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.

### Errors

Solsys uses conventional HTTP response codes to indicate the success or failure of an API request. In general: Codes in the 2xx range indicate success. Codes in the 4xx range indicate an error that failed given the information provided (e.g., a required parameter was omitted, etc.). Codes in the 5xx range indicate an error with Solsys's servers (these are rare).

Some 4xx errors that could be handled programmatically (e.g., a card is declined) include an error code that briefly explains the error reported.

#### HTTP STATUS CODE SUMMARY

- **200 - OK** : Everything worked as expected.
- **400 - Bad Request** : The request was unacceptable, often due to missing a required parameter.
- **401 - Unauthorized** : No valid API Key / access token provided.
- **402 - Request Failed** : The parameters were valid but the request failed.
- **403 - Forbidden** : The API key doesn't have permissions to perform the request.
- **404 - Not Found** : The requested resource doesn't exist.
- **405 - Validation Exception** : The properties in the request body are not right shape/type
- **500, 502, 503, 504 - Server Error** : Something went wrong on Solsys's end.

The API would need to allow for some of the following:

- Creation of a new account
- Retrieval of account information
- Changes to an existing account
- Deleting of an existing account
- Creation of a new subscription
- Retrieval of account information
- Changes to an existing subscription
- Deleting of an existing subscription
- Creation of a billing address
- Retrieval of a billing address
- Changes to an existing billing address
- Deleting of an existing billing address
