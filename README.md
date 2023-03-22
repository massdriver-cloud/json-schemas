# json-schemas

## Layout

Non-massdriver directories are for storing cloud definitions of fields/concepts, not our interpretations.

I.e.: K8s sees an ingress as multiple hosts, for our apps, its generally a single host.

The massdriver directory has two sub directories:

* properties: static json schemas of common concepts in MD. If your bundle derives from this common concept, $ref and update in your bundle

* controls: dhall wrappers around properties to build logic/controls around them. i.e. generate the json schema conditionals/dependencies/ifs around a particular field in a massdriver/properties schema
