# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Flexbox Layout</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="content">
            <h1>Welcome to Our Website</h1>
            <p>This is a flexible and responsive layout using Flexbox and media queries.</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 My Website</p>
    </footer>
</body>
</html>
/* Resetting margin and padding */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Styling the body */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
}

/* Header and navigation */
header {
    background-color: #333;
    color: white;
    padding: 20px 0;
}

nav ul {
    display: flex;
    justify-content: center;
    list-style: none;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
    transition: color 0.3s;
}

nav ul li a:hover {
    color: #f4a261;
}

/* Main content area */
main {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 60vh;
    background-color: #f4f4f4;
    padding: 20px;
}

.content {
    text-align: center;
}

.content h1 {
    font-size: 2.5rem;
    margin-bottom: 20px;
}

.content p {
    font-size: 1.2rem;
}

/* Footer */
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
}

/* Media Query for Tablets and Below (600px or less) */
@media (max-width: 600px) {
    nav ul {
        flex-direction: column;
        align-items: center;
    }

    nav ul li {
        margin-bottom: 10px;
    }

    main {
        flex-direction: column;
        height: auto;
    }

    .content h1 {
        font-size: 2rem;
    }

    .content p {
        font-size: 1rem;
    }
}

/* Media Query for Larger Screens (above 600px) */
@media (min-width: 601px) {
    .content h1 {
        font-size: 3rem;
    }
}

Happy Coding! 💻✨
