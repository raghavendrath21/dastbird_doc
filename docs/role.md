
### getOrganizationById

**Method**: GET

**URL**: /admin/role/organization/{organization_id}

**Summary**:
Get roles by organization_id

**Description**:
Get all roles by organization_id

**Parameters**

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| organization_id | path | Organization id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success response with all the role objects |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |



### /admin/role/add

#### POST
##### Summary:

Add role

##### Description:

Add role

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| RoleEntity | body |  | Yes | [RoleEntity](#roleentity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Success response with the role object added |
| 408 | Token expired or Invalid token |
| 409 | Role exists |
| 500 | Internal Server error |

### /admin/role/update

#### PUT
##### Summary:

Update role

##### Description:

Update role

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| RoleEntity | body |  | Yes | [RoleEntity](#roleentity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with the updated role object |
| 408 | Token expired or Invalid token |
| 409 | Role exists |
| 500 | Internal Server error |

### /admin/role

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

### /admin/role/{id}

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

### /admin/role/softdelete/{id}

#### DELETE
##### Summary:

Soft delete an entity by id

##### Description:

Soft delete an entity by id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | Entity id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with deleted object |
| 404 | Not found error with custom message |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /admin/role/delete/{id}

#### DELETE
##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | number |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 |  |
