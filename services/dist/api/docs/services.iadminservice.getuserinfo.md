<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@digitalpersona/services](./services.md) &gt; [IAdminService](./services.iadminservice.md) &gt; [GetUserInfo](./services.iadminservice.getuserinfo.md)

## IAdminService.GetUserInfo() method

Queries an information about a specific user.

<b>Signature:</b>

```typescript
GetUserInfo(ticket: Ticket, user: User): Promise<UserInfo>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  ticket | <code>Ticket</code> | a ticket with a JSON Web Token of the user who would like to request user information. The owner of the token must have permissions to query user information. |
|  user | <code>User</code> | a user whose information is to be requested. |

<b>Returns:</b>

`Promise<UserInfo>`

- an information about the user.
