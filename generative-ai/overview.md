# Overview

One of the unique abilities of our product is the ablility to create runnable workflows from natural language.&#x20;

1. Select a flow from the sidebar or create a new flow.
2. Click `Generate` from the top right corner of the header.
3. This will show a popup box asking for the model\_name and description of your flow in natural language.

<figure><img src="../.gitbook/assets/Screenshot 2024-04-18 at 5.08.04 PM.png" alt="" width="375"><figcaption></figcaption></figure>

4. Currently we only support OpenAI, but we plan to integrate other models soon. Let us know if you want a specific model integrated.
5. Now head to the directory where you created your collection in your file system. Create a `.env` file and enter `OPENAI_APIKEY=<api_key_value>` . Once you do that you should start seeing that in the `Generate` pop up box if you select OPENAI as your choice of model.

<figure><img src="../.gitbook/assets/Screenshot 2024-04-15 at 9.32.50 PM.png" alt="" width="375"><figcaption></figcaption></figure>

6. Now that you have everything set, describe your flow, click `Generate` and you will soon see a series of nodes connected together to form a workflow. You can run the workflow, modify it by adding more logical nodes and finally save it for future use.
