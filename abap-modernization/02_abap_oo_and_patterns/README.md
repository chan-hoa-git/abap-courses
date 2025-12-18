# 02 – ABAP OO et Patterns

- Singleton, Factory, Strategy
- Encapsulation, Interfaces
- Exemple de “Hello Service” pour préparer RAP
  
Exemple code – Factory Pattern simplifié

INTERFACE zm_if_greeter.

  METHODS greet RETURNING VALUE(rv_text) TYPE string.
  
ENDINTERFACE.

CLASS zm_cl_greeter DEFINITION.

  PUBLIC SECTION.
  
    INTERFACES zm_if_greeter.
    
ENDCLASS.

CLASS zm_cl_greeter IMPLEMENTATION.

  METHOD zm_if_greeter~greet.
  
    rv_text = 'Hello Pattern ABAP Modern';
    
  ENDMETHOD.
  
ENDCLASS.
