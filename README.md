# NERIS Data Framework
This repository contains the data framework for the National Emergency Response Information System (NERIS). This includes the Entity Specification for Fire Departments, Dispatch (CAD) Data Schema, and the Incident Data Schema. The schemas are broken down into modules and value sets. Modules define the data elements (i.e., what is being asked) and value sets are choices users can select (i.e., the choices in the drop down). Two file formats are included for ease of use: csv and yml.

The framework is a set of descriptive representations of the data elements an end user would expect to see in the system regarding their department or one of its incidents.  Most will need to be directly submitted to NERIS by the department or its vendor, but not all will be. For example, the augmentation modules and fields for which `computed is True` will be added by the system, based on geographic location and other submitted data elements. There are also a number of data elements that are required by the system to properly relate data that are not shown in the data framework, notably most of the database keys. You can get a sense of most of these in the database ERDs in [the neris-framework wiki](https://github.com/ulfsri/neris-framework/wiki). 

## NERIS API
The API on the other hand is the actual mechanisms by which data interchange will happen with NERIS, and as such necessarily embodies all the requirements for data formats: cardinality, nullability/optionality, nesting/grouping, arrays vs scalars, etc. In the interest of remaining comprehensible for the non-developer audience there arecases in which the framework does not give full specificity on these dimensions. While they are pointed to in the `group` and `possible_if` fields, but one should rely on the API documentation. This is served in two formats, but contain the same information:
### Production
 - [Swagger](https://api.neris.fsri.org/v1/docs#/)
 - [Redoc](https://api.neris.fsri.org/v1/redoc)

### Test
 - [Swagger](https://api-test.neris.fsri.org/v1/docs#/)
 - [Redoc](https://api-test.neris.fsri.org/v1/redoc)


## Additional information
Additional information about the framework, including Entity Relationship Diagrams (ERDs) and module flow schematics, can be found in [this repo's wiki](https://github.com/ulfsri/neris-framework/wiki).

To ask a question, make a suggestion, or otherwise get help with the NERIS framework, please visit [the NERIS helpdesk](https://neris.atlassian.net/servicedesk/customer/portals).

Also, be sure check out the [Discussions on all things NERIS development here in GitHub](https://github.com/ulfsri/neris-framework/discussions)
