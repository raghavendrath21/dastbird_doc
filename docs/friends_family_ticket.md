

### /s2s/friends_family_ticket/instance/{instance_id}

#### GET
##### Summary:

Get Friends & Family tickets by simulation instance id

##### Description:

Get Friends & Family tickets by simulation instance id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| instance_id | path | simulation instance id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with all the friends & family tickets |
| 408 | Token expired or Invalid token |
| 500 | Internal server error |

### /s2s/friends_family_ticket/add

#### POST
##### Summary:

Add Friends & Family ticket

##### Description:

POST call to add Friends & Family ticket

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| FriendsFamilyTicketEntity | body |  | Yes | [FriendsFamilyTicketEntity](#friendsfamilyticketentity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Success |
| 400 | Bad request with a custom error message |
| 408 | Token expired or Invalid token |

### /s2s/friends_family_ticket/update

#### PUT
##### Summary:

Update Friends & Family ticket

##### Description:

Update Friends and Family ticket

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| FriendsFamilyTicketEntity | body |  | Yes | [FriendsFamilyTicketEntity](#friendsfamilyticketentity) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Updated  successfully |
| 404 | Not found |
| 408 | Token expired or Invalid token |

### /s2s/friends_family_ticket

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

### /s2s/friends_family_ticket/{id}

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

### /s2s/friends_family_ticket/softdelete/{id}

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

### /s2s/friends_family_ticket/delete/{id}

#### DELETE
##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | number |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 |  |
