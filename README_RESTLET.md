# Restlet fork

## Reasons for this fork

The version 2.7.4 of this module is not able to deserialize a JSON schema v3 with `type` attribute defined. According to the [specification](https://tools.ietf.org/html/draft-zyp-json-schema-03#section-5), it is perfectly correct.

The versions 2.7.3 and below contain a vulnerability that needs to be mitigated.

## When to delete this fork

When the deserialization of a JSON schema v3 with no attribute `type` works in a future version of Jackson.

The issue to track is: https://github.com/FasterXML/jackson-module-jsonSchema/pull/110

## How to delete

- Delete this repository
- Remove artifacts on our nexus
- Change back to official implementation of Jackson JSON schema module in:
  - API definitions
  - APISpark (for all packagings)
