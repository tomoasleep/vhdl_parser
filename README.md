VHDL Parser
===========

VHDL Parser is an VHDL entity parser. It's not a full grammar but simply
extracts port and generic information from a VHDL entity for further use
inside Ruby, e.g. visualization or automation.

Classes
=======
VHDL Parser provides three different classes 

* VHDL\_Parser::Entity
* VHDL\_Parser::Port
* VHDL\_Parser::Generic


Examples
========
     entity = VHDL_Parser.parse(some_vhdl_string)
     # get ports
     puts entity.ports
     # get generics
     puts entity.generics
     # print the whole entity
     puts entity

