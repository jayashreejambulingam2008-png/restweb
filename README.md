# Ex.07 Restaurant Website
## Date:16/10/2025

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

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

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
home.html
{% extends 'base.html' %}
{% block title %}Home — Spice Delight{% endblock %}
{% block content %}
<section class="intro">
  <h1>Welcome to Spice Delight</h1>
  <p>Serving traditional flavors with a modern twist. Join us for an unforgettable experience.</p>
</section>
{% endblock %}

menu.html
{% extends 'base.html' %}
{% block title %}Menu — Spice Delight{% endblock %}
{% block content %}
<section class="menu">
  <h2>Our Menu</h2>
  <div class="menu-grid">
    {% for food in foods %}
      <div class="item">
        <img src="{% static 'images/'|add:food.image %}" alt="{{ food.name }}">
        <p>{{ food.name }}</p>
      </div>
    {% endfor %}
  </div>
</section>
{% endblock %}


administration.html
{% extends 'base.html' %}
{% block title %}Administration — Spice Delight{% endblock %}
{% block content %}
<section class="team">
  <h2>Our Team</h2>
  <div class="team-grid">
    {% for member in team %}
      <div class="member">
        <img src="{% static 'images/'|add:member.image %}" alt="{{ member.name }}">
        <p>{{ member.name }} – {{ member.role }}</p>
      </div>
    {% endfor %}
  </div>
</section>
{% endblock %}


contact.html
{% extends 'base.html' %}
{% block title %}Contact Us — Spice Delight{% endblock %}
{% block content %}
<section class="contact">
  <h2>Contact Us</h2>
  <p>📍 Address: {{ contact.address }}</p>
  <p>📞 Phone: {{ contact.phone }}</p>
  <p>✉️ Email: {{ contact.email }}</p>
</section>
{% endblock %}



```

## OUTPUT:

<img width="1920" height="1080" alt="Screenshot (43)" src="https://github.com/user-attachments/assets/2c3fa809-6a5b-49ae-b0f0-d3ec56e63481" />

<img width="1920" height="1080" alt="Screenshot (101)" src="https://github.com/user-attachments/assets/012b9c0a-05d8-41ec-b9a8-5e6f6021796b" />




## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
