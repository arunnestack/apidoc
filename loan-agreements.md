## Loan Agreement API

### POST
**Description:** Create a loan agreement
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/loanapplicationreferences/{loanApplicationID}/generated-documents/{documentName}`
-  **Method:**  `POST`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/loanapplicationreferences/25447/generated-documents/Sanction%20Letter`
  
**Sample Payload**
```json
{"loanAppId":"25447","generationKey":"Sanction Letter"}
```
**Sample Response**
```json
{"resourceId":12570,"resourceIdentifier":"12570"}
```

### GET
**Description:** Get loan agreement
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/loanapplicationreferences/{loanApplicationID}/generated-documents?generationKeys={documentName}`
-  **Method:**  `GET`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/loanapplicationreferences/25447/generated-documents?generationKeys=Sanction+Letter`

**Sample Response**
```json
[{"generationId":12570,"key":"Sanction Letter","displayName":"Sanction Letter","status":"SUCCESS","createdOn":1748596388000,"modifiedOn":1748596391000,"generatedDocument":{"id":91867,"parentEntityType":"loanapplication","parentEntityId":25447,"name":"Sanction Letter","fileName":"Sanction-Letter-2025-05-30-14-43-10.pdf","size":106273,"type":"application/pdf","reportIdentifier":0,"tagIdentifier":307,"tagValue":"Sanction Letter","status":{"id":1,"code":"INITIATED","value":"INITIATED"},"createdDate":1748596391000,"hasPassword":false},"type":"REPORT","tag":{"id":307,"name":"Sanction Letter","position":0,"description":"Sanction Letter","isActive":true,"codeScore":0,"mandatory":false}}]
```
