# Zabbix Template Solr statistics
Template for monitoring Solr using JSON statistics.

# Versions
I tested this using zabbix 5.0.9 and Solr 8.6.3, but maybe it works with different versions.

# Requirements
Zabbix version > 4.2 because template is using HTTP agent and JSON Path. 
You need to setup user and password for accessing Solr statistics JSON:
http://{USERNAME}@{PASSWORD}:{HOSTNAME}/solr/admin/metrics

# Installation
* Download Zabbix template
  * https://raw.githubusercontent.com/felipemvieira/zbx-solr-template/main/Template_App_Solr.xml
* Import the template on Zabbix
* Create host on Zabbix and apply the template
* On host configuration, modify macros {$SOLR_USERNAME} and {$SOLR_PASSWORD} with the information you created.
