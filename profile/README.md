
## Catering Manager Roadmap
- [ ] **Frontend and Backend** (same functions)
	- [ ] General
		- [ ] Authentication
		- [ ] Profile
	- [ ] Customer Side
		- [ ] Introduction to location
		- [ ] Displaying products (menu)
		- [ ] Checkout/order page
		- [ ] Call the waiter button
	- [ ] Company Side
		- [ ] Dashboard (Overview and single sections)
		- [ ] Displaying customers and orders + CRUD orders
		- [ ] Possibility of manage more subsidiaries
		- [ ] Table assignment
- [ ] **Landing page**
    - [ ] Introduction to the project
    - [ ] Feedback and Contact Us page
	- [ ] Affiliated local
	- [ ] Reservation section (with the cancelling option)


---
### Accessing to various part of the system
- The **landing page** is accessible from the web
- The **company dashboard** is accessible from the web
- The **customer side** web app is split in three parts:
	- Reservation: it is accessibile from the web and allows customers to make a reservation to not wait when they arrive at the place
	- Order and payment: this part is accessible just at the place and the device has to be connected at the local's wifi and the customer can order and pay

---


# General concepts

## Landing page
The landing page is an SPA, we will make it in angular and it should have the following sections:
- Home (with an introduction to the project and feedback section)
- Affiliated local
- Contact Us
### Reservation system
The customer can make a reservation (he can choose his seat from a little map, made specifically for each restaurant or with a simple form).
The reservation system should provide a security system to avoid receiving reservations by someone with bad intentions.

<br><br>

## Company dashboard
### Owner side features
- If a business has more than one place, its subsidiaries can be added in the profile: each one of them has different analytics and configurations.
- Analytics: orders, products (i.e. menu), customers, reservation
- Section of the dashboard sidebar:
	- Overview
	- Subsidiaries (based on the choice the dashboard will show different data)
	- Customers
	- Orders (including home delivery)
	- Customers complaints
	- Settings (with the possibility of customize)
### Staff side features
- Internal table management
- Orders Monitoring (if an order from the kitchen is ready or not and where to bring it)

<br><br>

## Customer Side
**Flow**: Menu --> order section --> online checkout section
**Other section**: Settings, profile
The profile section should include the following subsections:
- Orders (previous orders)
- Discount (claimed and to be claimed)
- Customer informations
- Deleting profile label

### Order and pay
The payment can be with the most used payment system (card, cash) and it can be made at checkout or through the web app.
Before leaving the local it's necessary to go through the cash register and confirm the payment or pay with cash.
It's possibile to pay:
- during the order
- after a single order
- online after all orders (at the end of the meal)
- physically then at the cash register (checkout)

### Settings and Profile personalization
The customers can personalize his profile and interface of the web app to improve the ux.

<br><br>

---
# Less important things

The company dashboard side has a different way to manage roles, below there's a table with all the possible roles:

| Role           | Purpose                                                                 |
|:-------------- |:----------------------------------------------------------------------- |
| Owner          | To manage and have under control all subsidiaries or single local       |
| Cashier        | To check the payment made by the customers before they leave the local  |
| Waiters        | To know which order is ready from the kitchen                           |
| Chefs          | To advice the waiter about the state of the orders                      |
| Security guard | To know which is the customers reserved table or to assign they a table |


For takeaway orders isn't necessary assign a table to the customer, but the customer has to order at the place and check the *takeaway order* checkbox.


The company dashboard is fully customizable and, with its interface, it's possible to change the business functions that are showed on the customers' web app.
