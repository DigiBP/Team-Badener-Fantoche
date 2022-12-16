# Team-Badener-Fantoche
### Team Members 
- Kui Hong Lim (Charlene) 
- Nino Bachmann
- Paul Tanner
- Sergio Guarino     

### Topic: Clinical Laboratories

### Abstract:
This project will focus on the automation and service optimisation of the clinical laboratory. Receiving patient samples from the customer (i.e. a doctor) and providing the results in a report will be the primary service of our model. We will also integrate supporting processes such as invoicing, testing and sample handling. 

### Scenario:
The laboratory process starts with a **Blood Sample Registration** order being received. The laboratory conducts the following tests:

| Number | Test Type               |
|:------:|:-----------------------:|
| 1.     | Pregnancy Test          |
| 2.     | STD Test                |
| 3.     | Blood Type Test         |
| 4.     | White Blood Cell Count  | 

The admin will check and approve the order requests before processing the request to examination. The lab researchers will then run the lab analysis on the sample. The examination results in a diagnostic interpretation which needs to be validated by a physician. The physician will request a rexamination from the lab team if the he/she feels that the analysis is invalid. There is a limit of 3 rexaminations request and if the physician is still not satisfied, the customer will be informed that more samples are required. The diagnostic interpretation that has been validated by the physician shall proceed to the next process. An analysis report shall be generated in parallel with the invoice generated automatically from the price list. The report and invoice will be sent to the customer. All samples and financial data will be stored securely in the lab CRM data storage.  

| Process Role | Group Type | Tasklist |
|:------------:|:----------:|:--------:|
| Engineer     | Engineer   | READ, START |
| Lab researcher | Initiator | READ, START |
| Physician | Physician | READ  |
| Accounting | Accounting | READ |
| Customer | Customer   | READ  |


