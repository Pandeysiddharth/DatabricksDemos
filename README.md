# DatabricksDemos
Contains demo setup created on Databricks Free Tier account

This repo consists of a demo which showcases a scenario of a bookstore which consists of a dataset. The bookstore dataset consists of three tables: customers, orders and books.

We use the medallion architecture as a design pattern to logically organize this data in a lakehouse, with the goal of incrementally and progressively improving the structure and quality of data as it flows through each layer of the architecture (from Bronze ⇒ Silver ⇒ Gold layer tables)

<img width="867" alt="image" src="https://github.com/user-attachments/assets/ba863953-eaa6-46ba-984c-e05a9e6776a8" />

The multi-hop architecture for this dataset looks like this:

<img width="966" alt="image" src="https://github.com/user-attachments/assets/bc96d77e-879b-4151-b2af-d232e6aaa038" />


