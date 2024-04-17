# Request Node

You can use a request node to execute a GET, POST, PUT and DELETE  request with proper request body and parameters.

Anything within double curly braces `{{ }}` is treated as a variable. Each request node takes two types of variables -&#x20;

### Pre-Request

These are the set of variables LOCAL to an API request and can be used by the API request before it fires. For Instance, you can define your url as `https://petstore3.swagger.io/api/v3/pet/{{petId}}` and then define a pre-request variable as shown below.

&#x20;A variable can of the following type -&#x20;

1. **Select** - Selects a part of the output from the previous node. For instance previous node is request node that outputs `{ "id": 10, "category" : [ {"id" : 10, "status" : "available"} ], .....}` , then you can use `petId = id` or `petId = category.0.id` The actual values will be calculated on the fly when the graph is run.
2. **String** - Assigns a value of type string to the variable.   `petId = "10"`
3. **Number** - Assigns a value of type number to the variable.   `petId = 10`
4. **Boolean** - Assigns a value of type boolean to the variable.   `petId = false`
5. **Now** - Assigns a value of type now() epoch timestamp to the variable. The value of now() is calculated on the fly during graph run.   `petId = Date.now()`

<figure><img src="../.gitbook/assets/Screenshot 2024-04-17 at 4.21.04 PM.png" alt=""><figcaption></figcaption></figure>

### Post-Response

Post response variables are GLOBAL and can be referenced by other downstream nodes. These are variables that are created after an API request has fired. One of the big advantages of these types of variable is that you can create a variable and assign it a value extracted from the response of an API request. For instance if the one node fired an API request, you can create a variable, assign it a value selected from it's response and use that in next node.

_If a node has a pre-request variable defined of the same name as post response variable of a previous node, it will take more precedence._

<figure><img src="../.gitbook/assets/Screenshot 2024-04-17 at 4.21.26 PM.png" alt=""><figcaption></figcaption></figure>

