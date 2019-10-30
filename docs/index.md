# DashBird Auth Server
The Auth Server API description

## Version: 1.0.0

### /validate/{token}

#### GET
##### Summary:

Validate token

##### Description:

Validates token

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| token | path | token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Returns decoded token |
| 408 | Token expired or Invalid token |

### /resetPassword

#### POST
##### Summary:

Reset Password

##### Description:

User can reset password

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| AuthRequest | body |  | Yes | [AuthRequest](#authrequest) |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Password reset done successfully |
| 403 | Token expired or Invalid token |
| 404 | User not found |

#### GET
##### Summary:

ResetPassword

##### Description:

ResetPassword

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | ResetPassword successfully |
| 404 | User not found |
| 500 | Internal Server error |

### /forgotPassword

#### POST
##### Summary:

Forgot Password

##### Description:

Forgot password

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| AuthRequest | body |  | Yes | [AuthRequest](#authrequest) |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Password reset done successfully |
| 403 | Token expired or Invalid token |
| 404 | User not found |

#### GET
##### Summary:

Forgot Password

##### Description:

Forgot Password

##### Responses

| Code | Description |
| ---- | ----------- |
| 404 | User not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /newPassword

#### POST
##### Summary:

New Password

##### Description:

New password

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| AuthRequest | body |  | Yes | [AuthRequest](#authrequest) |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Password changed successfully |
| 400 | Bad request |
| 403 | Token expired or Invalid token |

### /getImpersonateToken

#### POST
##### Summary:

Get the impersonated token

##### Description:

Get the impersonated token

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| AuthRequest | body |  | Yes | [AuthRequest](#authrequest) |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Returns impersonated token |
| 408 | Token expired or Invalid token |

### /tokenSignin

#### POST
##### Summary:

Token Sign in

##### Description:

User can sign in to the application using token

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| AuthRequest | body |  | Yes | [AuthRequest](#authrequest) |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | User logged in successfully |
| 404 | Invalid Token |

### /tokenSignUp

#### POST
##### Summary:

Token Signup

##### Description:

User can signup to the application using token

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| AuthRequest | body |  | Yes | [AuthRequest](#authrequest) |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | User signed up successfully |
| 404 | Invalid Token |
| 409 | An account with this email already exists |
| 500 | Internal Server error |

#### GET
##### Summary:

Token SignUp

##### Description:

Token SignUp

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | TokenSignIn successfully |
| 404 | User not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /

#### GET
##### Responses

| Code | Description |
| ---- | ----------- |
| 200 |  |

### /login

#### GET
##### Summary:

Login

##### Description:

Login

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Login successfully |
| 404 | User not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

#### POST
##### Summary:

Login

##### Description:

Login

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Login successfully |
| 404 | User not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /logout

#### GET
##### Summary:

Logout

##### Description:

Logout

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | Logout successfully |
| 404 | User not found |
| 500 | Internal Server error |

### /tokenSignIn

#### GET
##### Summary:

Token SignIn

##### Description:

Token SignIn

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | TokenSignIn successfully |
| 404 | User not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /changePassword

#### GET
##### Summary:

Change Password

##### Description:

Change Password

##### Responses

| Code | Description |
| ---- | ----------- |
| 404 | User not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /login-endpoints

#### GET
##### Summary:

Login Endpoints

##### Description:

login Endpoints

##### Responses

| Code | Description |
| ---- | ----------- |
| 404 | User not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /oauth2/authorize

#### GET
##### Summary:

Authorize

##### Description:

Authorize

##### Responses

| Code | Description |
| ---- | ----------- |
| 404 | User not found |
| 500 | Internal Server error |

### /oauth2/authorize/decision

#### POST
##### Summary:

Decision

##### Description:

Decision

##### Responses

| Code | Description |
| ---- | ----------- |
| 404 | User not found |
| 500 | Internal Server error |

### /oauth2/token

#### POST
##### Summary:

Token

##### Description:

Token

##### Responses

| Code | Description |
| ---- | ----------- |
| 404 | User not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /oauth2/.well-known/jwks.json

#### GET
##### Summary:

jwks json

##### Description:

jwks json

##### Responses

| Code | Description |
| ---- | ----------- |
| 404 | User not found |
| 500 | Internal Server error |

### /oauth2/access_token

#### GET
##### Summary:

Access Token

##### Description:

Access Token

##### Responses

| Code | Description |
| ---- | ----------- |
| 404 | User not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /oauth2/generateFFToken

#### POST
##### Summary:

Generate FFToken

##### Description:

Generate FFToken

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | generateFFToken successfully |
| 404 | User not found |
| 500 | Internal Server error |

### /getCustomAccessToken/{access_token}/{short_token}

#### GET
##### Summary:

Short Token

##### Description:

Short Token

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| short_token | path |  | Yes | string |
| access_token | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 404 | User not found |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /lti/loginhandler

#### POST
##### Summary:

Login Handler

##### Description:

Login Handler

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Success |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### /lti/callback

#### POST
##### Summary:

Call Back

##### Description:

Call Back

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| Authorization | header | Authorization token | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 201 | Success |
| 408 | Token expired or Invalid token |
| 500 | Internal Server error |

### Models


#### AuthRequest

| Name | Type | Description | Required |
| ---- | ---- | ----------- | -------- |
| client_id | string |  | Yes |
| client_secret | string |  | Yes |
| scope | string |  | Yes |
| state | string |  | Yes |
| code | string |  | Yes |
| email | string |  | Yes |
| password | string |  | Yes |
| confirmationCode | string |  | Yes |
| newPassword | string |  | Yes |
| confirmPassword | string |  | Yes |
| organizationName | string |  | Yes |
| ffToken | string |  | Yes |
| shortToken | string |  | Yes |
| first_name | string |  | Yes |
| last_name | string |  | Yes |
| clientToken | string |  | Yes |
| clientTokenType | string |  | Yes |
| reset_flag | boolean |  | Yes |
| organization | object |  | Yes |
| role | string |  | Yes |