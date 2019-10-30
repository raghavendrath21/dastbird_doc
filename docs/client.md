
### /admin/client/add

#### POST
##### Summary:

Add client 

##### Description:

Add client 

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| ClientEntity | body |  | Yes | [ClientEntity](#cliententity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Success response with user object |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /admin/client/update

#### PUT
##### Summary:

Update

##### Description:

Update

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| ClientEntity | body |  | Yes | [ClientEntity](#cliententity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 404 | Not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /admin/client/reset

#### POST
##### Summary:

Reset

##### Description:

Reset

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| ClientEntity | body |  | Yes | [ClientEntity](#cliententity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 404 | Not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /admin/client/softdelete/{id}

#### DELETE
##### Summary:

Soft Delete

##### Description:

Soft Delete

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with deleted  client |
| 404 | Not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /admin/client

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

### /admin/client/{id}

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

### /admin/client/delete/{id}

#### DELETE
##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | number |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 |  |
