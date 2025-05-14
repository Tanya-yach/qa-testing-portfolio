# Test scenarios for API Testing of Luxor.cz

|Product Name: | Luxor (https://www.luxor.cz/) |
|Prepared by:  | Tetiana Yachna                |
|Data:         | 05/14/2025                    |
|Version:      | 1.0                           |

---

| ID          | Title                         | Description                                                                              | Feature/Module    | Priority |Test Cases      |
|-------------|-------------------------------|------------------------------------------------------------------------------------------|-------------------|----------|----------------|
| TS_API-001  | Product search by keyword	  | Verify that the search returns relevant results for valid keyword,  empty keyword	     | Search API	     | P1       |                |
| TS_API-002  | Filtering the product list	  | Verify that the product list can be filtered by one or more parameters	                 | Filters API	     | P1       |                |
| TS_API-003  | Product detail page	          | Verify API returns complete details for a valid product ID	                             | Product Page API	 | P0       |                |
| TS_API-004  | Add product to cart	          | Verify that a product can be added to the cart (available product, unavailable product)	 | Cart  API	     | P0       |                |
| TS_API-005  | View products in the cart     | Verify that the correct items are listed in the cart	                                 | Cart  API	     | P0       |                |
| TS_API-006  | Remove products in the cart   | Verify a product can be removed/edit from the cart	                                     | Cart  API	     | P0       |                |
| TS_API-007  | Proceed to checkout	          | Validate successful order creation with valid items	                                     | Checkout API	     | P0       |                |
| TS_API-008  | Register new user	          | Verify user registration with valid input	                                             | User Account API	 | P0       |                |
| TS_API-009  | Login/Logout	              | Verify login/logout works and login returns a token	                                     | User Account API	 | P0       |                |
| TS_API-010  | User profile updates	      | Verify that the information can be updated in user profile	                             | User Account API	 | P1       |                |
