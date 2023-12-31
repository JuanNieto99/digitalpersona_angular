<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@digitalpersona/services](./services.md) &gt; [IAdminService](./services.iadminservice.md) &gt; [ExecuteSearch](./services.iadminservice.executesearch.md)

## IAdminService.ExecuteSearch() method

Executes a search on the DPCA Server database and returns the result of search operation. NOTE: The result of search operation is limited to 100 records.

<b>Signature:</b>

```typescript
ExecuteSearch(ticket: Ticket, query: SearchQuery): Promise<Attribute[][]>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  ticket | <code>Ticket</code> |  |
|  query | <code>SearchQuery</code> |  |

<b>Returns:</b>

`Promise<Attribute[][]>`

a promise to return a list of the rows, where each row is a list or requested object attributes. NOTE: The maximum number of rows is limited to 100, the rest of the result is truncated.

