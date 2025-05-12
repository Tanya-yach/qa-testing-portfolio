# Test scenarios for Manual Testing of Luxor.cz

|Product Name: | Luxor (https://www.luxor.cz/) |
|Prepared by:  | Tetiana Yachna                |
|Data:         | 05/06/2025                    |
|Version:      | 1.0                           |

---

| ID    | Title                              | Description                                                                                                      | Priority| Feature/Module   |Test Cases      |
|-------|------------------------------------|------------------------------------------------------------------------------------------------------------------|---------|------------------|----------------|
| TS-001| Homepage loads correctly           | Verify that the homepage loads with all key elements displayed (logo, search bar, cart icon, categories, etc.)   | P0      | Homepage         | TC-001         |
| TS-002| Main navigation menu works         | Check that top navigation menu links redirect to proper pages ("Knihy", "E-knihy", "Hry a hračky", "Akce", etc.) | P0      | Navigation       | TC-002         |
| TS-003| Product search by keyword          | Verify that the search returns relevant results for valid product                                                | P0      | Search           | TC-003         |
| TS-004| Filter products by category        | Check filtering by one or more parameters                                                                        | P1      | Search/Filters   | TC-004, TC-005 |
| TS-005| Product detail page                | Verify that clicking on a product opens its detail page                                                          | P0      | Product Page     | TC-006         |
| TS-006| Add product to cart                | Verify the process of adding the product to the cart                                                             | P0      | Cart             | TC-007 - TC-013|
| TS-007| View and edit products in the cart | Verify that the user can view and edit cart contents                                                             | P0      | Cart             | TC-014 - TC-017|
| TS-008| Proceed to checkout                | Verify navigation from cart to checkout page; order confirmation page appears                                    | P0      | Checkout         | TC-018 - TC-021|
| TS-009| Register new user                  | Check that the user can create an account with valid data                                                        | P1      | User Account     | TC-022 - TC-025|
| TS-010| Login/Logout                       | Check that the user can login and log out with valid credentials                                                 | P1      | User Account     | TC-026 - TC-029|
| TS-011| User profile updates               | Check that the user can update information                                                                       | P2      | User Account     | TC-030         |
| TS-012| Mobile responsiveness              | Verify mobile responsiveness (no horizontal scroll; buttons/forms usable).                                       | P1      | Responsive Layout| TC-031 - TC-033|
| TS-013| Mobile cart/checkout               | Check that cart and checkout are usable and readable on smaller screens                                          | P0      | Responsive Layout| TC-034 - TC-035|
| TS-014| Button interactions                | Validate button hover/click states                                                                               | P2      | UI/UX            | TC-036         |
| TS-015| Form validation                    | Test form validation (empty fields)                                                                              | P1      | UI/UX            | TC-023         |
