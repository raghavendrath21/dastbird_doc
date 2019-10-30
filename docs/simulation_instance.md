

### /s2s/simulation_instance

#### GET
##### Summary:

Get all

##### Description:

Get all Simulation instance

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

### /s2s/simulation_instance/simulation/{simulation_id}

#### GET
##### Summary:

Get simulation instance by simulation_id

##### Description:

Get simulation instance by simulation_id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| simulation_id | path | simulation instance id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with all the matching simulation instance objects |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/simulation_instance/add

#### POST
##### Summary:

Add simulation instance

##### Description:

Create simulation instance

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| SimulationInstance | body |  | Yes | [SimulationInstance](#simulationinstance) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Simulation instance added successfully |
| 408 | Token expired or Invalid token |
| 409 | Simulation instance already exists |
| 500 | Internal Server error with the custom error message |

### /s2s/simulation_instance/update

#### PUT
##### Summary:

Update simulation instance

##### Description:

Update simulation instance

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| SimulationInstance | body |  | Yes | [SimulationInstance](#simulationinstance) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Simulation instance updated successfully |
| 400 | Bad request with custom error message |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error with the custom error message |

### /s2s/simulation_instance/simulation/organization/{simulation_id}/{organization_id}

#### GET
##### Summary:

Get simulation instance by simulation id and organization id

##### Description:

Get simulation instance by simulation id and organization id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| organization_id | path | organization id | Yes | number |
| simulation_id | path | simulation instance id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with all the matching simulation instance objects |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/simulation_instance/organization/{organization_id}

#### GET
##### Summary:

Get simulation instance by organization_id

##### Description:

Get simulation instance by organization_id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| organization_id | path | Organization id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with all the matching simulation instance objects |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/simulation_instance/instance/{name}

#### GET
##### Summary:

Get simulation instance by instance name

##### Description:

Get simulation instance by instance name

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| name | path | simulation instance name | Yes | string |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with all the matching simulation instance objects |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/simulation_instance/users/{simulation_instance_id}

#### GET
##### Summary:

Get users

##### Description:

Get all users for a simulation instance

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| simulation_instance_id | path |  | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Users assigned to simulation successfully |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/simulation_instance/users/add

#### POST
##### Summary:

Add users

##### Description:

Add users to simulation instance

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| SimulationUser | body |  | Yes | [SimulationUser](#simulationuser) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Users assigned to simulation successfully |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/simulation_instance/users/update

#### PUT
##### Summary:

Update users

##### Description:

Update user role, first name, last name for the simulation instance

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| SimulationUser | body |  | Yes | [SimulationUser](#simulationuser) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Users assigned to simulation successfully |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/simulation_instance/users/delete

#### POST
##### Summary:

Delete users

##### Description:

Delete users from simulation instance based on the email

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| SimulationUser | body |  | Yes | [SimulationUser](#simulationuser) |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Users assigned to simulation successfully |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /s2s/simulation_instance/softdelete/{id}

#### DELETE
##### Summary:

Soft delete simulation instance by id

##### Description:

Soft delete simulation instance by simulation instance id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | simulation instance id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Simulation instance deleted successfully |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error with custom error message |

### /s2s/simulation_instance/delete/{id}

#### DELETE
##### Summary:

Delete simulation instance

##### Description:

Delete simulation instance by simulation instance id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | simulation instance id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Simulation instance deleted successfully |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error with custom error message |

### /s2s/simulation_instance/{id}

#### GET
##### Summary:

Get simulation instance by simulation instance id

##### Description:

Get simulation instance by simulation instance id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path | simulation instance id | Yes | number |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Success response with all the matching simulation instance objects |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |