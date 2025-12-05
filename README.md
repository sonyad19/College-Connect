
5. Scroll down → **Commit changes**.

---

### Step 2 – Add `index.html`

1. Again: **Add file → Create new file**  
2. Name: `index.html`  
3. Paste:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>College Connect</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link rel="stylesheet" href="style.css" />
</head>

<body>
  <header class="navbar">
    <div class="logo">College Connect</div>
    <nav class="nav-links">
      <a href="#home">Home</a>
      <a href="#events">Events</a>
      <a href="#community">Community</a>
      <a href="#about">About</a>
    </nav>
    <div class="auth-buttons">
      <button class="btn btn-outline">Log In</button>
      <button class="btn btn-primary">Sign Up</button>
    </div>
  </header>

  <main>
    <section id="home" class="hero">
      <div class="hero-text">
        <h1>Connect with your campus.</h1>
        <p>
          Find classmates, join clubs, discover events, and never miss out on what’s
          happening at your college.
        </p>
        <button class="btn btn-primary">Get Started</button>
      </div>
      <div class="hero-card">
        <h2>Today’s Highlights</h2>
        <ul id="highlights-list"></ul>
      </div>
    </section>

    <section id="events" class="section">
      <h2>Upcoming Events</h2>
      <div class="cards" id="events-container"></div>
    </section>

    <section id="community" class="section">
      <h2>Community Posts</h2>
      <div class="cards" id="posts-container"></div>
    </section>

    <section id="about" class="section about">
      <h2>About College Connect</h2>
      <p>
        College Connect is a student-focused platform designed to improve communication
        and collaboration on campus. This project is built as part of a Software
        Engineering / Agile course, demonstrating user stories, sprints, and iterative
        delivery.
      </p>
    </section>
  </main>

  <footer class="footer">
    <p>© 2025 College Connect · Built by Team 6</p>
  </footer>

  <script src="app.js"></script>
</body>
</html>
