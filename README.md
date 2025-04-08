# HYBRID-RECOMMENDER-SYSTEM
This project focuses on building a Hybrid Recommender System designed to suggest pizza dishes suitable to each customer's preferences.

## Dataset:

- The dataset consists of four sheets:
  - orders: Contains information on 21,350 orders made in 2015, including order ID, date, time, customer ID, and total payment per order.
  - order_details: Provides detailed information for each order, including the pizza ID and quantity of each pizza ordered.
  - pizzas: Includes data on each pizza ID, such as pizza type, size, and price.
  - pizza_types: Describes the name, category, and detailed ingredients of each pizza.

## Guideline:

This system combines both Content-Based Filtering and Collaborative Filtering to provide personalized food recommendations.

The recommendation flow is as follows:

**1. User Identification:**
- The system begins by asking the customer to input their customer ID.

  - If the ID exists, the customer is identified as a old customer.

  - If no ID is provided or found, the system will either prompt the customer to re-enter their ID or proceed by treating them as a new customer.


**2. For Old Customers:**
- Recommendations are based on the customer's two most recent orders. The logic depends on the number of items in those orders:

  - If an order contains only one item, we use Content-Based Filtering (recommend_cb) to suggest similar dishes based on item attributes.

  - If an order contains multiple items, we use Collaborative Filtering (recommend_pizza) to recommend dishes preferred by similar users.

** 3. For New Customers:**
- The system applies Content-Based Filtering to recommend items that are similar to the one the current customer is interested in, based on its features.

## Contact:
For any questions or feedback, please contact via email: l.vikiet21@gmail.com



