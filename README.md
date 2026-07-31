# Ex01 Portfolio
## Date:31/ 07/2026

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
```
index.html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="description" content="user portfolio" />
    <link href="style.css" rel="stylesheet" />
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css"
    />

    <title>Portfolio</title>
  </head>

  <body>
    <div class="container">
      <aside>
        <nav>
          <a href="#about"><i class="fa-solid fa-user"></i>About Me</a>
          <a href="#education"
            ><i class="fa-solid fa-graduation-cap"></i>Education</a
          >
          <a href="#skills"><i class="fa-solid fa-code"></i>Skills</a>
          <a href="#projects"
            ><i class="fa-solid fa-folder-open"></i>Projects</a
          >
          <a href="#contact"><i class="fa-solid fa-envelope"></i>Contact</a>
        </nav>
      </aside>

      <main>
        <section id="about">
          <div class="profile">
            <img src="pic.jpeg" />
            <h1>TANUSHREE G</h1>
            <p>Frontend developer and UI/UX designer</p>
          </div>
          <h2>About Me</h2>
          <p>
            I'm a second-year Computer Science and Engineering student who
            enjoys designing and developing user-friendly websites. I'm always
            eager to learn, explore emerging technologies, and deepen my
            knowledge of cybersecurity.
          </p>
        </section>

        <section id="skills">
          <h2>Skills</h2>
          <div class="skill-container">
            <div class="card">
              <h2>🌐 Web Development</h2>
              <ul>
                <li>HTML</li>
                <li>CSS</li>
                <li>JavaScript</li>
                <li>React</li>
                <li>Django</li>
              </ul>
            </div>

            <div class="card">
              <h2>💻 Programming</h2>
              <ul>
                <li>Python</li>
                <li>Java</li>
                <li>C</li>
              </ul>
            </div>

            <div class="card">
              <h2>🛠 Interests</h2>
              <ul>
                <li>Designing</li>
                <li>Cybersecurity</li>
              </ul>
            </div>
          </div>
        </section>

        <section id="education">
          <h2>Education</h2>
          <p>B.E. Computer Science and Engineering</p>
          <p>ABC Engineering College</p>
          <p>2025 – Present</p>
        </section>

        <section id="projects">
          <h2>Projects</h2>

          <div class="project-container">
            <div class="project-card">
              <h2>Portfolio Website</h2>

              <p>
                A personal portfolio website showcasing my skills, projects, and
                contact information.
              </p>
            </div>

            <div class="project-card">
              <h2>Todo List</h2>

              <p>
                A React-based task management application with add, delete, and
                edit functionality.
              </p>
            </div>

            <div class="project-card">
              <h2>Game UI Design</h2>

              <p>Designed the UI for an indie game.</p>
            </div>
          </div>
        </section>
      </main>

      <footer>
        <div class="left">
          <p>copyright&copy; Tanushree (25012099)</p>
        </div>

        <div class="right" id="contact">
          <h2>Contact</h2>
          <p>Email: tanushreeg@gmail.com</p>
          <p>Phone: 9347782197</p>

          <div class="socials">
            <i class="fa-brands fa-github"></i>
            <i class="fa-brands fa-linkedin"></i>
            <i class="fa-solid fa-envelope"></i>
          </div>
        </div>
      </footer>
    </div>
  </body>
</html>


```

```
style.css

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    background-color: #1A4A5A;
    color: rgb(3, 3, 23);
    font-size: 18px;
    font-family: 'Segoe UI', system-ui, sans-serif;
    line-height: 1.5;
}

.container{
    display: flex;
    flex-direction: column;
}

aside{
    position: fixed;
    top: 10px;
    right: 10px;
    width: 210px;
    height: auto;
    min-height: 340px;

    background-color: rgb(3, 3, 23);
    padding: 20px;
    font-size: 20px;
    border-radius: 30px;
    border-right: #EFBC75 outset 5px;
    border-bottom: #EFBC75 outset 5px;
    box-shadow: 0 10px 25px rgba(0,0,0,0.4);
    overflow: hidden;
}

nav{
    display: flex;
    flex-direction: column;
    gap: 15px;
}

nav a{
    color: #e8fcd8;
    text-decoration: none;
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 8px 15px;
    margin: 0 -15px;
    border-bottom: 2px solid rgba(230, 249, 214, 0.15);
    transition: color 0.2s ease, padding-left 0.2s ease;
}

nav a:hover{
    color: #EFBC75;
    padding-left: 20px;
}

nav a:last-child{
    border-bottom: none;
}

nav a i{
    width: 22px;
    font-size: 18px;
}

main{
    flex: 1;
    margin-right: 230px;
    padding: 50px;
}

.profile{
    margin-bottom: 40px;
}

.profile img{
    opacity: 0.8;
    width: 250px;
    height: 300px;
    object-fit: cover;
    border-radius: 15px;
    border: 5px outset #EFBC75;
    float: left;
    margin-right: 35px;
    margin-bottom: 20px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.35);
}

.profile h1{
    font-size: 42px;
    color: #e6f9d6;
    margin-bottom: 8px;
}

.profile p:last-child{
    font-size: 22px;
    color: #EFBC75;
    text-decoration: underline;
    text-decoration-color: #EFBC75;
    text-underline-offset: 5px;
}

#about{
    overflow: hidden;
}

#about h2{
    font-weight: bolder;
    font-size: 40px;
}

#about p{
    font-size: 19px;
    line-height: 1.7;
}

section{
    background-color: rgb(3, 3, 23);
    color: #e8fcd8;
    border-radius: 20px;
    padding: 35px;
    margin-bottom: 35px;
    box-shadow: 0 8px 20px rgba(0,0,0,0.3);
}

section h2{
    color: #EFBC75;
    margin-bottom: 20px;
    font-size: 28px;
}

.skill-container{
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
}

.card{
    background-color: #1A4A5A;
    border-radius: 15px;
    padding: 22px;
    flex: 1;
    min-width: 220px;
    transition: transform 0.2s ease;
}

.card:hover{
    transform: translateY(-5px);
}

.card h2{
    font-size: 22px;
    margin-bottom: 12px;
}

.card ul{
    list-style: disc;
    padding-left: 20px;
}

.card li{
    padding: 6px 0;
    color: #e8fcd8;
    font-size: 17px;
}

.card li::marker{
    color: #EFBC75;
}

.project-container{
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
}

.project-card{
    background-color: #1A4A5A;
    border-radius: 15px;
    padding: 22px;
    flex: 1;
    min-width: 250px;
    transition: transform 0.2s ease;
}

.project-card:hover{
    transform: translateY(-5px);
}

.project-card h2{
    font-size: 22px;
    margin-bottom: 12px;
}

.project-card p{
    font-size: 17px;
}

footer{
    border-top: 5px solid #EFBC75;
    display: flex;
    align-items: center;
    padding: 25px 5%;
    width: 100%;
    background-color: rgb(3, 3, 23);
    margin-top: 50px;
    color: #e6f9d6;
    font-size: 18px;
}

.left{
    flex: 1;
    display: flex;
    align-items: flex-start;
}

.right{
    border-left: 3px solid rgb(178, 211, 219);
    padding-left: 20px;
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 8px;
}

#contact{
    max-width: 250px;
}

#contact h2{
    font-size: 24px;
    color: #EFBC75;
    margin-bottom: 5px;
}

footer p{
    font-size: 18px;
}

.socials{
    display: flex;
    gap: 30px;
    font-size: 20px;
}

.socials i{
    transition: color 0.2s ease;
}

.socials i:hover{
    color: #EFBC75;
    cursor: pointer;
}
```

## OUTPUT
<img width="1920" height="1080" alt="Screenshot (422)" src="https://github.com/user-attachments/assets/7603fb14-770f-4465-a295-5db510e93572" />
<img width="1920" height="1080" alt="Screenshot (424)" src="https://github.com/user-attachments/assets/9d83a631-3958-4a83-9025-d31e123f9813" />
<img width="1920" height="1080" alt="Screenshot (425)" src="https://github.com/user-attachments/assets/e100173c-c42d-43ec-9522-0071d92454bf" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
