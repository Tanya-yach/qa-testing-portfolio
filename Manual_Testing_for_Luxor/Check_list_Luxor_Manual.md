# Checklist for Manual Testing of Luxor.cz

| Product Name:   | [Luxor](https://www.luxor.cz/)  
| Prepared by:    | Tetiana Yachna  
| Date:           | 21.05.2025  
| Version:        | 1.0  

---

| ID       | Area           | Check Item                                                                       | Priority |
|----------|----------------|----------------------------------------------------------------------------------|----------|
| CL-001   | Homepage       | Homepage loads correctly without errors                                          | P0       |
| CL-002   | Homepage       | Main menu (Knihy, Papírnictví, etc.) is visible and clickable                    | P1       |
| CL-003   | Homepage       | Search bar is present and accepts input                                          | P0       |
| CL-004   | Navigation     | All top menu and footer links navigate to correct pages                          | P1       |
| CL-005   | Search         | Search with a valid keyword returns matching products                            | P0       |
| CL-006   | Search         | Search with an empty string does not crash the page                              | P0       |
| CL-007   | Search         | Product titles, prices, and availability are shown in results                    | P1       |
| CL-008   | Filtering      | Product filters by category, age, price, and language are functional             | P1       |
| CL-009   | Filtering      | Applying multiple filters returns correct filtered products                      | P1       |
| CL-010   | Product Page   | Product detail page displays name, author, price, stock status                   | P0       |
| CL-011   | Product Page   | Add to cart button is visible and functional if product is in stock              | P0       |
| CL-012   | Product Page   | Out-of-stock products show correct availability message                          | P1       |
| CL-013   | Cart           | Products added to cart are displayed with correct quantity and price             | P0       |
| CL-014   | Cart           | User can increase/decrease product quantity in the cart                          | P1       |
| CL-015   | Cart           | User can remove product from cart                                                | P0       |
| CL-016   | Checkout       | User can proceed to checkout from cart                                           | P0       |
| CL-017   | Checkout       | Checkout confirmation message is shown after placing an order                    | P0       |
| CL-018   | User Account   | User can register with valid input                                               | P1       |
| CL-019   | User Account   | Registration form validates invalid input (e.g. missing password, invalid email) | P1       |
| CL-020   | User Account   | User can log in with valid credentials                                           | P0       |
| CL-021   | User Account   | Invalid login credentials return appropriate error                               | P0       |
| CL-022   | User Account   | Logged-in user can view and edit profile data                                    | P1       |
| CL-023   | Responsiveness | Layout adjusts correctly on tablet and mobile resolutions                        | P1       |
| CL-024   | Responsiveness | Key functions (search, cart, menu) are accessible on mobile devices              | P0       |
| CL-025   | UI/UX          | Buttons and labels have consistent styles across pages                           | P2       |
| CL-026   | Cross-browser  | Site is functional in Chrome, Firefox, and Safari                                | P1       |
| CL-027   | Cross-device   | Critical flows (search → add to cart → checkout) work on mobile and desktop      | P0       |