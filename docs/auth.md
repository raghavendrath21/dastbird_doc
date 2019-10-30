### Login

#### METHOD
POST
##### URL:
/s2s/auth/login

##### Description:

To verify login request from user

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Successful login response object |
| 404 | Organization not found |
| 500 | Internal Server error |

### Logout

#### GET
##### URL
/s2s/auth/logout


##### Description:

Log out

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Successful logout |
| 404 | Organization not found |
| 500 | Internal Server error |

### Callback

#### Method
GET
##### URL:

/s2s/auth/callback

##### Description:

Call back

##### Responses

| Code | Description |
| ---- | ----------- |
| 400 | Bad request |
| 401 | Unauthorized |
| 404 | Organization not found |
| 500 | Internal Server error |

### /s2s/auth/impersonate

#### POST
##### Summary:

Impersonate organization

##### Description:

To impersonate super user from one organization to another

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| ImpersonateOrganization | body |  | Yes | [ImpersonateOrganization](#impersonateorganization) |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Response is a token data |
| 400 | Bad request |
| 401 | Unauthorized |
| 404 | Organization not found |
| 500 | Internal Server error |
