refer official link: http://avro.apache.org/docs/current/gettingstartedjava.html
# avro-maven-plugin
Generate code avro serializer and deserializer using maven plugin
Some info for performance improvement:
1. Avro objects can be created either by invoking a constructor directly or by using a builder. Unlike constructors, builders will automatically set any default values specified in the schema. Additionally, builders validate the data as it set, whereas objects constructed directly will not cause an error until the object is serialized. However, using constructors directly generally offers better performance, as builders create a copy of the datastructure before it is written.
