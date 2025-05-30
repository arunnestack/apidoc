## Bank Accounts API
### GET
**Description:** Get list of bankaccountdetails
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/bankaccountdetails`
-  **Method:**  `GET`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/bankaccountdetails`

**Sample Response**
```json
[{"id":6604,"name":"Alka","accountNumber":"1234567890000","accountType":{"id":1,"code":"bankAccountType.savingsaccount","value":"Savings Account","systemCode":"SA"},"ifscCode":"AIRP0000001","mobileNumber":"","bankName":"Airtel Payments Bank","bankCity":"GURGOAN","status":{"id":200,"code":"bankAccountDetailsStatus.active","value":"active"},"branchName":"AIRTEL PAYMENTS BRANCH","isLocked":false,"verificationType":{"id":0,"code":"bankAccountVerificationType.invalid","value":"Invalid","systemCode":"invalid"},"verificationStatus":{"id":0,"code":"bankAccountVerificationStatus.invalid","value":"Invalid","systemCode":"invalid"},"isVerified":false,"createdDate":"Feb 26, 2025 11:17:29 AM","lastModifiedDate":"Feb 26, 2025 11:22:32 AM","useAsDefaultAccount":false,"bankAccountAssociationId":6671}]
```

### POST
**Description:** Create a bankaccountdetail
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/bankaccountdetails`
-  **Method:**  `POST`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/bankaccountdetails`
**Sample Payload**
```json
{"accountTypeId":1,"name":"Alka Verma","accountNumber":"0123456789","ifscCode":"AIRP0000001","bankName":"AIRTEL PAYMENTS BANK LIMITED","branchName":"AIRTEL PAYMENTS BRANCH","bankCity":"GURGOAN","locale":"en","dateFormat":"dd MMMM yyyy"}
```
**Sample Response**
```json
{"clientId":205,"resourceId":7883,"changes":{}}
```

### PUT
**Description:** Activate the bankaccount
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/bankaccountdetails/{documentID}/activate`
-  **Method:**  `PUT`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/bankaccountdetails/16965/activate`

**Sample Response**
```json
{"officeId":5,"clientId":205,"resourceId":16965}
```

### PUT
**Description:** Deactivate the bankaccount
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/bankaccountdetails/{documentID}/deactivate`
-  **Method:**  `PUT`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/bankaccountdetails/16965/deactivate`

**Sample Response**
```json
{"officeId":5,"clientId":205,"resourceId":16965}
```


### DELETE
**Description:** Delete a bankaccountdetail 
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/bankaccountdetails/{documentID}`
-  **Method:**  `DELETE`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/bankaccountdetails/16965`

**Sample Response**
```json
{"officeId":5,"clientId":205,"resourceId":16965}
```
