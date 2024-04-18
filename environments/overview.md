# Overview

An environment is a set of one or more variables that you can reference when designing workflows. Environments help you segregate different variable values for different context. For instance you might  have a variable `{{baseUrl}}` being used in a workflow that has one value for a staging environment but a different value for production environment. All the variables referenced in the current workflow take their values from the selected environment (until and unless they are defined using other means. See [request-node.md](../flow-nodes/request-node.md "mention") and  [set-variable-node.md](../flow-nodes/set-variable-node.md "mention") for other ways to define variables)

## Create an environment

1. Select `Environments` from the sidebar
2. Click the kebab menu icon and select create new environment.
3. Enter the name of the new environment and you should see it in the sidebar when created.

<figure><img src="../.gitbook/assets/Screenshot 2024-04-17 at 10.24.46 PM.png" alt=""><figcaption></figcaption></figure>

## Add environment variables

1. Select an environment from the sidebar that you wish to edit.
2. Once the selected environment tab is open, select `Add Variable` , enter key and value pair.
3. After adding click save in the top right corner to start using the added variables.
4. Each added environment variable is displayed in a list that you can remove/delete using the delete icon.

<figure><img src="../.gitbook/assets/Screenshot 2024-04-17 at 10.28.04 PM.png" alt=""><figcaption></figcaption></figure>

## Switch between environments

Select any workflow, then from the top right corner select `Select environment`. It will display a drop down list of all available environments. Choose any one of them to starting using it's set of variables.

<figure><img src="../.gitbook/assets/Screenshot 2024-04-17 at 10.30.23 PM.png" alt="" width="312"><figcaption></figcaption></figure>
