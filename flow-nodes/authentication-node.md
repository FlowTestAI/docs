# Authentication Node

Authentication node is used to define authentication to be used by successive API request nodes. Currently we support basic authentication using `Username` and `Password` but we plan to add more types of authentication.

Authentication is global during graph run, once you define an authentication, all successive request nodes will use that, you can add as many authentication nodes in the same graph to define different set of authentication parameters.
