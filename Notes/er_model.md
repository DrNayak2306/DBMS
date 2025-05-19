# ER Model

[Example](https://github.com/DrNayak2306/DBMS_OOP/blob/main/er_diagram.png)  
[Symbols](https://github.com/DrNayak2306/DBMS_OOP/blob/main/er_diagram_symbols.png)  
[Ternary relationship](https://github.com/DrNayak2306/DBMS_OOP/blob/main/ternary_relationship.png)  
[Weak entity relationship](https://github.com/DrNayak2306/DBMS_OOP/blob/main/weak_entity_relation.png)

**Entity** - Real world object distinguishable from others. BOX  
**Attribute** - A property of the entity. ELLIPSE  
**Domain** - Permissible values of an attribute.  
**Primary key** - A uniquely identifying attribute of the entity.  
**Entity set** - Set of entities sharing the same type, and set of attributes.  
**Relationship** - how one entity interacts with another. RHOMBUS  

## Types of attributes
**Simple** - Indivisible (e.g. ID.)  
**Composite** - Can be divided into simpler parts (e.g. address, name.)  
**Single-valued** - Can contain only a single value (e.g. ID.)  
**Multi-valued** - Can have multiple values (e.g. phone no., nominee name.) CONCENTRIC ELLIPSE  
**Derived** - Obtained from related attributes (e.g. age from DOB.) DOTTED

## Strong entity
Has independent existence (i.e. can be uniquely identified by a primary key)

## Weak entity
Has dependent existence (i.e. lacks a primary key and depends on a strong entity)  
e.g. loan is strong, payment is weak because although payment can have an ID, it is just for serialization.

## Types of relations
**Unary** - EMP manages EMP  
**Binary** - STUDENT enrolls in COURSE  
**Ternary** - EMP works in BRANCH as JOB  

## Cardinality - No. of entities linked to an entity via a relationship
1:1 - CITIZEN has AADHAAR  
1:N - CITIZEN has VEHICLE  
N:1 - COURSE taken by INSTRUCTOR  
N:N - CUSTOMER buys PRODUCT  

Participation constraints (minimum cardinality constraint)  
Partial participation - An entity in the set may or may not have any relationship with the other end. SINGLE LINE  
Total participation - Every entity in the set has at least one relationship with other end. DOUBLE LINE  

Weak entity has total participation, strong has partial participation.