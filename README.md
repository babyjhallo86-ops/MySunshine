# MySunshine
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday, My Love</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;700&display=swap');

        :root {
            --primary-color: #ffffff;
            --secondary-color: #a7a7a7;
            --background-color: #000000;
            --accent-color: #ff4081;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--background-color);
            color: var(--primary-color);
            overflow-x: hidden;
        }

        .hero {
            height: 100vh;
            position: relative;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            overflow: hidden;
        }

        #bg-video {
            position: absolute;
            top: 50%;
            left: 50%;
            min-width: 100%;
            min-height: 100%;
            width: auto;
            height: auto;
            z-index: -1;
            transform: translateX(-50%) translateY(-50%);
            background-size: cover;
        }

        .hero-content {
            z-index: 1;
            animation: fadeIn 3s ease-in-out;
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.5rem;
            color: var(--secondary-color);
        }

        .scroll-down {
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            animation: bounce 2s infinite;
        }

        .scroll-down a {
            color: var(--primary-color);
            text-decoration: none;
            font-size: 2rem;
        }

        .journey-section {
            padding: 100px 20px;
            text-align: center;
        }

        .journey-section h2 {
            font-size: 3rem;
            margin-bottom: 2rem;
            position: relative;
        }

        .journey-section h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 50px;
            height: 3px;
            background-color: var(--accent-color);
        }

        .memory-lane {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 4rem;
        }

        .memory {
            width: 300px;
            height: 400px;
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            cursor: pointer;
        }

        .memory img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .memory:hover img {
            transform: scale(1.1);
        }

        .memory-caption {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            background: rgba(0, 0, 0, 0.7);
            color: var(--primary-color);
            padding: 1rem;
            transform: translateY(100%);
            transition: transform 0.5s ease;
        }

        .memory:hover .memory-caption {
            transform: translateY(0);
        }

        .wishes-galaxy {
            position: relative;
            height: 100vh;
            overflow: hidden;
        }

        .star {
            position: absolute;
            width: 2px;
            height: 2px;
            background-color: var(--primary-color);
            border-radius: 50%;
            animation: twinkle 5s infinite ease-in-out;
        }

        .wish {
            position: absolute;
            color: var(--primary-color);
            background: rgba(255, 64, 129, 0.1);
            padding: 10px;
            border-radius: 5px;
            display: none;
        }

        .final-message {
            padding: 150px 20px;
            text-align: center;
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.9));
        }

        .final-message h2 {
            font-size: 3rem;
            margin-bottom: 2rem;
        }

        .final-message p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem;
            line-height: 1.6;
        }

        .cta-button {
            display: inline-block;
            padding: 1rem 2rem;
            background-color: var(--accent-color);
            color: var(--primary-color);
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: background-color 0.3s ease;
        }

        .cta-button:hover {
            background-color: #ff79b0;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {
                transform: translateX(-50%) translateY(0);
            }
            40% {
                transform: translateX(-50%) translateY(-30px);
            }
            60% {
                transform: translateX(-50%) translateY(-15px);
            }
        }

        @keyframes twinkle {
            0% { opacity: 0.5; }
            50% { opacity: 1; }
            100% { opacity: 0.5; }
        }
    </style>
</head>
<body>

    <section class="hero">
        <video autoplay muted loop id="bg-video">
            <source src="https://assets.mixkit.co/videos/preview/mixkit-flying-through-a-dazzling-galaxy-3280-large.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
        <div class="hero-content">
            <h1>Happy Birthday, My Love</h1>
            <p>Our journey is written in the stars.</p>
        </div>
        <div class="scroll-down">
            <a href="#our-universe"><span>&darr;</span></a>
        </div>
    </section>

    <section id="our-universe" class="journey-section">
        <h2>Our Universe</h2>
        <p>A collection of moments that created our own galaxy.</p>
        <div class="memory-lane">
            <div class="memory">
                <img src="https://images.pexels.com/photos/3785424/pexels-photo-3785424.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Memory 1">
                <div class="memory-caption">
                    <h3>Our First Adventure</h3>
                    <p>Remember that time we got lost and found the most beautiful view? That's when I knew our love was an adventure.</p>
                </div>
            </div>
            <div class="memory">
                <img src="https://images.pexels.com/photos/1024960/pexels-photo-1024960.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Memory 2">
                <div class="memory-caption">
                    <h3>The Day We Laughed Until We Cried</h3>
                    <p>Your laugh is my favorite sound in the universe. This day was a symphony of joy.</p>
                </div>
            </div>
            <div class="memory">
                <img src="https://images.pexels.com/photos/2253870/pexels-photo-2253870.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Memory 3">
                <div class="memory-caption">
                    <h3>A Quiet Moment</h3>
                    <p>Even in the silence, my heart beats for you. These quiet moments are as precious as the loud ones.</p>
                </div>
            </div>
        </div>
    </section>

    <section class="journey-section">
        <h2>A Galaxy of Wishes</h2>
        <p>Messages from across the cosmos, all for you.</p>
        <div class="wishes-galaxy" id="wishes-galaxy">
            <!-- Wishes will be dynamically added here -->
        </div>
    </section>

    <section class="final-message">
        <h2>To My Universe</h2>
        <p>"What we find in a soulmate is not something wild to tame, but something wild to run with." [22] With you, every day is a new adventure, a new star to discover in our ever-expanding universe. You are my greatest adventure, and I can't wait to see where our journey takes us next. "You are my greatest adventure, always and forever." [22]</p>
        <a href="#continue-our-adventure" class="cta-button">Continue Our Adventure</a>
    </section>

    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const wishesGalaxy = document.getElementById('wishes-galaxy');
            const wishes = [
                { text: "Wishing you a universe of happiness!", top: '10%', left: '20%' },
                { text: "May your birthday shine as bright as a supernova!", top: '30%', left: '80%' },
                { text: "Another trip around the sun with my favorite person!", top: '50%', left: '10%' },
                { text: "You're a star! Happy Birthday!", top: '70%', left: '60%' },
                { text: "To the moon and back, I love you!", top: '90%', left: '30%' }
            ];

            for (let i = 0; i < 100; i++) {
                const star = document.createElement('div');
                star.classList.add('star');
                star.style.top = `${Math.random() * 100}%`;
                star.style.left = `${Math.random() * 100}%`;
                star.style.animationDelay = `${Math.random() * 5}s`;
                wishesGalaxy.appendChild(star);
            }

            wishes.forEach(wishData => {
                const wishElement = document.createElement('div');
                wishElement.classList.add('wish');
                wishElement.textContent = wishData.text;
                wishElement.style.top = wishData.top;
                wishElement.style.left = wishData.left;
                wishesGalaxy.appendChild(wishElement);

                const starForWish = document.createElement('div');
                starForWish.classList.add('star');
                starForWish.style.top = wishData.top;
                starForWish.style.left = wishData.left;
                starForWish.style.width = '5px';
                starForWish.style.height = '5px';
                starForWish.style.backgroundColor = 'var(--accent-color)';
                wishesGalaxy.appendChild(starForWish);

                starForWish.addEventListener('mouseenter', () => {
                    wishElement.style.display = 'block';
                });

                starForWish.addEventListener('mouseleave', () => {
                    wishElement.style.display = 'none';
                });
            });
        });
    </script>

</body>
</html>

```
Sources
help
quantifimedia.com
elementor.com
dev.to
bluecompass.com
webtechneeq.com
dorik.com
designrush.com
digidop.com
designrush.com
youtube.com
reallygooddesigns.com
radicalwebdesign.co.uk
grocito.com
Google Search Suggestions
Display of Search Suggestions is required when using Grounding with Google Search. Learn more
Google logo
