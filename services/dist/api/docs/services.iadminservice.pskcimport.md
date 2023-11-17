<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@digitalpersona/services](./services.md) &gt; [IAdminService](./services.iadminservice.md) &gt; [PSKCImport](./services.iadminservice.pskcimport.md)

## IAdminService.PSKCImport() method

Imports PSKC data to DPCA database.

<b>Signature:</b>

```typescript
PSKCImport(ticket: Ticket, PSKCData: Base64UrlString, PSKCFileName?: string | null, password?: string | null, sharedKey?: string | null): Promise<PSKCOutput[]>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  ticket | <code>Ticket</code> | a ticket with a JSON Web Token of the user who would like to import PSKC data to DPCA database. The owner of the token must have permissions to import the data. |
|  PSKCData | <code>Base64UrlString</code> | a content of PSKC file provided by OTP vendor in Base64Url encoded format |
|  PSKCFileName | <code>string &#124; null</code> | a name of PSKC file provided by OTP vendor. This name is required for audit purposes only. |
|  password | <code>string &#124; null</code> | a password to protect PSKC data. This parameter is optional and will required only if Encryption Based on Passphrase-Based Keys is used for data protection in PSKC (see topic 6.2 of RFC6030, https://tools.ietf.org/html/rfc6030 for details) |
|  sharedKey | <code>string &#124; null</code> | an encoded value of Pre-Shared key for PSKC secrets. The format of the encoding is manufacturer depended and unknown. It is server's responsibility to find out a proper encoding format and decode the key. This parameter is optional and it is required only if Encryption Based on Pre-Shared Keys is used for data protection in PSKC (see topic 6.1 of RFC6030, https://tools.ietf.org/html/rfc6030 for details) |

<b>Returns:</b>

`Promise<PSKCOutput[]>`

a promise to return a list of objects in DPPSKCOutput format. It gives us information about result of importing operation for every OTP token inside PSKC file.
