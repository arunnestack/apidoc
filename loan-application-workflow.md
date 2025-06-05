## Loan Application Workflow

### POST 
**Description:** Initiate the credit bureau
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/enquiry/creditbureau/loanapplication/{loanApplicationID}/initiate`
-  **Method:**  `POST`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/enquiry/creditbureau/loanapplication/25643/initiate`
**Sample Payload**
```json
{"entityType":"loanapplication","entityId":"25643","isForce":false}
```
**Sample Response**
```json
{"cbStatus":{"id":3,"code":"SUCCESS","value":"SUCCESS"},"reportFileType":{"id":1,"code":"report.html","value":"HTML"},"totalAmountBorrowed":0,"totalCurrentOutstanding":0,"totalAmtOverdue":0,"totalInstallmentAmount":0,"cbInitiatedDateTime":"01-June-2025 13:56:46","errors":[{"code":"00","description":"Consumer record not found"}],"creditBureauEnquiryId":24191,"cbReportOrderNo":"10011294719"}
```
