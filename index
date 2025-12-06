<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>College Connect • ECU</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>
    :root {
      --bg: #0f172a;
      --card: #020617;
      --accent: #f97316; /* ECU-ish orange */
      --accent-soft: rgba(249, 115, 22, 0.12);
      --border: #1e293b;
      --text-main: #e5e7eb;
      --text-muted: #9ca3af;
      --pill-bg: #111827;
      --like: #fb7185;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: "Poppins", system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
    }

    body {
      background: radial-gradient(circle at top, #1f2937 0, #020617 40%, #000 100%);
      color: var(--text-main);
      min-height: 100vh;
    }

    /* ---------- HEADER ---------- */
    header {
      position: sticky;
      top: 0;
      z-index: 20;
      backdrop-filter: blur(16px);
      background: linear-gradient(to right, rgba(15, 23, 42, 0.95), rgba(15, 23, 42, 0.8));
      border-bottom: 1px solid rgba(31, 41, 55, 0.9);
    }

    .header-inner {
      max-width: 1180px;
      margin: 0 auto;
      padding: 0.55rem 1.2rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 1rem;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 0.7rem;
    }

    .logo-wrap {
      width: 40px;
      height: 40px;
      border-radius: 999px;
      background: radial-gradient(circle at top, #f97316, #ea580c);
      padding: 2px;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 0 16px rgba(248, 113, 113, 0.55);
    }

    .logo-wrap img {
      width: 100%;
      height: 100%;
      border-radius: 999px;
      object-fit: contain;
      background: #f9fafb;
    }

    .brand-text h1 {
      font-size: 1.1rem;
      font-weight: 600;
      letter-spacing: 0.03em;
    }

    .brand-text span {
      display: block;
      font-size: 0.7rem;
      color: var(--text-muted);
    }

    .nav-right {
      display: flex;
      align-items: center;
      gap: 1.2rem;
    }

    .nav-links button {
      background: transparent;
      border: none;
      color: var(--text-muted);
      font-size: 0.8rem;
      cursor: pointer;
      padding: 0.2rem 0;
      position: relative;
    }

    .nav-links button::after {
      content: "";
      position: absolute;
      left: 0;
      bottom: -0.25rem;
      width: 0;
      height: 2px;
      background: var(--accent);
      border-radius: 999px;
      transition: width 0.18s ease;
    }

    .nav-links button:hover::after {
      width: 100%;
    }

    .user-select {
      display: flex;
      align-items: center;
      gap: 0.4rem;
      font-size: 0.75rem;
      color: var(--text-muted);
    }

    .user-select select {
      background: #020617;
      border-radius: 999px;
      border: 1px solid var(--border);
      color: var(--text-main);
      font-size: 0.78rem;
      padding: 0.15rem 0.6rem;
      outline: none;
    }

    /* ---------- LAYOUT ---------- */
    main {
      max-width: 1180px;
      margin: 1rem auto 2.2rem;
      padding: 0 1.2rem;
      display: grid;
      grid-template-columns: 2fr 1.05fr;
      gap: 1rem;
    }

    @media (max-width: 900px) {
      main {
        grid-template-columns: 1fr;
      }
      .header-inner {
        flex-wrap: wrap;
      }
    }

    .card {
      background: radial-gradient(circle at top left, rgba(15, 23, 42, 1), var(--card));
      border-radius: 1.1rem;
      border: 1px solid var(--border);
      padding: 0.9rem 1rem;
      box-shadow: 0 18px 40px rgba(0, 0, 0, 0.7);
      margin-bottom: 0.9rem;
    }

    .card-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 0.35rem;
    }

    .card-header h2 {
      font-size: 0.98rem;
      font-weight: 600;
    }

    .badge {
      font-size: 0.68rem;
      padding: 0.15rem 0.6rem;
      border-radius: 999px;
      background: var(--pill-bg);
      color: var(--accent);
      border: 1px solid rgba(248, 113, 22, 0.3);
    }

    .subtext {
      font-size: 0.78rem;
      color: var(--text-muted);
      margin-bottom: 0.6rem;
    }

    label {
      font-size: 0.7rem;
      color: var(--text-muted);
      display: block;
      margin-bottom: 0.18rem;
    }

    input[type="text"],
    textarea,
    select.inputlike {
      width: 100%;
      background: #020617;
      border-radius: 0.7rem;
      border: 1px solid #1f2937;
      padding: 0.45rem 0.7rem;
      font-size: 0.78rem;
      color: var(--text-main);
      outline: none;
      margin-bottom: 0.45rem;
    }

    input::placeholder,
    textarea::placeholder {
      color: #6b7280;
    }

    input:focus,
    textarea:focus,
    select.inputlike:focus {
      border-color: var(--accent);
      box-shadow: 0 0 0 1px rgba(249, 115, 22, 0.5);
    }

    textarea {
      resize: vertical;
      min-height: 60px;
    }

    button.primary {
      border-radius: 999px;
      border: none;
      background: linear-gradient(135deg, var(--accent), #fb923c);
      color: #111827;
      font-size: 0.78rem;
      padding: 0.35rem 0.95rem;
      cursor: pointer;
      font-weight: 500;
      display: inline-flex;
      align-items: center;
      gap: 0.25rem;
      box-shadow: 0 10px 24px rgba(249, 115, 22, 0.55);
    }

    button.primary:hover {
      filter: brightness(1.05);
      transform: translateY(-0.5px);
    }

    button.chip {
      border-radius: 999px;
      border: none;
      background: var(--pill-bg);
      color: var(--text-muted);
      font-size: 0.68rem;
      padding: 0.22rem 0.6rem;
      cursor: pointer;
    }

    button.chip.active {
      background: var(--accent-soft);
      color: var(--accent);
      border: 1px solid rgba(249, 115, 22, 0.7);
    }

    /* ---------- POSTS FEED ---------- */
    .feed-controls {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 0.25rem;
      gap: 0.5rem;
    }

    .post-list {
      margin-top: 0.4rem;
      display: flex;
      flex-direction: column;
      gap: 0.55rem;
    }

    .post {
      border-radius: 0.9rem;
      border: 1px solid #1f2937;
      padding: 0.65rem 0.7rem;
      background: radial-gradient(circle at top left, #020617, #020617);
      box-shadow: 0 10px 24px rgba(0, 0, 0, 0.65);
    }

    .post-header {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      margin-bottom: 0.32rem;
      gap: 0.5rem;
    }

    .post-user {
      display: flex;
      align-items: center;
      gap: 0.45rem;
    }

    .avatar {
      width: 30px;
      height: 30px;
      border-radius: 999px;
      background: var(--pill-bg);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      font-size: 0.8rem;
      font-weight: 600;
      border: 1px solid rgba(148, 163, 184, 0.7);
    }

    .user-meta {
      font-size: 0.78rem;
    }

    .user-meta .name {
      font-weight: 500;
    }

    .user-meta .course {
      font-size: 0.68rem;
      color: var(--text-muted);
    }

    .post-time {
      font-size: 0.65rem;
      color: var(--text-muted);
      text-align: right;
    }

    .post-body {
      font-size: 0.82rem;
      color: #e5e7eb;
      margin-bottom: 0.45rem;
      white-space: pre-line;
    }

    .post-tags {
      font-size: 0.68rem;
      color: var(--accent);
      margin-bottom: 0.3rem;
    }

    .post-actions {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-top: 0.1rem;
      font-size: 0.72rem;
      color: var(--text-muted);
      gap: 0.5rem;
      flex-wrap: wrap;
    }

    .action-buttons {
      display: flex;
      gap: 0.4rem;
    }

    .action-btn {
      background: transparent;
      border: none;
      color: var(--text-muted);
      font-size: 0.75rem;
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      gap: 0.25rem;
      padding: 0;
    }

    .action-btn.like.active {
      color: var(--like);
    }

    .action-btn:hover {
      color: #e5e7eb;
    }

    .likes-summary {
      font-size: 0.7rem;
      color: var(--text-muted);
    }

    /* ---------- COMMENTS ---------- */
    .comments {
      border-top: 1px solid #111827;
      margin-top: 0.45rem;
      padding-top: 0.4rem;
    }

    .comment {
      font-size: 0.75rem;
      color: var(--text-main);
      margin-bottom: 0.25rem;
      display: flex;
      gap: 0.35rem;
    }

    .comment span.name {
      font-weight: 500;
      color: #e5e7eb;
    }

    .comment span.text {
      color: #d1d5db;
    }

    .add-comment {
      margin-top: 0.3rem;
      display: flex;
      gap: 0.3rem;
    }

    .add-comment input {
      flex: 1;
      font-size: 0.75rem;
      padding: 0.3rem 0.6rem;
    }

    .add-comment button {
      font-size: 0.7rem;
      padding: 0.26rem 0.6rem;
      box-shadow: none;
    }

    /* ---------- SIDEBAR ---------- */
    .student-list {
      display: flex;
      flex-direction: column;
      gap: 0.35rem;
      margin-top: 0.3rem;
    }

    .student-row {
      display: flex;
      align-items: center;
      justify-content: space-between;
      font-size: 0.76rem;
    }

    .student-row .left {
      display: flex;
      align-items: center;
      gap: 0.4rem;
    }

    .status-dot {
      width: 7px;
      height: 7px;
      border-radius: 999px;
      background: #22c55e;
      box-shadow: 0 0 0 4px rgba(34, 197, 94, 0.18);
    }

    .student-role {
      font-size: 0.64rem;
      color: var(--text-muted);
    }

    .pill {
      font-size: 0.65rem;
      padding: 0.18rem 0.5rem;
      border-radius: 999px;
      background: #111827;
      color: var(--text-muted);
    }

    footer {
      text-align: center;
      font-size: 0.7rem;
      color: var(--text-muted);
      padding-bottom: 1.5rem;
    }
  </style>
</head>
<body>
  <!-- HEADER -->
  <header>
    <div class="header-inner">
      <div class="brand">
        <div class="logo-wrap">
          <!-- Make sure eculogo.png is in the same folder as this file -->
          <img src="eculogo.png" alt="ECU Logo">
        </div>
        <div class="brand-text">
          <h1>College Connect • ECU</h1>
          <span>Classroom social hub for students to share, study & stay updated</span>
        </div>
      </div>

      <div class="nav-right">
        <div class="nav-links">
          <button onclick="scrollToSection('compose')">Feed</button>
          <button onclick="scrollToSection('students-card')">Students</button>
          <button onclick="scrollToSection('events-card')">Events</button>
        </div>
        <div class="user-select">
          <span>You are:</span>
          <select id="currentUserSelect"></select>
        </div>
      </div>
    </div>
  </header>

  <!-- MAIN -->
  <main>
    <!-- LEFT: compose + feed -->
    <section>
      <!-- Compose -->
      <div class="card" id="compose">
        <div class="card-header">
          <h2>Create a post</h2>
          <span class="badge">Live demo • No backend</span>
        </div>
        <p class="subtext">
          Share class questions, project updates, or campus news. You are posting as
          <span id="currentUserLabel" style="color: var(--accent); font-weight:500;"></span>.
        </p>

        <label for="postCourse">Course / Topic (optional)</label>
        <input id="postCourse" type="text" placeholder="e.g., CPSMA 3813, Operating Systems">

        <label for="postBody">What would you like to share?</label>
        <textarea id="postBody" placeholder="Ask for help, share resources, or plan a study group..."></textarea>

        <div class="feed-controls">
          <div>
            <button class="chip active" id="filter-all" onclick="setFilter('all')">All posts</button>
            <button class="chip" id="filter-mine" onclick="setFilter('mine')">My posts</button>
            <button class="chip" id="filter-course" onclick="setFilter('sameCourse')">Same course</button>
          </div>
          <button class="primary" onclick="createPost()">
            <span>➕ Post</span>
          </button>
        </div>
      </div>

      <!-- Feed -->
      <div class="card">
        <div class="card-header">
          <h2>Activity Feed</h2>
          <span class="badge" id="post-count">0 posts</span>
        </div>
        <p class="subtext" id="filterLabel">Showing all posts from the class.</p>

        <div id="postList" class="post-list"></div>
      </div>
    </section>

    <!-- RIGHT: students & events -->
    <section>
      <div class="card" id="students-card">
        <div class="card-header">
          <h2>Students in this space</h2>
          <span class="badge" id="student-count">0 online</span>
        </div>
        <p class="subtext">
          15 demo students are pre-loaded so you can switch perspectives and interact with posts.
        </p>
        <div class="student-list" id="studentList"></div>
      </div>

      <div class="card" id="events-card">
        <div class="card-header">
          <h2>Upcoming items</h2>
          <span class="badge">Demo data</span>
        </div>
        <p class="subtext">
          Example deadlines & meetups. In a real system these could come from a backend or campus calendar.
        </p>
        <ul style="font-size:0.78rem; color:var(--text-muted); list-style:none; padding-left:0;">
          <li style="margin-bottom:0.3rem;">
            <span class="pill">Dec 08</span>
            <span style="margin-left:0.4rem; color:var(--text-main);">OS project standup</span>
            <span style="display:block; margin-left:2.2rem;">Zoom • 7:00 PM</span>
          </li>
          <li style="margin-bottom:0.3rem;">
            <span class="pill">Dec 12</span>
            <span style="margin-left:0.4rem; color:var(--text-main);">Data Mining final report due</span>
            <span style="display:block; margin-left:2.2rem;">Canvas • 11:59 PM</span>
          </li>
          <li>
            <span class="pill">Dec 15</span>
            <span style="margin-left:0.4rem; color:var(--text-main);">College Connect demo day</span>
            <span style="display:block; margin-left:2.2rem;">CS Lab • 2:30 PM</span>
          </li>
        </ul>
      </div>
    </section>
  </main>

  <footer>
    College Connect • ECU • Front-end prototype (HTML, CSS, JavaScript only)
  </footer>

  <script>
    /* ---------- DATA ---------- */

    const students = [
      { id: 1, name: "Sonu Yadav", major: "Computer Science", role: "Scrum Master", courseFocus: "Operating Systems" },
      { id: 2, name: "Syntheia Harper", major: "Computer Science", role: "Product Owner", courseFocus: "Agile Software" },
      { id: 3, name: "Suman Budhathoki", major: "Computer Science", role: "Developer", courseFocus: "Data Mining" },
      { id: 4, name: "Prinsa Ghimire", major: "Design", role: "UI/UX", courseFocus: "HCI" },
      { id: 5, name: "Samrat Rijal", major: "Computer Science", role: "Testing", courseFocus: "Software Quality" },
      { id: 6, name: "Birat Bhatta", major: "Computer Science", role: "Testing", courseFocus: "Databases" },
      { id: 7, name: "Alex Johnson", major: "Math", role: "Student", courseFocus: "Discrete Structures" },
      { id: 8, name: "Maria Lopez", major: "CS", role: "Student", courseFocus: "Networks" },
      { id: 9, name: "Jordan Kim", major: "CS", role: "Student", courseFocus: "Data Structures" },
      { id: 10, name: "Taylor Smith", major: "CS", role: "Student", courseFocus: "Web Dev" },
      { id: 11, name: "Riya Patel", major: "IT", role: "Student", courseFocus: "Cybersecurity" },
      { id: 12, name: "Chris Evans", major: "CS", role: "Student", courseFocus: "AI" },
      { id: 13, name: "Emily Zhang", major: "CS", role: "Student", courseFocus: "Machine Learning" },
      { id: 14, name: "Liam Brown", major: "CS", role: "Student", courseFocus: "OS" },
      { id: 15, name: "Olivia Davis", major: "CS", role: "Student", courseFocus: "Data Mining" },
    ];

    const STORAGE_KEY = "college_connect_ecu_v1";

    function defaultPosts() {
      return [
        {
          id: Date.now() - 1000000,
          authorId: 1,
          body: "Hey everyone! I created this College Connect demo so we can share questions and plan study sessions. Feel free to post, like, and comment to try it out 👋",
          course: "College Connect / CS",
          createdAt: new Date().toISOString(),
          likes: [2, 3, 4],
          comments: [
            { id: 1, authorId: 2, text: "Looks awesome, Sonu! This will be perfect for our Agile class demo." },
            { id: 2, authorId: 3, text: "Nice! Can we also use it to track Data Mining group work?" },
          ],
        },
        {
          id: Date.now() - 800000,
          authorId: 3,
          body: "Does anyone have good resources for K-means vs DBSCAN? Need to finalize clustering part of the project.",
          course: "CPSMA 3813 Data Mining",
          createdAt: new Date().toISOString(),
          likes: [1, 13, 15],
          comments: [
            { id: 3, authorId: 13, text: "I can share my slides from last semester. I’ll post them here later today." },
          ],
        },
        {
          id: Date.now() - 600000,
          authorId: 5,
          body: "Reminder: we should run one more round of test cases on College Connect before we demo it.",
          course: "Software Testing",
          createdAt: new Date().toISOString(),
          likes: [1, 2, 6],
          comments: [],
        },
        {
          id: Date.now() - 400000,
          authorId: 10,
          body: "Anyone interested in making the UI even more polished? I can help tweak colors and layout.",
          course: "Web Development",
          createdAt: new Date().toISOString(),
          likes: [4, 7, 8, 9],
          comments: [
            { id: 4, authorId: 4, text: "Yes! Let’s meet after class and try a new layout." },
          ],
        },
      ];
    }

    function loadData() {
      try {
        const raw = localStorage.getItem(STORAGE_KEY);
        if (!raw) return { posts: defaultPosts() };
        const parsed = JSON.parse(raw);
        if (!parsed.posts) parsed.posts = defaultPosts();
        return parsed;
      } catch {
        return { posts: defaultPosts() };
      }
    }

    function saveData() {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(state));
    }

    let state = loadData();
    let currentUserId = 1;
    let currentFilter = "all"; // all | mine | sameCourse

    /* ---------- UTILITIES ---------- */

    function getStudentById(id) {
      return students.find(s => s.id === id);
    }

    function formatTime(iso) {
      const date = new Date(iso);
      return date.toLocaleString(undefined, {
        month: "short",
        day: "numeric",
        hour: "numeric",
        minute: "2-digit",
      });
    }

    function scrollToSection(id) {
      const el = document.getElementById(id);
      if (!el) return;
      window.scrollTo({
        top: el.getBoundingClientRect().top + window.scrollY - 80,
        behavior: "smooth",
      });
    }

    /* ---------- RENDER FUNCTIONS ---------- */

    function renderStudents() {
      const list = document.getElementById("studentList");
      const select = document.getElementById("currentUserSelect");
      list.innerHTML = "";
      select.innerHTML = "";

      students.forEach((s, idx) => {
        // sidebar row
        const row = document.createElement("div");
        row.className = "student-row";
        row.innerHTML = `
          <div class="left">
            <div class="avatar" style="font-size:0.72rem;">${s.name.split(" ").map(p => p[0]).join("")}</div>
            <div>
              <div>${s.name}</div>
              <div class="student-role">${s.major} • ${s.courseFocus}</div>
            </div>
          </div>
          <div style="display:flex;align-items:center;gap:0.3rem;">
            ${idx < 10 ? '<span class="status-dot"></span>' : ""}
            <span class="pill">${s.role}</span>
          </div>
        `;
        list.appendChild(row);

        // select option
        const opt = document.createElement("option");
        opt.value = s.id;
        opt.textContent = s.name;
        select.appendChild(opt);
      });

      select.value = currentUserId;
      document.getElementById("student-count").textContent = `${students.length} students`;
      updateCurrentUserLabel();
    }

    function updateCurrentUserLabel() {
      const user = getStudentById(currentUserId);
      const label = document.getElementById("currentUserLabel");
      if (user) label.textContent = user.name;
    }

    function applyFilter(posts) {
      const user = getStudentById(currentUserId);
      if (currentFilter === "mine") {
        return posts.filter(p => p.authorId === currentUserId);
      }
      if (currentFilter === "sameCourse" && user) {
        // simple: filter if course text contains the user's course focus keyword
        const keyword = user.courseFocus?.split(" ")[0]?.toLowerCase() || "";
        return posts.filter(p => (p.course || "").toLowerCase().includes(keyword));
      }
      return posts;
    }

    function setFilter(filter) {
      currentFilter = filter;
      document.getElementById("filter-all").classList.toggle("active", filter === "all");
      document.getElementById("filter-mine").classList.toggle("active", filter === "mine");
      document.getElementById("filter-course").classList.toggle("active", filter === "sameCourse");

      const label = document.getElementById("filterLabel");
      if (filter === "all") label.textContent = "Showing all posts from the class.";
      if (filter === "mine") label.textContent = "Showing only posts created by you.";
      if (filter === "sameCourse") label.textContent = "Showing posts related to your focus course.";
      renderPosts();
    }

    function renderPosts() {
      const list = document.getElementById("postList");
      list.innerHTML = "";

      let posts = state.posts.slice().sort((a, b) => b.id - a.id);
      posts = applyFilter(posts);

      const count = state.posts.length;
      document.getElementById("post-count").textContent = `${count} post${count === 1 ? "" : "s"}`;

      if (!posts.length) {
        const p = document.createElement("p");
        p.className = "subtext";
        p.textContent = "No posts match this filter yet — try creating one!";
        list.appendChild(p);
        return;
      }

      posts.forEach(post => {
        const author = getStudentById(post.authorId) || { name: "Unknown", courseFocus: "" };
        const likes = post.likes || [];
        const comments = post.comments || [];
        const youLiked = likes.includes(currentUserId);

        const div = document.createElement("div");
        div.className = "post";
        div.innerHTML = `
          <div class="post-header">
            <div class="post-user">
              <div class="avatar">${author.name.split(" ").map(p => p[0]).join("")}</div>
              <div class="user-meta">
                <div class="name">${author.name}</div>
                <div class="course">${post.course || author.courseFocus || "General"}</div>
              </div>
            </div>
            <div class="post-time">${formatTime(post.createdAt)}</div>
          </div>
          <div class="post-body">${escapeHtml(post.body)}</div>
          ${post.course ? `<div class="post-tags">#${post.course}</div>` : ""}
          <div class="post-actions">
            <div class="action-buttons">
              <button class="action-btn like ${youLiked ? "active" : ""}" onclick="toggleLike(${post.id})">
                <span>${youLiked ? "♥" : "♡"}</span>
                <span>Like</span>
              </button>
              <button class="action-btn" onclick="focusCommentInput(${post.id})">
                💬 <span>Comment</span>
              </button>
            </div>
            <div class="likes-summary">
              ${likes.length ? likesSummaryText(likes) : "No likes yet"}
            </div>
          </div>
          <div class="comments" id="comments-${post.id}">
            ${comments.map(c => renderCommentHTML(c)).join("")}
            <div class="add-comment">
              <input type="text" id="comment-input-${post.id}" placeholder="Write a comment as ${getStudentById(currentUserId).name}..." />
              <button class="primary" onclick="addComment(${post.id})">Post</button>
            </div>
          </div>
        `;
        list.appendChild(div);
      });
    }

    function renderCommentHTML(comment) {
      const author = getStudentById(comment.authorId) || { name: "Unknown" };
      return `
        <div class="comment">
          <span class="name">${author.name}:</span>
          <span class="text">${escapeHtml(comment.text)}</span>
        </div>
      `;
    }

    function likesSummaryText(likes) {
      const names = likes.slice(0, 3).map(id => getStudentById(id)?.name.split(" ")[0] || "Someone");
      const extra = likes.length - names.length;
      let base = names.join(", ");
      if (extra > 0) base += ` + ${extra} more`;
      return `${likes.length} like${likes.length === 1 ? "" : "s"} • ${base}`;
    }

    /* ---------- ACTIONS ---------- */

    function createPost() {
      const bodyInput = document.getElementById("postBody");
      const courseInput = document.getElementById("postCourse");
      const body = bodyInput.value.trim();
      const course = courseInput.value.trim();

      if (!body) {
        alert("Please write something before posting.");
        return;
      }

      const post = {
        id: Date.now(),
        authorId: currentUserId,
        body,
        course,
        createdAt: new Date().toISOString(),
        likes: [],
        comments: [],
      };

      state.posts.push(post);
      saveData();
      bodyInput.value = "";
      courseInput.value = "";
      setFilter(currentFilter); // re-render with same filter
    }

    function toggleLike(postId) {
      const post = state.posts.find(p => p.id === postId);
      if (!post) return;
      if (!post.likes) post.likes = [];

      const idx = post.likes.indexOf(currentUserId);
      if (idx === -1) {
        post.likes.push(currentUserId);
      } else {
        post.likes.splice(idx, 1);
      }
      saveData();
      renderPosts();
    }

    function addComment(postId) {
      const input = document.getElementById(`comment-input-${postId}`);
      if (!input) return;
      const text = input.value.trim();
      if (!text) return;

      const post = state.posts.find(p => p.id === postId);
      if (!post) return;
      if (!post.comments) post.comments = [];

      const newComment = {
        id: Date.now(),
        authorId: currentUserId,
        text,
      };
      post.comments.push(newComment);
      input.value = "";
      saveData();
      renderPosts();
      focusCommentInput(postId);
    }

    function focusCommentInput(postId) {
      const input = document.getElementById(`comment-input-${postId}`);
      if (input) input.focus();
    }

    function escapeHtml(text) {
      return text
        .replace(/&/g, "&amp;")
        .replace(/</g, "&lt;")
        .replace(/>/g, "&gt;");
    }

    /* ---------- INIT ---------- */

    function init() {
      // populate user select + sidebar
      renderStudents();

      document.getElementById("currentUserSelect").addEventListener("change", (e) => {
        currentUserId = Number(e.target.value);
        updateCurrentUserLabel();
        renderPosts();
      });

      setFilter("all");
    }

    init();
  </script>
</body>
</html>
