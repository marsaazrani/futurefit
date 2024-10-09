<!DOCTYPE html>
<html lang="en">
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta charset="UTF-8">
    <title>FutureFit - Youth Fitness</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&family=Montserrat:wght@400;700&family=Bubblegum+Sans&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #e8f5e9;
            color: #333;
            margin: 0;
            padding: 0;
        }

        header {
            display: flex;
            align-items: center;
            background-color: #66bb6a;
            padding: 20px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        .logo {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: #ffffff;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 20px;
        }

        h1 {
            font-family: 'Bubblegum Sans', cursive;
            font-size: 3em;
            margin: 0;
            color: #ffffff;
        }

        h2, h3 {
            margin: 5px 0 10px;
            font-weight: 400;
            color: #ffffff; /* Set color for h2 and h3 */
        }

        h3 {
            color: #43a047; /* Set color for h3 */
        }

        nav {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 10px;
            flex-grow: 1;
        }

        nav a {
            color: #fff;
            padding: 10px 15px;
            text-decoration: none;
            border-radius: 5px;
            margin: 5px;
            transition: background 0.3s;
            background-color: #43a047;
        }

        nav a:hover {
            background-color: #388e3c;
        }

        section {
            padding: 20px;
            margin: 10px;
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }

        form {
            display: flex;
            flex-direction: column;
            max-width: 300px;
            margin: auto;
        }

        input[type="number"] {
            padding: 10px;
            margin: 10px 0;
            border-radius: 5px;
            border: 1px solid #66bb6a;
            outline: none;
            transition: border 0.3s;
        }

        input[type="number"]:focus {
            border: 1px solid #43a047;
        }

        button {
            padding: 10px;
            background-color: #ff6700; /* Bright orange for buttons */
            border: none;
            border-radius: 5px;
            color: #fff;
            cursor: pointer;
            transition: background 0.3s, transform 0.3s;
        }

        button:hover {
            background-color: #e65100;
            transform: scale(1.05); /* Slight scaling on hover */
        }

        .home-image {
            width: 100%;
            max-width: 600px;
            border-radius: 10px;
            margin: 20px auto;
            display: block;
            border: 5px solid #66bb6a;
        }

        .learn-more {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #43a047;
            color: #fff;
            text-decoration: none;
            border-radius: 5px;
            transition: background 0.3s, transform 0.3s;
        }

        .learn-more:hover {
            background-color: #388e3c;
            transform: scale(1.05);
        }

        footer {
            text-align: center;
            padding: 20px;
            background-color: #66bb6a;
            color: #fff;
            font-size: 1.2em;
            font-weight: bold;
        }

        footer p {
            margin: 5px 0;
        }

        footer p span {
            color: #ff6700; /* Adding a pop of color */
        }

        .team-container {
            display: flex;
            justify-content: space-around;
            align-items: center;
            flex-wrap: wrap;
            margin-top: 20px;
        }

        .team-member {
            text-align: center;
            max-width: 200px;
        }

        .team-member img {
            border-radius: 50%;
            width: 150px;
            height: 150px;
            object-fit: cover;
            margin-bottom: 10px;
        }

        .challenge {
            background-color: #f1f8e9; /* Light green for challenge cards */
            border: 1px solid #66bb6a;
            border-radius: 8px;
            padding: 15px;
            margin: 15px 0;
            position: relative;
            overflow: hidden;
            transition: transform 0.3s;
        }

        .challenge:hover {
            transform: scale(1.02);
        }

        .challenge-button {
            background-color: #ff6700; /* Bright orange for buttons */
            border: none;
            border-radius: 5px;
            color: white;
            padding: 10px 15px;
            cursor: pointer;
            transition: background 0.3s, transform 0.3s;
        }

        .challenge-button:hover {
            background-color: #e65100;
            transform: scale(1.05);
        }

        .challenge-status {
            margin-top: 10px;
            font-weight: bold;
            color: #4caf50; /* Green color for success message */
        }

        .menu-item {
            text-align: center;
            margin: 20px;
        }

        .menu-item img {
            width: 200px;
            height: 150px;
            border-radius: 10px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }

        @media (max-width: 600px) {
            header {
                flex-direction: column;
                align-items: flex-start;
            }
            nav {
                justify-content: flex-start;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <img src="[C:\UNESA\futurefit\logo futurefit.jpg](https://github.com/marsaazrani/futurefit/blob/main/logo%20futurefit.jpg?raw=true)" alt="FutureFit Logo" style="width: 100%; height: 100%; border-radius: 50%;">
        </div>
        <div>
            <h1>FutureFit</h1>
            <h2>Your Health and Fitness Hub</h2>
        </div>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About Us</a>
            <a href="#bmi">BMI Calculator</a>
            <a href="#challenge">Daily Challenge</a>
            <a href="#menu">Healthy Menu</a>
            <a href="#articles">Health Articles</a>
        </nav>
    </header>
    
    <section id="home">
        <h2 style="color: #43a047;">Welcome to FutureFit!</h2> <!-- Solid green for heading -->
        <p class="welcome-message" style="color: #333;">Discover ways to maintain your health and fitness in a fun and engaging way.</p>
        <p style="color: #333;">
            Maintaining a healthy body is essential for a fulfilling life. Regular physical activity, balanced nutrition, and proper hydration are key components to keeping your body in shape. Exercise not only improves your physical appearance but also boosts your mood, increases energy levels, and enhances overall well-being.
        </p>
        <p style="color: #333;">
            Moreover, a well-balanced diet fuels your body and mind, providing the nutrients needed for optimal performance in daily activities. Consuming a variety of fruits, vegetables, whole grains, and lean proteins can significantly impact your overall health. It’s important to remember that your body is your most valuable asset, and taking care of it should be a priority.
        </p>
        <p style="color: #333;">
            By adopting healthy habits, you can prevent illnesses, improve your concentration, and achieve your goals, whether in academics or sports. A strong and healthy body leads to a healthy mind, enabling you to tackle challenges more effectively and with greater confidence.
        </p>
        <img src="https://blog-edutore-partner.s3.ap-southeast-1.amazonaws.com/wp-content/uploads/2021/03/01110106/Jurusan-Kesehatan-Masyarakat-01-626x430-1.png" alt="Healthy Lifestyle" class="home-image">
        <p style="color: #333;">Join us on this journey to fitness and well-being, where every small step you take towards a healthier lifestyle counts!</p>
        <a href="#about" class="learn-more">Learn More</a>
    </section>
    
    <section id="about">
        <h2 style="color: #43a047;">About Us</h2>
        <p>We are a health education platform committed to helping you live a healthier, more active, and happier lifestyle. Here, we believe that health is the foundation of a quality life, and we are here to support your journey towards optimal well-being.</p>
        <p>We provide a variety of articles, and infographics that discuss the importance of exercise, movement recommendations, exercise challenges, as well as nutrition tips and calorie counting. From the benefits of exercise to healthy diet guidelines, we are here to help you understand and apply this knowledge in your daily life. Each piece of content is designed for different fitness levels, so everyone can get involved and reap the benefits.</p>
        <p>We are committed to constantly updating our content with the latest and most reliable information. Our team of health experts, fitness trainers and nutritionists are ready to give you the best guidance. We invite you to join our community and start your journey towards a healthier and happier life. Thank you for visiting FutureFit. Let's move towards a healthier and happier life together!</p>
        <div class="team-container">
            <div class="team-member">
                <img src="C:\UNESA\futurefit\marsa foto.jpg" alt="Team Member 1">
                <h3>Marsa Azrani</h3>
                <p>Health Coach</p>
            </div>
            <div class="team-member">
                <img src="C:\UNESA\futurefit\rena foto.jpg" alt="Team Member 2">
                <h3>Renasabylla Putri</h3>
                <p>Nutritionist</p>
            </div>
            <div class="team-member">
                <img src="C:\UNESA\futurefit\sasi foto.jpg" alt="Team Member 3">
                <h3>Ni Luh Kadek Tri Sasi</h3>
                <p>Fitness Trainer</p>
            </div>
        </div>
    </section>

    <section id="bmi">
        <h2 style="color: #43a047;">BMI Calculator</h2>
        <form id="bmiForm" onsubmit="return calculateBMI(event);">
            <label for="weight">Weight (kg):</label>
            <input type="number" id="weight" required>
            <label for="height">Height (cm):</label>
            <input type="number" id="height" required>
            <button type="submit">Calculate BMI</button>
        </form>
        <p id="bmiResult" style="font-size: 1.5em; text-align: center;"></p>
        <p style="text-align: center;">
            <strong>Categories are defined as:</strong><br>
            Underweight: BMI < 18.5<br>
            Normal weight: 18.5 ≤ BMI < 24.9<br>
            Overweight: 25 ≤ BMI < 29.9<br>
            Obesity: BMI ≥ 30
        </p>
    </section>

    <section id="challenge">
        <h2 style="color: #43a047;">Daily Challenge</h2>
        
        <div class="challenge">
            <h3>Challenge 1: Reduce Sugar Intake</h3>
            <p>Your goal for this challenge is to reduce your sugar intake to below 25 grams per day. This means cutting back on sugary snacks, drinks, and desserts.</p>
            <p><strong>Tips:</strong></p>
            <ul>
                <li>Read nutrition labels to check for added sugars.</li>
                <li>Opt for natural sweeteners like honey or maple syrup in moderation.</li>
                <li>Replace sugary drinks with water or herbal tea.</li>
                <li>Snack on fruits instead of candy or cookies.</li>
            </ul>
            <p><strong>Benefits:</strong> Reducing sugar can help prevent weight gain, decrease the risk of chronic diseases, and improve your overall energy levels.</p>
            <button class="challenge-button" onclick="completeChallenge(1)">Complete Challenge</button>
            <p class="challenge-status" id="status-1"></p>
        </div>
        
        <div class="challenge">
            <h3>Challenge 2: Walk 3,000 Steps</h3>
            <p>This challenge encourages you to walk at least 3,000 steps each day. Use a pedometer or a smartphone app to keep track of your progress.</p>
            <p><strong>Tips:</strong></p>
            <ul>
                <li>Take the stairs instead of the elevator.</li>
                <li>Park further away from your destination.</li>
                <li>Incorporate short walks into your breaks during school or work.</li>
                <li>Join friends or family for a walking challenge to make it more fun!</li>
            </ul>
            <p><strong>Benefits:</strong> Walking can help improve your cardiovascular health, boost your mood, and enhance your fitness levels.</p>
            <button class="challenge-button" onclick="completeChallenge(2)">Complete Challenge</button>
            <p class="challenge-status" id="status-2"></p>
        </div>
        
        <div class="challenge">
            <h3>Challenge 3: Sleep Before 10 PM</h3>
            <p>Your goal is to get to bed before 10 PM. Good sleep is essential for recovery and overall health.</p>
            <p><strong>Tips:</strong></p>
            <ul>
                <li>Create a relaxing bedtime routine.</li>
                <li>Avoid screens at least an hour before bed.</li>
                <li>Keep the room dark, cool, and quiet.</li>
                <li>Limit caffeine intake in the afternoon and evening.</li>
            </ul>
            <p><strong>Benefits:</strong> Quality sleep can enhance memory, boost your immune system, and lower stress levels.</p>
            <button class="challenge-button" onclick="completeChallenge(3)">Complete Challenge</button>
            <p class="challenge-status" id="status-3"></p>
        </div>
    </section>

    <section id="menu">
        <h2 style="color: #43a047;">Healthy Menu</h2>
        <p>Explore our curated healthy menu options that promote balanced nutrition and delicious meals.</p>
        
        <div class="menu-item">
            <a href="https://cookpad.com/id/resep/24150429-papaya-miyo-milk-yogurt-juice-healthy-breakfast?ref=search&search_term=menu+masakan+sehat" target="_blank">
                <img src="https://img-global.cpcdn.com/recipes/b228c68d2f496d75/680x482cq70/papaya-miyo-milk-yogurt-juice-healthy-breakfast-foto-resep-utama.webp" alt="Oatmeal">
            </a>
            <h3>Papaya milk Yogurt </h3>
        </div>
        
        <div class="menu-item">
            <a href="https://cookpad.com/id/resep/24038786-ayam-sambal-matah-healthy?ref=search&search_term=menu+masakan+sehat" target="_blank">
                <img src="https://img-global.cpcdn.com/recipes/09c4f046967900f4/680x482cq70/ayam-sambal-matah-healthy-foto-resep-utama.webp" alt="Quinoa Salad">
            </a>
            <h3>Ayam Sambal Matah rendah Kalori</h3>
        </div>
        
        <div class="menu-item">
            <a href="https://cookpad.com/id/resep/24032312-minuman-pir-gojiberry-sehat?ref=search&search_term=menu+masakan+sehat" target="_blank">
                <img src="https://img-global.cpcdn.com/recipes/da20c69d3459234e/680x482cq70/minuman-pir-gojiberry-sehat-foto-resep-utama.webp" alt="Grilled Chicken">
            </a>
            <h3>Gojiberry Sehat</h3>
        </div>
        
        <div style="text-align: center; margin-top: 20px;">
            <a href="https://cookpad.com/id/cari/menu%20masakan%20sehat" class="learn-more" target="_blank">See More</a>
        </div>
    </section>    

    <section id="articles">
        <h2 style="color: #43a047;">Health Articles</h2>
        <p>Discover our collection of informative articles that cover various health and wellness topics.</p>
        
        <!-- Article 1 -->
        <div class="menu-item">
            <a href="https://kemkes.go.id/id/aksi-bergizi--gerakan-sehat-untuk-remaja-masa-kini" target="_blank">
                <img src="https://kemkes.go.id/app_asset/image_content/1665372457634391293d54a0.24601924.jpg" alt="Aksi Bergizi - Gerakan Sehat untuk Remaja Masa Kini">
            </a>
            <h3>Aksi Bergizi - Gerakan Sehat untuk Remaja Masa Kini</h3>
        </div>
        
        <!-- Article 2 -->
        <div class="menu-item">
            <a href="https://kemkes.go.id/id/gizi-saat-remaja-tentukan-kualitas-keturunan" target="_blank">
                <img src="http://sehatnegeriku.kemkes.go.id/wp-content/uploads/2020/01/WhatsApp-Image-2020-01-24-at-11.57.42.jpeg">
            </a>
            <h3>Gizi Saat Remaja Tentukan Kualitas Keturunan</h3>
        </div>
        
        <!-- Article 3 -->
        <div class="menu-item">
            <a href="https://kemkes.go.id/id/pesan-untuk-remaja-putri-indonesia-cantik-itu-sehat-bukan-kurus" target="_blank">
                <img src="http://sehatnegeriku.kemkes.go.id/wp-content/uploads/2018/11/IMG_20181123_091433.jpg" alt="Pesan untuk Remaja Putri: Cantik Itu Sehat, Bukan Kurus">
            </a>
            <h3>Pesan untuk Remaja Putri: Cantik Itu Sehat, Bukan Kurus</h3>
        </div>
        
        <!-- Button to see more articles -->
        <div style="text-align: center; margin-top: 20px;">
            <a href="https://kemkes.go.id/id/category/artikel-kesehatan" class="learn-more" target="_blank">See More</a>
        </div>
    </section>    

    <footer>
        <p>&copy; 2024 FutureFit. All rights reserved.</p>
        <p>Contact us: <span>info@futurefit.com</span></p>
    </footer>

    <script>
        function calculateBMI(event) {
            event.preventDefault();
            const weight = parseFloat(document.getElementById("weight").value);
            const height = parseFloat(document.getElementById("height").value) / 100; // Convert height to meters
            const bmi = (weight / (height * height)).toFixed(2);
            const resultElement = document.getElementById("bmiResult");
            resultElement.innerHTML = `Your BMI is: <strong>${bmi}</strong>`;

            // Determine BMI category
            let category;
            if (bmi < 18.5) {
                category = "Underweight";
            } else if (bmi < 24.9) {
                category = "Normal weight";
            } else if (bmi < 29.9) {
                category = "Overweight";
            } else {
                category = "Obesity";
            }
            resultElement.innerHTML += `<br>Category: <strong>${category}</strong>`;
        }

        function completeChallenge(challengeNumber) {
            const statusElement = document.getElementById(`status-${challengeNumber}`);
            statusElement.innerHTML = "Challenge Completed! Keep up the great work!";
        }
    </script>
</body>
</html>
