# RE-ITSM
Robotic Enterprise ITSM framework

This is an extended framework for the ITSM process. ITSM platforms deals with huge number of incidents/Requests in a day. Most of the cases are repeated and manual process which can be automated to reduce cost, faster turnaround, avoid human errors and adhere to SLAs

ITSM framework follows the below process,

1. Init  
2. Get Incident Data (WebAPI, Orchestrator queues etc..)
3. Analyze the incident and categorize into 3 categories (Pending, Manual and Auto)
4. Auto - Incident will be processed and details updated to ITSM patform. Status - Closed
5. Pending - In case of missing information to categorize or process automatically. Status - Pending
6. Manual - Set in case of any Business errors.
7. Other the System Error, process goes to the next Incident in the queue.
