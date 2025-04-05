# REST

## Beispiel APIs

### Nominatim

> [API-Dokumentation](https://nominatim.org/release-docs/develop/api/Search/)

„Free-form query“ mit `q=`
* [https://nominatim.openstreetmap.org/search?format=json&q=dresden](https://nominatim.openstreetmap.org/search?format=json&q=dresden)

„Structured query“ mit `city=` und optional `countrycodes=`
* [https://nominatim.openstreetmap.org/search?format=json&city=dresden&countrycodes=de](https://nominatim.openstreetmap.org/search?format=json&city=dresden&countrycodes=de)

Mit `format=xml`
* [https://nominatim.openstreetmap.org/search?format=xml&city=dresden&countrycodes=de](https://nominatim.openstreetmap.org/search?format=xml&city=dresden&countrycodes=de)

Ohne `format=`
* [https://nominatim.openstreetmap.org/search?city=dresden&countrycodes=de](https://nominatim.openstreetmap.org/search?city=dresden&countrycodes=de)


### [Swagger Petstore](https://petstore.swagger.io/)


## Beispiel Code

* [Node-RED](nodered.md)
* Python: [./examples/rest/python/](./examples/rest/python/)
