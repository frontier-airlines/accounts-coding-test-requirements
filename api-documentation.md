# Accounts Endpoint

**URL:** https://frontiercodingtests.azurewebsites.net/api/accounts/getall

**HTTP Actions:** GET

**Authentication:** None

**Input Parameters:** None

**Expected Output Schema:**

HTTP Status: 200

```json
[
    {
        "Id": int,
        "FirstName": string,
        "LastName": string,
        "Email": string,
        "PhoneNumber": string,
        "AmountDue": decimal,
        "PaymentDueDate": datetimeoffset,
        "AccountStatusId": int
    }
]
```

**Account Statuses:** AccountStatusId in the response object is derived from the following C# enum.

```csharp
enum AccountStatuses
{
	Active,
	Inactive,
	Overdue
}
```

**Specifications:** 

- C#
- .NET Core 2.1
- Azure Function v2