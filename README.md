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
        - Chen Style: Represented by an oval shape, Specific type of attributes also exists: multivalue derived, unique(key), partial etc
        - Relationship Cardinality: Cardinality defines possible number of attributes occurance in one entity with another entity

    
    * Steps to Create an ERD:
   Identify Entity ---> Identify Relationship ---> I dentify Cardinality ---> Identify Attributes ---> ERD

* Types of Data Model: 3 types
  --
  - Conceptual Data Modle -> Business
      - Identify what the system contains but not the details
      - focus is to identify what data is used in business
      - This is the first version of the data model and can't be used to build a database
      - Goal of a conceptual data model is to act as a business requirement reference
      - Gives us understanding of high level and how each entity relates to each other
      - Doesn't describe the process flow itself
        
      - Features of Conceptual Data Model:
          - Doesn't show primary key or attributes
          - Shows entities and relationship
          - It's a high-level view for the business and shows a structure of data for business
          - It's independent of a database and not implementable ready
          - Very early stage of the modelling process where most of the concepts or objects might never made to the final pyhsical model
          - Identify and help with scoping requirements
          - Useful for PM as communication tool
          - It is part of what builds the final Entity Relationship Model
  --          
  - Logical Data Model -> Architect & BA
     - Identify how the system should be implemented
     - Focus on business requirements
     - Focus on the design of the data not physical implementation
     - Add additional information to the conceptual # Advantages of ELT
       
     - Features of Logical Data  Model
         - Primary key & foreign keys are present
         - All attributes are specified within an entity, will have data types
         - Relationships are specified using primary and foreign keys
         - Independent from DBMS
         - Normalization happens usually to 3NF
--
   - Physical Data Model
     - Identify how the system will be implemented for specific DBMS system
     - It is the blueprint for the developer
     - Depending on data modelling choice denormalisation can occur
     - Final result of Physical design can be different from Logical design
    
     - Features of Physical Data Model
         - Entities are now tables names
         - Attributes become columns names
         - Each column datatype, length, nullable is specified
         - Relationshíp cardinality is defined


   --
  - Different Types of Keys
     - Primary
     - Foreign key
     - Surrogate Key
     - Composite key
     - Natural key

--
  - Recommended Tools for ERD
      - Lucidchart
      - Draw.io
      - erwin Data Modeller
      - ER/Studio
      - MySQL Workbench









      

- More data storage space required
- Could be slow due to muilti persistent of data
- Low compliance due to everything stored
- Security risk if not handled PII data correctly
- Fairly new technology due to popularity in cloud solutions








---
# DATA MODELLING & ERD NOTATION
#### Data Model:
- Foundation to building DWH & BI solutions
- Primary goal of the data model is to act as a blueprint
- Helps buidling conceptual, logic, physical and models and define relatiosnhips
- Defines how the logical structure of database is modeled
- Specifies business requirements and data structure
- Provides visual way to communicate with business at various level
- Data Model is important part of the developement process(main communication methid between team)

# Data Modelling
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
   to give further level of datails
     - It is independent of specific database design
     - It is a foundational layer for Physical model
     - Creates common understanding of business data
     - Sometimes called Business Model
  - Physical Data Model -> DBA & Developer
 

    
    All start with Gathering Business requirements


