# Answers to Questions

1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

In the provided schema, the "Product" table has a foreign key column named category_id, which references the primary key column id in the "Product_Category" table. This establishes a one-to-many relationship between the "Product" entity and the "Product_Category" entity.

Specifically, each product in the "Product" table is associated with one category from the "Product_Category" table. However, a category in the "Product_Category" table can have multiple products associated with it.


2. How could you ensure that each product in the "Product" table has a valid category assigned to it?

we can ensure that each product in the "Product" table has a valid category assigned to it by adding a foreign key constraint on the category_id column of the "Product" table, referencing the id column of the "Product_Category" table. This ensures that every value in the category_id column of the "Product" table corresponds to an existing category in the "Product_Category" table, thus guaranteeing the integrity of the relationship between products and categories.