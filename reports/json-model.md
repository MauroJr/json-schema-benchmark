# [`json-model`](https://github.com/geraintluff/json-model) - test summary

# All validators fail this test

`some languages do not distinguish between different types of numeric value, a float is not an integer even without fractional part`

# [`json-model`](https://github.com/geraintluff/json-model) failed tests

Some validators have deliberately chosen not to support parts of the spec. Go to the [`json-model`](https://github.com/geraintluff/json-model) homepage to learn if
that is the case for these tests.

|test failed|reason
|-----------|------
|`valid definition, valid definition schema`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://json-schema.org/draft-04/schema"}`)
|`invalid definition, invalid definition schema`|Expected result: `false` but validator returned: `true`
|`simple enum validation, something else is invalid`|Expected result: `false` but validator returned: `true`. **This excludes this validator from performance tests**
|`heterogeneous enum validation, something else is invalid`|Expected result: `false` but validator returned: `true`
|`heterogeneous enum validation, objects are deep compared`|Expected result: `false` but validator returned: `true`. **This excludes this validator from performance tests**
|`an array of schemas for items, incomplete array of items`|Expected result: `true` but validator returned: `false`
|`an array of schemas for items, empty array`|Expected result: `true` but validator returned: `false`
|`not, disallowed`|Expected result: `false` but validator returned: `true`. **This excludes this validator from performance tests**
|`not multiple types, mismatch`|Expected result: `false` but validator returned: `true`. **This excludes this validator from performance tests**
|`not multiple types, other mismatch`|Expected result: `false` but validator returned: `true`. **This excludes this validator from performance tests**
|`not more complex schema, mismatch`|Expected result: `false` but validator returned: `true`. **This excludes this validator from performance tests**
|`forbidden property, property present`|Expected result: `false` but validator returned: `true`. **This excludes this validator from performance tests**
|`ECMA 262 regex non-compliance, ECMA 262 has no support for \Z anchor from .NET`|Expected result: `false` but validator returned: `true`
|`validation of date-time strings, an invalid date-time string`|Expected result: `false` but validator returned: `true`
|`validation of date-time strings, only RFC3339 not all of ISO 8601 are valid`|Expected result: `false` but validator returned: `true`
|`validation of URIs, an invalid protocol-relative URI Reference`|Expected result: `false` but validator returned: `true`
|`validation of URIs, an invalid URI`|Expected result: `false` but validator returned: `true`
|`validation of URIs, an invalid URI though valid URI reference`|Expected result: `false` but validator returned: `true`
|`validation of e-mail addresses, an invalid e-mail address`|Expected result: `false` but validator returned: `true`
|`validation of IP addresses, an IP address with too many components`|Expected result: `false` but validator returned: `true`
|`validation of IP addresses, an IP address with out-of-range values`|Expected result: `false` but validator returned: `true`
|`validation of IP addresses, an IP address without 4 components`|Expected result: `false` but validator returned: `true`
|`validation of IP addresses, an IP address as an integer`|Expected result: `false` but validator returned: `true`
|`validation of IPv6 addresses, an IPv6 address with out-of-range values`|Expected result: `false` but validator returned: `true`
|`validation of IPv6 addresses, an IPv6 address with too many components`|Expected result: `false` but validator returned: `true`
|`validation of IPv6 addresses, an IPv6 address containing illegal characters`|Expected result: `false` but validator returned: `true`
|`validation of host names, a host name starting with an illegal character`|Expected result: `false` but validator returned: `true`
|`validation of host names, a host name containing illegal characters`|Expected result: `false` but validator returned: `true`
|`validation of host names, a host name with a component too long`|Expected result: `false` but validator returned: `true`
|`remote ref, containing refs itself, remote ref invalid`|Expected result: `false` but validator returned: `true`
|`Recursive references between schemas, valid tree`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://localhost:1234/node"}`)
|`Recursive references between schemas, invalid tree`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://localhost:1234/node"}`)
|`remote ref, remote ref valid`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://localhost:1234/integer.json"}`)
|`remote ref, remote ref invalid`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://localhost:1234/integer.json"}`)
|`fragment within remote ref, remote fragment valid`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://localhost:1234/subSchemas.json"}`)
|`fragment within remote ref, remote fragment invalid`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://localhost:1234/subSchemas.json"}`)
|`ref within remote ref, ref within ref invalid`|Expected result: `false` but validator returned: `true`
|`base URI change, base URI change ref valid`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://localhost:1234/folder/folderInteger.json"}`)
|`base URI change, base URI change ref invalid`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://localhost:1234/folder/folderInteger.json"}`)
|`base URI change - change folder, string is invalid`|Expected result: `false` but validator returned: `true`
|`base URI change - change folder in subschema, string is invalid`|Expected result: `false` but validator returned: `true`
|`root ref in remote ref, string is valid`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://localhost:1234/name.json"}`)
|`root ref in remote ref, null is valid`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://localhost:1234/name.json"}`)
|`root ref in remote ref, object is invalid`|The schema failed to load(`Requests not enabled - try JsonModel.setRequestFunction(func): {"method":"GET","url":"http://localhost:1234/name.json"}`)
|`uniqueItems validation, non-unique array of integers is invalid`|Expected result: `false` but validator returned: `true`
|`uniqueItems validation, numbers are unique if mathematically unequal`|Expected result: `false` but validator returned: `true`
|`uniqueItems validation, non-unique array of objects is invalid`|Expected result: `false` but validator returned: `true`
|`uniqueItems validation, non-unique array of nested objects is invalid`|Expected result: `false` but validator returned: `true`
|`uniqueItems validation, non-unique array of arrays is invalid`|Expected result: `false` but validator returned: `true`
|`uniqueItems validation, non-unique heterogeneous types are invalid`|Expected result: `false` but validator returned: `true`

**All other tests passed**.

[back to benchmarks](https://github.com/ebdrup/json-schema-benchmark)