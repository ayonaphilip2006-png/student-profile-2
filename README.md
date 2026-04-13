<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Profile - Alex Johnson</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            background: white;
            border-radius: 10px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.3);
            overflow: hidden;
        }
        
        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 40px 20px;
            text-align: center;
        }
        
        .profile-photo {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 4px solid white;
            margin: 0 auto 20px;
            object-fit: cover;
            display: block;
        }
        
        .header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }
        
        .header p {
            font-size: 1.1em;
            opacity: 0.9;
        }
        
        .content {
            padding: 40px;
        }
        
        .section {
            margin-bottom: 35px;
        }
        
        .section h2 {
            color: #667eea;
            border-bottom: 3px solid #667eea;
            padding-bottom: 10px;
            margin-bottom: 20px;
            font-size: 1.8em;
        }
        
        .course-details {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            border-left: 4px solid #667eea;
        }
        
        .course-item {
            margin-bottom: 15px;
        }
        
        .course-item:last-child {
            margin-bottom: 0;
        }
        
        .course-item strong {
            color: #333;
            display: block;
            margin-bottom: 5px;
        }
        
        .course-item p {
            color: #666;
            margin-left: 10px;
            line-height: 1.5;
        }
        
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .skill-category {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            border-left: 4px solid #764ba2;
        }
        
        .skill-category h3 {
            color: #764ba2;
            margin-bottom: 12px;
            font-size: 1.2em;
        }
        
        .skill-category ul {
            list-style-position: inside;
            line-height: 1.8;
        }
        
        .skill-category li {
            color: #555;
            padding: 5px 0;
        }
        
        .skill-category li:before {
            content: "✓ ";
            color: #667eea;
            font-weight: bold;
            margin-right: 8px;
        }
        
        .contact-details {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .contact-item {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .contact-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.2);
        }
        
        .contact-item h3 {
            color: #667eea;
            margin-bottom: 10px;
            font-size: 1.1em;
        }
        
        .contact-item a {
            color: #764ba2;
            text-decoration: none;
            font-weight: 500;
            word-break: break-all;
            transition: color 0.3s ease;
        }
        
        .contact-item a:hover {
            color: #667eea;
            text-decoration: underline;
        }
        
        .contact-item p {
            color: #666;
            margin: 5px 0;
        }
        
        .footer {
            background: #f8f9fa;
            padding: 20px;
            text-align: center;
            color: #666;
            border-top: 1px solid #ddd;
        }
        
        @media (max-width: 768px) {
            .header h1 {
                font-size: 1.8em;
            }
            
            .content {
                padding: 20px;
            }
            
            .skills-container,
            .contact-details {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header Section -->
        <div class="header">
            <img src="https://via.placeholder.com/150" alt="Student Profile Photo" class="profile-photo">
            <h1>Alex Johnson</h1>
            <p>Computer Science Student</p>
        </div>
        
        <!-- Main Content -->
        <div class="content">
            <!-- Course Details Section -->
            <section class="section">
                <h2>📚 Course Details</h2>
                <div class="course-details">
                    <div class="course-item">
                        <strong>Program:</strong>
                        <p>Bachelor of Science in Computer Science</p>
                    </div>
                    <div class="course-item">
                        <strong>University:</strong>
                        <p>Tech University - Main Campus</p>
                    </div>
                    <div class="course-item">
                        <strong>Current Semester:</strong>
                        <p>5th Semester (Junior Year)</p>
                    </div>
                    <div class="course-item">
                        <strong>GPA:</strong>
                        <p>3.8 / 4.0</p>
                    </div>
                    <div class="course-item">
                        <strong>Expected Graduation:</strong>
                        <p>May 2027</p>
                    </div>
                </div>
            </section>
            
            <!-- Skills Section -->
            <section class="section">
                <h2>💡 Skills</h2>
                <div class="skills-container">
                    <!-- Programming Languages -->
                    <div class="skill-category">
                        <h3>Programming Languages</h3>
                        <ul>
                            <li>Python</li>
                            <li>JavaScript</li>
                            <li>Java</li>
                            <li>C++</li>
                            <li>SQL</li>
                        </ul>
                    </div>
                    
                    <!-- Web Development -->
                    <div class="skill-category">
                        <h3>Web Development</h3>
                        <ul>
                            <li>HTML5 & CSS3</li>
                            <li>React.js</li>
                            <li>Node.js</li>
                            <li>REST APIs</li>
                            <li>MongoDB</li>
                        </ul>
                    </div>
                    
                    <!-- Tools & Technologies -->
                    <div class="skill-category">
                        <h3>Tools & Technologies</h3>
                        <ul>
                            <li>Git & GitHub</li>
                            <li>Docker</li>
                            <li>VS Code</li>
                            <li>Figma</li>
                            <li>Agile Methodology</li>
                        </ul>
                    </div>
                </div>
            </section>
            
            <!-- Contact Details Section -->
            <section class="section">
                <h2>📞 Contact Details</h2>
                <div class="contact-details">
                    <div class="contact-item">
                        <h3>📧 Email</h3>
                        <a href="mailto:alex.johnson@techuniversity.edu">alex.johnson@techuniversity.edu</a>
                    </div>
                    <div class="contact-item">
                        <h3>📱 Phone</h3>
                        <a href="tel:+1-555-123-4567">+1 (555) 123-4567</a>
                    </div>
                    <div class="contact-item">
                        <h3>🔗 LinkedIn</h3>
                        <a href="https://linkedin.com/in/alexjohnson" target="_blank">linkedin.com/in/alexjohnson</a>
                    </div>
                    <div class="contact-item">
                        <h3>🐙 GitHub</h3>
                        <a href="https://github.com/alexjohnson" target="_blank">github.com/alexjohnson</a>
                    </div>
                    <div class="contact-item">
                        <h3>🐦 Twitter</h3>
                        <a href="https://twitter.com/alexjohnson" target="_blank">@alexjohnson</a>
                    </div>
                    <div class="contact-item">
                        <h3>📍 Location</h3>
                        <p>San Francisco, CA, USA</p>
                    </div>
                </div>
            </section>
        </div>
        
        <!-- Footer -->
        <div class="footer">
            <p>&copy; 2026 Alex Johnson. All rights reserved. | Last Updated: April 13, 2026</p>
        </div>
    </div>
</body>
</html>
