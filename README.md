# Wacky-Wisdom-University

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wacky Wisdom University - Complete Website</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: sans-serif; margin: 0; background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%); }
        .container, .contener { margin: auto; max-width: 1200px; padding: 20px; }
        header { padding: 20px; background: #ec2113; text-align: center; border-bottom: 5px solid black; margin-bottom: 20px; }
        #WWU { max-width: 400px; height: auto; border-radius: 10px; box-shadow: 0 4px 20px rgba(0,0,0,0.5); }
        h1 { text-align: center; color: red; background: white; border: 2px solid darkred; font-family: sans-serif; padding: 5px; margin-top: 10px; font-size: 2em; }
        #nav1 { background: white; padding: 10px 0; text-align: center; box-shadow: 0 2px 5px rgba(0,0,0,0.1); margin-bottom: 20px; }
        #nav1 a { color: black; text-decoration: none; padding: 15px 20px; margin: 0 10px; border-radius: 5px; font-family: 'Trirong', serif; display: inline-block; }
        #nav1 a:hover, #nav1 a.active { font-weight: bold; color: white; background: red; padding: 0.6em; }
        #nav { text-align: center; margin-bottom: 30px; background: white; padding: 20px 0; }
        #nav a { text-decoration: none; padding: 15px 25px; margin: 0 10px; border-radius: 5px; background-color: white; color: black; border: 3px solid black; display: inline-block; }
        #nav a:hover { font-weight: bold; color: white; background: red; border: 3px solid red; }
        article { background: lightgray; margin: 20px 0; padding: 20px; border-radius: 10px; box-shadow: 0 4px 10px rgba(0,0,0,0.3); }
        article h2 { color: red; font-size: 27px; text-align: center; margin-bottom: 20px; }
        #intro1, #intro2, #intro3, #frist { text-align: center; font-family: serif; margin: 15px 0; }
        #intro4 { font-family: serif; color: red; font-weight: bold; padding-top: 20px; padding-left: 20px; font-size: 16px; }
        label { font-family: serif; display: block; margin: 10px 0; }
        fieldset { border: 1px solid red; margin-bottom: 20px; padding: 20px; border-radius: 5px; }
        legend { font-family: serif; text-align: left; color: red; font-weight: bold; padding: 0 10px; }
        input[type="text"], input[type="password"], input[type="file"], input[type="email"] { width: 100%; padding: 10px; margin: 10px 0; border: 1px solid red; border-radius: 5px; }
        input[type="radio"] { margin-right: 10px; }
        input[type="submit"], input[type="reset"], input[type="button"] { background: red; color: white; border: none; padding: 12px 20px; border-radius: 5px; cursor: pointer; margin: 10px 5px; font-weight: bold; }
        input[type="submit"]:hover, input[type="reset"]:hover, input[type="button"]:hover { background: darkred; }
        input#result { background: #f0f0f0; border: 2px solid red; }
        article p { margin: 15px 0; line-height: 1.6; font-size: 1.1em; color: black; }
        article h2.major { color: rgba(0,0,128,1); margin-top: 40px; font-size: 2em; }
        span.grade { font-weight: bold; display: block; margin: 15px 0; color: red; }
        h3 { text-align: center; font-weight: bold; color: red; }
        footer { background: red; color: white; text-align: center; padding: 15px; margin-top: 40px; border-top: 5px solid black; }
        .ContactUs { text-align: center; }
        .ContactUs a { font-weight: bold; color: white; text-decoration: none; }
        #AboutUs { color: white; }
        #a6 { font-family: serif; color: black; font-style: italic; }
        .page { display: none; }
        .page.active { display: block; }
        .login-form { max-width: 500px; margin: 0 auto; }
        .forgot-password { text-align: center; margin-top: 20px; }
        .forgot-password a { color: #ec2113; text-decoration: none; font-weight: bold; }
        .forgot-password a:hover { text-decoration: underline; }
    </style>
</head>
<body>
    <div class="container">
        <!-- SHARED HEADER -->
        <header>
            <img src="UN2.png" id="WWU" alt="WWU Logo">
            <h1 id="page-title">Wacky Wisdom University</h1>
        </header>

        <!-- SHARED NAVIGATION -->
        <nav id="nav1">
            <a href="#" onclick="showPage('home')" class="nav-link">Home</a>
            <a href="#" onclick="showPage('majors')" class="nav-link">Majors</a>
            <a href="#" onclick="showPage('calculations')" class="nav-link">Calculations</a>
            <a href="#" onclick="showPage('login')" class="nav-link">Login</a>
        </nav>

        <!-- HOME PAGE -->
        <div id="home" class="page active">
            <article>
                <form action="resultwwu.html">
                    <h2>The World's Best University!</h2>
                    <p id="intro1">Wacky Wisdom University is your one stop shop for all of your off-beat specializations, found nowhere else because they are too unique to teach! We provide students with the latest skills and knowledge that are in high demand by employers.</p>
                    <p id="intro2">Our graduates don't just leave with diplomas... they earn recognized certifications that define them in their fields. These credentials lead to exceptional career opportunities and inspire our students to become the leaders and innovators of tomorrow.</p>
                    <p id="intro3">We cultivate an environment where creativity and excellence thrive, preparing our students for remarkable careers. Join us in this amazing adventure at Wacky Wisdom University---the first step towards your future!</p>
                    <p id="intro4">To join us, fill this form correctly</p>

                    <fieldset>
                        <legend>Personal Information</legend>
                        <label>First Name: <input type="text" name="firstName" required></label>
                        <label>Last Name: <input type="text" name="lastName" required></label>
                        <label>National ID: <input type="text" name="nationalId" required></label>
                        <label>School Grade: <input type="text" name="schoolGrade" required></label>
                        <label>Certificates: <input type="file" name="certificates" id="certificates"></label>
                        <label>Email: <input type="email" name="email" required></label>
                        <label>Mobile Number: <input type="text" name="mobile" required></label>
                        <label>Password: <input type="password" name="password" id="password" required></label>
                        <label>Confirm Password: <input type="password" name="confirmPassword" required></label>
                    </fieldset>

                    <fieldset>
                        <legend>Gender</legend>
                        <label><input type="radio" name="gender" value="male" required> Male</label>
                        <label><input type="radio" name="gender" value="female"> Female</label>
                    </fieldset>

                    <fieldset>
                        <legend>Choose Your Major</legend>
                        <p><label><input type="radio" name="majors" value="CIT" required> Computer Information Technology (CIT)</label></p>
                        <p><label><input type="radio" name="majors" value="HR"> Human Resources (HR)</label></p>
                        <p><label><input type="radio" name="majors" value="ISE"> Intergalactic Sandwich Engineering (ISE)</label></p>
                        <p><label><input type="radio" name="majors" value="ENS"> Extreme Napping Studies (ENS)</label></p>
                    </fieldset>

                    <input type="submit" value="Submit">
                    <input type="reset" value="Reset">
                </form>
            </article>
        </div>

        <!-- MAJORS PAGE -->
        <div id="majors" class="page">
            <article style="margin: 0 20px;">
                <nav id="nav">
                    <a id="n1" href="#CIT">Computer Information Technology</a>
                    <a id="n2" href="#HR">Human Resources</a>
                    <a id="n3" href="#ISE">Intergalactic Sandwich Engineering</a>
                    <a id="n4" href="#ENS">Extreme Napping Studies</a>
                </nav>
                
                <p id="intro1">Wacky Wisdom University takes pride in its unique specializations that are not offered anywhere else. This distinctive focus sets us apart from other institutions.</p>
                <p id="intro2">Our graduates receive a specialized diploma that is considered a mark of excellence in their respective fields. This prestigious credential opens doors to exceptional career opportunities.</p>
                <p id="intro3">We cultivate an environment where innovation and excellence thrive, preparing our students for remarkable careers in their chosen fields.</p>

                <h2 class="major" id="CIT">Computer Information Technology (CIT)</h2>
                <p>CIT is a gateway to an incredible world of limitless opportunities! Students acquire exceptional skills that position them as pioneers in the technological revolution. CIT graduates are innovators, leaders, and influencers who shape the future.</p>
                <span class="grade">The lowest accepted grade in this major is 100.</span>

                <h2 class="major" id="HR">Human Resources (HR)</h2>
                <p>The Human Resources major leads to routine jobs with limited opportunities for real impact. It's seen as a place of comfort rather than innovation and change.</p>
                <span class="grade">The lowest accepted grade in this major is 12.22.</span>

                <h2 class="major" id="ISE">Intergalactic Sandwich Engineering (ISE)</h2>
                <p>This extraordinary major celebrates culinary creativity with cosmic sandwiches using exotic ingredients from various planets. Graduates become culinary visionaries in an interstellar revolution!</p>
                <span class="grade">The lowest accepted grade in this major is 99.9.</span>

                <h2 class="major" id="ENS">Extreme Napping Studies (ENS)</h2>
                <p>Master the science of napping to optimize rest and rejuvenation. Graduates become advocates for balance and efficiency through strategic napping techniques.</p>
                <span class="grade">The lowest accepted grade in this major is 101.</span>
            </article>
        </div>

        <!-- CALCULATIONS PAGE -->
        <div id="calculations" class="page">
            <article>
                <p id="frist">Many people are registering at our university, we have set clearer conditions to save time for everyone. We take 5% from the school GPA, 50% from the aptitude test score, and 45% from the achievement test score.</p>
                <h3>We wish you all the best.</h3>

                <form>
                    <fieldset>
                        <legend>Enter School GPA</legend>
                        <label><input type="text" id="gpa" placeholder="Enter GPA"> <input type="file" id="picture" style="border:0;"></label>
                    </fieldset>
                    <fieldset>
                        <legend>Enter Aptitude Test Score</legend>
                        <label><input type="text" id="aptitude" placeholder="Enter Aptitude Score"> <input type="file" id="picture2" style="border:0;"></label>
                    </fieldset>
                    <fieldset>
                        <legend>Enter Achievement Test Score</legend>
                        <label><input type="text" id="achievement" placeholder="Enter Achievement Score"> <input type="file" id="picture3" style="border:0;"></label>
                    </fieldset>
                    <fieldset>
                        <legend>Result</legend>
                        <input type="button" id="calculateButton" onclick="calculate()" value="Calculate">
                        <input type="text" id="result" disabled>
                    </fieldset>
                </form>
            </article>
        </div>

        <!-- LOGIN PAGE -->
        <div id="login" class="page">
            <article>
                <form class="login-form">
                    <h2>Login to Wacky Wisdom University</h2>
                    <fieldset>
                        <legend>Login Credentials</legend>
                        <label for="login-email">Email:</label>
                        <input type="email" id="login-email" name="email" required>
                        <label for="login-password">Password:</label>
                        <input type="password" id="login-password" name="password" required>
                        <input type="submit" value="Login">
                    </fieldset>
                    <div class="forgot-password">
                        <a href="#" onclick="alert('Forgot Password feature coming soon!')">Forgot Password?</a>
                    </div>
                </form>
            </article>
        </div>

        <!-- SHARED FOOTER -->
        <footer>
            <h3 id="AboutUs">About us</h3>
            <div class="ContactUs">
                <p><a id="a2" href="tel:013555005">013 555 005</a></p>
                <p><a id="a3" href="mailto:info@wwu.edu.sa">info@wwu.edu.sa</a></p>
                <p><a id="a4" href="#" onclick="showPage('home')">Home</a></p>
                <p><a id="a5" href="https://maps.app.goo.gl/9Y91y5HyxttNEMsGA">Find us</a></p>
                <p id="a6">If you want to join us <a href="#" onclick="showPage('home')">click here</a></p>
            </div>
        </footer>
    </div>

    <script>
        function showPage(pageName) {
            // Hide all pages
            const pages = document.querySelectorAll('.page');
            pages.forEach(page => page.classList.remove('active'));
            
            // Show selected page
            document.getElementById(pageName).classList.add('active');
            
            // Update active nav link
            document.querySelectorAll('.nav-link').forEach(link => link.classList.remove('active'));
            event.target.classList.add('active');
            
            // Update page title
            const titles = {
                'home': 'Welcome to Wacky Wisdom University!',
                'majors': 'Specializations',
                'calculations': 'Wacky Wisdom University',
                'login': 'Login to Wacky Wisdom University'
            };
            document.getElementById('page-title').textContent = titles[pageName];
        }

        function calculate() {
            const gpa = parseFloat(document.getElementById('gpa').value);
            const aptitude = parseFloat(document.getElementById('aptitude').value);
            const achievement = parseFloat(document.getElementById('achievement').value);
            
            if (isNaN(gpa) || isNaN(aptitude) || isNaN(achievement)) {
                alert('Please enter valid numbers for all fields.');
                return;
            }
            
            const result = (gpa * 0.05) + (aptitude * 0.50) + (achievement * 0.45);
            document.getElementById('result').value = result.toFixed(2);
        }
    </script>
</body>
</html>
