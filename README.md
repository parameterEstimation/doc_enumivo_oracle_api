# About

This is the reference for the Enumivo Oracle REST APIs. The REST APIs are for developers who want to integrate Enumivo Oracle REST APIs with other applications or administrators that want to automate their workflows and processes.

# Members
#### Get members
`GET /api/public/members/`

This method returns a list of members registered in enumivo oracle.

###### Responses
| Code | Type | Description |
| --- | --- | --- |
| `200` OK | application/json | Returns paginated list of organizations. |

##### Query parameters
**limit** *integer* The maximum number of items to return per page.

**search** *string* Search filter lookup to screen name and enumivo mainnet account.

#### Get member
`GET /api/public/members/{memberId or mainNetAccount}/`

This method returns details of a member. Use this method to get member's details by passing member's id or members enumivo mainnet account.

###### Responses
| Code | Type | Description |
| --- | --- | --- |
| `200` OK | application/json | Returns the requested member. |
