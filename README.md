# solution-for-lesson-34

# Task 1
```sql
SELECT * FROM categories
```
![image](https://user-images.githubusercontent.com/81769242/221096088-319aaf41-d23a-4bfa-b2d7-24193b44fda6.png)

# Task 2
```sql
SELECT category_name, description FROM categories
```
![image](https://user-images.githubusercontent.com/81769242/221096302-67b051ee-ac29-4b92-8a4e-aee418c24338.png)

# Task 3
```sql
SELECT
    category_id as "Kategoriya ID",
    category_name as "Kategoriya nomi",
    description as "Tavsifi",
    picture as "Rasmi"
FROM categories
```
![image](https://user-images.githubusercontent.com/81769242/221096961-defeaf82-f8b3-49f1-ba2c-8155635b4668.png)

# Task 4
```sql
SELECT * FROM categories
WHERE category_name = 'Confections'
```
![image](https://user-images.githubusercontent.com/81769242/221097297-2dd5fb75-90b7-4fc9-8d0c-aebf00b711df.png)

# Task 5
```sql
SELECT * FROM categories
WHERE category_name = 'Produce' OR category_name = 'Seafood'
```
![image](https://user-images.githubusercontent.com/81769242/221097451-cca265f5-f133-45cb-9008-fbbaded98020.png)

# Task 6
```sql
SELECT * FROM categories
WHERE category_id BETWEEN 6 AND 8
```
![image](https://user-images.githubusercontent.com/81769242/221097867-a0b86981-af29-4b4e-bd39-0564954aec16.png)

# Task 7
```sql
SELECT * FROM categories
ORDER BY description DESC
```
![image](https://user-images.githubusercontent.com/81769242/221098443-23ecfe77-efb2-4f8a-96ad-4c9b0c6763dd.png)


# Task 8
```sql
SELECT * FROM customers
```
![image](https://user-images.githubusercontent.com/81769242/221098589-460a9530-cded-4a7b-aef3-e8822047caeb.png)


# Task 9
```sql
SELECT
    customer_id as "Mijoz ID",
    company_name as "Kompaniya nomi",
    contact_name as "Kontakt nomi",
    contact_title as "Lavozimi",
    address as "Manzili",
    city as "Shahri",
    region as "Hududi",
    postal_code as "Postal kodi",
    country as "Davlati",
    phone as "Telefoni",
    fax as "Faks"
FROM customers
```
![image](https://user-images.githubusercontent.com/81769242/221099243-6353474b-4e50-4311-b2df-ab618e537907.png)


# Task 10
```sql
SELECT * FROM customers
WHERE contact_title = 'Owner'
```
![image](https://user-images.githubusercontent.com/81769242/221099481-773d265a-81db-4c43-9c38-2a31abc297ca.png)


# Task 11
```sql
SELECT * FROM customers
WHERE city = 'London'
```
![image](https://user-images.githubusercontent.com/81769242/221099627-b3ab4c56-2096-4844-982a-9fe08ad5c230.png)


# Task 12
```sql
SELECT * FROM customers
WHERE region IS NULL
```
![image](https://user-images.githubusercontent.com/81769242/221099737-ab727a81-c2d2-4206-8e61-b9d8234f8a71.png)


# Task 13
```sql
SELECT * FROM customers
WHERE region IS NOT NULL
```
![image](https://user-images.githubusercontent.com/81769242/221099913-2423fc2b-d3e9-46fd-87f2-10effd8c1809.png)


# Task 14
```sql
SELECT * FROM customers
WHERE country = 'Germany'
```
![image](https://user-images.githubusercontent.com/81769242/221100043-dc8df7ac-dcef-43c8-9947-9ca69c9f5610.png)


# Task 15
```sql
SELECT COUNT(*) FROM customers
WHERE country = 'Germany'
```
![image](https://user-images.githubusercontent.com/81769242/221100286-da81d789-ebaa-483b-9464-d2393b5a88f9.png)


# Task 16
```sql
SELECT * FROM customers
WHERE fax IS NOT NULL ORDER BY contact_name DESC
```
![image](https://user-images.githubusercontent.com/81769242/221103053-c3cf9ad4-de79-47ed-9e90-32b05b05a722.png)


# Task 17
```sql
SELECT * FROM employees
```
![image](https://user-images.githubusercontent.com/81769242/221100755-a43a19d7-538b-494a-89bf-3edac5aabb94.png)


# Task 18
```sql
SELECT
    employee_id as "Xodim ID",
    last_name as "Familiyasi",
    first_name as "Ismi",
    title as "Lavozimi",
    title_of_courtesy as "xushmuomalalik unvoni",
    birth_date as "Tug'ilgan sanasi",
    hire_date as "Ishga olingan sanasi",
    address as "Manzili",
    city as "Shahri",
    region as "Hududi",
    postal_code as "Postal kodi",
    country as "Davlati",
    home_phone as "Uy telefoni",
    extension as "Ilovasi",
    photo as "Rasmi",
    notes as "Eslatma",
    reports_to as "E'tirozlar",
    photo_path as "Rasm joylashuvi"
FROM employees
```
![image](https://user-images.githubusercontent.com/81769242/221101917-1904d5e5-1ccf-4e9f-8286-e94cb163e1d8.png)


# Task 19
```sql
SELECT * FROM employees
WHERE title_of_courtesy = 'Mr.' ORDER BY first_name DESC
```
![image](https://user-images.githubusercontent.com/81769242/221102266-e84195cc-60cf-49b3-b316-de91c76ebf66.png)


# Task 20
```sql
SELECT COUNT(*) FROM employees
WHERE title = 'Sales Representative'
```
![image](https://user-images.githubusercontent.com/81769242/221102974-6f81b7ea-cdf8-462c-a5c4-4b5339223534.png)


# Task 21
```sql
SELECT * FROM employees
WHERE hire_date between '1994-01-01' and '1994-12-31'
```
![image](https://user-images.githubusercontent.com/81769242/221103507-ed62ac3e-54c2-4057-a553-8096c2b9cd8f.png)


# Task 22
```sql
SELECT
    first_name,
    last_name,
    title,
    city,
    home_phone
FROM employees WHERE region IS NOT NULL
ORDER BY first_name DESC
```
![image](https://user-images.githubusercontent.com/81769242/221104168-6fa2d0f7-2fb7-4a7c-a249-8a290b069a45.png)


# Task 23
```sql
SELECT * FROM orders
WHERE customer_id = 'VINET'
```
![image](https://user-images.githubusercontent.com/81769242/221104366-ecdf44a4-008d-417f-8e5c-f345900a859a.png)


# Task 24
```sql
SELECT * FROM orders
WHERE order_date BETWEEN '1996-01-01' AND '1996-12-31';
```
![image](https://user-images.githubusercontent.com/81769242/221104567-ecc4d3d8-91ef-40a3-b2fa-238340aa4ebb.png)


# Task 25
```sql
SELECT * FROM orders
WHERE ship_region IS NOT NULL
```
![image](https://user-images.githubusercontent.com/81769242/221104795-50884268-a268-4af3-8294-9e8e0d62a419.png)


# Task 26
```sql
SELECT * FROM orders
WHERE order_id BETWEEN 10300 AND 10400
```
![image](https://user-images.githubusercontent.com/81769242/221104951-75411315-fb7d-49d5-878b-6e09708ae888.png)


# Task 27
```sql
SELECT SUM(unit_price) FROM order_details
```
![image](https://user-images.githubusercontent.com/81769242/221105158-30571004-d47c-4396-a8d6-68823900e0b9.png)


