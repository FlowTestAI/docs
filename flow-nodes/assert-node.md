# Assert Node

An assert node can be used to define a condition and then whether that condition is true or false, one can define two different paths in the flow. An assert node takes two variables and an operator.

## Variables

Each variable can be of the following type -&#x20;

* **Select** - Selects a part of the output from the previous node. For instance previous node is request node that outputs `{ "id": 10, "category" : [ {"id" : 10, "status" : "available"} ], .....}` , then you can use `id` or `category.0.id`  to assign value to the variable. The actual values will be calculated on the fly when the graph is run.
* **String** - Assigns a value of type string to the variable. &#x20;
* **Number** - Assigns a value of type number to the variable.&#x20;
* **Boolean** - Assigns a value of type boolean to the variable. &#x20;
* **Now** - Assigns a value of type now() epoch timestamp to the variable. The value of now() is calculated on the fly during graph run.&#x20;
* **Variable** - You can reference any other variable from the set of global variables defined in the workflow.

<figure><img src="../.gitbook/assets/Screenshot 2024-04-17 at 4.52.45 PM.png" alt=""><figcaption></figcaption></figure>

## Operator

Currently we support `isEqualTo, isNotEqualTo, isGreaterThan, isLessThan` but feel free to contribute other types of operators.
