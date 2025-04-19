# Peer-group--database-design_-ecommerce-
creating a database EDR for ecommerce.sql

## Table of Contents

- [Step 1: creating table formulation
- [Step 2: Plan the data flow
- [Screenshorts of the data flow in mysql workbench
- Technologies Used
- Authors and Contributors

## Steps of creating table formulation
## Setp 1: Create an ERD
Entities and Attributes
product_image
image_id (Primary Key)
product_id (Foreign Key)
url (URL or file reference)
color
color_id (Primary Key)
name (e.g., Red, Blue)
product_category
category_id (Primary Key)
name (e.g., Clothing, Electronics)
product
product_id (Primary Key)
name
brand_id (Foreign Key)
base_price
category_id (Foreign Key)
product_item
item_id (Primary Key)
product_id (Foreign Key)
variation_id (Foreign Key)
price
quantity
brand
brand_id (Primary Key)
name
description
product_variation
variation_id (Primary Key)
product_id (Foreign Key)
size_option_id (Foreign Key)
color_id (Foreign Key)
size_category
size_category_id (Primary Key)
name (e.g., Clothing Sizes, Shoe Sizes)
size_option
size_option_id (Primary Key)
size_category_id (Foreign Key)
size (e.g., S, M, L, 42)
product_attribute
attribute_id (Primary Key)
product_id (Foreign Key)
attribute_type_id (Foreign Key)
value
attribute_category
attribute_category_id (Primary Key)
name (e.g., Physical, Technical)
attribute_type
attribute_type_id (Primary Key)
attribute_category_id (Foreign Key)
type (e.g., Text, Number, Boolean)
Relationships
A product can have multiple product_images.
A product belongs to one product_category.
A product is associated with one brand.
A product can have multiple product_variations.
A product_variation is linked to one size_option and one color.
A size_option belongs to one size_category.
A product can have multiple product_attributes.
An attribute_type belongs to one attribute_category.
## step 2: Plan the Data Flow
Data Flow Mapping
Product Creation: When a new product is added, it should be linked to a category, brand, and can have multiple images.
Product Variation: When a product variation is created, it should link to specific sizes and colors.
Product Attributes: Attributes should be assigned to products based on their type and category.
Product Items: Each purchasable item should link to a product and its specific variation.

## Screenshorts

-![Screenshot (6)](https://github.com/user-attachments/assets/94390917-2e9e-45f4-a5cc-6f9937e8442c)

-![Screenshot (7)](https://github.com/user-attachments/assets/861ac25e-4470-46fb-8746-bb1e6b9ddd6d)

## Technologies Used
- Mysql - workbench
- Deepseek.qi
- Kimi.ai
- 
# Authors and Contributors

This project was developed as part of the **PLP Academy Group Assignment**. Below are the contributors:

### Group 568 Members

#### Liso Mlunguza

- **Role**: Leader
- **Email**: [lisomlunguza8@gmail.com](mailto:lisomlunnguza8@gmail.com)
- **GitHub**: [@Liso15](https://github.com/Liso15)


