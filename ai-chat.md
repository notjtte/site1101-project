# Personal portfolio HTML template
_Exported on 12/18/2025 at 22:42:41 GMT+4 from Cursor (2.2.36)_

---

**User**

I am a student in SITE. I need to build a personal portfolio with a Navigation bar, a footer and three pages (Home, about, projects). Can you provide me a clean HTML template for @index.html that includes a place for my profile photo and a footer with links to my Github and Codeacademy profiles?

---

**Cursor**


Reviewing the project structure, then creating a clean HTML template for the home page with a navigation bar, profile photo section, and footer.



Creating a clean HTML template for `index.html` with a navigation bar, profile photo section, and footer. Updating the other pages for consistency and adding basic CSS.


```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home - My Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="nav-logo">
                <a href="index.html">My Portfolio</a>
            </div>
            <ul class="nav-menu">
                <li><a href="index.html" class="nav-link active">Home</a></li>
                <li><a href="about.html" class="nav-link">About</a></li>
                <li><a href="projects.html" class="nav-link">Projects</a></li>
            </ul>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="main-content">
        <div class="container">
            <section class="hero">
                <div class="profile-section">
                    <div class="profile-photo-container">
                        <img src="profile-photo.jpg" alt="Profile Photo" class="profile-photo" id="profilePhoto">
                        <p class="photo-placeholder">Add your profile photo here</p>
                    </div>
                    <div class="hero-content">
                        <h1>Welcome to My Portfolio</h1>
                        <p class="subtitle">Student at SITE</p>
                        <p class="description">
                            This is my personal portfolio showcasing my work, skills, and projects.
                        </p>
                    </div>
                </div>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="footer">
        <div class="footer-container">
            <p class="footer-text">&copy; 2024 My Portfolio. All rights reserved.</p>
            <div class="footer-links">
                <a href="https://github.com/yourusername" target="_blank" rel="noopener noreferrer" class="footer-link">
                    GitHub
                </a>
                <a href="https://www.codecademy.com/profiles/yourusername" target="_blank" rel="noopener noreferrer" class="footer-link">
                    Codecademy
                </a>
            </div>
        </div>
    </footer>
</body>
</html>

```

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About - My Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="nav-logo">
                <a href="index.html">My Portfolio</a>
            </div>
            <ul class="nav-menu">
                <li><a href="index.html" class="nav-link">Home</a></li>
                <li><a href="about.html" class="nav-link active">About</a></li>
                <li><a href="projects.html" class="nav-link">Projects</a></li>
            </ul>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="main-content">
        <div class="container">
            <section class="page-section">
                <h1>About Me</h1>
                <p>Add your about content here.</p>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="footer">
        <div class="footer-container">
            <p class="footer-text">&copy; 2024 My Portfolio. All rights reserved.</p>
            <div class="footer-links">
                <a href="https://github.com/yourusername" target="_blank" rel="noopener noreferrer" class="footer-link">
                    GitHub
                </a>
                <a href="https://www.codecademy.com/profiles/yourusername" target="_blank" rel="noopener noreferrer" class="footer-link">
                    Codecademy
                </a>
            </div>
        </div>
    </footer>
</body>
</html>

```

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projects - My Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="nav-logo">
                <a href="index.html">My Portfolio</a>
            </div>
            <ul class="nav-menu">
                <li><a href="index.html" class="nav-link">Home</a></li>
                <li><a href="about.html" class="nav-link">About</a></li>
                <li><a href="projects.html" class="nav-link active">Projects</a></li>
            </ul>
        </div>
    </nav>

    <!-- Main Content -->
    <main class="main-content">
        <div class="container">
            <section class="page-section">
                <h1>My Projects</h1>
                <p>Add your projects here.</p>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="footer">
        <div class="footer-container">
            <p class="footer-text">&copy; 2024 My Portfolio. All rights reserved.</p>
            <div class="footer-links">
                <a href="https://github.com/yourusername" target="_blank" rel="noopener noreferrer" class="footer-link">
                    GitHub
                </a>
                <a href="https://www.codecademy.com/profiles/yourusername" target="_blank" rel="noopener noreferrer" class="footer-link">
                    Codecademy
                </a>
            </div>
        </div>
    </footer>
</body>
</html>

```

```css
/* Reset and Base Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
    line-height: 1.6;
    color: #333;
    background-color: #f5f5f5;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

/* Navigation Bar */
.navbar {
    background-color: #fff;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    padding: 1rem 0;
    position: sticky;
    top: 0;
    z-index: 100;
}

.nav-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 2rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav-logo a {
    font-size: 1.5rem;
    font-weight: bold;
    color: #333;
    text-decoration: none;
    transition: color 0.3s ease;
}

.nav-logo a:hover {
    color: #007bff;
}

.nav-menu {
    display: flex;
    list-style: none;
    gap: 2rem;
}

.nav-link {
    color: #333;
    text-decoration: none;
    font-weight: 500;
    transition: color 0.3s ease;
    position: relative;
}

.nav-link:hover {
    color: #007bff;
}

.nav-link.active {
    color: #007bff;
}

.nav-link.active::after {
    content: '';
    position: absolute;
    bottom: -5px;
    left: 0;
    width: 100%;
    height: 2px;
    background-color: #007bff;
}

/* Main Content */
.main-content {
    flex: 1;
    padding: 3rem 0;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 2rem;
}

/* Hero Section */
.hero {
    background-color: #fff;
    border-radius: 8px;
    padding: 3rem;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.profile-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 2rem;
}

.profile-photo-container {
    text-align: center;
}

.profile-photo {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    object-fit: cover;
    border: 4px solid #007bff;
    display: none;
}

.profile-photo-container:has(.profile-photo[src]) .photo-placeholder {
    display: none;
}

.profile-photo-container:has(.profile-photo[src]) .profile-photo {
    display: block;
}

.photo-placeholder {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    border: 4px dashed #ccc;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #999;
    font-size: 0.9rem;
    text-align: center;
    padding: 1rem;
    margin: 0 auto;
}

.hero-content {
    text-align: center;
}

.hero-content h1 {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
    color: #333;
}

.subtitle {
    font-size: 1.2rem;
    color: #666;
    margin-bottom: 1rem;
}

.description {
    font-size: 1.1rem;
    color: #555;
    max-width: 600px;
    margin: 0 auto;
}

/* Page Section (for About and Projects) */
.page-section {
    background-color: #fff;
    border-radius: 8px;
    padding: 3rem;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.page-section h1 {
    font-size: 2.5rem;
    margin-bottom: 1.5rem;
    color: #333;
}

.page-section p {
    font-size: 1.1rem;
    color: #555;
    line-height: 1.8;
}

/* Footer */
.footer {
    background-color: #333;
    color: #fff;
    padding: 2rem 0;
    margin-top: auto;
}

.footer-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 2rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 1rem;
}

.footer-text {
    margin: 0;
    color: #ccc;
}

.footer-links {
    display: flex;
    gap: 2rem;
}

.footer-link {
    color: #fff;
    text-decoration: none;
    font-weight: 500;
    transition: color 0.3s ease;
}

.footer-link:hover {
    color: #007bff;
}

/* Responsive Design */
@media (max-width: 768px) {
    .nav-container {
        flex-direction: column;
        gap: 1rem;
    }

    .nav-menu {
        gap: 1rem;
    }

    .hero-content h1 {
        font-size: 2rem;
    }

    .footer-container {
        flex-direction: column;
        text-align: center;
    }

    .profile-section {
        gap: 1.5rem;
    }
}

```


Created a clean HTML template for your portfolio. Here's what's included:

## What I've Created:

1. **index.html** — Home page with:
   - Navigation bar linking to Home, About, and Projects
   - Profile photo section (placeholder until you add your photo)
   - Footer with GitHub and Codecademy links

2. **about.html** and **projects.html** — Consistent navigation and footer

3. **style.css** — Styling with:
   - Responsive layout
   - Sticky navigation
   - Clean, modern design

## Next Steps:

1. Add your profile photo: Place an image named `profile-photo.jpg` in the same folder, or update the `src` attribute in `index.html` to point to your photo file.

2. Update the footer links: Replace `yourusername` in the GitHub and Codecademy URLs with your actual usernames.

3. Customize content: Add your information to the About and Projects pages.

The template is ready to use. Open `index.html` in a browser to view it. The navigation highlights the active page, and the layout is responsive for mobile devices.

