# A demo of using prism to mock an API endpoint

Run with the modified swagger doc in the project
```
$ prism mock petstore-expanded.yaml -h 0.0.0.0
```

Example with the raw unmidified swagger doc
```
$ prism mock https://raw.githack.com/OAI/OpenAPI-Specification/master/examples/v3.0/petstore-expanded.yaml
```

The `-h 0.0.0.0` flag in needed when deploying to docker because the default `mock` command binds to `localhost` and localhost can not be accessed outside the container.


### References

- example swagger doc https://raw.githack.com/OAI/OpenAPI-Specification/master/examples/v3.0/petstore-expanded.yaml
- prism https://stoplight.io/open-source/prism/
- prism guthub page https://github.com/stoplightio/prism#-documentation-and-community
- Book I learned about this from https://www.manning.com/books/designing-apis-with-swagger-and-openapi
