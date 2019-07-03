# Case API
Version: v1
#### Base URL: /tieto/collection/casesvc

The case API fetches the list of all cases from Nova for a particular debtor. It exposes the basic and detailed case information and performs Nova case operations.


## API Endpoints Description

### `GET /debtors/{debtorNo}/cases`

Get the list of debtor cases with some basic information using Nova Debtor number.


#### Parameters

| Name | Type | Format | Required | In | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| debtorNo | integer | int32 | Yes | path | Nova debtor number |


#### Responses

| Status | Description |
| :--- | :--- |
| 200 | Returns the core case information (object_identifiers, state, registration and closed) for the specified Nova debtor number |
| 204 | No records found |
| 400 | Incorrect input parameters |
| 401 | Unauthorized request |
| 500 | The server encountered an error while processing the request |

### Models

<details>
  <summary>CaseDto - Case details</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

