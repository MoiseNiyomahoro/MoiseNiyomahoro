
<!-- ========================= -->
<!--        MOTTO              -->
<!-- ========================= -->

<h2 align="center">💡 Motto</h2>

<p align="center">
  <em>"Building Secure, Scalable, and Intelligent Systems for the Future."</em>
</p>

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Professional Typing Animation</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    background:#0d1117;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    font-family:'Segoe UI',sans-serif;
}

.container{
    text-align:center;
}

.static-text{
    color:#8b949e;
    font-size:22px;
    margin-bottom:15px;
    letter-spacing:1px;
}

.dynamic-text{
    color:#58a6ff;
    font-size:42px;
    font-weight:700;
    min-height:60px;
    border-right:4px solid #58a6ff;
    white-space:nowrap;
    overflow:hidden;
    display:inline-block;
    animation:blink .7s infinite;
}

@keyframes blink{
    50%{
        border-color:transparent;
    }
}
</style>
</head>
<body>

<div class="container">
    <div class="static-text">Professional Skills</div>
    <div class="dynamic-text" id="typing"></div>
</div>

<script>

const words = [
    "Computer System Engineer",
    "IoT Developer",
    "Network Administrator",
    "Cybersecurity Assistant"
];

let wordIndex = 0;
let charIndex = 0;
let deleting = false;

const text = document.getElementById("typing");

function typeEffect(){

    const current = words[wordIndex];

    if(!deleting){
        text.textContent = current.substring(0,charIndex++);
        if(charIndex > current.length){
            deleting = true;
            setTimeout(typeEffect,1800);
            return;
        }
    }else{
        text.textContent = current.substring(0,charIndex--);
        if(charIndex < 0){
            deleting = false;
            wordIndex = (wordIndex + 1) % words.length;
            charIndex = 0;
        }
    }

    setTimeout(typeEffect,deleting ? 45 : 90);
}

typeEffect();

</script>

</body>
</html>
<!-- ========================= -->
<!--      CONNECT WITH ME      -->
<!-- ========================= -->

<h2 align="center">📬 Connect With Me</h2>

<p align="center">
I'm always open to collaborating on <strong>Cybersecurity</strong>,
<strong>Computer Networks</strong>, <strong>IoT</strong>, and
<strong>Open Source</strong> projects.
</p>

<p align="center">
  <a href="mailto:niyomahoromoise04@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>

  
<a href="https://wa.me/+250733926182">
  <img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/>
</a>



  <a href="https://www.linkedin.com/in/YOUR_LINKEDIN_USERNAME">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>

  <a href="#">
    <img src="https://img.shields.io/badge/Portfolio-2563EB?style=for-the-badge&logo=google-chrome&logoColor=white"/>
  </a>
</p>

<p align="center">
  📍 <strong>Kigali, Rwanda</strong>
</p>

<p align="center">
  <i>"Code with Purpose • Secure by Design • Innovate Without Limits"</i>
</p>
```
