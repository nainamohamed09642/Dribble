# Project Responsive Web Design using Bootstrap
## Date:

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Sports World</title>
    <link rel="stylesheet" href="style.css">
    <!-- You can link a Google font if you wish -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <!-- Navigation Bar -->
    <header class="header">
        <div class="logo">
            <h1>Sports World</h1>
        </div>
        <nav class="nav">
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#news">News</a></li>
                <li><a href="#events">Events</a></li>
                <li><a href="#teams">Teams</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section (Featured Image) -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h2>Welcome to the Sports World</h2>
            <p>Your go-to platform for all things sports!</p>
            <button><a href="#news">Get Latest News</a></button>
        </div>
    </section>

    <!-- News Section -->
    <section id="news" class="news">
        <h2>Latest Sports News</h2>
        <div class="news-grid">
            <article class="news-item">
                <img src="IMG1.png" alt="Sports News 1">
                <h3>Breaking News: The Championship Finals</h3>
                <p>Get the latest updates on the Championship finals, including exclusive interviews and predictions.</p>
                <a href="#">Read More</a>
            </article>
            <article class="news-item">
                <img src="IMG4.png" alt="Sports News 2">
                <h3>New Record in Swimming</h3>
                <p>Learn about the latest record-breaking performance in swimming.</p>
                <a href="#">Read More</a>
            </article>
            <article class="news-item">
                <img src="IMG2.png" alt="Sports News 3">
                <h3>Top Football Transfers of the Year</h3>
                <p>Check out the top football transfers and rumors that have shaken the sports world.</p>
                <a href="#">Read More</a>
            </article>
        </div>
    </section>

    <!-- Upcoming Events Section -->
    <section id="events" class="events">
        <h2>Upcoming Sports Events</h2>
        <div class="event-grid">
            <div class="event-item">
                <h3>Football World Cup</h3>
                <p>Starts: 1st July 2024</p>
            </div>
            <div class="event-item">
                <h3>Summer Olympics 2024</h3>
                <p>Starts: 15th July 2024</p>
            </div>
            <div class="event-item">
                <h3>Tennis Grand Slam</h3>
                <p>Starts: 5th August 2024</p>
            </div>
        </div>
    </section>

    <!-- Teams Section -->
    <section id="teams" class="teams">
        <h2>Featured Teams</h2>
        <div class="teams-grid">
            <div class="team">
                <img src="IMG5.png" alt="Team 1">
                <h3>Team A</h3>
                <p>League: Football</p>
            </div>
            <div class="team">
                <img src="IMG7.png" alt="Team 2">
                <h3>Team B</h3>
                <p>League: Basketball</p>
            </div>
            <div class="team">
                <img src="IMG6.png" alt="Team 3">
                <h3>Team C</h3>
                <p>League: Tennis</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>If you have any questions, feel free to reach out to us:</p>
        <form action="#" method="POST">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" placeholder="Your Message" rows="4" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <!-- Footer Section -->
    <footer class="footer">
        <p>&copy; 2024 Sports World | All Rights Reserved</p>
    </footer>
</body>
</html>

```
```

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Roboto', sans-serif;
    background-color: #f9f9f9;
    color: #333;
}

a {
    text-decoration: none;
    color: inherit;
}

ul {
    list-style: none;
}

/* Header Styles */
.header {
    display: flex;
    justify-content: space-between;
    padding: 20px 50px;
    background-color: #333;
    color: white;
}

.header .logo h1 {
    font-size: 28px;
}

.nav ul {
    display: flex;
    gap: 20px;
}

.nav li a {
    color: white;
    font-weight: bold;
    font-size: 16px;
}

.nav li a:hover {
    color: #ea4c89;
}

/* Hero Section */
.hero {
    background-color: #ea4c89;
    color: white;
    text-align: center;
    padding: 80px 20px;
}

.hero h2 {
    font-size: 48px;
    margin-bottom: 20px;
}

.hero button {
    padding: 12px 30px;
    background-color: white;
    color: #ea4c89;
    font-weight: bold;
    border: none;
    cursor: pointer;
    border-radius: 5px;
}

.hero button a {
    color: #ea4c89;
}

.hero button:hover {
    background-color: #f7f7f7;
}


.news {
    padding: 50px 20px;
}

.news h2 {
    text-align: center;
    font-size: 36px;
    margin-bottom: 20px;
}

.news-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 20px;
}

.news-item img {
    width: 100%;
    border-radius: 10px;
}

.news-item h3 {
    margin-top: 10px;
    font-size: 20px;
}

.news-item a {
    color: #ea4c89;
    font-weight: bold;
}

/* Event Section */
.events {
    padding: 50px 20px;
    background-color: #f7f7f7;
}

.event-grid {
    display: flex;
    justify-content: space-around;
}

.event-item {
    text-align: center;
    padding: 20px;
    background-color: white;
    border-radius: 10px;
    width: 250px;
}


.teams {
    padding: 50px 20px;
}

.teams-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 20px;
}

.team {
    text-align: center;
    background-color: white;
    padding: 20px;
    border-radius: 10px;
}

.team img {
    width: 100%;
    border-radius: 10px;
}

/* Contact Section */
.contact {
    padding: 50px 20px;
    background-color: #ea4c89;
    color: white;
    text-align: center;
}

.contact form {
    max-width: 500px;
    margin: 0 auto;
    text-align: left;
}

.contact input, .contact textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border-radius: 5px;
    border: 1px solid #ddd;
}

.contact button {
    padding: 12px 30px;
    background-color: white;
    color: #ea4c89;
    font-weight: bold;
    border: none;
    cursor: pointer;
    border-radius: 5px;
}

.contact button:hover {
    background-color: #f7f7f7;
}

/* Footer Section */
.footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 20px;
}

```

## OUTPUT:

![Screenshot 2024-11-14 114229](https://github.com/user-attachments/assets/c6014595-9353-4163-ac1b-e426d25d4f51)
![Screenshot 2024-11-14 114248](https://github.com/user-attachments/assets/44cf7b6e-f7a4-485b-8560-f1807f385514)


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
