---
layout: function
generate: false
typeInfo:
    namespace: ThorsAnvil::Serialize
    header:    ThorSerialize/YamlThor.h
    function:  yamlExport
    description: 
    template:  template<typename T> 
    return:
        type: 'Exporter<Yaml, T>'
        description: 'Object that can be passed to operator<< for serialization.'
    parameters:
        - name: value
          type: 'T const&'
          default: 
          description: 'The object to be serialized.'
        - name: characteristics
          type: 'PrinterInterface::OutputType'
          default:  PrinterInterface::OutputType::Default
          description: 'Default: is verbose and logical. Stream: remove all white space.'
        - name: catchExceptions
          type: 'bool'
          default:  false 
          description: 
children: []
---
