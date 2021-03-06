=================
Schema validation
=================

CityJSON schema download
------------------------

version 0.5: 
- :download:`download cityjson-v05.schema.json <../schema/cityjson-v03.schema.json>`

version 0.3: 
- :download:`download cityjson-v03.schema.json <../schema/cityjson-v03.schema.json>`

version 0.2: 
- :download:`download cityjson-v02.schema.json <../schema/cityjson-v02.schema.json>`

version 0.1:
- :download:`download cityjson-v01.schema.json <../schema/cityjson-v01.schema.json>`


Software to validate a file against the schema
----------------------------------------------

`cjvalschema <https://github.com/tudelft3d/cityjson/tree/master/software/cjvalschema/c%2B%2B11>`_ validates a CityJSON against the schema and does extra validation, eg:

- are the attributes of City Objects and metadata according to CityGML?
- do the BuildingParts have a parent Building?
- do the BuildingInstallation have a parent Building?
- are the arrays for the boundaries and the semantics coherent? (same structure)
- are there duplicate keys (IDs) for the City Objects? If yes then an error is returned.

Errors and warnings are returned to the user.

`JSON Schema <https://json-schema.org>`_ is used to validate.

