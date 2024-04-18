# Complex Node

This is the most interesting node in my opinion.

One can imagine each flow as a utility/function that can be referenced by other flows.

For Instance, let's say my I have a workflow 1 that takes a user's query, sends it to an llm to get some output. Now we want to check if the llm output does not contain too strong of a language or does not contain some profanity. Now we can create another workflow 2 that does this checking and we can refer that in workflow 1 via a complex node.
