<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@digitalpersona/services](./services.md) &gt; [IAdminService](./services.iadminservice.md) &gt; [AdminDeleteUserCredentials](./services.iadminservice.admindeleteusercredentials.md)

## IAdminService.AdminDeleteUserCredentials() method

Deletes specified user credentias without the user's presence.

<b>Signature:</b>

```typescript
AdminDeleteUserCredentials(ticket: Ticket, user: User, credentials: Credential[]): Promise<void>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  ticket | <code>Ticket</code> | a ticket with a JSON Web Token of the user who would like to delete user credentials. The owner of the token must have permissions to reset user credentials. |
|  user | <code>User</code> | a user whose credentials will be deleted. |
|  credentials | <code>Credential[]</code> | a list of credentials ID to delete. NOTE: currently the <code>data</code> part of credentials is ignored. |

<b>Returns:</b>

`Promise<void>`

