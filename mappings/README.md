This folder contains information on cross-system data mappings required by NERIS.

## map_location.csv
Location elements are natively structured in NERIS to align with the [National Emergency Number Association (NENA)](https://www.nena.org/) [Civic Location Data Exchange Format (CLDXF)](https://cdn.ymaws.com/www.nena.org/resource/resmgr/standards/NENA-STA-004.2-2024_CLDXFUS_.pdf) standard. Recognizing that not all systems have implemented this standard, [map_location.csv](map_location.csv) gives guidance on where commonly used location (`Common Name`) elements should be submitted in the NERIS location structure. Additionally, mappings are given for ESRI and AWS geocoders.

## template__dispatch_code_to_incidenty_type.csv
Departments are responsible for maintaining a table of mappings from their dispatch codes to NERIS incident types. This is accomplished by uplaod of a spreadsheet via a file upload tool in the NERIS UI. [template__dispatch_code_to_incidenty_type.csv](template__dispatch_code_to_incidenty_type.csv) provides a template for the spreadsheet file.