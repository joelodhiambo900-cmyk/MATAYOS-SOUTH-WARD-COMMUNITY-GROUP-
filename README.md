# MATAYOS-SOUTH-WARD-COMMUNITY-GROUP-
Landing page for Matayos South Ward Community Group, promoting community growth, youth empowerment, and collaborative engagement. Features dynamic CTA buttons for Nasewa and Matayos blocs, responsive design, and placeholders for leadership info and images.
matayos-landing-page/
│
├── index.html          <-- Main landing page
├── style.css           <-- CSS styles
├── script.js           <-- Dynamic JS for buttons
└── images/             <-- Placeholder folder for your photos
      └── (add photos here later)<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Matayos South Ward Community Group</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Hero Section -->
    <header>
        <h1>MATAYOS SOUTH WARD COMMUNITY GROUP</h1>
        <p>Community Growth • Youth Empowerment • Sustainable Development</p>
        <div class="cta-buttons">
            <button class="nasewa-btn" id="nasewaBtn">NASEWA BLOC COMMUNITY GROUP</button>
            <button class="matayos-btn" id="matayosBtn">MATAYOS BLOC COMMUNITY GROUP</button>
        </div>
    </header>

    <!-- Focus Areas -->
    <section class="focus-areas">
        <div class="focus-card">
            <h3>Community Growth</h3>
            <p>Strengthening unity, proper structure, and ensuring long-term sustainability of our community.</p>
        </div>
        <div class="focus-card">
            <h3>Employment Opportunities</h3>
            <p>EPZ jobs and Nasewa Affordable Housing projects providing large-scale employment for youth.</p>
        </div>
        <div class="focus-card">
            <h3>Youth Empowerment</h3>
            <p>Prioritizing local youth for jobs, skills training, and active participation in community development.</p>
        </div>
        <div class="focus-card">
            <h3>Collaborative Engagement</h3>
            <p>Inclusive meetings where all members contribute ideas, raise concerns, and co-create solutions.</p>
        </div>
    </section>

    <!-- Administration Section -->
    <section class="administration">
        <h2>Administration & Leadership</h2>
        <div class="admin-list">
            <p>Administration list will be published here once finalized.</p>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>Hon. Lucas Wakuloba</p>
        <p>A Vision for Development & Unity</p>
        <p>&copy; 2026 Matayos South Ward Community Group</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>/* Reset & base styles */
* {margin:0; padding:0; box-sizing:border-box; font-family: 'Arial', sans-serif;}
body {background-color: #f4f7f9; color: #333;}
a {text-decoration: none;}
button {cursor: pointer;}

/* Header / Hero */
header {
    background: linear-gradient(135deg, #0d6efd, #6610f2);
    color: #fff;
    text-align: center;
    padding: 80px 20px;
}
header h1 {font-size: 2.8em; margin-bottom: 10px;}
header p {font-size: 1.2em; margin-bottom: 20px;}
header .cta-buttons button {
    padding: 15px 25px;
    margin: 10px;
    border: none;
    border-radius: 8px;
    font-size: 1em;
    font-weight: bold;
    transition: transform 0.2s;
}
header .cta-buttons button:hover {transform: scale(1.05);}
.nasewa-btn {background-color: #0dcaf0; color: #fff;}
.matayos-btn {background-color: #198754; color: #fff;}

/* Focus areas */
.focus-areas {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    padding: 60px 20px;
    text-align: center;
}
.focus-card {
    background: #fff;
    padding: 30px 20px;
    border-radius: 12px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.08);
    transition: transform 0.2s;
}
.focus-card:hover {transform: translateY(-5px);}
.focus-card h3 {color: #0d6efd; margin-bottom: 15px;}
.focus-card p {font-size: 0.95em; line-height: 1.5;}

/* Administration section */
.administration {
    background-color: #e9ecef;
    padding: 60px 20px;
    text-align: center;
}
.administration h2 {margin-bottom: 20px; color: #6610f2;}
.admin-list p {margin: 8px 0; font-weight: 500;}

/* Footer */
footer {
    background-color: #212529;
    color: #fff;
    padding: 40px 20px;
    text-align: center;
}
footer p {margin-bottom: 5px;}// Dynamic group links (update here when ready)
const groupLinks = {
    nasewa: "https://chat.whatsapp.com/your_nasewa_group_link_here",
    matayos: "https://chat.whatsapp.com/your_matayos_group_link_here"
};

// Assign links to buttons
document.getElementById('nasewaBtn').addEventListener('click', function() {
    window.open(groupLinks.nasewa, "_blank");
});

document.getElementById('matayosBtn').addEventListener('click', function() {
    window.open(groupLinks.matayos, "_blank");
});
