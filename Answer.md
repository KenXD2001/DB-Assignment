<!-- Questions -->

1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

Answer:
The relationship between the "Product" and "Product_Category" entities is a one-to-many relationship. Each product in the "Product" table is associated with a category through the "category_id" column, which is a foreign key referencing the "id" column in the "Product_Category" table. This means that each product belongs to exactly one category, while a category can have multiple products associated with it.

2. How could you ensure that each product in the "Product" table has a valid category assigned to it?

Answer:
To ensure that each product in the "Product" table has a valid category assigned to it, you can enforce referential integrity by creating a foreign key constraint on the "category_id" column in the "Product" table that references the "id" column in the "Product_Category" table. This constraint will ensure that every value in the "category_id" column of the "Product" table corresponds to a valid "id" in the "Product_Category" table.
