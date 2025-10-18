use hafta4;
 
 create table date_dimension(
 day_number int primary key,
 day_date date,
 week_number int,
 month_number int,
 year_number int);
 create table customer_dimension(
 customer_id int ,
 customer_name char,
 customer_adress int,
 other_details int);
 create table data_warehouse_facts(
 fact_id int,
 customer_id int,
 day_number varchar (20),
 geographic_area int,
 product_code int,
 fact_name varchar(20),
 fact_description int,
 fact_amount int,
 fact_count int,
 other_fact_details int);
 create table product_dimension(
 product_code int primary key,
 product_name varchar(20),
 product_description int,
 other_product_details int);
 create table geographic_dimension(
 geographic_area int primary key,
 geographic_name varchar(20),
 region varchar(20),
 country varchar(20),
 other_region_details varchar(20));
