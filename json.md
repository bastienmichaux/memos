# JSON

- MIME: `application/json`
- uniform type identifier: public.json
- top-most object is a POJO: {}
- null is authorized
- undefined isn't authorized
- forbidden too: NaN, Infinity, octal & hexadecimal formats
- strings: beware some characters must be escaped

JSON Schema: validation libraries:
- c: WJElement
- Java: json-schema-validator
- .NET: Json.NET
- Haskell: aeson-schema
- python: jsonschema
- ruby: autoparse, ruby-jsonschema
- php: php-json-schema, json-schema
- js: many... schema.js, json-schema
