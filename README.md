# analytical-engineer-course

# ELT
# T in ETL

# Transformation:
- Cleansing: Solving and cleaning out any inconsistency
- Standardization: By applying formatting rules
- Deduplication: Removing duplicates and redduncy
- Verification: Flagging anomalies and remove unusable data
- Sorting: Organizing by type
- Other Task: Any other rules/tasks needed to apply


Tools: Airflow, Fivetran

# Advantages of ELT
- More flexibility than ETL approach, stores any type of data
- Enables to perform analysis on various data types with ease
- Ensures architecture future proof due to the data lake habdling data growth
- No longer requires DE to setup complicated pipelines
- Data access security happens within data warehouse

# Advantages of ELT
- More data storage space required
- Could be slow due to muilti persistent of data
- Low compliance due to everything stored
- Security risk if not handled PII data correctly
- Fairly new technology due to popularity in cloud solutions

---
# DATA MODELLING & ERD NOTATION
* Data Model:
   - Foundation to building DWH & BI solutions
   - Primary goal of the data model is to act as a blueprint
   - Helps buidling conceptual, logic, physical and models and define relatiosnhips
   - Defines how the logical structure of database is modeled
   - Specifies business requirements and data structure
   - Provides visual way to communicate with business at various level
   - Data Model is important part of the developement process(main communication methid between team)

* Data Modelling
   - Data modeling is the process itself
   - identifying and anylyse business requiremennts
   - Work with business on defining the dta model
       - Interview, meetings, reviewing existing process
   - Define ERD notation style
      - Information Engineering(IE), Chen's Style, Barker UML
   - Define the model type
      - Conceptual, Logic, Physical
   - Define Data Modelling Methodology
      - Relational data Models (ER data model)
      - Dimension Model

* ERD Notation
   - Creates a visual representation of the entities and the attributes
   - Provides a preview of how all  the tables should connect, what fields are going to be on each table
   - Puts forth the conceptual ideas in a readable format
   - ER diagrams used as  a blueprint for implementation

* Entity, Attributes Relationship
  - Entity: is a class of objects represented by a rectangle. This can be something that exists in the real world logically, physically or conceptually. Such as person, customer, employee, product, transaction, account.
 
  - Attributes are properties that describe an entity(for customer it'll be name, email, address etc
        - IE Notation: Attributes listed within the rectangle box
        - Chen Style: Represented by an oval shape, Specific type of attributes also exists: multivalue derived, unique(key), partila etc
        - Relationship Cardinality: Cardinality defines possible number of attributes occurance in one entity with another entity

    
    * Steps to Create an ERD:
   Identify Entity ---> Identify Relationship ---> I dentify Cardinality ---> Identify Attributes --->

