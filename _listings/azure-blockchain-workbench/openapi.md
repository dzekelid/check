swagger: "2.0"
x-collection-name: Azure Blockchain Workbench
x-complete: 1
info:
  title: Azure Blockchain Workbench REST API
  description: the-azure-blockchain-workbench-rest-api-is-a-workbench-extensibility-point-which-allows-developers-to-create-and-manage-blockchain-applications-manage-users-and-organizations-within-a-consortium-integrate-blockchain-applications-into-services-and-platforms-perform-transactions-on-a-blockchain-and-retrieve-transactional-and-contract-data-from-a-blockchain-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/checkers/checkApplication:
    post:
      summary: Post Checkers Check Application
      description: Checks if the supplied application configuration file is valid
        for Workbench.
      operationId: CheckApplicationPost
      x-api-path-slug: apiv1checkerscheckapplication-post
      parameters:
      - in: formData
        name: appFile
        description: Upload Application File
      responses:
        200:
          description: OK
      tags:
      - Checkers
      - Check
      - Application
  /api/v1/checkers/checkContractCode:
    post:
      summary: Post Checkers Check Contract Node
      description: Check if the application smart contract implementation file is
        valid for Workbench.
      operationId: CheckContractCodePost
      x-api-path-slug: apiv1checkerscheckcontractcode-post
      parameters:
      - in: formData
        name: appFile
        description: Upload Application File
      - in: formData
        name: contractFile
        description: Upload Contract Code File
      - in: query
        name: ledgerId
        description: The index of the chain type
      responses:
        200:
          description: OK
      tags:
      - Checkers
      - Check
      - Contract
      - Node
  /api/v1/capabilities:
    get:
      summary: Get Capabilities
      description: |-
        List all capabilities the user can perform within Workbench.
                     Checked capabilities include ability to add blockchain applications, add smart contract implementations,
                     add or edit user role assignments, and add new users.
      operationId: CapabilitiesGet
      x-api-path-slug: apiv1capabilities-get
      responses:
        200:
          description: OK
      tags:
      - Capabilities
  /api/v1/capabilities/canCreateContract/{workflowId}:
    get:
      summary: Get Capabilities Can Create Contract
      description: Checks if user has capability to create new smart contract instance
        for a specific workflow ID.
      operationId: CanCreateContract
      x-api-path-slug: apiv1capabilitiescancreatecontractworkflowid-get
      parameters:
      - in: path
        name: workflowId
        description: The id of the workflow
      responses:
        200:
          description: OK
      tags:
      - Capabilities
      - Can
      - Contract