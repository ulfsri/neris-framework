## value sets

This metadata is a descriptive representation of the data elements that will be served by NERIS back to departments via the NERIS API. Accordingly, it does not represent 1-1 the data elements sent by a department and its vendors. 

- `active`
    - Boolean
    - Whether the value is still valid, and thus available for new data creation.
    - Must be populated for all fields.
- `value`
    - Text
    - CAPITAL_CASE-formatted representation of the value, as used in database ENUMs etc.
    - Must be populated for all fields.
- `description`
    - Text
    - The "real world" value, for use in the UI and other human-oriented applications.
    - Must be populated for all fields.