# **Creating and Uploading a Personal Portfolio Website on GitHub**

## **Introduction**
A personal portfolio website is a great way to showcase your skills, projects, and experience online. In this guide, we will go step by step on how to create a portfolio website using **HTML, CSS, and JavaScript** and host it on **GitHub Pages**.

---

## **Step 1: Planning Your Portfolio Website**
Before writing any code, you should plan the structure of your website. Your portfolio should include:
- **Homepage** (Introduction, About Me, Skills, Contact Information)
- **Projects Section** (Showcase your best work)
- **Resume or CV** (Downloadable PDF or online version)
- **Contact Form** (For visitors to reach out to you)
- **Social Media Links** (LinkedIn, GitHub, Twitter, etc.)

You can sketch a wireframe using tools like **Figma, Adobe XD, or even pen and paper**.

---

## **Step 2: Setting Up the Project Folder**

Create a new project folder on your computer:
```
portfolio-website/
   ├── index.html
   ├── style.css
   ├── script.js
   ├── images/
   ├── projects.html
   ├── contact.html
   ├── README.md
```

- `index.html`: Main landing page
- `style.css`: Stylesheet for design
- `script.js`: JavaScript file for interactivity
- `images/`: Folder for images and icons
- `projects.html`: Page for portfolio projects
- `contact.html`: Contact form page
- `README.md`: Project description

---

## **Step 3: Creating the HTML Structure**

### **Basic HTML Structure (`index.html`)**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Welcome to My Portfolio</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="projects.html">Projects</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>
    
    <section id="about">
        <h2>About Me</h2>
        <p>I am a web developer passionate about creating beautiful websites.</p>
    </section>
    
    <footer>
        <p>&copy; 2024 My Portfolio</p>
    </footer>
</body>
</html>
```

---

## **Step 4: Adding CSS for Styling**

### **Basic Styling (`style.css`)**
```css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    text-align: center;
}

header {
    background: #333;
    color: white;
    padding: 10px;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 10px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

section {
    padding: 20px;
}

footer {
    background: #333;
    color: white;
    padding: 10px;
    position: fixed;
    bottom: 0;
    width: 100%;
}
```

---

## **Step 5: Adding JavaScript for Interactivity**

### **Basic JavaScript (`script.js`)**
```js
document.addEventListener("DOMContentLoaded", function() {
    console.log("Welcome to My Portfolio Website!");
});
```
This script ensures the page loads properly and logs a message to the console.

---

## **Step 6: Uploading to GitHub**

### **Creating a GitHub Repository**
1. Go to [GitHub](https://github.com/) and log in.
2. Click on `+` (top right) and select **New repository**.
3. Name your repository, e.g., `personal-portfolio`.
4. Set it to **Public** or **Private**.
5. Click **Create repository**.

### **Uploading Files via Git**
Run these commands in the terminal:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/personal-portfolio.git
git push -u origin main
```

---

## **Step 7: Deploying with GitHub Pages**
1. Go to your repository settings.
2. Click on **Pages**.
3. Under "Source," select `main` branch and `/root`.
4. Click **Save**.
5. Your website will be live at `https://YOUR_USERNAME.github.io/personal-portfolio/`.


