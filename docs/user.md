
### /s2s/user/organization/{organization_id}

#### GET
##### Summary:

Get users by organization_id

##### Description:

Get users by organization_id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| organization_id | path | organization id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with matching user objects |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/user/role/{name}

#### GET
##### Summary:

Get users by role

##### Description:

Get users by role

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path | Role name | Yes | string |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with matching user objects |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/user/cognito/{organization_id}

#### GET
##### Summary:

Get users by organization_id

##### Description:

Get users by organization_id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| organization_id | path | organization id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with matching user objects |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/user/add

#### POST
##### Summary:

Add user

##### Description:

Create user

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| UserEntity | body |  | Yes | [UserEntity](#userentity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Success response with user object |
| 400 | Bad request with custom error message |
| 404 | Not found response with custom error message |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/user/uploadUsers

#### POST
##### Summary:

Upload users

##### Description:

Upload users

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| Array | body |  | Yes | [Array](#array) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Success response with user objects |
| 400 | Bad request with custom error message |
| 404 | Not found response with custom error message |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/user/update

#### PUT
##### Summary:

Update user

##### Description:

Update user by user id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| UserEntity | body |  | Yes | [UserEntity](#userentity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | User updated successfully |
| 400 | Bad request with custom error message |
| 404 | Not found response with custom error message |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/user/softdelete/{id}

#### DELETE
##### Summary:

Soft delete user by id

##### Description:

Soft delete user by user id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | user id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | User deleted successfully |
| 404 | Not found response with custom error message |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/user/resource/{access_token}

#### GET
##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| access_token | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 |  |

### /s2s/user

#### GET
##### Summary:

Get all entities

##### Description:

Get all entities

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with all objects |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/user/{id}

#### GET
##### Summary:

Get an entity by id

##### Description:

Get an entity by id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with matching object |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/user/delete/{id}

#### DELETE
##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | number |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 |  |
