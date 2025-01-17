<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Career Development & Skill Matching</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: #333;
            background-color: #f4f4f4;
        }

        header {
            background: linear-gradient(to right, #007BFF, #00C6FF);
            color: #fff;
            padding: 50px 0;
            text-align: center;
            background-image: url('https://via.placeholder.com/1920x500');
            background-size: cover;
            background-position: center;
            position: relative;
        }

        header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.5);
            z-index: 1;
        }

        header h1 {
            margin: 0;
            font-size: 3em;
            z-index: 2;
            position: relative;
        }

        header nav ul {
            list-style: none;
            padding: 0;
            margin: 20px 0 0;
            z-index: 2;
            position: relative;
        }

        header nav ul li {
            display: inline;
            margin-right: 15px;
        }

        header nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.2em;
            transition: color 0.3s;
        }

        header nav ul li a:hover {
            color: #00C6FF;
        }

        section {
            padding: 40px;
            background-color: #fff;
            margin: 20px 0;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease-in-out;
        }

        section:hover {
            transform: translateY(-10px);
        }

        section h2 {
            border-bottom: 3px solid #007BFF;
            padding-bottom: 10px;
            margin-bottom: 20px;
        }

        .container {
            width: 85%;
            margin: 0 auto;
            max-width: 1200px;
        }

        .checkbox-group label {
            display: block;
            margin-bottom: 10px;
        }

        form input[type="button"] {
            background-color: #007BFF;
            color: #fff;
            border: none;
            padding: 15px 30px;
            font-size: 1.2em;
            cursor: pointer;
            border-radius: 50px;
            transition: background-color 0.3s ease, transform 0.3s ease;
            margin-top: 20px;
            display: inline-block;
        }

        form input[type="button"]:hover {
            background-color: #0056b3;
            transform: translateY(-5px);
        }

        footer {
            background-color: #007BFF;
            color: #fff;
            text-align: center;
            padding: 20px 0;
            margin-top: 40px;
        }

        .job-recommendations, .study-recommendations {
            margin-top: 30px;
            padding: 20px;
            background-color: #e9ecef;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        .job-recommendations ul, .study-recommendations ul {
            list-style: none;
            padding: 0;
        }

        .job-recommendations li, .study-recommendations li {
            background-color: #fff;
            border-radius: 5px;
            padding: 10px;
            margin: 8px 0;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.05);
            transition: transform 0.2s;
        }

        .job-recommendations li:hover, .study-recommendations li:hover {
            transform: translateY(-5px);
        }

        .job-recommendations h3, .study-recommendations h3 {
            margin-top: 0;
            font-size: 1.5em;
            color: #007BFF;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Career Development & Skill Matching</h1>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#skills">Find Your Skills</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="home">
        <div class="container">
            <h2>Understanding Career Development</h2>
            <p>Career development is a dynamic and lifelong journey of learning, adapting, and building towards fulfilling work. Developing relevant skills is key to unlocking opportunities and staying competitive in the ever-changing job market. Whether you're at the beginning of your career or looking to transition to a new role, investing in your skillset will drive your career forward.</p>
        </div>
    </section>

    <section id="skills">
        <div class="container">
            <h2>Discover Your Skills and Explore Opportunities</h2>
            <p>Select the skills that resonate with you, and let's find your next career move:</p>
            <form id="skills-form">
                <div class="checkbox-group">
                    <label><input type="checkbox" name="skills" value="Programming"> Programming</label>
                    <label><input type="checkbox" name="skills" value="Design"> Design</label>
                    <label><input type="checkbox" name="skills" value="Data Science"> Data Science</label>
                    <label><input type="checkbox" name="skills" value="Project Management"> Project Management</label>
                    <label><input type="checkbox" name="skills" value="Marketing"> Marketing</label>
                    <label><input type="checkbox" name="skills" value="Communication"> Communication</label>
                    <label><input type="checkbox" name="skills" value="Leadership"> Leadership</label>
                    <label><input type="checkbox" name="skills" value="Finance"> Finance</label>
                    <label><input type="checkbox" name="skills" value="Sales"> Sales</label>
                    <label><input type="checkbox" name="skills" value="Cybersecurity"> Cybersecurity</label>
                    <label><input type="checkbox" name="skills" value="AI and Machine Learning"> AI and Machine Learning</label>
                    <label><input type="checkbox" name="skills" value="Cloud Computing"> Cloud Computing</label>
                    <label><input type="checkbox" name="skills" value="Blockchain"> Blockchain</label>
                    <label><input type="checkbox" name="skills" value="Business Analysis"> Business Analysis</label>
                    <label><input type="checkbox" name="skills" value="Graphic Design"> Graphic Design</label>
                    <label><input type="checkbox" name="skills" value="Web Development"> Web Development</label>
                    <label><input type="checkbox" name="skills" value="Database Management"> Database Management</label>
                    <label><input type="checkbox" name="skills" value="Networking"> Networking</label>
                    <label><input type="checkbox" name="skills" value="Technical Support"> Technical Support</label>
                </div>
                <input type="button" value="Show Job Recommendations" onclick="displayRecommendations()">
            </form>
            <div id="job-recommendations" class="job-recommendations"></div>
            <div id="study-recommendations" class="study-recommendations"></div>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <p>Have questions or need guidance? Reach out to us:</p>
            <address>
                <p>Email: <a href="mailto:support@careerfinder.com">support@careerfinder.com</a></p>
                <p>Phone: (123) 456-7890</p>
                <p>Address: 456 Career Lane, Skilltown, ST 67890</p>
            </address>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2024 Career Development & Skill Matching. All rights reserved.</p>
        </div>
    </footer>

    <script>
        function displayRecommendations() {
            const selectedSkills = Array.from(document.querySelectorAll('input[name="skills"]:checked'))
                .map(checkbox => checkbox.value);

            const recommendations = {
                'Programming': {
                    jobs: ['Software Developer', 'Web Developer', 'Data Scientist'],
                    study: ['Coursera', 'Udemy', 'Codecademy', 'MIT OpenCourseWare']
                },
                'Design': {
                    jobs: ['Graphic Designer', 'UX/UI Designer', 'Creative Director'],
                    study: ['Adobe Creative Cloud Tutorials', 'Skillshare', 'LinkedIn Learning', 'Canva Design School']
                },
                'Data Science': {
                    jobs: ['Data Analyst', 'Machine Learning Engineer', 'Data Scientist'],
                    study: ['DataCamp', 'Kaggle', 'Coursera', 'edX']
                },
                // Add other skill recommendations as needed
            };

            let jobs = new Set();
            let studies = new Set();

            selectedSkills.forEach(skill => {
                if (recommendations[skill]) {
                    recommendations[skill].jobs.forEach(job => jobs.add(job));
                    recommendations[skill].study.forEach(study => studies.add(study));
                }
            });

            document.getElementById('job-recommendations').innerHTML = '<h3>Job Recommendations:</h3><ul>' +
                Array.from(jobs).map(job => `<li>${job}</li>`).join('') +
                '</ul>';

            document.getElementById('study-recommendations').innerHTML = '<h3>Where to Study:</h3><ul>' +
                Array.from(studies).map(study => `<li>${study}</li>`).join('') +
                '</ul>';
        }
    </script>
</body>
</html>
