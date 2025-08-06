# Online Jewelry Shop System in Django with Source Code

The **Online Jewelry Shop System Project in Django** created based on **Python**, **Django**, and **SQLITE3 Database**. 

The **Online Jewelry Shop System** project that will assist a Jewelry store or store in providing an online ordering system for their customers.

The system has two user interfaces: one for the admin user, or Jewelry management, and the other for the client, or the system’s website. Customers must register on the website before they can conduct business with the Jewelry shop.

An **Online Jewelry Shop System** is simple to navigate, and the features are similar to those found in other online stores.

The Jewelry items are grouped by item categories to make it easier for consumers to find what they’re looking for.

Each product can have a different color, size, sample image, and thorough description thanks to the system. Since some of the jewelry products do not need this area, the sizes and colors fields are not needed.

>[!NOTE]
> To start creating an **Online Jewelry Shop System Project in Python Django**, makes sure that you have PyCharm Professional IDE Installed in your computer.

## Online Jewelry Shop System in Django: Admin Features 

* **Login Page**

The page where the system administrator enters their system credentials in order to gain access to the system’s administrative side.

* **New Category Page**

This is the page where an administrator can add a new jewelry category.

**Category List**

The page with a list of jewellery categories that can be navigated to change or delete a category.

* **New Product Page**

The page to which an administrator can add new product.

* **Product List**

The page on which the jewelry pieces or goods are mentioned and can be viewed, modified, or deleted.

* **Orders Page**

The location where the admin can handle customer orders.

* **New User Page**

The page where a new admin or customer’s system credentials are created by an admin.

* **Users list**

This is the page that lists and manages the added users.

## Customer Features of Online Jewelry Shop System in Django

* **Login Page**

Customers enter their website credentials on this page to gain access to all of the website’s features.

* **Register Page**

The page where new customers created their login credentials for the website.

* **Home Page**

When customers visit the website, this is the system’s default page. 

This page shows the jewelry pieces for sale in the store, and the items can be sorted using the category filter checklist on the right side of the page, or by entering a keyword in the search box above the products.

* **Product View Page**

The page on which the product’s specific information is shown, as well as the page on which the customer adds the product to his or her cart.

* **Cart List Page**

The page that lists the items that customers have chosen. This is the page where the customer can complete the order checkout process.

* **My Order Page**

The page that lists the customer’s orders.

## How to Create an Online Jewelry Shop System in Django?

Here are the steps on how to create a Online Jewelry Shop System in Django with Source Code.

1. **Open file**.

Open “pycharm professional” after that click “file” and click “new project”.

<img width="484" height="453" alt="image" src="https://github.com/user-attachments/assets/171885fb-02fe-464b-84b2-c8e82e290119" />


2. **Choose Django**.

Next, after click “new project“, choose “Django” and click.

<img width="152" height="325" alt="image" src="https://github.com/user-attachments/assets/acfcd433-1fd6-4b11-9f98-c9ab3916067b" />


3. **Select file location**.

Then, select a file location wherever you want.

4. **Create application name**.

After that, name your application.

5. **Click create**.

Lastly, finish creating project by clicking “create” button.

6. **Start Coding**.

Finally, we will now start adding functionality to our Django Framework by adding some functional codes.

## Functionality and Codes of the Online Jewelry Shop System in Django

* **Create template for the homepage in Online Jewelry Shop System in Django**.

In this section, we will learn on how create a templates for the homepage. 

To start with, add the following code in your base.html under the folder of shop/templates/shop.

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Myrel Jewellery</title>
    {% load staticfiles %}
    <link href="{% static 'shop/bootstrap/css/bootstrap.min.css' %}" rel="stylesheet">
    <link href="{% static 'shop/bootstrap/css/style.css' %}" rel="stylesheet">
  </head>
  <body style="background-color: green">
    <!--  navbar starts -->
    <nav class="" style="border-radius:0px !important;margin-bottom:0px; background-color: black;">
      <div class="container-fluid">
        <!-- Brand and toggle get grouped for better mobile display -->
        <div class="navbar-header">
          <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
            <span class="sr-only">Toggle navigation</span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
          </button>
          <a class="navbar-brand" href="{% url 'shop:home' %}"><span id="lione" style="color: red;">Myrel Jewellery Shop</span></a>
        </div>

        <!-- Collect the nav links, forms, and other content for toggling -->
        <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
            <ul class="nav navbar-nav navbar-center">
              <li><a href="{% url 'shop:home' %}"><span id="" style="color: red">Home </span><span class="sr-only">(current)</span></a></li>
              <li><a href="{% url 'shop:home' %}"><span id="lione" style="color: red">Rings & Neklace </span></a></li>
              
              <li><a href="{% url 'shop:about' %}"><span id="lione" style="color: red">About </span></a></li>
              {% if user.username %} <li><a href="{% url 'shop:logout' %}"><span id="lione" style="color: red">Logout {{user.username}}</span></a></li>{% endif %}
              <li><a href="{% url 'shop:cart' %}"><span class="glyphicon glyphicon-shopping-cart" style="color:red;"></span></a></li>
            </ul>
        </div><!-- /.navbar-collapse -->
      </div><!-- /.container-fluid -->
    </nav>
    <!--  navbar ends -->
    {% block body %}{% endblock %}
    <hr class="divider">
    <center><footer style="color:white;margin-left:70px;">&copy Myrel Online Jewellery Shop System 2021 | All Rights Reserved</footer></center>
    <hr class="divider">

    <script src="{% static 'shop/jquery-1.12.4.min.js' %}"></script>
    <script src="{% static 'shop/bootstrap/js/bootstrap.min.js' %}"></script>
  </body>
</html>
<!-- <span class="badge">{{ length }}</span> -->
```

### 📌 Here's the full documentation for the [Online Jewelry Shop System in Django](https://itsourcecode.com/free-projects/python-projects/online-jewelry-shop-system-in-django-with-source-code/) 
