
### /admin/organization/code/{organization_code}

#### GET
##### Summary:

Get organization by organization code

##### Description:

Get organization by organization code

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| organization_code | path | Organization code | Yes | string |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with the matching organization object |
| 408 | Token expired or Invalid token |
| 500 | Internal Sever error |

### /admin/organization/name/{name}

#### GET
##### Summary:

Get organization by organization name

##### Description:

Get organization by organization name

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path | Organization name | Yes | string |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with the matching organization object |
| 408 | Token expired or Invalid token |
| 500 | Internal Sever error |

### /admin/organization/add

#### POST
##### Summary:

Add organization

##### Description:

Create new organization

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| OrganizationEntity | body |  | Yes | [OrganizationEntity](#organizationentity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Success response with organization object that is added |
| 400 | Bad request with custom error message |
| 408 | Token expired or Invalid token |
| 409 | Organization exits |
| 500 | Internal Server error |

### /admin/organization/update

#### PUT
##### Summary:

Update organization

##### Description:

Update organization

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| OrganizationEntity | body |  | Yes | [OrganizationEntity](#organizationentity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with updated organization object |
| 400 | Bad request with custom error message |
| 408 | Token expired or Invalid token |
| 409 | Organization exits |
| 500 | Internal Server error |

### /admin/organization/softdelete/{id}

#### DELETE
##### Summary:

Soft delete an organization by id

##### Description:

Soft delete an organization by organization_id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | Organization id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with deleted organization object |
| 404 | Organization not found |
| 408 | Token expired or Invalid token |
| 500 | Internal server error |

### /admin/organization

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

### /admin/organization/{id}

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

### /admin/organization/delete/{id}

#### DELETE
##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | number |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 |  |

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

