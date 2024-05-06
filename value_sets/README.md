## value sets

This metadata is a descriptive representation of the data elements in NERIS value sets. Value sets serve as the pre-populated list from which users choose the most appropriate response. 

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