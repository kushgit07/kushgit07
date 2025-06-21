<h1 align="center">Hi 👋, I'm KUSHAGRA SISODIA</h1>
<h3 align="center">A passionate frontend developer from India with knowledge in computer science stuff</h3>
<svg width="400" height="80" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="textGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#ffffff;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#f0f8ff;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#ffffff;stop-opacity:1" />
    </linearGradient>
    
    <linearGradient id="hoverGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#ffd700;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#ffeb3b;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#ffd700;stop-opacity:1" />
    </linearGradient>
    
    <radialGradient id="bgGradient" cx="50%" cy="50%" r="70%">
      <stop offset="0%" style="stop-color:#1a1a2e;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#16213e;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#0f0f23;stop-opacity:1" />
    </radialGradient>
    
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge> 
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  
  <style>
    .background {
      fill: url(#bgGradient);
    }
    
    .star {
      fill: #ffffff;
      opacity: 0.8;
    }
    
    .star-twinkle {
      animation: twinkle 2s ease-in-out infinite;
    }
    
    .star-float {
      animation: float 4s ease-in-out infinite;
    }
    
    .star-pulse {
      animation: pulse 3s ease-in-out infinite;
    }
    
    @keyframes twinkle {
      0%, 100% { opacity: 0.3; transform: scale(0.8); }
      50% { opacity: 1; transform: scale(1.2); }
    }
    
    @keyframes float {
      0%, 100% { transform: translateY(0px) translateX(0px); }
      25% { transform: translateY(-3px) translateX(2px); }
      50% { transform: translateY(2px) translateX(-1px); }
      75% { transform: translateY(-1px) translateX(3px); }
    }
    
    @keyframes pulse {
      0%, 100% { opacity: 0.5; }
      50% { opacity: 1; }
    }
    
    .name-text {
      font-family: 'Arial', sans-serif;
      font-size: 28px;
      font-weight: bold;
      fill: url(#textGradient);
      cursor: pointer;
      transition: all 0.3s ease;
      filter: url(#glow);
    }
    
    .name-text:hover {
      fill: url(#hoverGradient);
      transform: scale(1.05);
      filter: url(#glow) drop-shadow(0px 0px 10px rgba(255,215,0,0.6));
    }
    
    .letter {
      animation: wave 2s ease-in-out infinite;
    }
    
    .letter:nth-child(1) { animation-delay: 0s; }
    .letter:nth-child(2) { animation-delay: 0.1s; }
    .letter:nth-child(3) { animation-delay: 0.2s; }
    .letter:nth-child(4) { animation-delay: 0.3s; }
    .letter:nth-child(5) { animation-delay: 0.4s; }
    .letter:nth-child(6) { animation-delay: 0.5s; }
    .letter:nth-child(7) { animation-delay: 0.6s; }
    .letter:nth-child(8) { animation-delay: 0.7s; }
    .letter:nth-child(9) { animation-delay: 0.8s; }
    .letter:nth-child(10) { animation-delay: 0.9s; }
    .letter:nth-child(11) { animation-delay: 1.0s; }
    .letter:nth-child(12) { animation-delay: 1.1s; }
    .letter:nth-child(13) { animation-delay: 1.2s; }
    .letter:nth-child(14) { animation-delay: 1.3s; }
    .letter:nth-child(15) { animation-delay: 1.4s; }
    
    @keyframes wave {
      0%, 100% { transform: translateY(0px); }
      50% { transform: translateY(-5px); }
    }
    
    .name-text:hover .letter {
      animation: bounce 0.6s ease;
    }
    
    @keyframes bounce {
      0%, 100% { transform: translateY(0px); }
      25% { transform: translateY(-8px); }
      50% { transform: translateY(-4px); }
      75% { transform: translateY(-6px); }
    }
  </style>
  
  <!-- Starry Background -->
  <rect width="400" height="80" class="background"/>
  
  <!-- Animated Stars -->
  <!-- Large twinkling stars -->
  <circle cx="50" cy="20" r="1.5" class="star star-twinkle" style="animation-delay: 0s;"/>
  <circle cx="120" cy="15" r="1" class="star star-pulse" style="animation-delay: 0.5s;"/>
  <circle cx="180" cy="25" r="1.2" class="star star-float" style="animation-delay: 1s;"/>
  <circle cx="280" cy="18" r="1" class="star star-twinkle" style="animation-delay: 1.5s;"/>
  <circle cx="350" cy="22" r="1.3" class="star star-pulse" style="animation-delay: 2s;"/>
  
  <!-- Medium stars -->
  <circle cx="30" cy="60" r="0.8" class="star star-float" style="animation-delay: 0.3s;"/>
  <circle cx="90" cy="65" r="1" class="star star-twinkle" style="animation-delay: 0.8s;"/>
  <circle cx="150" cy="70" r="0.7" class="star star-pulse" style="animation-delay: 1.3s;"/>
  <circle cx="220" cy="62" r="0.9" class="star star-float" style="animation-delay: 1.8s;"/>
  <circle cx="320" cy="68" r="0.8" class="star star-twinkle" style="animation-delay: 2.3s;"/>
  <circle cx="380" cy="65" r="1" class="star star-pulse" style="animation-delay: 2.8s;"/>
  
  <!-- Small scattered stars -->
  <circle cx="70" cy="35" r="0.5" class="star star-pulse" style="animation-delay: 0.2s;"/>
  <circle cx="140" cy="55" r="0.4" class="star star-twinkle" style="animation-delay: 0.7s;"/>
  <circle cx="200" cy="10" r="0.6" class="star star-float" style="animation-delay: 1.2s;"/>
  <circle cx="260" cy="70" r="0.5" class="star star-pulse" style="animation-delay: 1.7s;"/>
  <circle cx="300" cy="40" r="0.4" class="star star-twinkle" style="animation-delay: 2.2s;"/>
  <circle cx="370" cy="45" r="0.6" class="star star-float" style="animation-delay: 2.7s;"/>
  <circle cx="25" cy="40" r="0.4" class="star star-pulse" style="animation-delay: 3.2s;"/>
  <circle cx="110" cy="30" r="0.5" class="star star-twinkle" style="animation-delay: 3.7s;"/>
  <circle cx="240" cy="35" r="0.4" class="star star-float" style="animation-delay: 4.2s;"/>
  
  <!-- Tiny stars for depth -->
  <circle cx="60" cy="50" r="0.3" class="star star-float" style="animation-delay: 0.1s;"/>
  <circle cx="100" cy="45" r="0.2" class="star star-pulse" style="animation-delay: 0.6s;"/>
  <circle cx="160" cy="40" r="0.3" class="star star-twinkle" style="animation-delay: 1.1s;"/>
  <circle cx="290" cy="55" r="0.2" class="star star-float" style="animation-delay: 1.6s;"/>
  <circle cx="340" cy="35" r="0.3" class="star star-pulse" style="animation-delay: 2.1s;"/>
  <circle cx="15" cy="25" r="0.2" class="star star-twinkle" style="animation-delay: 2.6s;"/>
  <circle cx="390" cy="30" r="0.3" class="star star-float" style="animation-delay: 3.1s;"/>
  
  <g class="name-text">
    <text x="200" y="45" text-anchor="middle">
      <tspan class="letter">K</tspan><tspan class="letter">U</tspan><tspan class="letter">S</tspan><tspan class="letter">H</tspan><tspan class="letter">A</tspan><tspan class="letter">G</tspan><tspan class="letter">R</tspan><tspan class="letter">A</tspan><tspan class="letter"> </tspan><tspan class="letter">S</tspan><tspan class="letter">I</tspan><tspan class="letter">S</tspan><tspan class="letter">O</tspan><tspan class="letter">D</tspan><tspan class="letter">I</tspan><tspan class="letter">A</tspan>
    </text>
  </g>
</svg>

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

