# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Silicon Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'img/titleicon.png' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
        Silicon Private Limited.
    </div>
    <div class="menu">
        <div class="menuitem"><a href="/home">Home</a></div> 
        <div class="menuitem"><a href="/products">Products</a></div> 
        <div class="menuitem"><a>People</a></div>
        <div class="menuitem"><a>Contact Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2020 Silicon Private Limited, Developed by Obed Otto.
    </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/building3.jpeg" alt="Building">
    <div class="contenttext">
    Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c1.jpg" alt="product image">
            </div>
            <div class="itemname">4GB DDRA4 laptop memory</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c2.jpg"  alt="product image">
            </div>
            <div class="itemname">1TB Laptop HDD</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c3.jpg"  alt="product image">
            </div>
            <div class="itemname">HP SSD EX900 M.2 250GB</div>
            <div class="itemprice">Price: Rs.4000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c4.jpg"  alt="product image">
            </div>
            <div class="itemname">Crucial P2 250GB 3D NAND</div>
            <div class="itemprice">Price: Rs.50000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c5.jpg"  alt="product image">
            </div>
            <div class="itemname">WD Blue PCIe NVMe SSD 250GB</div>
            <div class="itemprice">Price: Rs.3485.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c6.jpg"  alt="product image">
            </div>
            <div class="itemname">Kingston 250GB A2000 M.2</div>
            <div class="itemprice">Price: Rs.3400.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c7.jpg"  alt="product image">
            </div>
            <div class="itemname">Samsung 970 EVO Plus 250GB </div>
            <div class="itemprice">Price: Rs.4600.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c8.jpg"  alt="product image">
            </div>
            <div class="itemname">WD Black PCIe NVMe SSD</div>
            <div class="itemprice">Price: Rs.4900.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c9.jpg"  alt="product image">
            </div>
            <div class="itemname">Samsung 860 EVO 250GB SATA M.2</div>
            <div class="itemprice">Price: Rs.3700.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c10.jpg"  alt="product image">
            </div>
            <div class="itemname">HP EX900 M.2 250GB PCIe 3.1</div>
            <div class="itemprice">Price: Rs.4100.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c11.jpg"  alt="product image">
            </div>
            <div class="itemname">Seagate Barracuda 510 250GB SSD </div>
            <div class="itemprice">Price: Rs.5300.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c12.jpg"  alt="product image">
            </div>
            <div class="itemname">WD Blue 250GB M.2 Internal</div>
            <div class="itemprice">Price: Rs.4700.00 </div>
        </div>
    </div> 
    </div>
{% endblock  %}
```
### people.html:
```
{% extends "website/base.html" %}

{% block content %}
<div class="peoplecontent">
    <h1>OUR PEOPLE IN CREW</h1>
    <div class="crewmembers">
        <div class="crewmember">
            <div class="memberimage">
            <img src="/static/img/vijay.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">Mr.Vijay</div>
            <div class="designation">FOUNDER</div>
            </div>
        <div class="crewmember">
            <div class="memberimage">
            <img src="/static/img/chrishemsworth.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">Mr.chris hemsworth</div>
            <div class="designation">C.E.O</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
            <img src="/static/img/rashmika.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">Ms.rashmika</div>
            <div class="designation">MD</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
            <img src="/static/img/poojahegde.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">Ms.pooja hegde</div>
            <div class="designation"> TECHNICAL TEAM </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
            <img src="/static/img/nayanthara.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">Ms.nayanthara</div>
            <div class="designation"> DESIGN TEAM </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
            <img src="/static/img/aariarjunan.jpg" alt="member image" style="width:200px;height:200px;">
            </div>
            <div class="membername">Mr.aari arjunan</div>
            <div class="designation"> MARKETING HEAD </div>
        </div>
    </div>



{% endblock  %}
```
### contactus:
```
{% extends "website/base.html" %}

{% block content %}
<div class="contactuscontent" align="center">    
    <h1>CONTACT US</h1>
    <div class="contactustext" align="center">
    <h2> RAGHU (General Manager),</h2>
    <h2> M. K. Silicone Products Private Limited,</h2>
    <h2>OMR ROAD, CHENNAI - 400086</h2>
    <h2>TAMILNADU, India,</h2>
    <h2> contact number-9880893170</h2>

    </div>
   
    </div>
{% endblock  %}
```
## OUTPUT:
![output](./static/img/home.jpg)

![output](./static/img/products.jpg)

![output](./static/img/people.jpg)

![output](./static/img/contactus.jpg)

## CODE VALIDATION REPORT:
![output](./static/img/vhome.jpg)

![output](./static/img/vproducts.jpg)

![output](./static/img/vpeople.jpg)

![output](./static/img/vcontactus.jpg)


## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://veeramalai.student.saveetha.in:8000/. HTML code is validated.