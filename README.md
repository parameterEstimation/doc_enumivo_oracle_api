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
###### **limit** *integer*

The maximum number of items to return per page.

###### **organizationId** *integer*

Filters customer requests that belong to a specific organization (note that the user must be a member of that organization). **Note:** Valid only when used with requestOwnership=ORGANIZATION.

###### **requestOwnership** *array*

#### Get member
`GET /api/public/members/{memberId or mainNetAccount}/`

This method returns details of a member. Use this method to get member's details by passing member's id or members enumivo mainnet account.

###### Responses
| Code | Type | Description |
| --- | --- | --- |
| `200` OK | application/json | Returns the requested member. |
