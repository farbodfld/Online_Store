# Online_Store
Online store implementation in the console environment with object-oriented.

Introducing the parts of the project

#### Different users
4 types of users are defined in this store.

### Admin
The site admin is only one person. In the first run of the program, he must register his username and password in the system. Admin should also create producer and porter users and assign them username and password.
Discount options are explained in the relevant section. Also, this user has access to all statistics. You will learn more about the statistics in the continuation of the project.

### Producer
The producer user has a product that he wants to put on the site for sale, and in case of sale, he will earn profit and get money. When the producer enters the system with the username and password defined by the admin user, he has the ability to add and delete his own species. Note that the added product has no sales limit! That is, the manufacturer only imports his own type of products, thereby guaranteeing that he has an unlimited amount of this product in stock.

### porter
Porters are responsible for the transfer of customer orders (shipments), so after logging into the system, they deal with the type, name and volume of orders. Porters log in to the system with the username and password defined for them by the administrator. After logging in to the system, they can access the four menus of customer orders, shipments being sent, orders sent and changing the vehicle.

1.	Customers' orders: In this menu, every porter sees a list of products ordered by customers. Each carrier can choose a number of them from among the orders and take the responsibility of delivering them to the customer. By selecting an order by the carrier, that order is removed from the list of customer orders and added to the list of shipments being sent by that carrier.

2.	Shipments currently being sent: In this menu, the carrier sees a list of orders that he has undertaken to deliver to the destination, but have not yet delivered to the destination. The carrier can select the shipments that have arrived at the destination from this list. In this case, the shipment is removed from this list and added to the list of orders sent by that carrier.

3.	Sent orders: In this menu, the porter sees a list of orders that he has delivered to the destination.

4.	Changing the vehicle: In this menu, the porter can choose his vehicle from the options of motor, van and car. The default vehicle of each carrier is selected by the admin when defining a carrier.
Note that for each carrier, only orders are displayed whose packaging volume is proportional to their vehicle. The acceptable volume for the engine is up to 0.5, for the car 2 and for the van 12 cubic meters. Also note that the list of customer orders is a public list that all carriers have access to, but the other three lists are private for each carrier, and only the carrier and admin have access to these three lists.

In addition, in each list, at your own discretion, details of the goods that can be effective and useful in their selection and processing should be displayed.
Customer

Every store is established with the purpose of selling goods to customers. Your program should provide the possibility of registering and logging in as a customer by taking the user name and password of your choice. Naturally, in this section it is necessary to check the uniqueness of the username, and to show the appropriate message to the user. The customer can buy them by searching and selecting the products available in the store.

Each customer can view one of the following lists by logging into their account:

1.	Producers: In this way, every customer can get a list of producers, and choose the desired producer from among them. With this, a list of products provided by the manufacturer along with its features will be displayed to the customer. If needed, the user can select one of the items and place it in the sending queue.

2.	Product categories: In this way, each customer can prepare a list of product categories, and enter the product list by entering the desired category. This list should include the characteristics of the available goods and the name of its manufacturer. If needed, the user can select one of the items and place it in the sending queue.

3.	Purchased items: Each customer can see a list of all the items they have purchased so far along with their features.

4.	Goods in the shipping order: When the user chooses a product for purchase, the product does not reach him immediately, but it happens when one of the carriers transfers the goods for him. Meanwhile, the user can see the list of products that are being sent.

### Shop items
The goods that can be sold in this store are divided into three main categories:
    * Food
    * clothing
    * Electronic devices
    
Every product must have a category, volume and the name of the manufacturer.
Edible materials include categories of snacks, dairy products, and fruits and vegetables. In addition to the mentioned characteristics, each food item must have an expiration date. The expiration date is a number in days that shows the deadline for using the product after purchase.
The goods that are classified as fruits and vegetables must carry the name of the city of their producer.
Clothing, which can be shoes, pants, or shirts, includes men's, women's, and children's categories.
Every product must have a material and size. For the classification of shoes, this size should be displayed with a number, and for the size of the categories, it should be displayed as L, M, or S.
Electronic devices include the categories of mobile phones, televisions and game consoles. Every product that fits in this category must have the year of production.
Products that fit in the category of mobile phones and televisions must have the screen size.
Products that fall into the game console category must have a list of accompanying item names.

### Discount system
One of the criteria for choosing an online store is the amount of discount on its products. The discount can be applied to different products, which is the application of the discount in the hands of the manufacturer or admin.
Statistics and reports
As mentioned in different sections, there are different statistics. In fact, you should store the information related to various events in your program, and when the statistics are requested, output the relevant statistics depending on who requested what statistics. The statistics that can be obtained are:

* The producer's profit amount (Each producer can only receive his own profit. The admin can see the profit of all producers. "Profit" means the money that the producer earns from the sale of goods, so the cost of producing goods is not mentioned.).

* Customer's spending amount (each customer can only see his own spending amount. Admin can see all customers' spending.).

* The amount of transported volume of each porter (each porter can see his own statistics. The admin can see everyone's statistics.).

* List of goods purchased by each customer

* List of orders moved by each carrier

* List of products sold by each manufacturer

### User interface section
The program communicates with the user through the console. Note that the details of how the application and the user communicate are up to you, but it must support all parts of the application.
