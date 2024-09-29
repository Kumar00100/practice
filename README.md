<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Navbar with Dropdown</title>
    <link rel="stylesheet" href="navbar.css">
</head>
<body>
    <nav class="navbar">
        <div class="logo">MyWebsite</div>
        <ul class="nav-links">
            <li><a href="#">Home</a></li>
            <li>
                <a href="#" class="dropdown-toggle">Services</a>
                <ul class="dropdown">
                    <li><a href="#">Web Design</a></li>
                    <li><a href="#">SEO</a></li>
                    <li><a href="#">Marketing</a></li>
                </ul>
            </li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>
</body>
</html>
// Css part

body {
    margin: 0;
    font-family: Arial, sans-serif;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #4CAF50;
    padding: 10px 20px;
}

.logo {
    color: white;
    font-size: 24px;
    font-weight: bold;
}

.nav-links {
    list-style: none;
    display: flex;
    margin: 0;
    padding: 0;
}

.nav-links li {
    position: relative;
    margin-left: 20px;
}

.nav-links a {
    color: white;
    text-decoration: none;
    padding: 8px 16px;
}

.nav-links a:hover {
    background-color: #45a049;
    border-radius: 4px;
}

.dropdown {
    display: none;
    position: absolute;
    background-color: white;
    min-width: 160px;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    z-index: 1;
}

.dropdown li {
    margin: 0;
}

.dropdown a {
    color: #333;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
}

.dropdown a:hover {
    background-color: #f1f1f1;
}

.nav-links li:hover .dropdown {
    display: block;
}


