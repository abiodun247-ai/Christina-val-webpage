<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Valentine's, Christiana! 💖</title>
    <style>
        /* Full-Screen Neon Background */
        body {
            background: radial-gradient(circle, #ff4e50, #fc913a, #ff4081);
            color: white;
            text-align: center;
            font-family: 'Arial', sans-serif;
            margin: 0;
            overflow: hidden;
        }

        /* Valentine's Heading */
        h1 {
            font-size: 3em;
            text-shadow: 0px 0px 20px white;
            animation: glow 1.5s infinite alternate;
            margin-top: 30px;
        }

        @keyframes glow {
            from { text-shadow: 0px 0px 20px white; }
            to { text-shadow: 0px 0px 30px yellow; }
        }

        /* Animated Colorful Name */
        .neon-name {
            font-size: 4em;
            font-weight: bold;
            background: linear-gradient(90deg, #ff0000, #ff7300, #ffeb00, #00ff6a, #006eff, #c200ff);
            background-size: 400% 400%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: neonMove 4s infinite alternate;
            text-shadow: 0px 0px 10px white;
        }

        @keyframes neonMove {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Love Message */
        .message {
            font-size: 1.5em;
            background: rgba(255, 255, 255, 0.2);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0px 0px 15px white;
            margin: 20px;
        }

        /* Image Slideshow */
        .slideshow-container {
            position: relative;
            width: 90%;
            max-width: 400px;
            margin: auto;
            overflow: hidden;
            border-radius: 15px;
            box-shadow: 0px 0px 15px white;
        }

        .slides {
            display: none;
            width: 100%;
            border-radius: 15px;
        }

        /* Love Quote Button */
        .quote-button {
            background-color: white;
            color: #ff4081;
            font-size: 1.2em;
            padding: 10px 20px;
            border: none;
            border-radius: 10px;
            margin-top: 20px;
            cursor: pointer;
            font-weight: bold;
            box-shadow: 0px 0px 15px white;
        }

        .quote-button:hover {
            background-color: #ff4081;
            color: white;
        }

        /* Quote Display */
        #loveQuote {
            font-size: 1.5em;
            margin-top: 20px;
            font-style: italic;
        }

        /* Footer */
        .footer {
            margin-top: 30px;
            font-size: 1.3em;
            color: #fdfd96;
        }

        /* Responsive */
        @media (max-width: 600px) {
            h1 { font-size: 2.5em; }
            .neon-name { font-size: 3em; }
            .message { font-size: 1.2em; }
            .quote-button { font-size: 1em; }
        }
    </style>
</head>
<body>

    <h1>💖 Happy Valentine's,</h1>
    <h1 class="neon-name">Christiana! 💖</h1>

    <!-- Love Message -->
    <div class="message">
        My dearest Christiana, you are more beautiful than a sunrise and more precious than gold.  
        You light up my world and make every moment magical. I appreciate and cherish you more than words can express.  
        <br><br>
        **With all my heart, from Samuel, your love.** ❤️
    </div>

    <!-- Slideshow -->
    <div class="slideshow-container">
        <img class="slides" src="image1.jpg" alt="Christiana">
        <img class="slides" src="image2.jpg" alt="Christiana">
        <img class="slides" src="image3.jpg" alt="Christiana">
        <!-- Add more images here -->
    </div>

    <!-- Love Quote Button -->
    <button class="quote-button" onclick="showLoveQuote()">Click for a Love Quote ❤️</button>

    <!-- Quote Display -->
    <p id="loveQuote">"Love is in the air..."</p>

    <!-- Footer -->
    <div class="footer">
        **Forever yours, Samuel** ❤️
    </div>

    <script>
        // Slideshow Functionality
        let slideIndex = 0;
        function showSlides() {
            let slides = document.getElementsByClassName("slides");
            for (let i = 0; i < slides.length; i++) {
                slides[i].style.display = "none";
            }
            slideIndex++;
            if (slideIndex > slides.length) { slideIndex = 1; }
            slides[slideIndex - 1].style.display = "block";
            setTimeout(showSlides, 3000); // Change image every 3 seconds
        }
        showSlides();

        // Love Quotes
        const quotes = [
            "Christiana, you are my today and all of my tomorrows. ❤️",
            "In your eyes, Christiana, I see my entire world. 💫",
            "Every love story is beautiful, but ours, Christiana, is my favorite. 💕",
            "I love you more than words can say, Christiana. 🌹",
            "Christiana, you are the sunshine that lights up my darkest days. ☀️"
        ];

        function showLoveQuote() {
            let randomIndex = Math.floor(Math.random() * quotes.length);
            document.getElementById("loveQuote").innerText = quotes[randomIndex];
        }
    </script>

</body>
</html>
