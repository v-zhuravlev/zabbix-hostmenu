# zabbix-hostmenu  

Frontend JS patch that allows to add additional External or internal URLs to Host Menu everywhere in the Zabbix Frontend  
Work in progress..  

## Features  

1. Use host's `URL_A`, `URL_B`, `URL_C` Inventory fields    
2. Macros {HOST.ID}, {HOST.HOST}, {HOST.NAME}, {HOST.CONN} and {INTENVORY.*} can be used in URLs  
3. Add a name to URL link like so: `Google|http://google.com`  


## TODO  
1. Make sure that {HOST.IP} and {HOST.CONN} always return main interface   
2. Remove possible race condition for RPC object  
3. Extend functionality to Map context menu  


## Example  
1. Fill in inventory fiels:  
![image](https://cloud.githubusercontent.com/assets/14870891/21094122/6764a7d2-c066-11e6-805c-6941181ce078.png)  

2. Use it on the Dashboard or anywhere else (except for map):  
![image](https://cloud.githubusercontent.com/assets/14870891/21094249/21254190-c067-11e6-944c-c252dd8d177f.png)  

3. Hosts without URL_*  inventory fields stay clean:
![image](https://cloud.githubusercontent.com/assets/14870891/21094290/5dd4f8d8-c067-11e6-8015-9263551803d5.png)  


## Known issues  


## More info and help  
You may vote for this kind of functionality included in Zabbix itself if you found this useful:
https://support.zabbix.com/browse/ZBXNEXT-3496
