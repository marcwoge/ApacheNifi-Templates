# ApacheNifi Templates
 Templates for Apache Nifi

## Timebuzzer
Template used with the SAAS Timebuzzer (https://timebuzzer.com/) 
Everyday (0:00) Connects to API, requests Userdata and performs a request for every userID grapping Activities for the last four weeks. 
Everyday (23:00) connects to API and asks for Tiles.
All Data is stored in MySQL and for debugging purposes FlowFiles are written to Disk. 
In cases of errors FlowFiles are put into Funnels and need to be reused manually.

Requires Group variable: API_key to be set with the API Key provided from Timebuzzer (Settings/API) looks like: 
"APIKey azkxs234ftdsh.1234ojsnfgdl21ßsadfgnsdklmfbv" (littel bit longer)
Requires MySQL Connection

