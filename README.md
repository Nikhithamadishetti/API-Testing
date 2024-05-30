Gorest API Chaining
﻿

Authorization
Bearer Token
Token
<token>
POST
New Request
https://gorest.co.in/public/v2/users
The endpoint makes an HTTP POST request to create a new user at the specified URL. The request body should contain the user's name, gender, email, and status. The name and email are expected to be provided as variables ({{username}} and {{useremail}}).

Response
The response to the request is in JSON format with a status code of 401. The response body includes a "message" field, which is expected to contain a message related to the unauthorized access. Below is the JSON schema representing the response:

JSON
{
    "type": "object",
    "properties": {
        "message": {
            "type": "string"
        }
    }
}
﻿

Authorization
Bearer Token
This request is using an authorization helper from collection Gorest API Chaining
Body
raw (json)
json
    {
        "name": "{{user_name}}",
        "email": "{{user_email}}",
        "gender": "female",
        "status": "inactive"
    }

    
GET
Get User details
https://gorest.co.in/public/v2/users/
﻿

Authorization
Bearer Token
This request is using an authorization helper from collection Gorest API Chaining
DELETE
delete user
https://gorest.co.in/public/v2/users/
﻿

Authorization
Bearer Token
This request is using an authorization helper from collection Gorest API Chaining
