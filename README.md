# Task-3-SQL
SQL Script with select  specific columns , where clause, order by clause, Like ,OR ,AND operator, BETWEEN ...AND Operator  


// To retriviews the all columns 

select * from customer;
<img width="1920" height="1080" alt="Screenshot (21)" src="https://github.com/user-attachments/assets/1164a821-0acc-42f6-ab5b-ea083697de04" />


// to select only specific columns

select CUSTOMER_ID, first_name, Last_name, mobile_no , city from customer;

<img width="1920" height="1080" alt="Screenshot (22)" src="https://github.com/user-attachments/assets/6b1d2f54-acb2-4b99-bee0-dbb65027714d" />


// to retriview records of maharastra state only  using where clause

select * from customer where state = 'Maharastra';

<img width="1920" height="1080" alt="Screenshot (23)" src="https://github.com/user-attachments/assets/d305a92b-52db-4679-a1a1-3b42a5839dce" />



// to retriview only mg road customers 
select * from customer where CUSTOMER_ADDRESS = 'MG Road';

<img width="1920" height="1080" alt="Screenshot (24)" src="https://github.com/user-attachments/assets/e8e3986b-ae67-4851-a3fe-6d95baefcc66" />



// to those customers are retriviews which customers city pune and state maharastra

select * from customer
 where CITY='pune'
  AND STATE='Maharastra';

<img width="1920" height="1080" alt="Screenshot (25)" src="https://github.com/user-attachments/assets/d57c8e34-d81f-4ddc-a4f6-7eb565c17874" />



// using OR operator to fetch the data 

select * from customer where CUSTOMER_ADDRESS= 'MG Road' OR CUSTOMER_ADDRESS='Gandhi Road Pune';



select * from customer where Last_name= 'Shinde' Or FIRST_NAME = 'Arjun';

<img width="1920" height="1080" alt="Screenshot (26)" src="https://github.com/user-attachments/assets/be9d5176-d877-43a0-b273-fad5ef0a6049" />


// using Like oprator retriviews data 
// to fetch the data only which customer username start with r

 select * from customer 
 where USERNAME Like 'r%';

<img width="1920" height="1080" alt="Screenshot (27)" src="https://github.com/user-attachments/assets/1c9f4129-1b85-4055-8e89-f59648bd045a" />



 // to fetch the data only which customer last name end with e

 select * from customer 
 where LAST_NAME Like '%e';

<img width="1920" height="1080" alt="Screenshot (28)" src="https://github.com/user-attachments/assets/a30560dc-4d87-4896-abe2-976ec1d4f14b" />




// to fetch the data only which customer first name start with A and after one letter j 

 select * from customer 
 where FIRST_NAME Like 'A_j%';

<img width="1920" height="1080" alt="Screenshot (29)" src="https://github.com/user-attachments/assets/3eccd4cd-f475-40d1-9e92-a43f154b8b6f" />


select * from PRODUCTS;

// to retriviews the only price between 100 to 300

select * from PRODUCTS where Price Between 100 and 300;

<img width="1920" height="1080" alt="Screenshot (30)" src="https://github.com/user-attachments/assets/ebc5b668-bd04-4330-83a9-eb1de1cab814" />


// to arrange the all data using category assending order

 select * from PRODUCTS 
  order by CATEGORY asc;

  or 
  select * from PRODUCTS 
  order by CATEGORY ;

<img width="1920" height="1080" alt="Screenshot (32)" src="https://github.com/user-attachments/assets/8647d7bf-17db-4d99-b0ae-6b043425d790" />



  // to arrange the result in descending order 
  
  select * from PRODUCTS 
  order by CATEGORY  desc;

  <img width="1920" height="1080" alt="Screenshot (33)" src="https://github.com/user-attachments/assets/4d8d4e04-7873-419b-b64a-4e054ae3500f" />
