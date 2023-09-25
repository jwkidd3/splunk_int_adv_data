# splunk_int_adv_data

# Splunk Int/Adv

## Data Load
There are 4 indexes in this class: web, security, sales and network <br>

Load based on table below:

| Index |   Type |                    SourceType  |      host(s)    |    Source (File)			 |
| ----- | ------ | -------------------------------| -------------| ----------------------|
| Web		| Online Sales |		          access_combined	|	segment in path 2|		access.zip   |
| Security|	   Web Server		|            linux_secure	 |	  segment in path 2	|	secure.zip  |
| Sales		 |    sales_entries |		        sales_entries |		  appserver |		sample_sales_entries_data.json  |
| Sales		 |    retail_sales	|	          vendor_sales	|	  appserver |		vendor_sales.log  |
| Network	|	   Web Security Appliance |	  cisco_wsa_squid |		webserver |		sample_cisco_wsa_sqid_data.json  |
| Network	|	   firewall_data	|	        cisco_firewall |		firewall	|	sample_cisco_firewall_data.json  |


3. Before exercises can be done walk students through creating auto lookups for the following:
   | SourceType|Lookup File|LookupId|
   |-----------|-----------|--------|
   |access_combined*|products.csv|productId|
   |vendor_sales|products.csv|Code|
   |vendor_sales|vendors.csv|VendorID|


   *** NOTE: on all exercises and demos you may have to adjust timeframe to see data depending on when the last time data generation took place

   *** Remember, this is not a production environment. The UI for splunk changes on a semi regular basis and sometimes screenshots do not 100% match the product. Data for labs should be consistent but there are cicurmstanses where we will need to adapt an exercise based on data availability.
