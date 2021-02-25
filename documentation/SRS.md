# Storage system
### Vision 
“Storage system” is web-application which allows users to record information about equipment in stock, clients and sales. 
#### Application should provide:
* Storing equipment in stock, clients and sales in a database; 
* Display list of sales; 
* Updating the list of sales (adding, editing, removing); 
* Display list of clients;
* Updating the list of clients (adding, editing, removing); 
* Display list of equipment in stock; 
* Updating the list of equipment in stock (adding, editing, removing); 
* Display number of the orders for equipment and clients; 
* Filtering by date for sales and clients; 
* Search by code or name of the equipment.

## 1. Equipment
### 1.1 Display list of equipment
This mode is intended for viewing and editing the equipment list 
#### Main scenario:
* User selects item “Equipment”; 
* Application displays list of equipment. 

![ Pic. 1.1 View the equipment list.]( https://lh6.googleusercontent.com/C-JdC60gTuol_-YQSy-owBKEIz9Eo3ztKNPIvAXbLxGItTfpq3lZu_b0IbvJGN30Hbmlp5iV4VgBEgqTAdGT=w1920-h942-rw)

The list displays the following columns: 
* Code – code of the equipment; 
* Name – name of the equipment;
* Description – description of the equipment;
* In stock – number of equipment in stock;
* Number of orders – number of orders of the equipment;
* Purchase price - price for the purchase of the equipment from a supplier;
* Selling price - prices for sale.

#### *Search by code or name of the equipment:* 
* In the equipment list view mode, the user sets a code or name of the equipment and presses the refresh list button; 
* The application will display a form to view the list of equipment with updated data.
### 1.2 Add equipment
#### Main scenario: 
* User clicks the “Add” button in the equipment list view mode; 
* Application displays form to enter equipment data; 
* User enters equipment data and presses “Save” button; 
* If any data is entered incorrectly, incorrect data messages are displayed; 
* If entered data is valid, then record is adding to database; 
* If error occurs, then error message is displaying; 
* If new equipment record is successfully added, then list of equipment with added records is displaying. 
#### Cancel operation scenario: 
* User clicks the “Add” button in the equipment list view mode; 
* Application displays form to enter equipment data; 
* User enters equipment data and presses “Cancel” button; 
* Data don’t save in data base, then list of equipment records is displaying to user. 
* If the user selects the menu item " Sales”, ”Clients” or "Equipment ", the data will not be saved to the database and the corresponding form with updated data will be opened.

![ Pic. 1.2 Add equipment.]( https://lh4.googleusercontent.com/BYSV95vcXvmB1aB_NlygPSEeSgufWT1ySiC3p1Y3ybNkTxs-NtenJOpftymw4-vv_jYg2tnBpXdQph-Xd2M8=w1920-h942)

When adding a equipment, the following details are entered: 
* Code – code of the equipment; 
* Name – name of the equipment;
* Description – description of the equipment;
* In stock – number of equipment in stock;
* Purchase price - price for the purchase of the equipment from a supplier;
* Selling price - prices for sale.
Constraints for data validation: 
* Equipment description – maximum length of 90 characters; 
* Code - unique, maximum length of 30 characters; 
### 1.3 Edit equipment
 #### Main scenario: 
* User clicks the “Edit” button in the equipment list view mode; 
* Application displays form to enter equipment data; 
* User enters equipment data and presses “Save” button; 
* If any data is entered incorrectly, incorrect data messages are displayed; 
* If entered data is valid, then edited data is added to database; 
* If error occurs, then error message is displaying; 
* If equipment record is successfully edited, then list of equipment with added records is displaying. 
#### Cancel operation scenario: 
* User clicks the “Edit” button in the equipment list view mode; 
* Application displays form to enter equipment data; 
* User enters equipment data and presses “Cancel” button; 
* Data don’t save in data base, then list of equipment records is displaying to user. 
* If the user selects the menu item " Sales”, ”Clients” or "Equipment ", the data will not be saved to the database and the corresponding form with updated data will be opened.

![Pic. 1.3 Edit equipment.]( https://lh6.googleusercontent.com/aheSoMcukyfJ0keVR3r3mmrQFenNZrfCmbGkBlcoGvlvfkfnp1CL90O0VzXAELvNu21tspWDwTeEBtLa7gaQ=w1227-h942)

### 1.4 Removing the equipment
#### Main scenario: 
* The user, while in the list of equipment mode, presses the "Delete" button in the selected equipment line; 
* Application displays confirmation dialog “Please confirm delete equipment?”; 
* The user confirms the removal of the equipment; 
* Record is deleted from database; 
* If error occurs, then error message displays; 
* If equipment record is successfully deleted, then list of equipment without deleted records is displaying. 
#### Cancel operation scenario: 
* User is in display mode of equipment list and press “Delete” button; 
* Application displays confirmation dialog “Please confirm delete equipment?”; 
* User press “Cancel” button; 
* List of equipment without changes is displaying. 

![Pic. 1.4 Delete equipment dialog.]( https://lh3.googleusercontent.com/uR2_qIrbTwUFQNKc1xz9XcPK1TL8Wh4IwQThaCmlIi3cPzFonG0mEyWJUM744DZR6M8Pm-jrBpJ73QQlUKUk=w1227-h942)

## 2. Clients 
### 2.1 Display list of Clients 
This mode is intended for viewing and editing the clients list. 
#### Main scenario: 
* User selects item “Clients”; 
* Application displays list of clients.

![ Pic 2.1 View the clients list.]( https://lh4.googleusercontent.com/xdTAQbDS6zUBOa603TPrPQ8S1fpcIOCMevvZXxYUzvnj2PK2ZnOYINNOoMqilmv1qnQRaSS_SYtOm0rid-DA=w1227-h942)
#### The list displays the following columns: 
* Code – client’s code; 
* Full name – client’s full name; 
* Organization - client’s organization;
* Registration date – client’s date registration; 
* Number of orders – client’s number of orders. 
#### Filtering by date: 
* In the clients list view mode, the user sets a date filter and presses the refresh list button; 
* The application will show the clients only for a certain period of time. 
* Restrictions: *
* Start date of the period should be less then end date of the period; 
* If start date is blank, then filtering by end date only. 
* If end date is blank, then filtering by start date only. 
* Updating data after selecting the filtering conditions is carried out by pressing the “Refresh” button.
### 2.2 Add client 
#### Main scenario: 
* User clicks the “Add” button in the clients list view mode; 
* Application displays form to enter client data; 
* User enters client’s data and presses “Save” button; 
* If any data is entered incorrectly, incorrect data messages are displayed; 
* If entered data is valid, then record is adding to database; 
* If error occurs, then error message is displaying; 
* If new client record is successfully added, then list of clients with added records is displaying. 
#### Cancel operation scenario: 
* User clicks the “Add” button in the clients list view mode; 
* Application displays form to enter client’s data; 
* User enters client’s data and presses “Cancel” button; 
* Data don’t save in data base, then list of clients records is displaying to user. 
* If the user selects the menu item " Sales”, “Clients” or "Equipment ", the data will not be saved to the database and the corresponding form with updated data will be opened.

![ Pic. 2.2 Add client.]( https://lh3.googleusercontent.com/Of7yrQbvgI6dDzgGuJf0eDHCfCd8GZXn0LjruUvGI2g4toqQbssOGdkklZMSDvIrhYQ3CLd7-aIpLWk3eVlV=w1227-h942)

When adding a client, the following details are entered: 
* Code – client’s code; 
* Full name – client’s full name; 
* Organization - client’s organization;
* Registration date – client’s date registration; 
Constraints for data validation: 
* Full name – maximum length of 45 characters; 
* Organization – maximum length of 45 characters; 
* Code – unique, maximum length of 30 characters; 
* Registration date – client’s registration date in format dd/mm/yyyy.
### 2.3 Edit client 
#### Main scenario: 
* User clicks the “Edit” button in the clients list view mode; 
* Application displays form to enter client data; 
* User enters client’s data and presses “Save” button; 
* If any data is entered incorrectly, incorrect data messages are displayed; 
* If entered data is valid, then edited data is added to database; 
* If error occurs, then error message is displaying; 
* If client’s record is successfully edited, then list of clients with added records is displaying. 
#### Cancel operation scenario: 
* User clicks the “Edit” button in the clients list view mode; 
* Application displays form to enter client data; 
* User enters client data and presses “Cancel” button; 
* Data don’t save in data base, then list of clients records is displaying to user. 
* If the user selects the menu item " Sales”, “Clients” or "Equipment ", the data will not be saved to the database and the corresponding form with updated data will be opened.

![ Pic. 2.3 Edit client.]( https://lh3.googleusercontent.com/Of7yrQbvgI6dDzgGuJf0eDHCfCd8GZXn0LjruUvGI2g4toqQbssOGdkklZMSDvIrhYQ3CLd7-aIpLWk3eVlV=w1227-h942)

### 2.4 Removing client 
#### Main scenario: 
* The user, while in the list of clients mode, presses the "Delete" button in the selected client line; 
* Application displays confirmation dialog “Please confirm delete client?”; 
* The user confirms the removal of the client; 
* Record is deleted from database; 
* If error occurs, then error message displays; 
* If client record is successfully deleted, then list of clients without deleted records is displaying. 

![ Pic. 2.4 Delete client dialog.]( https://lh6.googleusercontent.com/GzlTDAYmenzMeYZc4VOX_eivC_Zugq3-DHMyGZoI8-w7FdgWmI2xOyys3GiYVK1pgFTd44kJ4Iqki3iPUYZG=w1227-h942)

Cancel operation scenario: 
* User is in display mode of clients list and press “Delete” button; 
* Application displays confirmation dialog “Please confirm delete client?”; 
* User press “Cancel” button; 
* List of clients without changes is displaying.
## 3. Sales 
### 3.1 Display list of sales 
The mode is designed to view the list of sales, if it possible to display the number of sails for a specified period of time. 
#### Main scenario: 
* User selects item “Sales”; 
* Application displays list of sales.

![ Pic. 3.1 View the sales list.]( https://lh5.googleusercontent.com/DL31UGdXCu-CRVCzKi9KDyWYjsfMie9a4xhpY_5YdOV8yeu0PrPfam0OfSazLnuSO5qk8NC_6X5CwvFx3NkS=w1227-h942)

The list displays the following columns: 
* Code – sale’s code; 
* Client code – code of the client; 
* Equipment code – code of the equipment; 
* Date – date of adding a sale order; 
* Selling price – cost of equipment. 
#### Filtering by date: 
* In the order list view mode, the user sets a date filter and presses the refresh list button;
* The application will display a form to view the list of sales with updated data.
### 3.2 Add sales 
#### Main scenario: 
* User clicks the “Add” button in the sales list view mode; 
* Application displays form to enter order data; 
* User enters order data and presses “Save” button; 
* If any data is entered incorrectly, incorrect data messages are displayed; 
* If entered data is valid, then record is adding to database; 
* If error occurs, then error message is displaying; 
* If new order record is successfully added, then list of sales with added records is displaying. 
#### Cancel operation scenario: 
* User clicks the “Add” button in the sales list view mode; 
* Application displays form to enter order data; 
* User enters order data and presses “Cancel” button; 
* Data don’t save in data base, then list of sales records is displaying to user. 
* If the user selects the menu item " Sales”, “Clients” or "Equipment ", the data will not be saved to the database and the corresponding form with updated data will be opened.

![Pic. 3.2 Add order.]( https://lh6.googleusercontent.com/-uWCq3jFs2iYlPatad_Hb7QGtAjl2EURXhhvBlV8vxi8GZ3Ll0b22WPRpTCcisjBAUEVJMrgaO5nFD1RBiEd=w1227-h942)

When adding a sale, the following details are entered: 
* Code – sale’s code; 
* Client code – code of the client; 
* Equipment code – code of the equipment; 
* Date – date of adding a sale order.
### 3.3 Edit sale. 
#### Main scenario: 
* User clicks the “Edit” button in the sales list view mode; 
* Application displays form to enter order data; 
* User enters sale data and presses “Save” button; 
* If any data is entered incorrectly, incorrect data messages are displayed; 
* If entered data is valid, then edited data is added to database; 
* If error occurs, then error message is displaying; 
* If sale record is successfully edited, then list of orders with added records is displaying. 
#### Cancel operation scenario: 
* User clicks the “Edit” button in the sales list view mode; 
* Application displays form to enter sale data; 
* User enters order data and presses “Cancel” button; 
* Data don’t save in data base, then list of sales records is displaying to user. 
* If the user selects the menu item " Sales”, “Clients” or "Equipment ", the data will not be saved to the database and the corresponding form with updated data will be opened.

![ Pic. 3.3 Edit order.]( https://lh3.googleusercontent.com/8WBCPbkenyNucPconwi2dEljFbV6YoVidOIRGqhX65d2jdU3n4EoIs9_oeXM0CbiD-uqOq9cauz_cJK6TA7a=w1227-h942)

When editing a sale, the following details are entered: 
* Code – sale’s code; 
* Client code – code of the client; 
* Equipment code – code of the equipment; 
* Date – date of adding a sale order.
Constraints for data validation: 
* Code – unique, maximum length of 30 characters; 
* Add date – order add date in format dd/mm/yyyy.
### 3.4 Removing the sale 
#### Main scenario: 
* The user, while in the list of sales, presses the "Delete" button in the selected sale line; 
* If the sale can be removed, a confirmation dialog is displayed; 
* The user confirms the removal of the sale; 
* Record is deleted from database; 
* If error occurs, then error message displays; 
* If order record is successfully deleted, then list of sales without deleted records is displaying. 

![Pic. 3.4 Delete order dialog.]( https://lh3.googleusercontent.com/DQyBFzM5WgKvJwEMQYO-jR4KbyyE6yDEHGWz__QYoPrk67-23LaTOrO9eohWMZaWYdPYu9ZvcPUeOHOciTxf=w1227-h942)

#### Cancel operation scenario: 
* User is in display mode of orders list and press “Delete” button; 
* Application displays confirmation dialog “Please confirm delete sale?”; 
* User press “Cancel” button; 
* List of sales without changes is displaying.



