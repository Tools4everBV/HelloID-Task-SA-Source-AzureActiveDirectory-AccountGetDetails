# HelloID-Task-SA-Source-AzureActiveDirectory-AccountGetDetails

## Prerequisites
- [ ] This script uses the Microsoft Graph API and requires an App Registration with App permissions:
  - [ ] Read all users' full profiles <b><i>User.Read.All</i></b>

## Description

This code snippet executes the following tasks:

1. Define `$userPrincipalName` based on the `selectedUser` data source input `$dataSource.selectedUser.UserPrincipalName`
2. Creates a token to connect to the Graph API.
3. List user's details using the API call: [Get a user](https://learn.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0&tabs=http)
4. Return a hash table for each user account using the `Write-Output` cmdlet.

> To view an example of the data source output, please refer to the JSON code pasted below and select the `Interpreted as JSON` option in HelloID

```json
{
    "UserPrincipalName": "a.acevedo@domain.local"
}
```