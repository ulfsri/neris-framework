## value sets

This metadata is a descriptive representation of the data elements in NERIS value sets. Value sets serve as the pre-populated list exists from which users choose the most appropriate response. 

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
- `definition`
    - Text
    - Potentially longer-form definition of the value.
    - Must be populated for all fields.
- `source`
    - Text
    - The third party source from which the value was replicated.
    - Must be populated for all fields.
- `xor`
    - Text
    - For value sets in which one or more values control the logical possibility of other data elements, this defines the logical group into which a value falls. 
    - Must be populated for all fields.
    