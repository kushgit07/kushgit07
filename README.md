<h1 align="center">Hi 👋, I'm KUSHAGRA SISODIA</h1>
<h3 align="center">A passionate frontend developer from India with knowledge in computer science stuff</h3>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kushagra Sisodia - Animated</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            background: 
                radial-gradient(ellipse at top, #1e3c72 0%, #2a5298 50%, #0f0f23 100%),
                linear-gradient(45deg, #0a0a0a, #1a1a2e, #16213e, #0f0f23);
            background-size: 100% 100%, 400% 400%;
            animation: spaceShift 20s ease infinite;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            position: relative;
        }

        @keyframes spaceShift {
            0% { background-position: 0% 0%, 0% 50%; }
            25% { background-position: 0% 0%, 50% 25%; }
            50% { background-position: 0% 0%, 100% 50%; }
            75% { background-position: 0% 0%, 50% 75%; }
            100% { background-position: 0% 0%, 0% 50%; }
        }

        .name-container {
            position: relative;
            text-align: center;
            z-index: 10;
        }

        .name {
            font-size: 4rem;
            font-weight: bold;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1, #96ceb4, #ffeaa7, #fd79a8);
            background-size: 600% 600%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: gradientShift 3s ease-in-out infinite;
            position: relative;
            display: inline-block;
            text-shadow: 0 0 30px rgba(255, 107, 107, 0.5);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .name:hover {
            transform: scale(1.1) rotateY(10deg);
            text-shadow: 
                0 0 20px rgba(255, 107, 107, 0.8),
                0 0 40px rgba(78, 205, 196, 0.6),
                0 0 60px rgba(69, 183, 209, 0.4);
            animation: pulse 0.5s ease-in-out infinite alternate;
        }

        @keyframes pulse {
            0% { transform: scale(1.1) rotateY(10deg); }
            100% { transform: scale(1.15) rotateY(-5deg); }
        }

        .name::before {
            content: '';
            position: absolute;
            top: -10px;
            left: -10px;
            right: -10px;
            bottom: -10px;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1, #96ceb4);
            background-size: 400% 400%;
            border-radius: 10px;
            z-index: -1;
            filter: blur(20px);
            opacity: 0;
            animation: glowShift 4s ease-in-out infinite;
            transition: opacity 0.3s ease;
        }

        .name:hover::before {
            opacity: 0.7;
        }

        @keyframes glowShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: radial-gradient(circle, #fff, #4ecdc4);
            border-radius: 50%;
            pointer-events: none;
            animation: float 6s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { 
                transform: translateY(0px) rotate(0deg);
                opacity: 0;
            }
            10%, 90% {
                opacity: 1;
            }
            50% { 
                transform: translateY(-100px) rotate(180deg);
                opacity: 0.8;
            }
        }

        .star {
            position: absolute;
            background: white;
            border-radius: 50%;
            animation: twinkle 2s ease-in-out infinite alternate;
        }

        .star:before {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 100%;
            height: 2px;
            background: white;
            border-radius: 1px;
        }

        .star:after {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%) rotate(90deg);
            width: 100%;
            height: 2px;
            background: white;
            border-radius: 1px;
        }

        @keyframes twinkle {
            0% { 
                opacity: 0.3;
                transform: scale(0.8);
                box-shadow: 0 0 5px rgba(255, 255, 255, 0.3);
            }
            100% { 
                opacity: 1;
                transform: scale(1.2);
                box-shadow: 0 0 15px rgba(255, 255, 255, 0.8);
            }
        }

        .shooting-star {
            position: absolute;
            width: 3px;
            height: 3px;
            background: linear-gradient(45deg, #fff, #4ecdc4);
            border-radius: 50%;
            animation: shoot 3s linear infinite;
        }

        .shooting-star:before {
            content: '';
            position: absolute;
            top: 50%;
            right: 100%;
            width: 50px;
            height: 1px;
            background: linear-gradient(to right, transparent, #fff, transparent);
            transform: translateY(-50%);
        }

        @keyframes shoot {
            0% {
                transform: translateX(-100px) translateY(100px);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateX(100vw) translateY(-100px);
                opacity: 0;
            }
        }

        .nebula {
            position: absolute;
            width: 300px;
            height: 300px;
            background: radial-gradient(circle, 
                rgba(78, 205, 196, 0.1) 0%,
                rgba(255, 107, 107, 0.1) 30%,
                rgba(69, 183, 209, 0.1) 60%,
                transparent 100%);
            border-radius: 50%;
            filter: blur(30px);
            animation: nebulaDrift 25s ease-in-out infinite;
        }

        @keyframes nebulaDrift {
            0%, 100% { 
                transform: translate(0, 0) scale(1);
                opacity: 0.3;
            }
            25% { 
                transform: translate(50px, -30px) scale(1.2);
                opacity: 0.6;
            }
            50% { 
                transform: translate(-30px, 50px) scale(0.8);
                opacity: 0.4;
            }
            75% { 
                transform: translate(30px, 30px) scale(1.1);
                opacity: 0.5;
            }
        }

        .constellation {
            position: absolute;
            width: 200px;
            height: 200px;
            opacity: 0.6;
            animation: constellationRotate 30s linear infinite;
        }

        @keyframes constellationRotate {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        .constellation-star {
            position: absolute;
            width: 2px;
            height: 2px;
            background: #fff;
            border-radius: 50%;
            box-shadow: 0 0 4px rgba(255, 255, 255, 0.8);
        }

        .constellation-line {
            position: absolute;
            height: 1px;
            background: linear-gradient(to right, transparent, rgba(255, 255, 255, 0.3), transparent);
            transform-origin: left center;
        }

        .letter {
            display: inline-block;
            transition: all 0.3s ease;
            animation: letterFloat 4s ease-in-out infinite;
        }

        .letter:nth-child(even) {
            animation-delay: 0.2s;
        }

        .letter:nth-child(odd) {
            animation-delay: 0.4s;
        }

        @keyframes letterFloat {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        .name:hover .letter {
            animation: letterBounce 0.6s ease-in-out infinite;
        }

        @keyframes letterBounce {
            0%, 50%, 100% { transform: translateY(0px); }
            25% { transform: translateY(-15px); }
            75% { transform: translateY(-5px); }
        }

        .name:hover .letter:nth-child(1) { animation-delay: 0.1s; }
        .name:hover .letter:nth-child(2) { animation-delay: 0.2s; }
        .name:hover .letter:nth-child(3) { animation-delay: 0.3s; }
        .name:hover .letter:nth-child(4) { animation-delay: 0.4s; }
        .name:hover .letter:nth-child(5) { animation-delay: 0.5s; }
        .name:hover .letter:nth-child(6) { animation-delay: 0.6s; }
        .name:hover .letter:nth-child(7) { animation-delay: 0.7s; }
        .name:hover .letter:nth-child(8) { animation-delay: 0.8s; }

        .surname {
            font-size: 2.5rem;
            margin-top: 20px;
            background: linear-gradient(45deg, #a8edea, #fed6e3, #d299c2, #fef9d7);
            background-size: 400% 400%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: gradientShift 4s ease-in-out infinite reverse;
            display: inline-block;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .surname:hover {
            transform: scale(1.05) skew(-5deg);
            filter: drop-shadow(0 0 20px rgba(168, 237, 234, 0.8));
        }

        .ripple {
            position: absolute;
            border-radius: 50%;
            background: radial-gradient(circle, rgba(255, 107, 107, 0.6), transparent);
            transform: scale(0);
            animation: rippleEffect 0.6s ease-out;
            pointer-events: none;
        }

        @keyframes rippleEffect {
            to {
                transform: scale(4);
                opacity: 0;
            }
        }

        @media (max-width: 768px) {
            .name {
                font-size: 2.5rem;
            }
            .surname {
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>
    <div class="name-container">
        <div class="name" id="firstName">
            <span class="letter">K</span>
            <span class="letter">u</span>
            <span class="letter">s</span>
            <span class="letter">h</span>
            <span class="letter">a</span>
            <span class="letter">g</span>
            <span class="letter">r</span>
            <span class="letter">a</span>
        </div>
        <div class="surname" id="lastName">
            <span class="letter">S</span>
            <span class="letter">i</span>
            <span class="letter">s</span>
            <span class="letter">o</span>
            <span class="letter">d</span>
            <span class="letter">i</span>
            <span class="letter">a</span>
        </div>
    </div>

    <!-- Space Background Elements -->
    <div class="nebula" style="top: 10%; left: 20%;"></div>
    <div class="nebula" style="top: 60%; right: 15%; animation-delay: -10s;"></div>
    <div class="nebula" style="bottom: 20%; left: 10%; animation-delay: -15s;"></div>

    <script>
        // Create floating particles
        function createParticle() {
            const particle = document.createElement('div');
            particle.className = 'particle';
            particle.style.left = Math.random() * window.innerWidth + 'px';
            particle.style.top = window.innerHeight + 'px';
            particle.style.animationDelay = Math.random() * 6 + 's';
            particle.style.animationDuration = (Math.random() * 4 + 4) + 's';
            document.body.appendChild(particle);

            // Remove particle after animation
            setTimeout(() => {
                if (particle.parentNode) {
                    particle.parentNode.removeChild(particle);
                }
            }, 8000);
        }

        // Create stars
        function createStar() {
            const star = document.createElement('div');
            star.className = 'star';
            star.style.left = Math.random() * window.innerWidth + 'px';
            star.style.top = Math.random() * window.innerHeight + 'px';
            star.style.width = (Math.random() * 3 + 1) + 'px';
            star.style.height = star.style.width;
            star.style.animationDelay = Math.random() * 2 + 's';
            star.style.animationDuration = (Math.random() * 3 + 2) + 's';
            document.body.appendChild(star);
        }

        // Create shooting stars
        function createShootingStar() {
            const shootingStar = document.createElement('div');
            shootingStar.className = 'shooting-star';
            shootingStar.style.left = '-100px';
            shootingStar.style.top = Math.random() * (window.innerHeight * 0.6) + 'px';
            shootingStar.style.animationDelay = Math.random() * 2 + 's';
            shootingStar.style.animationDuration = (Math.random() * 2 + 2) + 's';
            document.body.appendChild(shootingStar);

            setTimeout(() => {
                if (shootingStar.parentNode) {
                    shootingStar.parentNode.removeChild(shootingStar);
                }
            }, 5000);
        }

        // Create constellation
        function createConstellation() {
            const constellation = document.createElement('div');
            constellation.className = 'constellation';
            constellation.style.left = Math.random() * (window.innerWidth - 200) + 'px';
            constellation.style.top = Math.random() * (window.innerHeight - 200) + 'px';

            // Create constellation pattern (Big Dipper-like)
            const stars = [
                {x: 20, y: 30},
                {x: 40, y: 20},
                {x: 70, y: 25},
                {x: 90, y: 35},
                {x: 110, y: 45},
                {x: 140, y: 55},
                {x: 170, y: 60}
            ];

            stars.forEach((starPos, index) => {
                const star = document.createElement('div');
                star.className = 'constellation-star';
                star.style.left = starPos.x + 'px';
                star.style.top = starPos.y + 'px';
                constellation.appendChild(star);

                // Connect stars with lines
                if (index < stars.length - 1) {
                    const line = document.createElement('div');
                    line.className = 'constellation-line';
                    const nextStar = stars[index + 1];
                    const distance = Math.sqrt(Math.pow(nextStar.x - starPos.x, 2) + Math.pow(nextStar.y - starPos.y, 2));
                    const angle = Math.atan2(nextStar.y - starPos.y, nextStar.x - starPos.x) * (180 / Math.PI);
                    
                    line.style.width = distance + 'px';
                    line.style.left = starPos.x + 'px';
                    line.style.top = starPos.y + 'px';
                    line.style.transform = `rotate(${angle}deg)`;
                    constellation.appendChild(line);
                }
            });

            document.body.appendChild(constellation);
        }

        // Initialize space elements
        function initializeSpace() {
            // Create multiple stars
            for (let i = 0; i < 100; i++) {
                createStar();
            }

            // Create constellations
            for (let i = 0; i < 3; i++) {
                setTimeout(() => createConstellation(), i * 1000);
            }
        }

        // Initialize everything
        initializeSpace();

        // Create particles periodically
        setInterval(createParticle, 300);

        // Create shooting stars periodically
        setInterval(createShootingStar, 4000);

        // Add ripple effect on click
        function createRipple(e) {
            const ripple = document.createElement('div');
            ripple.className = 'ripple';
            
            const rect = e.target.getBoundingClientRect();
            const size = Math.max(rect.width, rect.height);
            
            ripple.style.width = ripple.style.height = size + 'px';
            ripple.style.left = (e.clientX - rect.left - size / 2) + 'px';
            ripple.style.top = (e.clientY - rect.top - size / 2) + 'px';
            
            e.target.appendChild(ripple);
            
            setTimeout(() => {
                if (ripple.parentNode) {
                    ripple.parentNode.removeChild(ripple);
                }
            }, 600);
        }

        // Add click event listeners
        document.getElementById('firstName').addEventListener('click', createRipple);
        document.getElementById('lastName').addEventListener('click', createRipple);

        // Add keyboard interaction
        document.addEventListener('keydown', (e) => {
            if (e.key === ' ') {
                const names = document.querySelectorAll('.name, .surname');
                names.forEach(name => {
                    name.style.transform = 'scale(1.2) rotate(360deg)';
                    setTimeout(() => {
                        name.style.transform = '';
                    }, 1000);
                });
            }
        });

        // Add mouse trail effect
        let mouseTrail = [];
        document.addEventListener('mousemove', (e) => {
            const trail = document.createElement('div');
            trail.style.position = 'absolute';
            trail.style.left = e.clientX + 'px';
            trail.style.top = e.clientY + 'px';
            trail.style.width = '6px';
            trail.style.height = '6px';
            trail.style.background = 'radial-gradient(circle, rgba(255, 107, 107, 0.8), transparent)';
            trail.style.borderRadius = '50%';
            trail.style.pointerEvents = 'none';
            trail.style.zIndex = '5';
            trail.style.animation = 'trailFade 0.5s ease-out forwards';
            
            document.body.appendChild(trail);
            mouseTrail.push(trail);
            
            if (mouseTrail.length > 10) {
                const oldTrail = mouseTrail.shift();
                if (oldTrail.parentNode) {
                    oldTrail.parentNode.removeChild(oldTrail);
                }
            }
            
            setTimeout(() => {
                if (trail.parentNode) {
                    trail.parentNode.removeChild(trail);
                }
            }, 500);
        });

        // Add CSS for trail fade animation
        const style = document.createElement('style');
        style.textContent = `
            @keyframes trailFade {
                0% { opacity: 1; transform: scale(1); }
                100% { opacity: 0; transform: scale(0); }
            }
        `;
        document.head.appendChild(style);

        // Add subtle 3D rotation on mouse move
        document.addEventListener('mousemove', (e) => {
            const names = document.querySelectorAll('.name, .surname');
            const centerX = window.innerWidth / 2;
            const centerY = window.innerHeight / 2;
            
            const rotateX = (e.clientY - centerY) / 20;
            const rotateY = (e.clientX - centerX) / 20;
            
            names.forEach(name => {
                if (!name.matches(':hover')) {
                    name.style.transform = `perspective(1000px) rotateX(${rotateX}deg) rotateY(${rotateY}deg)`;
                }
            });
        });
    </script>
</body>
</html>


<p align="left"> <img src="https://komarev.com/ghpvc/?username=kushgit07&label=Profile%20views&color=0e75b6&style=flat" alt="kushgit07" /> </p>

<p align="left"> <a href="https://github.com/ryo-ma/github-profile-trophy"><img src="https://github-profile-trophy.vercel.app/?username=kushgit07" alt="kushgit07" /></a> </p>


- 🔭 I’m currently working on [promptforage](https://kushgit07.github.io/PromptForge/)

- 🌱 I’m currently learning **react js , node js , next js , express js , mongodb ....**

- 👯 I’m looking to collaborate on **MERN STACK**

- 👨‍💻 All of my projects are available at [https://github.com/kushgit07](https://github.com/kushgit07)

- 💬 Ask me about **react , javascript ,express js , sql , mongodb ...**

- 📫 How to reach me **kushagrasisodia27@gmail.com**

- 📄 Know about my experiences [https://github.com/kushgit07/MY_RESUME/blob/main/Kushagra%20Sisodia_Resume.pdf](https://github.com/kushgit07/MY_RESUME/blob/main/Kushagra%20Sisodia_Resume.pdf)

- ⚡ Fun fact **I AM A FUNNY GUY WITH A GOOD SENSE OF HUMOUR**

  
<!-- Snake Game Repo View -->

<div align="center">
  <img src="https://profile-readme-generator.com/assets/snake.svg" alt="Snake animation" />
</div>


<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://www.linkedin.com/in/kushagra-s-72758a250?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3B3%2FWYQct%2FTfiGZ6ABNu9%2B5w%3D%3D" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="KUSHAGRA SISODIA" height="30" width="40" /></a>
<a href="https://www.leetcode.com/kushagrasisodia27" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/leet-code.svg" alt="kushagrasisodia27" height="30" width="40" /></a>
<a href="https://auth.geeksforgeeks.org/user/kushagras4v4d" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/geeks-for-geeks.svg" alt="kushagras4v4d" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://angular.io" target="_blank" rel="noreferrer"> <img src="https://angular.io/assets/images/logos/angular/angular.svg" alt="angular" width="40" height="40"/> </a> <a href="https://aws.amazon.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"/> </a> <a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a> <a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/> </a> <a href="https://canvasjs.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/Hardik0307/Hardik0307/master/assets/canvasjs-charts.svg" alt="canvasjs" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cpp/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cs/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg" alt="csharp" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.electronjs.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/electron/electron-original.svg" alt="electron" width="40" height="40"/> </a> <a href="https://expressjs.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/express/express-original-wordmark.svg" alt="express" width="40" height="40"/> </a> <a href="https://www.figma.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" alt="figma" width="40" height="40"/> </a> <a href="https://firebase.google.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" alt="firebase" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://golang.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/go/go-original.svg" alt="go" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.adobe.com/in/products/illustrator.html" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/adobe_illustrator/adobe_illustrator-icon.svg" alt="illustrator" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://kafka.apache.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/apache_kafka/apache_kafka-icon.svg" alt="kafka" width="40" height="40"/> </a> <a href="https://www.mathworks.com/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/2/21/Matlab_Logo.png" alt="matlab" width="40" height="40"/> </a> <a href="https://www.mongodb.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://nextjs.org/" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/nextjs-2.svg" alt="nextjs" width="40" height="40"/> </a> <a href="https://www.nginx.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nginx/nginx-original.svg" alt="nginx" width="40" height="40"/> </a> <a href="https://nodejs.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a> <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a> <a href="https://www.php.net" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg" alt="php" width="40" height="40"/> </a> <a href="https://postman.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" alt="postman" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> </a> <a href="https://reactnative.dev/" target="_blank" rel="noreferrer"> <img src="https://reactnative.dev/img/header_logo.svg" alt="reactnative" width="40" height="40"/> </a> <a href="https://redux.js.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redux/redux-original.svg" alt="redux" width="40" height="40"/> </a> <a href="https://www.sqlite.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/sqlite/sqlite-icon.svg" alt="sqlite" width="40" height="40"/> </a> <a href="https://tailwindcss.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tailwindcss/tailwindcss-icon.svg" alt="tailwind" width="40" height="40"/> </a> <a href="https://www.typescriptlang.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="typescript" width="40" height="40"/> </a> </p>

<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=kushgit07&show_icons=true&locale=en&layout=compact" alt="kushgit07" /></p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=kushgit07&show_icons=true&locale=en" alt="kushgit07" /></p>

<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=kushgit07&" alt="kushgit07" /></p>

