**index.html**  
  
<!DOCTYPE html>  
<html lang="es">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>El Kristy | Official Links</title>  
  
    <link rel="stylesheet" href="style.css">  
  
    <link rel="preconnect" href="https://fonts.googleapis.com">  
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>  
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;500;700&display=swap" rel="stylesheet">  
</head>  
  
<body>  
  
<div class="container">  
  
    <img src="elkristy.jpg" class="profile">  
  
    <h1>EL KRISTY</h1>  
  
    <p class="bio">  
        Artista Urbano • Trap • Reggaetón  
    </p>  
  
    <a class="btn spotify"  
    href="https://open.spotify.com/artist/5P2CBfpJFDrIPCrwav9Q4v?si=oOxGGQneTL68UUF-g6xLIg&utm_source=copy-link"  
    target="_blank">  
    Spotify  
    </a>  
  
    <a class="btn apple"  
    href="https://music.apple.com/us/artist/el-kristy/1853299600?l=es-MX"  
    target="_blank">  
    Apple Music  
    </a>  
  
    <a class="btn youtube"  
    href="https://youtube.com/@elkristy01?si=ZwKznB94GUO8C38n"  
    target="_blank">  
    YouTube  
    </a>  
  
    <a class="btn instagram"  
    href="https://www.instagram.com/el_kristy_01"  
    target="_blank">  
    Instagram  
    </a>  
  
    <a class="btn tiktok"  
    href="https://www.tiktok.com/@el.kristy3"  
    target="_blank">  
    TikTok  
    </a>  
  
    <a class="btn facebook"  
    href="https://www.facebook.com/share/1Ev33Pxrcy/"  
    target="_blank">  
    Facebook  
    </a>  
  
</div>  
  
<script src="script.js"></script>  
  
</body>  
</html>  
  
**style.css**  
  
*{  
    margin:0;  
    padding:0;  
    box-sizing:border-box;  
}  
  
body{  
    background:#0d0d0d;  
    color:white;  
    font-family:'Montserrat',sans-serif;  
    display:flex;  
    justify-content:center;  
    align-items:center;  
    min-height:100vh;  
}  
  
.container{  
    width:90%;  
    max-width:420px;  
    text-align:center;  
    padding:30px 20px;  
}  
  
.profile{  
    width:170px;  
    height:170px;  
    border-radius:50%;  
    object-fit:cover;  
    border:4px solid #D4AF37;  
    margin-bottom:20px;  
    box-shadow:0 0 30px rgba(212,175,55,.45);  
}  
  
h1{  
    font-size:2rem;  
    letter-spacing:2px;  
    margin-bottom:10px;  
}  
  
.bio{  
    color:#cfcfcf;  
    margin-bottom:35px;  
}  
  
.btn{  
    display:block;  
    text-decoration:none;  
    color:white;  
    padding:16px;  
    margin:15px 0;  
    border-radius:14px;  
    font-weight:700;  
    transition:.3s;  
}  
  
.btn:hover{  
    transform:scale(1.04);  
}  
  
.spotify{  
    background:#1DB954;  
}  
  
.apple{  
    background:#fc3c44;  
}  
  
.youtube{  
    background:#FF0000;  
}  
  
.instagram{  
    background:linear-gradient(45deg,#833AB4,#FD1D1D,#FCAF45);  
}  
  
.tiktok{  
    background:#111;  
    border:2px solid white;  
}  
  
.facebook{  
    background:#1877F2;  
}  
  
footer{  
    margin-top:40px;  
    color:#777;  
    font-size:.9rem;  
}  
  
**script.js**   
  
document.addEventListener("DOMContentLoaded", () => {  
    const buttons = document.querySelectorAll(".btn");  
  
    buttons.forEach((button, index) => {  
        button.style.opacity = "0";  
        button.style.transform = "translateY(20px)";  
  
        setTimeout(() => {  
            button.style.transition = "all .5s ease";  
            button.style.opacity = "1";  
            button.style.transform = "translateY(0)";  
        }, 200 * index);  
    });  
  
    const profile = document.querySelector(".profile");  
  
    profile.style.opacity = "0";  
    profile.style.transform = "scale(.8)";  
  
    setTimeout(() => {  
        profile.style.transition = "all .8s ease";  
        profile.style.opacity = "1";  
        profile.style.transform = "scale(1)";  
    }, 300);  
});  
