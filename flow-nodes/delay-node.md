# Delay Node

This node can be used to add a wait time of x ms before processing to the next node in the graph. Delay nodes are great at forming a loop when checking a status of an endpoint.

Let's say you have a node that created a resource using POST request, the endpoint executes an asynchronous job and returns back a jobId.  You can use that jobId to check for status and if it's not a Success, add a delay and then check for status again. This loop keeps on executing until and unless status is Success or the graph run times out

<figure><img src="../.gitbook/assets/Screenshot 2024-04-17 at 5.06.23 PM.png" alt=""><figcaption></figcaption></figure>
