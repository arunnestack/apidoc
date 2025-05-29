## Client Address API
### GET
**Description:** Get list of address
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/addresses`
-  **Method:**  `GET`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/addresses`

**Sample Response**
```json
[{"addressId":13112,"addressLineOne":"638Q+CGR, Tiruvannamalai, Tamil Nadu 606601, India","districtData":{"districtId":644,"stateId":35,"isoDistrictCode":"AI","districtName":"Tiruvannamalai","talukaDatas":[],"cityDatas":[],"isWorkflowEnabled":false,"status":{"id":300,"code":"districtStatus.active","value":"ACTIVE"},"activationDate":[2021,8,27],"isWorkflowArchived":false},"stateData":{"stateId":35,"countryId":101,"isoStateCode":"TN","stateName":"Tamil Nadu","districtDatas":[],"isUt":false},"countryData":{"countryId":101,"isoCountryCode":"IN","countryName":"India"},"postalCode":"606601","noOfYrsAtCurrentResidence":0,"latitude":0,"longitude":0,"addressEntityData":[{"id":13112,"addressId":13112,"addressType":{"id":13,"name":"Permanent Address","isActive":true,"mandatory":false},"entityId":205,"entityType":{"id":1,"code":"addressEntityType.clients","value":"CLIENTS"},"isActive":true}]}]
```

### POST
**Description:** Create an address
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/addresses`
-  **Method:**  `POST`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/addresses`
**Sample Payload**
```json
{"addresses":[{"countryId":101,"stateId":21,"districtId":65,"talukaId":4,"addressRegionValueId":4,"postalCode":"606601","locale":"en","dateFormat":"dd MMMM yyyy","addressTypes":[74]}]}
```
**Sample Response**
```json
{"clientId":205,"resourceId":16905,"changes":{"resourceIds":[16905]}}
```

### DELETE
**Description:** Delete an address 
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/addresses/{addressID}`
-  **Method:**  `DELETE`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/addresses/16905`

**Sample Response**
```json
{"clientId":205,"resourceId":16905,"changes":{"entityType":1,"action":"delete"}}
```
