
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



