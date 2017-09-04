# NLS-Collection
Nagios Log Server Collection 

A collection of add-ons for Nagios Log Server.

## Inputs
* Inputs allow Nagios Log Server to collect data from various sources like TCP/UDP ports, SNMP Traps, Unix Sockets, log files
* Each file in the Inputs folder is a separate input
  * The header of the file explains it's purpose
  * The remaining contents of the file are what needs to be pasted into a new input
  * Administration > Global Configuration > Inputs > Add Input

## Filters
* Filters are applied to input data before it is stored in the Elasticsearch Database
* This allows the data to be broken down into more granular fields, allows for a more detailed analysis of the data
* Each file in the Filters folder is a separate filter
  * The header of the file explains it's purpose
  * The remaining contents of the file are what needs to be pasted into a new filter
  * Administration > Global Configuration > Filters > Add Filter

## Outputs
* Outputs allow Nagios Log Server to perform actions on the received data afer the Inputs and Filters have been applied
* Each file in the Outputs folder is a separate input
  * The header of the file explains it's purpose
  * The remaining contents of the file are what needs to be pasted into a new output
  * Administration > Global Configuration > Show Outputs > Add Output

## Dashboards
* Dashboards are how you analyze the data in the Elasicsearch Database
* Each file in the Dashboards folder is a separate dashboard
* Dashboards usually rely on a filter that has defined specific fields
  * For example the Nagios dashboards rely on the Nagios_Core input filter
* The dashboard file needs to be uploaded so it can be used
  * Dashboards > Load (Folder icon) > Advanced > Browse
  * Once you upload a dashboard it needs to be saved using the Save As button

