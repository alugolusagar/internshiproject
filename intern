<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>StudentHub - Data Management</title>
    <style>
        :root {
            --bg: #0f0f12;
            --card: #1a1a20;
            --text: #e0e0e0;
            --accent: #00d4ff;
            --accent-dark: #00a8cc;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: var(--bg);
            color: var(--text);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        nav {
            background: rgba(26, 26, 32, 0.95);
            backdrop-filter: blur(10px);
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 1px solid #333;
        }
        
        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: var(--accent);
        }
        
        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }
        
        .nav-links a {
            color: var(--text);
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--accent);
        }
        
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            background: linear-gradient(135deg, #1a1a20 0%, #0a0a0f 100%);
            position: relative;
        }
        
        .hero-content {
            max-width: 800px;
            padding: 2rem;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            background: linear-gradient(90deg, #00d4ff, #ffffff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }
        
        .btn {
            display: inline-block;
            background: var(--accent);
            color: #000;
            padding: 14px 32px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s;
        }
        
        .btn:hover {
            background: #ffffff;
            transform: translateY(-3px);
        }
        
        section {
            padding: 5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .section-title {
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 3rem;
            color: var(--accent);
        }
        
        .dashboard-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
        }
        
        .card {
            background: var(--card);
            border-radius: 16px;
            padding: 2rem;
            border: 1px solid #333;
            transition: transform 0.3s;
        }
        
        .card:hover {
            transform: translateY(-8px);
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 1rem;
        }
        
        th, td {
            padding: 14px 12px;
            text-align: left;
            border-bottom: 1px solid #333;
        }
        
        th {
            background: #25252b;
            color: var(--accent);
        }
        
        tr:hover {
            background: #25252b;
        }
        
        .attendance-bar {
            height: 10px;
            background: linear-gradient(90deg, #00ff88, #00d4ff);
            border-radius: 5px;
            margin: 10px 0;
        }
        
        .stats {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin-bottom: 3rem;
        }
        
        .stat-card {
            background: var(--card);
            padding: 1.5rem;
            border-radius: 12px;
            text-align: center;
        }
        
        .stat-number {
            font-size: 2.8rem;
            font-weight: bold;
            color: var(--accent);
        }
        
        footer {
            background: #0a0a0f;
            padding: 3rem 2rem;
            text-align: center;
            border-top: 1px solid #333;
        }
        
        /* Contact Page Styles */
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background: var(--card);
            padding: 3rem;
            border-radius: 16px;
        }
        
        input, textarea {
            width: 100%;
            padding: 14px;
            margin-bottom: 1rem;
            background: #25252b;
            border: 1px solid #444;
            border-radius: 8px;
            color: white;
            font-size: 1rem;
        }
        
        input:focus, textarea:focus {
            outline: none;
            border-color: var(--accent);
        }
        
        .modal {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: var(--card);
            padding: 2rem;
            border-radius: 12px;
            z-index: 200;
            box-shadow: 0 0 30px rgba(0, 212, 255, 0.3);
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav>
        <div class="nav-container">
            <div class="logo">StudentHub</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#students">Students</a></li>
                <li><a href="#attendance">Attendance</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- HOME PAGE -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Student Data Management System</h1>
            <p>Modern, secure, and easy-to-use platform for managing student records, attendance, and academic performance.</p>
            <a href="#students" class="btn">Manage Students</a>
        </div>
    </section>

    <!-- Stats -->
    <section>
        <div class="stats">
            <div class="stat-card">
                <div class="stat-number">1248</div>
                <p>Total Students</p>
            </div>
            <div class="stat-card">
                <div class="stat-number">96%</div>
                <p>Average Attendance</p>
            </div>
            <div class="stat-card">
                <div class="stat-number">87</div>
                <p>Classes Today</p>
            </div>
            <div class="stat-card">
                <div class="stat-number">14</div>
                <p>Pending Reports</p>
            </div>
        </div>
    </section>

    <!-- Students Section -->
    <section id="students">
        <h2 class="section-title">Student Records</h2>
        <div class="card">
            <div style="display: flex; justify-content: space-between; margin-bottom: 1rem;">
                <h3>Student List</h3>
                <button onclick="addStudent()" style="background: var(--accent); color: black; border: none; padding: 10px 20px; border-radius: 8px; cursor: pointer;">+ Add Student</button>
            </div>
            
            <table id="studentTable">
                <thead>
                    <tr>
                        <th>ID</th>
                        <th>Name</th>
                        <th>Class</th>
                        <th>Email</th>
                        <th>Phone</th>
                        <th>Actions</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>S101</td>
                        <td>Aarav Sharma</td>
                        <td>10th A</td>
                        <td>aarav@school.edu</td>
                        <td>9876543210</td>
                        <td><button onclick="viewStudent(this)" style="background:#00d4ff; color:black; border:none; padding:6px 12px; border-radius:6px;">View</button></td>
                    </tr>
                    <tr>
                        <td>S102</td>
                        <td>Priya Patel</td>
                        <td>9th B</td>
                        <td>priya@school.edu</td>
                        <td>9876543211</td>
                        <td><button onclick="viewStudent(this)" style="background:#00d4ff; color:black; border:none; padding:6px 12px; border-radius:6px;">View</button></td>
                    </tr>
                    <tr>
                        <td>S103</td>
                        <td>Rohan Gupta</td>
                        <td>11th C</td>
                        <td>rohan@school.edu</td>
                        <td>9876543212</td>
                        <td><button onclick="viewStudent(this)" style="background:#00d4ff; color:black; border:none; padding:6px 12px; border-radius:6px;">View</button></td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <!-- Attendance Section -->
    <section id="attendance" style="background: #0a0a0f;">
        <h2 class="section-title">Attendance Overview</h2>
        <div class="dashboard-grid">
            <div class="card">
                <h3>Today's Attendance</h3>
                <div style="margin: 20px 0; font-size: 3rem; font-weight: bold; color: #00ff88;">92%</div>
                <div class="attendance-bar" style="width: 92%;"></div>
                <p><strong>Present:</strong> 187 | <strong>Absent:</strong> 16</p>
            </div>
            
            <div class="card">
                <h3>Monthly Summary</h3>
                <table>
                    <tr>
                        <td>Class 10A</td>
                        <td><div class="attendance-bar" style="width: 95%;"></div></td>
                        <td>95%</td>
                    </tr>
                    <tr>
                        <td>Class 9B</td>
                        <td><div class="attendance-bar" style="width: 88%;"></div></td>
                        <td>88%</td>
                    </tr>
                    <tr>
                        <td>Class 11C</td>
                        <td><div class="attendance-bar" style="width: 97%;"></div></td>
                        <td>97%</td>
                    </tr>
                </table>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 StudentHub • Student Data Management System</p>
        <p style="margin-top: 1rem; opacity: 0.7;">Dark Mode • Responsive Design</p>
    </footer>

    <!-- Simple Modal -->
    <div id="studentModal" class="modal">
        <h3 id="modalTitle">Student Details</h3>
        <p id="modalContent"></p>
        <button onclick="closeModal()" style="margin-top: 20px; padding: 10px 20px;">Close</button>
    </div>

    <script>
        // Add new student (demo)
        function addStudent() {
            const name = prompt("Enter student name:");
            if (!name) return;
            
            const table = document.getElementById('studentTable').getElementsByTagName('tbody')[0];
            const row = table.insertRow();
            
            const id = "S" + Math.floor(100 + Math.random() * 900);
            
            row.innerHTML = `
                <td>${id}</td>
                <td>${name}</td>
                <td>10th A</td>
                <td>${name.toLowerCase().replace(' ', '')}@school.edu</td>
                <td>98${Math.floor(10000000 + Math.random() * 90000000)}</td>
                <td><button onclick="viewStudent(this)" style="background:#00d4ff; color:black; border:none; padding:6px 12px; border-radius:6px;">View</button></td>
            `;
            
            alert("Student added successfully!");
        }
        
        function viewStudent(btn) {
            const row = btn.parentElement.parentElement;
            const cells = row.cells;
            
            const content = `
                <strong>ID:</strong> ${cells[0].textContent}<br>
                <strong>Name:</strong> ${cells[1].textContent}<br>
                <strong>Class:</strong> ${cells[2].textContent}<br>
                <strong>Email:</strong> ${cells[3].textContent}<br>
                <strong>Phone:</strong> ${cells[4].textContent}<br><br>
                <strong>Attendance:</strong> 94%<br>
                <strong>Last Updated:</strong> Today
            `;
            
            document.getElementById('modalContent').innerHTML = content;
            document.getElementById('modalTitle').textContent = cells[1].textContent + " - Profile";
            document.getElementById('studentModal').style.display = 'block';
        }
        
        function closeModal() {
            document.getElementById('studentModal').style.display = 'none';
        }
        
        // Keyboard support
        document.addEventListener('keydown', function(e) {
            if (e.key === "Escape") {
                const modal = document.getElementById('studentModal');
                if (modal.style.display === 'block') closeModal();
            }
        });
        
        // Welcome message
        console.log("%c✅ StudentHub loaded successfully in Dark Theme", "color: #00d4ff; font-size: 16px;");
    </script>
</body>
</html>
