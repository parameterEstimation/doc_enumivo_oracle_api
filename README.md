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

###### Query parameters
| Query | Type | Behavior | Description |
| --- | --- | --- | --- |
| limit | integer | | The maximum number of items to return per page. |
| search | string | contains |Search filter lookup to screen name and enumivo mainnet account. |
| screen_name | string | exact |Search by screen name. |
| user__enu_account_info__enu_mainnet_account | string | exact |Search by enumivo mainnet account. |
| user__enu_user_class__is_profile_verified | boolean | exact |Search filter by profile verification status. |
| user__enu_user_class__is_email_verified | boolean | exact |Search filter by email verification status . |
| user__enu_user_class__is_denied | boolean | exact |Search filter by denied status. |


#### Get member
`GET /api/public/members/{memberId or mainNetAccount}/`

This method returns details of a member. Use this method to get member's details by passing member's id or members enumivo mainnet account.

###### Responses
| Code | Type | Description |
| --- | --- | --- |
| `200` OK | application/json | Returns the requested member. |
