# Getting Started

FlowTestAI stands as the world’s first GenAI powered OpenSource Integrated Development Environment (IDE) specifically designed to craft, visualize, and manage API-driven workflows. Characterized by its speed, lightweight architecture, and local operation, FlowTestAI safeguards privacy while facilitating the seamless integration of API driven workflows.

<figure><img src="https://lh7-us.googleusercontent.com/WVPX9JB0YGWLdbCG_tO0IKGvolHsizLQdmUmFD_oh-HzKhszenjYzJ14kakwfWxpYqIy6eLQZwXTjnIi6jMOHlVqWBqjCvR_Vxl17nzBN6Kg5jY17jpa01aQBkyiUPHHFRLFlgB_x0IGhCF-LY0GKFU" alt=""><figcaption></figcaption></figure>

## Installation

With a developer first approach in mind, we have designed FlowTestAI to offer an experience of an IDE just like VS Code, Intellij etc. Every operation that you perform inside FlowTestAI is local to your file system keeping privacy at the forefront.

Download the latest release

| Platform | Binary         |
| -------- | -------------- |
| MacOs    |                |
| Windows  | Coming Soon... |
| Linux    | Coming Soon... |

## Import

&#x20;\* Currently we require an OpenAPI spec to import/open a collection. Very soon we will allow operations without it too.&#x20;

1. Click Import
2. Select an OpenAPI spec. You can download a sample petstore OpenAPI spec from [here](https://github.com/swagger-api/swagger-petstore/blob/master/src/main/resources/openapi.yaml).
3. Select directory where you want to store your collection.
4. You will see a directory created with the name of the OpenAPI spec title at the location you chose in step 3.

## Create your first Flow

1. After importing an OpenAPI spec, you will see an entry by the name of the OpenAPI spec title in the IDE sidebar.
2. Click the kebab menu icon to the right of it, you can now created nested folder structure or a new flow all of which will be replicated to your local system.&#x20;
3. Click create new flow, enter a name and click create. You should see a new tab with the flow name opened with a fresh canvas.&#x20;
4. At the bottom right corner, you will see a :heavy\_plus\_sign: button. Click it and it will display all the possible logical nodes that you can drag and drop onto the canvas.
5. To know more about each of the nodes, refer to the [flow-nodes](../flow-nodes/ "mention") section.
6. Instead of manual drag and drop, one can also use [generative-ai.md](../generative-ai.md "mention") to create a flow using natural language. For that refer to [this](../generative-ai.md) section for step by step instruction.
