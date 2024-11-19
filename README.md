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

### References:

- Addleshaw Goddard. (n.d.). Data Diaries - January 2024 | Addleshaw Goddard LLP. [online] Available at: [https://www.addleshawgoddard.com/en/insights/insights-briefings/2024/data-protection/data-diaries-january-2024/#:~:text=The%20Data%20Protection%20and%20Digital](https://www.addleshawgoddard.com/en/insights/insights-briefings/2024/data-protection/data-diaries-january-2024/#:~:text=The%20Data%20Protection%20and%20Digital)

- Al-Farsi, M. A., & Al-Salami, A. J. (2015). Developing Database Management System for Schools. *International Journal of Advanced Computer Science and Applications (IJACSA)*, 6(1), 127-131.

- Amazon Web Services, Inc. (n.d.). Logical vs Physical Data Model - Difference in Data Modeling - AWS. [online] Available at: [https://aws.amazon.com/compare/the-difference-between-logical-and-physical-data-model/#:~:text=With%20logical%20data%20models%2C%20you](https://aws.amazon.com/compare/the-difference-between-logical-and-physical-data-model/#:~:text=With%20logical%20data%20models%2C%20you)

- Big Data Analytics News. (2021). Difference between conceptual and logical data models. [online] Available at: [https://bigdataanalyticsnews.com/difference-between-conceptual-logical-data-models/](https://bigdataanalyticsnews.com/difference-between-conceptual-logical-data-models/)

- Chen, Y., Wu, Y., & Yu, J. (2020). A Study on the Development of Educational Information Management System Based on Oracle Database. In *2020 3rd International Conference on Education Science and Social Development (ICESSD 2020)*. Atlantis Press.

- Garcia, A., & Martinez, L. (2018). Limitations of Standardized Approaches in Educational Database Design: A Case Study Analysis. *International Journal of Educational Technology*, 20(4), 231-246.

- Johnson, R. (2019). Best Practices in Educational Database Design: A Comprehensive Guide. *Educational Technology Review*, 12(2), 45-62.

- Jones, R., & Smith, T. (2021). Challenges and Considerations in Logical Data Modeling: A Critical Analysis. *Journal of Data Management*, 18(2), 45-62.

- Lee, H., & Park, S. (2021). Challenging the Status Quo: A Critical Examination of Industry Standards in Educational Database Design. *Journal of Information Systems Education*, 32(2), 78-95.

- Liu, Z., Hu, Y., & Cai, Y. (2021). Study on Big Data Management in Colleges and Universities Based on Data Mining Technology. In *2021 International Conference on Big Data Engineering and Technology (BDET)* (pp. 95-98). IEEE.

- Marr, B. (2020). Big Data: The 3 Vs Everyone Should Know. *Forbes*. Retrieved from [https://www.forbes.com/sites/bernardmarr/2020/05/18/big-data-the-3-vs-everyone-should-know/](https://www.forbes.com/sites/bernardmarr/2020/05/18/big-data-the-3-vs-everyone-should-know/)

- Nguyen, T., & Patel, S. (2020). Balancing Industry Standards and Institutional Needs: A Framework for Educational Database Design. *Journal of Information Technology in Education*, 15(1), 56-72.

- Park, S., & Lee, J. (2019). Design and Implementation of a School Database System Using MongoDB. *International Journal of Engineering Trends and Technology*, 67(7), 38-41.

- Smith, A., Johnson, B., & Williams, C. (2021). Relational Database Management Systems for Educational Institutions: A Comprehensive Review. *Recent Advances in Computer Science*, 14(4), 235-249.

- Smith, J., Anderson, M., & Williams, K. (2020). Designing Educational Databases: Tailoring Systems to Support Student Success. *Journal of Educational Technology*, 25(3), 112-129.

- TIBCO. (2024). What is a Logical Data Model? | TIBCO. [online] Available at: [https://www.tibco.com/glossary/what-is-a-logical-data-model](https://www.tibco.com/glossary/what-is-a-logical-data-model)

- Zhang, J., Ma, Z., Yan, Y., & Zhang, H. (2021). Design and Implementation of University Data Management System Based on Big Data. In *2021 IEEE International Conference on Big Data (Big Data)* (pp. 1157-1162). IEEE.
