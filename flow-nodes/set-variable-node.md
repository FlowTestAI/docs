# Set Variable Node

This node is used to create a GLOBAL variable and assign it a value.

The value assigned can be of type -&#x20;

* **Select** - Selects a part of the output from the previous node. For instance previous node is request node that outputs `{ "id": 10, "category" : [ {"id" : 10, "status" : "available"} ], .....}` , then you can use `id` or `category.0.id` to assign value to the variable. The actual values will be calculated on the fly when the graph is run.
* **String** - Assigns a value of type string to the variable. &#x20;
* **Number** - Assigns a value of type number to the variable.&#x20;
* **Boolean** - Assigns a value of type boolean to the variable. &#x20;
* **Now** - Assigns a value of type now() epoch timestamp to the variable. The value of now() is calculated on the fly during graph run. &#x20;
* **Expression** - You can compute an expression on the fly to assign value to this variable. For instance , create a variable `startTime` that is assigned `now() - 3minutes`

<figure><img src="../.gitbook/assets/Screenshot 2024-04-17 at 10.06.20 PM.png" alt="" width="375"><figcaption></figcaption></figure>

