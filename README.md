## feature-schema

feature-schema defines XML schemata for
[FeatureIDE](https://featureide.github.io) feature models and configurations.

[Click here](https://ekuiter.github.io/feature-schema) for an online
demonstration. You can validate any FeatureIDE feature model or configuration
there.

### Intention

FeatureIDE has XML formats for feature models and configurations in its source
code, but there is no proper documentation or specification of these formats.

This project consists of XML schemata written in XSD which specify these XML
formats. They are useful for validating XML documents, but they also serve as
documentation for generating a valid XML document.

### Usage

When parsing an XML document, point your validator to the
**[configuration.xsd](https://raw.githubusercontent.com/ekuiter/feature-schema/master/configuration.xsd)**
or
**[model.xsd](https://raw.githubusercontent.com/ekuiter/feature-schema/master/model.xsd)**
file. To try it out, [click here](https://ekuiter.github.io/feature-schema).

- `configuration.xsd` is modeled after FeatureIDE's
[XMLConfFormat](https://github.com/FeatureIDE/FeatureIDE/blob/develop/plugins/de.ovgu.featureide.fm.core/src/de/ovgu/featureide/fm/core/configuration/XMLConfFormat.java).
- `model.xsd` is modeled after FeatureIDE's
[XmlFeatureModelFormat](https://github.com/FeatureIDE/FeatureIDE/blob/develop/plugins/de.ovgu.featureide.fm.core/src/de/ovgu/featureide/fm/core/io/xml/XmlFeatureModelFormat.java)
(only `struct` and `constraints` are validated).

### License

This project is released under the [LGPL v3 license](LICENSE.txt).