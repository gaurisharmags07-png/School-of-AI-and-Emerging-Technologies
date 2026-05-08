# School-of-AI-and-Emerging-Technologies
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Meta tags for character encoding and viewport responsiveness -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>School of AI and Emerging Technologies</title>
    
    <!-- Internal CSS Styling -->
    <style>
        /* ========================================
           1. GENERAL STYLES & RESET
           ======================================== */
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f4f4f4;
        }
        
        /* ========================================
           2. HEADER & NAVIGATION
           ======================================== */
        
        header {
            background-color: #0066cc;
            color: white;
            padding: 1rem 0;
            position: sticky;
            top: 0;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            z-index: 1000;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1rem;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .school-name {
            font-size: 1.8rem;
            font-weight: bold;
            text-decoration: none;
            color: white;
        }
        
        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }
        
        nav a {
            color: white;
            text-decoration: none;
            font-size: 1rem;
            transition: 0.3s ease;
            padding: 0.5rem 1rem;
            border-radius: 4px;
        }
        
        /* Hover effect on navigation links */
        nav a:hover {
            background-color: #0052a3;
            transform: translateY(-2px);
        }
        
        /* Mobile menu toggle button (hidden by default) */
        .menu-toggle {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        /* ========================================
           3. SECTIONS STYLING
           ======================================== */
        
        section {
            padding: 4rem 1rem;
            scroll-margin-top: 80px;
        }
        
        section h2 {
            text-align: center;
            font-size: 2.5rem;
            color: #0066cc;
            margin-bottom: 2rem;
        }
        
        /* ========================================
           4. HOME SECTION
           ======================================== */
        
        #home {
            background: linear-gradient(135deg, #0066cc 0%, #004499 100%);
            color: white;
            text-align: center;
            padding: 6rem 1rem;
        }
        
        #home h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        #home p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .banner-image {
            width: 100%;
            max-width: 600px;
            height: 300px;
            background: linear-gradient(135deg, #87ceeb 0%, #e0f6ff 100%);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 4rem;
            margin: 1rem auto;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
        }
        
        /* Welcome button in home section */
        .welcome-btn {
            background-color: white;
            color: #0066cc;
            padding: 0.75rem 2rem;
            font-size: 1rem;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-weight: bold;
            transition: 0.3s ease;
            margin-top: 1rem;
        }
        
        .welcome-btn:hover {
            background-color: #e6f2ff;
            transform: translateY(-3px);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
        }
        
        /* ========================================
           5. ABOUT SECTION
           ======================================== */
        
        #about {
            background-color: white;
        }
        
        .about-content {
            max-width: 800px;
            margin: 0 auto;
            line-height: 1.8;
            font-size: 1.05rem;
            text-align: justify;
        }
        
        /* ========================================
           6. COURSES SECTION
           ======================================== */
        
        #courses {
            background-color: #f9f9f9;
        }
        
        .courses-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1100px;
            margin: 0 auto;
        }
        
        .course-card {
            background-color: white;
            border-radius: 8px;
            padding: 2rem;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
            transition: 0.3s ease;
        }
        
        /* Hover effect on course cards */
        .course-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 6px 20px rgba(0, 102, 204, 0.3);
        }
        
        .course-card h3 {
            color: #0066cc;
            margin-bottom: 1rem;
            font-size: 1.5rem;
        }
        
        .course-card p {
            color: #666;
            margin-bottom: 1.5rem;
        }
        
        .course-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        /* ========================================
           7. CONTACT SECTION
           ======================================== */
        
        #contact {
            background-color: white;
        }
        
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background-color: #f4f4f4;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        
        .form-group {
            margin-bottom: 1.5rem;
        }
        
        label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: bold;
            color: #333;
        }
        
        input, textarea {
            width: 100%;
            padding: 0.75rem;
            border: 2px solid #ddd;
            border-radius: 4px;
            font-size: 1rem;
            font-family: inherit;
            transition: 0.3s ease;
        }
        
        input:focus, textarea:focus {
            outline: none;
            border-color: #0066cc;
            box-shadow: 0 0 8px rgba(0, 102, 204, 0.3);
        }
        
        textarea {
            resize: vertical;
            min-height: 120px;
        }
        
        /* Submit button styling */
        .submit-btn {
            background-color: #0066cc;
            color: white;
            padding: 0.75rem 2rem;
            font-size: 1rem;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-weight: bold;
            width: 100%;
            transition: 0.3s ease;
        }
        
        .submit-btn:hover {
            background-color: #0052a3;
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
        }
        
        /* Error message styling */
        .error-message {
            color: #d32f2f;
            font-size: 0.875rem;
            margin-top: 0.25rem;
            display: none;
        }
        
        .form-group.error .error-message {
            display: block;
        }
        
        .form-group.error input,
        .form-group.error textarea {
            border-color: #d32f2f;
            background-color: #ffebee;
        }
        
        /* ========================================
           8. FOOTER
           ======================================== */
        
        footer {
            background-color: #0066cc;
            color: white;
            text-align: center;
            padding: 1.5rem;
            margin-top: 3rem;
        }
        
        /* ========================================
           9. SUCCESS MESSAGE
           ======================================== */
        
        .success-message {
            background-color: #4caf50;
            color: white;
            padding: 1rem;
            border-radius: 4px;
            margin-bottom: 1rem;
            text-align: center;
            display: none;
            animation: slideDown 0.5s ease;
        }
        
        .success-message.show {
            display: block;
        }
        
        /* Animation for success message */
        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        /* ========================================
           10. RESPONSIVE DESIGN (MOBILE)
           ======================================== */
        
        @media (max-width: 768px) {
            /* Header adjustments for mobile */
            .header-content {
                flex-wrap: wrap;
            }
            
            .menu-toggle {
                display: block;
            }
            
            nav {
                width: 100%;
                order: 3;
            }
            
            nav ul {
                flex-direction: column;
                gap: 0;
                display: none;
                width: 100%;
                background-color: #0052a3;
            }
            
            nav ul.active {
                display: flex;
            }
            
            nav a {
                display: block;
                padding: 1rem;
                border-radius: 0;
                border-bottom: 1px solid #0066cc;
            }
            
            /* Home section mobile */
            #home h1 {
                font-size: 2rem;
            }
            
            #home p {
                font-size: 1rem;
            }
            
            .banner-image {
                height: 200px;
                font-size: 3rem;
            }
            
            /* Courses grid mobile */
            .courses-grid {
                grid-template-columns: 1fr;
            }
            
            /* Section headings mobile */
            section h2 {
                font-size: 1.8rem;
            }
            
            /* Contact form mobile */
            .contact-form {
                padding: 1.5rem;
            }
        }
        
        @media (max-width: 480px) {
            #home h1 {
                font-size: 1.5rem;
            }
            
            nav a {
                padding: 0.75rem;
            }
            
            section {
                padding: 2rem 1rem;
            }
            
            section h2 {
                font-size: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- ========================================
         HEADER & NAVIGATION
         ======================================== -->
    <header>
        <div class="container">
            <div class="header-content">
                <!-- School Logo/Name -->
                <a href="#home" class="school-name">🎓School of AI and Emerging Technologies</a>
                
                <!-- Mobile menu toggle button -->
                <button class="menu-toggle" id="menuToggle">☰</button>
                
                <!-- Navigation Menu -->
                <nav>
                    <ul id="navMenu">
                        <li><a href="#home" class="nav-link">Home</a></li>
                        <li><a href="#about" class="nav-link">About</a></li>
                        <li><a href="#courses" class="nav-link">Courses</a></li>
                        <li><a href="#contact" class="nav-link">Contact</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
    
    <!-- ========================================
         HOME SECTION
         ======================================== -->
    <section id="home">
        <div class="container">
            <h1>Welcome to School of AI and Emerging Technologies</h1>
            <p>Providing quality education and fostering excellence in learning since 2010. 
               Join us on a journey of knowledge, growth, and success!</p>
            
            <!-- Banner Image (placeholder with emoji) -->
            <div class="banner-image">📚</div>
            
            <!-- Interactive Welcome Button -->
            <button class="welcome-btn" id="welcomeBtn">Click to Get Welcome Message</button>
            
            <!-- Welcome message display area -->
            <p id="welcomeMessage" style="margin-top: 1rem; font-size: 1.1rem; display: none;"></p>
        </div>
    </section>
    
    <!-- ========================================
         ABOUT SECTION
         ======================================== -->
    <section id="about">
        <div class="container">
            <h2>About Our School</h2>
            <div class="about-content">
                <p>
                    School of AI and Emerging Technology is committed to providing world-class education to students of all backgrounds. 
                    Our dedicated team of experienced educators focuses on nurturing both academic excellence 
                    and personal development.
                </p>
                <p style="margin-top: 1rem;">
                    With state-of-the-art facilities, innovative teaching methods, and a supportive learning environment, 
                    we prepare our students for success in higher education and beyond. We believe in holistic development 
                    that combines classroom learning with extracurricular activities, sports, and community service.
                </p>
                <p style="margin-top: 1rem;">
                    Our mission is to inspire, educate, and empower the next generation of leaders, thinkers, and innovators 
                    who will make a positive impact on society.
                </p>
            </div>
        </div>
    </section>
    
    <!-- ========================================
         COURSES SECTION
         ======================================== -->
    <section id="courses">
        <div class="container">
            <h2>Our Courses</h2>
            <div class="courses-grid">
                <!-- Course 1 -->
                <div class="course-card">
                    <div class="course-icon">🔬</div>
                    <h3>Science</h3>
                    <p>Explore the wonders of Physics, Chemistry, and Biology. 
                       Hands-on experiments and interactive learning experiences await you.</p>
                </div>
                
                <!-- Course 2 -->
                <div class="course-card">
                    <div class="course-icon">📖</div>
                    <h3>English & Literature</h3>
                    <p>Master communication skills and explore classic and contemporary literature. 
                       Develop critical thinking and creative writing abilities.</p>
                </div>
                
                <!-- Course 3 -->
                <div class="course-card">
                    <div class="course-icon">🧮</div>
                    <h3>Mathematics</h3>
                    <p>Build strong mathematical foundations with engaging problem-solving sessions. 
                       From basic arithmetic to advanced calculus concepts.</p>
                </div>
                
                <!-- Course 4 (Bonus) -->
                <div class="course-card">
                    <div class="course-icon">🎨</div>
                    <h3>Arts & Design</h3>
                    <p>Unleash your creativity through painting, drawing, and design. 
                       Express yourself and develop artistic skills under expert guidance.</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- ========================================
         CONTACT SECTION
         ======================================== -->
    <section id="contact">
        <div class="container">
            <h2>Contact Us</h2>
            
            <!-- Success message (shown after form submission) -->
            <div class="success-message" id="successMessage">
                ✓ Thank you for your message! We will get back to you soon.
            </div>
            
            <!-- Contact Form -->
            <form class="contact-form" id="contactForm">
                <!-- Name Field -->
                <div class="form-group" id="nameGroup">
                    <label for="name">Full Name *</label>
                    <input type="text" id="name" name="name" placeholder="Enter your full name">
                    <span class="error-message">Please enter your name</span>
                </div>
                
                <!-- Email Field -->
                <div class="form-group" id="emailGroup">
                    <label for="email">Email Address *</label>
                    <input type="email" id="email" name="email" placeholder="Enter your email address">
                    <span class="error-message">Please enter a valid email address</span>
                </div>
                
                <!-- Message Field -->
                <div class="form-group" id="messageGroup">
                    <label for="message">Message *</label>
                    <textarea id="message" name="message" placeholder="Enter your message here..."></textarea>
                    <span class="error-message">Please enter your message</span>
                </div>
                
                <!-- Submit Button -->
                <button type="submit" class="submit-btn">Send Message</button>
            </form>
        </div>
    </section>
    
    <!-- ========================================
         FOOTER
         ======================================== -->
    <footer>
        <p>&copy; 2024 School of AI and Emerging Technologies. All rights reserved. | 📧 info@aiandtechnologies.com | 📞 +1-800-SCHOOL-1</p>
    </footer>
    
    <!-- ========================================
         JAVASCRIPT - Internal Script
         ======================================== -->
    <script>
        // ========================================
        // 1. MOBILE MENU TOGGLE
        // ========================================
        
        // Get the menu toggle button and navigation menu
        const menuToggle = document.getElementById('menuToggle');
        const navMenu = document.getElementById('navMenu');
        
        // Add click event listener to toggle menu on mobile
        menuToggle.addEventListener('click', function() {
            navMenu.classList.toggle('active');
        });
        
        // Close menu when a link is clicked
        const navLinks = document.querySelectorAll('.nav-link');
        navLinks.forEach(link => {
            link.addEventListener('click', function() {
                navMenu.classList.remove('active');
            });
        });
        
        // ========================================
        // 2. WELCOME BUTTON - Interactive Feature
        // ========================================
        
        // Get the welcome button and message display area
        const welcomeBtn = document.getElementById('welcomeBtn');
        const welcomeMessage = document.getElementById('welcomeMessage');
        
        // Add click event listener to show welcome message
        welcomeBtn.addEventListener('click', function() {
            welcomeMessage.textContent = '🎉 Welcome to our school! We are excited to have you here!';
            welcomeMessage.style.display = 'block';
            
            // Optional: Hide the message after 5 seconds
            setTimeout(function() {
                welcomeMessage.style.display = 'none';
            }, 5000);
        });
        
        // ========================================
        // 3. FORM VALIDATION & SUBMISSION
        // ========================================
        
        // Get the contact form and success message
        const contactForm = document.getElementById('contactForm');
        const successMessage = document.getElementById('successMessage');
        
        // Get form input fields
        const nameInput = document.getElementById('name');
        const emailInput = document.getElementById('email');
        const messageInput = document.getElementById('message');
        
        // Function to validate email format
        // This function checks if the email follows a valid email pattern
        function isValidEmail(email) {
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            return emailRegex.test(email);
        }
        
        // Function to validate the form fields
        function validateForm() {
            // Flag to track if form is valid
            let isValid = true;
            
            // Clear previous error states
            document.getElementById('nameGroup').classList.remove('error');
            document.getElementById('emailGroup').classList.remove('error');
            document.getElementById('messageGroup').classList.remove('error');
            
            // Validate Name Field - check if name is not empty
            if (nameInput.value.trim() === '') {
                document.getElementById('nameGroup').classList.add('error');
                isValid = false;
            }
            
            // Validate Email Field - check if email is not empty and is valid format
            if (emailInput.value.trim() === '' || !isValidEmail(emailInput.value.trim())) {
                document.getElementById('emailGroup').classList.add('error');
                isValid = false;
            }
            
            // Validate Message Field - check if message is not empty
            if (messageInput.value.trim() === '') {
                document.getElementById('messageGroup').classList.add('error');
                isValid = false;
            }
            
            return isValid;
        }
        
        // Add submit event listener to the form
        contactForm.addEventListener('submit', function(event) {
            // Prevent default form submission behavior
            event.preventDefault();
            
            // Validate the form
            if (validateForm()) {
                // If form is valid, show success message
                successMessage.classList.add('show');
                
                // Reset the form fields (clear all inputs)
                contactForm.reset();
                
                // Hide the success message after 3 seconds
                setTimeout(function() {
                    successMessage.classList.remove('show');
                }, 3000);
            }
        });
        
        // Optional: Remove error styling when user starts typing
        nameInput.addEventListener('input', function() {
            if (this.value.trim() !== '') {
                document.getElementById('nameGroup').classList.remove('error');
            }
        });
        
        emailInput.addEventListener('input', function() {
            if (this.value.trim() !== '' && isValidEmail(this.value.trim())) {
                document.getElementById('emailGroup').classList.remove('error');
            }
        });
        
        messageInput.addEventListener('input', function() {
            if (this.value.trim() !== '') {
                document.getElementById('messageGroup').classList.remove('error');
            }
        });
    </script>
</body>
</html>
