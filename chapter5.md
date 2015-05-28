#chapter5 ALTER

##
```
ALTER TABLE my_contacts
ADD COLUMN contact_id INT NOT NULL AUTO_INCREMENT FIRST,
ADD PRIMARY KEY(contact_id);

ALTER TABLE my_contacts
ADD COLUMN phone_number VARCHAR(10) NOT NULL ;

ALTER TABLE my_contacts
ADD COLUMN phone_number VARCHAR(10)
AFTER first_name;

ALTER TABLE my_contacts
ADD COLUMN phone VARCHAR(10) FIRST;

ALTER TABLE my_contacts
ADD COLUMN phone VARCHAR(10) AFTER email;

ALTER TABLE my_contacts
ADD COLUMN phone VARCHAR(10) AFTER contact_id;

ALTER TABLE my_contacts
ADD COLUMN phone VARCHAR(10) AFTER last_name;

CREATE TABLE projekts(
       number INT,
       descriptionofpoj varchar(50),
       contractoroniob  varchar(20)
);


ALTER TABLE projekts 
RENAME TO project_list;

ALTER TABLE project_list
CHANGE COLUMN number proj_id INT NOT NULL AUTO_INCREMENT,
ADD PRIMARY KEY(proj_id);

ALTER TABLE project_list
CHANGE COLUMN descriptionofpoj proj_desc VARCHAR(100),
CHANGE COLUMN contractoroniob  proj_name VARCHAR(30);

ALTER TABLE project_list
MODIFY COLUMN proj_desc VARCHAR(120);


ALTER TABLE project_list
ADD COLUMN phone_num VARCHAR(10),
ADD COLUMN start DATE,
ADD COLUMN price INT; 

=>
ALTER TABLE project_list
ADD COLUMN con_phone VARCHAR(10),
ADD COLUMN start_date DATE,
ADD COLUMN est_cost DEC(7,2); 


ALTER TABLE project_list
MODIFY COLUMN start_date NULL; => DROP COLUMN start_date;

ALTER TABLE
CHANGE COLUMN  mo  model,
CHANGE COLUMN  howmuch price,
ADD COLUMN car_id INT AUTO_INCREMENT NOT NULL,
ADD COLUMN VIN BLOB,
ADD PRIMARI KEY(car_id);

ALTER TABLE hooptie
RENAME TO car_table,
ALTER TABLE car_table
ADD COLUMN car_id INT NOT NULL AUTO_INCREMENT FIRST,
ADD PRIMARY KEY(car_id),
ALTER TABLE car_table
ADD COLUMN VIN VARCHAR(16) AFTER car_id,
CHANGE COLUMN mo model VARCHAR(20),
MODIFY COLUMN color AFTER model,
MODIFY COLUMN year AFTER color,
CHANGE COLUMN howmuch price DECIMAL(7,2);

ALTER TALBLE contact_id
ADD COLUMN state VARCHAR(20),
ADD COLUMNT city VARCHAR(50);

SELECT CONCAT(SUBSTRING_INDEX(location,'州',1),'州') FROM my_contacts;

SELECT SUBSTRING_INDEX(location,'州',-1) FROM my_contacts;

SELECT RIGHT(location,2) FROM my_contacts;

SELECT SUBSTRING('テキサス州サンアントニオ',6,3);

SELECT UPPER('uSa');

SELECT LOWER('spaGHEtti');

SELECT LTRIM(' dogfood ');

SELECT RTRIM(' catfood ');

SELECT LENGTH('テキサス州サンアントニオ');

1->SELECT

2->ADD COLUMN

3->RIGHT(),LEFT()

4->INSERT

SUBSTRING_INDEX() -> 

UPDATE my_contacts SET state = CONCAT(SUBSTRING_INDEX(location,'州',1),'州');


```

