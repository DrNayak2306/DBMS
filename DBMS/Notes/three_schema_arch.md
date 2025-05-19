# Three schema architecture

## Physical level
Aimed at efficiency of computations.

## Logical level
Semantics of data - what data and relationships between them.  
Most relevant for programmers designing end user applications.

## View level
Subschema for each group of users.

## Instance
The collection of information present in the DB at a particular moment.

## Data models
DB design at logical level.  
A set of conceptual tools for describing data, data relationships, semantics and consistency constraints.

DDL defines database schema.  
DML defines retrieval, insertion, deletion and updation logics.

JDBC - Java API  
ODBC - C/C++ API

Database administrator (DBA) Has central control of DBMS
## Functions of DBA:
1. Schema definition
2. Schema and physical organization modifications
3. Authorization control
4. Routine maintenance - periodic backups, security patches, upgrades

## DBMS application architecture

### Tier 1
client, server, DB all in one computer.  
Useful for self service applications.

### Tier 2
client ---API---> server (DB)  
Useful for office purposes.

### Tier 3
client ---API---> app server ---API---> DB  
Scalable and used for large applications like WWW.  
Higher security and integrity since no direct contact between client and DB.