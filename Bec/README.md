Project 2 
 
# ERD code in Quick Based Diagrams 
# https://app.quickdatabasediagrams.com/#/

Campaign
-
cf_id INT PK
contact_id INT FK >- Contacts.contact_id
company_name VARCHAR(50)
description VARCHAR(100)
goal INT
pledged INT
outcome VARCHAR(30)
backers_count INT
country VARCHAR(2)
currency VARCHAR(3)
launched_date VARCHAR(30)
end_date VARCHAR(30)
category_id VARCHAR(10) FK >- Category.category_id
subcategory_id VARCHAR(10) FK >- Subcategory.subcategory_id

Category
-
category_id VARCHAR(10) PK FK
category VARCHAR(30)

Contacts
-
contact_id INT PK FK 
first_name VARCHAR(30)
last_name VARCHAR(30)
email VARCHAR(50)

Subcategory
-
subcategory_id VARCHAR(10) PK FK
subcategory VARCHAR(30)

# -------------------------------

Note: 
Code used from class activity solutions 