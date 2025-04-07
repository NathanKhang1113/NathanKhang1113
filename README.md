<!-- Folder Structure:
portfolio/
├── index.html (Resume)
├── cover-letter.html
├── career-goals.html
├── style.css
├── assets/
│   ├── image.jpg
│   ├── audio.mp3
│   └── video.mp4
-->

<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Resume</title>
    <link rel="stylesheet" href="style.css">
    <script>
        window.onload = function() {
            const dateDiv = document.getElementById("date");
            const today = new Date();
            dateDiv.textContent = today.toDateString();
            console.log("Resume page loaded on", today);
        };
    </script>
</head>
<body>
    <header>
        <h1>John Doe</h1>
        <p><em>Web Developer</em></p>
    </header>
    <nav>
        <ul>
            <li><a href="index.html">Resume</a></li>
            <li><a href="cover-letter.html">Cover Letter</a></li>
            <li><a href="career-goals.html">Career Goals</a></li>
        </ul>
    </nav>
    <main>
        <section>
            <h2>Profile</h2>
            <p><strong>Experienced developer</strong> with a passion for creating modern, user-friendly websites.</p>
        </section>
        <section>
            <h3>Skills</h3>
            <ul>
                <li>HTML</li>
                <li>CSS</li>
                <li>JavaScript</li>
            </ul>
        </section>
        <section>
            <h3>Experience</h3>
            <table>
                <caption>Work History</caption>
                <tr><th>Company</th><th>Role</th><th>Years</th><th>Location</th></tr>
                <tr><td>ABC Corp</td><td>Front-End Dev</td><td>2</td><td>New York</td></tr>
                <tr><td>XYZ Ltd</td><td>UI Designer</td><td>1</td><td>Boston</td></tr>
                <tr><td>123 Inc</td><td>Intern</td><td>0.5</td><td>Remote</td></tr>
            </table>
        </section>
        <hr>
        <section>
            <article>
                <h4>Education</h4>
                <p>B.S. in Computer Science, University of Technology</p>
            </article>
        </section>
        <br>
        <div id="date"></div>
    </main>
    <footer>
        <p><span>Email:</span> john@example.com</p>
    </footer>
</body>
</html>

<!-- cover-letter.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Cover Letter</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header><h1>Cover Letter</h1></header>
    <nav>
        <ul>
            <li><a href="index.html">Resume</a></li>
            <li><a href="cover-letter.html">Cover Letter</a></li>
            <li><a href="career-goals.html">Career Goals</a></li>
        </ul>
    </nav>
    <main>
        <section>
            <article>
                <p>Dear Hiring Manager,</p>
                <p><em>I am excited</em> to apply for the Web Developer role. With a background in <strong>modern front-end technologies</strong>, I am confident in my ability to contribute meaningfully to your team.</p>
                <p>I have experience with <mark>HTML, CSS, JavaScript</mark>, and I'm eager to continue growing in a collaborative environment.</p>
                <p>Sincerely,<br><span>John Doe</span></p>
            </article>
        </section>
        <hr>
    </main>
    <footer>
        <p>Contact me for more info</p>
    </footer>
</body>
</html>

<!-- career-goals.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Career Goals</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header><h1>Career Goals</h1></header>
    <nav>
        <ul>
            <li><a href="index.html">Resume</a></li>
            <li><a href="cover-letter.html">Cover Letter</a></li>
            <li><a href="career-goals.html">Career Goals</a></li>
        </ul>
    </nav>
    <main>
        <p>In the next five years, I aspire to become a full-stack web developer and lead innovative projects.</p>
        <img src="assets/image.jpg" alt="Career Vision" width="300">
        <audio controls>
            <source src="assets/audio.mp3" type="audio/mp3">
        </audio>
        <video width="320" height="240" controls>
            <source src="assets/video.mp4" type="video/mp4">
        </video>
        <form>
            <h2>Contact Me</h2>
            <label for="name">Name:</label>
            <input type="text" id="name" name="name"><br><br>
            <label for="message">Message:</label><br>
            <textarea id="message" name="message"></textarea><br><br>
            <input type="submit" value="Send">
        </form>
    </main>
    <footer>
        <p>Thank you for visiting my portfolio!</p>
    </footer>
</body>
</html>

/* style.css */
* {
    box-sizing: border-box;
}
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f5;
    color: #333;
    margin: 0;
    padding: 0;
}
header, footer {
    background-color: #333;
    color: white;
    padding: 1em;
    text-align: center;
}
nav ul {
    list-style-type: square;
    padding: 0;
}
nav li {
    display: inline;
    margin: 0 10px;
}
a:hover {
    color: red;
}
main {
    padding: 1em;
}
h1, h2, h3 {
    color: #004080;
}
span {
    font-style: italic;
}
#date {
    color: green;
    font-weight: bold;
}
.article-section strong {
    color: darkblue;
}
form input, form textarea {
    margin: 5px;
    padding: 5px;
    border: 1px solid #ccc;
}
img, audio, video {
    margin: 10px 0;
}
