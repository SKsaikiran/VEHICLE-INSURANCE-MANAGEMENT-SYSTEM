# VEHICLE-INSURANCE-MANAGEMENT-SYSTEM

|SYNOPSIS|[Click here](https://github.com/SKsaikiran/VEHICLE-INSURANCE-MANAGEMENT-SYSTEM/blob/2aad7133cb5a7b3220e1ad215296059b6997b7b7/Documents/SYNOPSIS.md)|

## CONTENTS
### 1.Introduction 		
- Problem statement									
- Objectives										
- Dataset Description	
### 2.  System Design
- ER Diagram										
- ER to Relation Mapping								
- Schema Diagram									

## <ins>Introduction :</ins>

The **"Vehicle Insurance Management System"** has been developed to override the problems prevailing in the practicing manual system. This software is supported to eliminate and in some cases reduce the hardships faced by this existing system. Moreover this system is designed for the particular need of the company to carry out operations in a smooth and effective manner.

The application is reduced as much as possible to avoid errors while entering the data. It also provides error message while entering invalid data. No formal knowledge is needed for the user to use this system. Thus by this all it proves it is user-friendly. Vehicle Insurance Management System, as described above, can lead to error free, secure, reliable and fast management system. It can assist the user to concentrate on their other activities rather to concentrate on the record keeping. Thus it will help organization in better utilization of resources.

Every organization, whether big or small, has challenges to overcome and managing the information of Insurance, Customer, Vehicle Type, Customer ID Type, Vehicle Maker. Every Vehicle Insurance Management System has different Customer needs, therefore we design exclusive employee management systems that are adapted to your managerial requirements. This is designed to assist in strategic planning, and will help you ensure that your organization is equipped with the right level of information and details for your future goals. Also, for those busy executive who are always on the go, our systems come with remote access features, which will allow you to manage your workforce anytime, at all times. manage resources. These systems will ultimately allow you to better manage resources.

## <ins>Problem statement :</ins>

The purpose of Vehicle Insurance Management System is to automate the existing manual system by the help of computerized equipment and full-fledged computer software, fulfilling their requirements, so that their valuable data/information can be stored for a longer period with easy accessing and manipulation of the same. The required software and hardware are easily available easy to work with.

## <ins>Objectives :</ins>

The main objective of the Project on Vehicle Insurance Management System is to manage the details of Customer, Insurance, Vehicle, Vehicle Type, Vehicle Maker. It manages all the information about Customer, Customer ID Type, Vehicle Maker, Customer. The project is totally built at administrative end and thus only the administrator is guaranteed the access. The purpose of the project is to build an application program to reduce the manual work for managing the Customer, Insurance, Customer ID Type, Vehicle. It tracks all the details about the Vehicle, Vehicle Type, Vehicle Maker.

## <ins>Dataset description :</ins>
- Customer Module: Used for managing the Customer details.(name, cust_id, address, email)
- Insurance Module: Used for managing the information and details of the Insurance.(poly_id, price, ins_desc, validity)
- Vehicle Module: Used for managing the Vehicle details.(reg_no, veh_desc, veh_type, veh_no)
- Login Module: Used for managing the login details.(login_id, user_name, email, password)
- Admin Module : Used to fetch and collect the details of the customer.(id, name, phone, email)
- Accident Module : Used for getting the details of accident.(location, date)

## <ins>E-R Diagram :</ins>

- Entity – Relationship model (ER model) describes inter-related things of interest in a specific domain of knowledge. An ER model is composed of entity types (which classify the things of interest) and specifies relationships that can exist between instances of those entity types. 
- The ER Diagram below shows all the entities, their attributes and the relation between them.

![ER](https://user-images.githubusercontent.com/89591339/205450286-969500dd-c84b-4a56-98b8-7a1dd6496da9.png)

## <ins>ER to relation maping :</ins>

- Admin, Inusrance, Login, Accident and Vehicle are the main entity in the vehicle insurance management system.
- Admin and Insurance has 1: n relationship called ‘Manages’.
- Admin and Login has 1 : 1 relationship called ‘Has’.
- Insurance and Customer has n : 1 relationship called ‘Insurance holder’.
- Customer and Accident has 1 : n relationship called ‘Involved’.
- Customer and Vehicle has 1 : n relationship called ‘Occurs’.
- Accident and Vehicle has 1 :1 relationship called ‘Happened’.

## <ins>Schema diagram :</ins>
The term **"schema"** refers to the organization of data as a blueprint of how the database is constructed (divided into database tables in the case of relational databases. 

![Schema](https://user-images.githubusercontent.com/89591339/205450353-f279516e-093a-4132-b016-f37dd8a11704.png)

