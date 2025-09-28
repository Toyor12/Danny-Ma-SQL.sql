# Danny's-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences
![Danny's Diner](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/bf8e59c0-a0a4-41c4-afe9-3d21216c60fc)

## Introduction

Danny seriously loves Japanese food so in the beginning of 2021, he decides to embark upon a risky venture and opens up a cute little restaurant that sells his 3 favourite foods: sushi, curry and ramen. The restaurant is facing the challenges that many new establishments encounter. The diner has collected basic operational data over the initial months, but the utilization of this data to make informed business decision remains a problem to them.

The objective of this report is to assist Danny's Diner in navigating through these challenges by leveraging the collected data. By employing SQL-based analysis, this report aims to unearth valuable insights into customer behavior, spending patterns, and menu item preferences. These insights are crucial for making informed decisions to enhance the customer experience, potentially expanding the customer loyalty program, and ultimately ensuring the sustained growth and success of Danny’s Diner


## Problem Statement

Danny wants to use the data to answer a few simple questions about his customers, especially about their visiting patterns, how much money they’ve spent and also which menu items are their favourite. Having this deeper connection with his customers will help him deliver a better and more personalised experience for his loyal customers.

He plans on using these insights to help him decide whether he should expand the existing customer loyalty program - additionally he needs help to generate some basic datasets so his team can easily inspect the data without needing to use SQL.


## Case Study Questions

- What is the total amount each customer spent at the restaurant?
- How many days has each customer visited the restaurant?
- What was the first item from the menu purchased by each customer?
- What is the most purchased item on the menu and how many times was it purchased by all customers?
- Which item was the most popular for each customer?
- Which item was purchased first by the customer after they became a member?
- Which item was purchased just before the customer became a member?
- What is the total items and amount spent for each member before they became a member?
- If each $1 spent equates to 10 points and sushi has a 2x points multiplier - how many points would each customer have?
- In the first week after a customer joins the program (including their join date) they earn 2x points on all items, not just sushi - how many points do customer A and B have at the end of January? 

## Data Source

Danny company provided the data to be used for the analysis to write fully functioning SQL queries to help him answer his questions!
The 3 key datasets for this case study are:

- **sales**
- **menu**
- **members**

## Data Model and Schema
![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/fad94450-03c1-4c63-8598-208e7c7f46ed)

## Solutions
1. What is the total amount each customer spent at the restaurant?
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/8a2f960f-3112-41f9-9d12-737c8b7905b8)

   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/3d7d8db5-0b34-4b4b-be45-8a04dd4631e7)

The three customers A, B and C have spent $76, $74 and $36 respectively

2. How many days has each customer visited the restaurant?
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/dcf84375-f0a0-425e-bfb7-8ae39cb3c039)
   
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/5ecba840-5418-41fe-81d4-dd3c17044053)

Customer B has visited the restaurant 6 times which is the most among all customers studied. 

3. What was the first item from the menu purchased by each customer?
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/0a0a29b9-1c9d-4eac-8f93-72f3b95e95d6)
   
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/f084298d-9ffd-4c93-a203-9a8af9fec97a)

4. What is the most purchased item on the menu and how many times was it purchased by all customers?
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/d4002f55-f23f-4e11-a3e7-8f0d46428708)

   
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/c39d8e17-ca48-40f9-8fad-967121a90f35)

The most purchased item is Ramen. It has been purchased 8 times.

5. Which item was the most popular for each customer?
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/6e3fb6c1-8297-40eb-8cae-e0b40d431c8a)
   
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/4e445287-a4d4-4c5f-b760-79d32426925b)

6. Which item was purchased first by the customer after they became a member?
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/d6f457ea-55c0-4990-aca8-433505f10aa1)
   
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/e77e297e-ed36-46d4-a498-afd8ed39b33a)

   Of the 3 customers, only 2 of them customer A and B are members, they purchased curry and sushi first after they became a member
   
7. Which item was purchased just before the customer became a member?
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/cbd429f4-10b3-4e85-b1e0-5bf160c6e2b8)

   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/ac8edd6a-e090-498f-9150-7427b0253e17)

8. What is the total items and amount spent for each member before they became a member?
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/3f241c9a-ff94-4973-baa7-380ef4bf6a0a)

   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/03d678ac-844a-466d-a6ca-02ce173a81c7)

9. If each $1 spent equates to 10 points and sushi has a 2x points multiplier - how many points would each customer have?
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/96bf26a9-b5c1-42bb-a16e-d9d7dea3f2a8)

   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/bbf5dad3-03c1-474e-8a8e-7792a94f9502)

10. In the first week after a customer joins the program (including their join date) they earn 2x points on all items, not just sushi - how many points do customer A and B have at the end of January?
   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/1db09106-fa1a-4bf3-a668-9917d838bfb3)

   ![image](https://github.com/Taofik06/Danny-s-Diner-SQL-Based-Analysis-of-Customer-Spending-and-Preferences/assets/123642327/f5a38040-4e2a-495c-9cc2-73825b8c8154)


