# School Database Management System
## Building school DBMS using mySQL

---

# 1. Introduction

## 1.1 Review
The project team engaged in requirements-gathering sessions to identify the client’s needs, focusing on key data entities and relationships. An Entity-Relationship (ER) diagram (Figure 1) was created using Chen's notation, and data types were specified for consistency. 
<br>

<p align="center">
<img src="images\sdb_1.png" alt="ER Diagram" alt="Centered Image" title="Entity-Relationship Diagram" width="500">
</p>

<br>

Updates to the design included new entities such as "Parent," "Classroom", "Exam," and "Exam Result". See image below of database created using mySQL.

<br>

<p align="center">
<img src="images\sdb_2.png" alt="ER Diagram" alt="Centered Image" title="Entity-Relationship Diagram" width="500">
</p>

<br>

[For code click here](mysql_code.sql)


Normalisation techniques were applied to reduce redundancy and maintain data integrity. The design decisions were justified based on client requirements, industry standards, and academic principles, proposing a MySQL solution to improve decision-making and academic outcomes. However, the report could be more thorough in discussing theoretical aspects and presenting the implementation plan.

<br>

## 1.2 Design Process

The design process began with the team holding meetings to understand the client’s specific needs and constraints. This included outlining requirements for course information, student and teacher registrations, class schedules, attendance tracking, and exam results. These requirements ensured that the design aligned with stakeholders’ needs (Du Mortier, 2022), contributing to a comprehensive and effective database solution.

<br>

---


## 2. Database management in schools
Schools increasingly rely on technology for administrative and educational purposes. Traditional paper-based systems are becoming obsolete due to inefficiencies like data redundancy, inconsistency, and lack of centralized access. Digital systems, particularly Database Management Systems (DBMS), address these challenges by enabling efficient organization, storage, and management of data.

Key benefits of DBMS include:
- **Data-driven decision-making**: Real-time access, reporting, and analytics improve administrative decisions.
- **Transparency and accountability**: Stakeholders gain easy access to consistent and accurate information.
- **Data security**: Access controls, encryption, and audit trails protect sensitive data like student records.
- **Automation**: Routine tasks (e.g., enrollment, attendance, grade management) are streamlined, saving staff time (Al-Farsi & Al-Salami, 2015).

## 3. Conceptual Database Design
Entity-Relationship (ER) modeling was used to draft the database structure, visualizing relationships between entities with Chen's notation. Attributes were assigned consistent data types to ensure accuracy. While effective for initial design, the ER model requires ongoing refinement to remain agile for evolving institutional needs. Continuous evaluation is crucial to maintaining the database’s relevance as requirements and technologies change.

## 4. Logical Database Schema Construction
The logical database schema was developed as a blueprint for data elements and their relationships. While the schema effectively represented complex relationships and ensured consistency, challenges in scalability and flexibility were identified. To address these issues, optimizing data structures and leveraging emerging technologies are recommended to handle large volumes of data and accommodate evolving needs.

## 5. Challenges and Considerations
Logical data modeling for school databases faces challenges like scalability, flexibility, and alignment with educational requirements (Jones & Smith, 2021). Additional considerations include:
- Balancing precision and computational efficiency for sensitive data.
- Adapting to evolving workflows and administrative processes.
  
Logical models focus on business logic, while physical models optimize data storage and implementation. Figure 3 highlights the hierarchy of model types, emphasizing their distinct but complementary roles.

<p align="center">
<img src="images\sdb_3.png" alt="ER Diagram" alt="Centered Image" title="Entity-Relationship Diagram" width="500">
</p>



## 7. Selection of Database Technology
The decision to use a relational database model, specifically **MySQL**, was based on its ability to efficiently organise data, ensure normalisation, and optimise queries (Smith et al., 2021). MySQL’s relational structures use tables, keys, and constraints, making it effective for managing complex data relationships in schools.

### Alternative Technologies:
- **PostgreSQL**: Enhanced SQL compliance, extensibility, and support for advanced data types, offering greater flexibility and performance for specific needs (Johnson & Brown, 2020).
- **MongoDB**: A document-oriented NoSQL database ideal for handling unstructured data, dynamic schemas, and scalability (Park & Lee, 2019).
- **Oracle Database**: Enterprise-grade reliability and high availability for mission-critical systems, though at higher costs (Chen et al., 2020).

Selecting the most suitable database technology involves evaluating requirements, scalability, and budget constraints to ensure optimal data management.

---

## 8. Implementation Challenges and Solutions
### Key Challenges:
- **Scalability**: MySQL struggles with large datasets and high transaction volumes (Chen, Wu & Yu, 2020).
- **Flexibility**: Rigid schema structures may hinder frequent changes and diverse data types (Park & Lee, 2019).

### Proposed Solutions:
- Evaluate alternative data storage models for better scalability and adaptability.
- Use technologies and design patterns that enhance performance and flexibility.

---

## 9. Legality and Confidentiality
### Compliance Requirements:
- **Data Privacy Laws**: GDPR, CCPA, and FERPA require safeguarding sensitive data like student records.
- **Standards**: ISO/IEC 27001 offers guidelines for secure information management.
- **Emerging Regulations**: The UK’s Data Protection and Digital Information Bill introduces new roles and rules for compliance.

### Steps for Compliance:
1. Regular audits and policy reviews.
2. Secure data with encryption, access controls, and monitoring.
3. Stay updated on laws such as the EU AI Act and UK privacy bills.

---

## 10. Recommendations
- **Compliance Assessments**: Regularly review data policies to align with legal and regulatory updates.
- **System Updates**: Continuously adapt requirements and refine the ER diagram for relevance.
- **Data Protection**: Implement robust security measures like encryption and access controls.
- **Scalability**: Optimise data structures for growth and flexibility.
- **Collaboration**: Foster teamwork among stakeholders for ongoing improvements.

---

## 11. Conclusion
The development of a logical database system for school management showcased a methodical approach.  
- **Design**: The use of MySQL, supported by an Entity-Relationship (ER) diagram based on Chen's notation, addressed the school’s needs.
- **Exploration**: Consideration of PostgreSQL, MongoDB, and Oracle highlights the importance of tailored database solutions.
- **Compliance**: Legal adherence and robust data security measures ensure the system remains effective and secure.

This project established a functional database while creating a foundation for future enhancements, enabling informed decision-making, improved transparency, and streamlined administrative processes in schools.
