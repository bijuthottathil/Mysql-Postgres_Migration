Migration of on prem Mysql tables to Azure Postgres DB using Azure Data Factory

<img width="1006" height="471" alt="image" src="https://github.com/user-attachments/assets/8ad09e00-70d9-4456-9bc0-cffa795d053c" />


1. Mysql setup
   
2.    ![image](https://github.com/user-attachments/assets/8e922356-0c49-4094-8995-b764b9084e27)
3.![image](https://github.com/user-attachments/assets/4802cc06-e706-4e7d-b9c6-c5beeff993e3)
  ![image](https://github.com/user-attachments/assets/e3ee2e76-2777-4393-b037-9cbef8b7d4db)
4. ![image](https://github.com/user-attachments/assets/f4ad9e2b-7e8e-479e-ad9d-cd98d676c1d4)
5. ![image](https://github.com/user-attachments/assets/0579df81-6576-48df-978d-e59d7d6632f7)
6. Setting up ADF dataset and linked sevices for Mysql  ![image](https://github.com/user-attachments/assets/cb9615e7-ac62-461b-8ef3-bb77154179f7)
7. Creating postgres DB in Azure  ![image](https://github.com/user-attachments/assets/672f577e-d213-445e-bb43-e1fc85985ac2)
8. ![image](https://github.com/user-attachments/assets/1bd38d33-260a-4039-8b59-0779189bd523)
9. ![image](https://github.com/user-attachments/assets/aa3bbcc3-382a-41cd-b0d9-173ed0c5e460)
10. ![image](https://github.com/user-attachments/assets/fbd656a8-d588-482b-a00b-bb41c4050513)
11. ![image](https://github.com/user-attachments/assets/8809e737-1fe1-40fe-b4c3-e704ab72ee97)
12. ![image](https://github.com/user-attachments/assets/ae6009f8-21c7-4505-8202-0f05472612d6)
13. Data migrated successfully
14. ![image](https://github.com/user-attachments/assets/afbdd004-a686-4e7c-8206-709937aa8e21)

# Adding incrimental logic

1. Added lookup activity ()  with below condition to get latest data from destination table to do increment load
   ![image](https://github.com/user-attachments/assets/815a7dc7-008b-4ca5-ac26-3952ea28183a)
2. Added proper sql query to take only data > watermark

3. ![image](https://github.com/user-attachments/assets/27660acb-13c7-4a89-93db-19eef8739291)

4. Deleted all records from table inventory and added only 25 records (old) in Mysql DB

5. ![image](https://github.com/user-attachments/assets/1a2bf0ed-c592-4058-95b0-ea940180aa96)

6. 













