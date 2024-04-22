
# ECOM Website PHP 

This PHP represents the frontend of an E-commerce website. It dynamically generates HTML content based on server-side logic and data retrieved from a database. Below is an overview of the key components and functionalities of the template:


## Components

1. **User Authentication and Session Management**:
   - The script starts a PHP session to manage user authentication and store session variables.

2. **Header Section**:
   - The `components/user_header.php` file is included to display the header section, which typically contains navigation links and user-related information.

3. **Homepage Content**:
   - The homepage (`index.php`) displays a slideshow of featured products using the Swiper library.
   - Each slide showcases a product category with a relevant image and a "Shop Now" button that links to the corresponding category page (`category.php`).

4. **Category Section**:
   - The category section displays a swiper slider with various product categories.
   - Each category slide contains an icon and text, linking to the respective category page (`category.php`).

5. **Latest Products Section**:
   - The latest products section displays a swiper slider with the latest products fetched from the database.
   - Each product slide includes an image, name, price, quantity input field, and "Add to Cart" button.
   - Users can add products to their wishlist or cart by clicking on the heart icon or the "Add to Cart" button, respectively.
   - Clicking on the eye icon opens a quick view modal for the corresponding product.

6. **Footer Section**:
   - The `components/footer.php` file is included to display the footer section, containing copyright information and social media links.

7. **JavaScript Functionality**:
   - JavaScript code at the end of the file initializes Swiper sliders with responsive breakpoints for optimal display across different screen sizes.

## External Dependencies

- [Swiper](https://swiperjs.com/): A modern JavaScript slider library used for creating sliders and carousels.
- [Font Awesome](https://fontawesome.com/): An iconic font and CSS toolkit used for displaying icons.


### MySQL Database Schema 

This file contains the SQL dump of the `shop_db` database, including table structures, data, indexes, and auto-increment settings. It is generated using phpMyAdmin with version 5.1.1. Below is a breakdown of its contents:

#### 1. Database Information
- **Name**: `shop_db`
- **Server Version**: MariaDB 10.4.22
- **PHP Version**: 8.1.2

#### 2. Tables
The dump includes the schema and data for the following tables:
1. `admins`
2. `cart`
3. `messages`
4. `orders`
5. `products`
6. `users`
7. `wishlist`

#### 3. Table Structure
Each table's structure includes columns, data types, constraints, and indexing. For example, the `admins` table has columns for `id`, `name`, and `password`, with the `id` column set as the primary key.

#### 4. Data Insertion
Data insertion statements are provided for some tables, such as `admins`. These statements populate the tables with initial data, such as admin credentials.

#### 5. Indexes
Primary key indexes are defined for each table to ensure data integrity and optimize query performance.

#### 6. Auto-increment Settings
Auto-increment settings are configured for the primary key columns of each table to ensure unique identifiers for new records.

#### 7. Transaction
The SQL dump is enclosed within a transaction to ensure atomicity and consistency during database restoration.

#### 8. SQL Mode and Time Zone
The SQL mode is set to `NO_AUTO_VALUE_ON_ZERO`, and the time zone is set to `+00:00`.

#### Usage
To use this SQL dump:
1. Import it into a MySQL/MariaDB database using a database management tool or command-line interface.
2. Adjust database credentials and connection settings as needed in your application configuration.


