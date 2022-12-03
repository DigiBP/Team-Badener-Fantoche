## How to configure Make to send requests from a Google form

1. Add Google form connector (you have to create a Google spreadsheet associated with the form)
2. Add HTTP request connector
3. Configure the HTTP connector as follows:
- URL: `https://digibp.herokuapp.com/engine-rest/process-definition/key/Price/tenant-id/fantoche/start`, where **Price** is the Process ID of the bpmn (you can find that in the XML) and **fantoche** is the tenant ID
- Method: **POST**, because we want to send some data to the destination
- Body type: **RAW**
- Content type: **JSON**
- Request content ```{
 "variables":{
   "testtype" : {
     "value" : "...",
     "type": "String"}
	}
}``` where the **...** corresponds to the field of the test we want the lab to perform. In Make you can select this value to come from the Google spreadsheet.

4. Save. Submit a form and then click on Run Once.
