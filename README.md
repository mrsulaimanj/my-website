# my-website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sulaiman J. Adas | Business Leader & Strategist</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <main class="container">
        <header>
            <div class="header-top">
                <button id="theme-toggle" class="theme-btn">🌙 Dark Mode</button>
            </div>
            <h1>Sulaiman J. Adas</h1>
            <p class="tagline">Sales-Driven Business Leader & Operations Strategist</p>
        </header>

        <article class="content-section">
            <p><strong>Sulaiman</strong> J. Adas is a sales-driven business leader, operations strategist, and consultant with extensive experience helping companies grow revenue, optimize operations, and build high-performing teams. His background spans sales leadership, account management, training, and strategic consulting across multiple industries in both the Middle East and the United States.</p>
            <p>Sulaiman holds a <strong>Bachelor’s degree in Mechanical Engineering</strong> and began his career working in an engineering company, where he developed a strong foundation in structured problem-solving, process optimization, and real-world operational execution. This engineering background complements his commercial expertise, allowing him to approach business challenges with both analytical rigor and practical insight.</p>
            <p>As the <strong>Founder & CEO of Thrivals</strong>, Sulaiman has led consulting and implementation initiatives that enabled businesses to improve efficiency, scale operations, and increase performance through structured processes and modern tools. He has overseen the delivery of <strong> 8+ business programs</strong>, directly supporting the growth and expansion of <strong>over 5 companies</strong>, while also providing <strong>hands-on training to more than 200 professionals</strong> in sales, operations, and technology adoption.</p>
            <p>Sulaiman has a strong track record in <strong>sales execution and revenue growth</strong>. In technical and consultative sales roles, he consistently exceeded targets, closing <strong>over $120,000 in sales</strong> within short timeframes. His ability to combine consultative selling with a deep understanding of client needs allows him to deliver solutions that create long-term value rather than one-time transactions.</p>
            <p>In <strong>operations and account management leadership roles</strong>, Sulaiman managed onboarding, client success, and cross-functional teams, ensuring smooth delivery, retention, and operational excellence. He has led account management teams, improved onboarding processes, and aligned sales, operations, and service delivery to support sustainable growth.</p>
            <p><strong>Training and knowledge transfer</strong> are central to Sulaiman’s work. He has designed and delivered practical training programs focused on sales performance, operational efficiency, and technology enablement, equipping individuals and organizations with tools they can immediately apply. His training approach emphasizes clarity, execution, and measurable outcomes.</p>
         
            <section class="expertise">
                <h3>Sulaiman works closely with founders, executives, and teams to:</h3>
                <ul>
                    <li>Improve sales strategy and conversion</li>
                    <li>Optimize operations and workflows</li>
                    <li>Build scalable processes and teams</li>
                    <li>Implement practical training programs</li>
                    <li>Align strategy with execution</li>
                </ul>
            </section>

            <p>Sulaiman believes that successful businesses are built at the intersection of <strong>strong sales, efficient operations, and continuous learning</strong>. His mission is to help organizations grow with structure, discipline, and clear execution.</p>
        </article>

        <footer>
            <p>&copy; 2026 Sulaiman J. Adas | Consultant</p>
        </footer>
    </main>

    <script>
        const toggleBtn = document.getElementById('theme-toggle');
        const body = document.body;

        // Check for saved user preference
        if (localStorage.getItem('dark-mode') === 'enabled') {
            body.classList.add('dark-mode');
            toggleBtn.textContent = '☀️ Light Mode';
        }

        toggleBtn.addEventListener('click', () => {
            body.classList.toggle('dark-mode');
            
            if (body.classList.contains('dark-mode')) {
                toggleBtn.textContent = '☀️ Light Mode';
                localStorage.setItem('dark-mode', 'enabled');
            } else {
                toggleBtn.textContent = '🌙 Dark Mode';
                localStorage.setItem('dark-mode', 'disabled');
            }
        });
    </script>
</body>
</html>


/* 1. Global Styles & Reset */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
    line-height: 1.8;
    color: #2d3436;
    background-color: #f4f7f6;
    padding: 40px 20px;
    transition: background 0.3s ease, color 0.3s ease;
}

/* 2. Layout Container */
.container {
    max-width: 800px;
    margin: 0 auto;
    background: #ffffff;
    padding: 50px;
    border-radius: 12px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.05);
    transition: background 0.3s ease;
}

/* 3. Header & Toggle */
.header-top {
    display: flex;
    justify-content: flex-end;
    margin-bottom: 20px;
}

.theme-btn {
    cursor: pointer;
    padding: 8px 16px;
    border: 1px solid #0984e3;
    background: transparent;
    color: #0984e3;
    border-radius: 20px;
    font-weight: 600;
    font-size: 0.85rem;
    transition: 0.2s;
}

.theme-btn:hover {
    background: #0984e3;
    color: white;
}

header {
    text-align: center;
    border-bottom: 1px solid #eee;
    margin-bottom: 40px;
    padding-bottom: 30px;
}

h1 {
    font-size: 2.5rem;
    color: #2d3436;
    margin-bottom: 10px;
}

.tagline {
    color: #0984e3;
    font-weight: 500;
    font-size: 1.1rem;
}

/* 4. Content Styles */
.content-section p {
    margin-bottom: 20px;
    font-size: 1.1rem;
}

.expertise {
    background: #f8f9fa;
    padding: 30px;
    border-radius: 8px;
    margin: 30px 0;
    border-left: 5px solid #0984e3;
}

.expertise h3 {
    margin-bottom: 15px;
}

ul {
    padding-left: 20px;
}

li {
    margin-bottom: 10px;
}

footer {
    text-align: center;
    margin-top: 50px;
    font-size: 0.9rem;
    color: #999;
}

/* 5. Dark Mode Overrides */
.dark-mode {
    background-color: #121212;
    color: #e0e0e0;
}

.dark-mode .container {
    background-color: #1e1e1e;
    box-shadow: 0 10px 40px rgba(0,0,0,0.4);
}

.dark-mode h1, .dark-mode h3 {
    color: #ffffff;
}

.dark-mode .tagline {
    color: #74b9ff;
}

.dark-mode .expertise {
    background: #2d2d2d;
    color: #e0e0e0;
}

.dark-mode footer {
    color: #666;
}

/* 6. Mobile Responsiveness */
@media (max-width: 600px) {
    .container {
        padding: 25px;
    }
    h1 {
        font-size: 1.8rem;
    }
}
