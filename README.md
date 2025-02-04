# DatabricksDemos
Contains demo setup created on Databricks Free Tier account

This repo consists of a demo which showcases a scenario of a bookstore which consists of a dataset. The bookstore dataset consists of three tables: customers, orders and books.

We use the medallion architecture as a design pattern to logically organize this data in a lakehouse, with the goal of incrementally and progressively improving the structure and quality of data as it flows through each layer of the architecture (from Bronze ⇒ Silver ⇒ Gold layer tables)

<img width="867" alt="image" src="https://github.com/user-attachments/assets/ba863953-eaa6-46ba-984c-e05a9e6776a8" />

The multi-hop architecture for this dataset looks like this:

<img width="966" alt="image" src="https://github.com/user-attachments/assets/bc96d77e-879b-4151-b2af-d232e6aaa038" />

First, we receive data into the bronze table from a kafka streaming source.

Post this, we refine the data further by moving it into different silver tables. Below are the various silver tables along with mini feature demos included while processing those tables:

1. Orders table: First we start processing data into orders table where we will also see concepts like quality enforcement and streaming deduplication.
2. Books table: In this, we will explore the concept of slowly changing dimensions and create the books table.
3. Current Books table: From books table, we will move on to creating Current_books table while showcasing the batch override feature.
4. Customers: Next we will explore the feature of Change Data Capture (CDC) and create customers table.
5. CDF: Following customers table, we will also explore CDF inbuilt feature which enables incremental changes into downstream tables.
6. Customers Orders table: Next, we will explore streaming joints feature and create customers_orders table.
7. Books Sales table: We will explore how stream static joins work in a datalake and create books_sales table.
8. Finally, we create materialized views in the datalake in the form of gold tables countries_stats_vw and authors_stats






