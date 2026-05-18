<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Shakir Ali | Author</title>

<!-- Google Font -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

<style>
body{margin:0;font-family:'Poppins',sans-serif;background:#0b0b0b;color:#fff}
:root{--gold:#d4af37}

header{text-align:center;padding:50px;background:#000}
header img{width:140px;height:140px;border-radius:50%;border:3px solid var(--gold)}
h1{color:var(--gold);margin:10px 0}

.container{max-width:1100px;margin:auto;padding:20px}

section{margin:50px 0}
h2{color:var(--gold)}

.card{background:#141414;padding:20px;border-radius:12px;margin-top:15px;transition:0.3s}
.card:hover{transform:scale(1.03)}

a{color:var(--gold);text-decoration:none}

button{padding:10px 15px;border:none;background:var(--gold);cursor:pointer;border-radius:6px}

/* WhatsApp Button */
.whatsapp{
position:fixed;
bottom:20px;
right:20px;
background:#25D366;
padding:12px 15px;
border-radius:50%;
font-size:20px;
}

/* Gallery */
.gallery img{
width:100%;
max-width:250px;
margin:10px;
border-radius:10px;
}

</style>
</head>
<body>

<header>
<img src="1000118516.jpg">
<h1>Shakir Ali ।  शाकिर अली</h1>
<p>Author | Book Formatter</p>
</header>

<div class="container">

<section>
<h2>👤 Introduction</h2>
<div class="card">
<p>Main ek author aur professional book formatter hoon. Mai Hindi aur Urdu content likhta hoon aur logon ke liye books design karta hoon.</p>
</div>
</section>

<section>
<h2>💼 Profession</h2>
<div class="card">
<ul>
<li>📖 Book Writing</li>
<li>📐 Book Formatting (InDesign, PDF)</li>
<li>📚 Magazine Layout Design</li>
</ul>
</div>
</section>

<section>
<h2>📚 My Books</h2>
<div class="card">
<p><a href="books/bachpan/index.html">📖 बचपन</a></p>
</div>
</section>

<section>
<h2>🖼 Photo Gallery</h2>
<div class="card gallery">
<img src="gallery/1.jpg">
<img src="gallery/2.jpg">
</div>
</section>

<section>
<h2>📝 Articles</h2>
<div class="card">
<p><a href="#">Article 1 - Jaldi add karo</a></p>
</div>
</section>

<section>
<h2>📞 Contact</h2>
<div class="card">
<p>📱 WhatsApp: <a href="https://wa.me/91XXXXXXXXXX">Click Here</a></p>
<p>📷 Instagram: <a href="#">imshakiralii</a></p>
</div>
</section>

</div>

<!-- WhatsApp Floating Button -->
<a href="https://wa.me/91XXXXXXXXXX" class="whatsapp">💬</a>

</body>
</html>

<!-- ================= BOOK PAGE ================= -->

<!DOCTYPE html>
<html>
<head>
<title>Book</title>
<style>
body{font-family:Poppins;background:#111;color:#fff;padding:20px}
a{color:gold}
.highlight{background:yellow;color:black}
</style>

<script>
function searchText(){
let input=document.getElementById('search').value;
let content=document.getElementById('content');
let text=content.innerHTML;
let regex=new RegExp(input,'gi');
content.innerHTML=text.replace(regex,match=>`<span class='highlight'>${match}</span>`);
}
</script>

</head>
<body>

<h1>📖 Book Title</h1>
<img src="cover.jpg" width="200">

<p><a href="book.pdf" download>📥 Download PDF</a></p>

<input type="text" id="search" placeholder="Search...">
<button onclick="searchText()">Search</button>

<ul>
<li><a href="chapter1.html">Chapter 1</a></li>
<li><a href="chapter2.html">Chapter 2</a></li>
</ul>

<div id="content">
Yahan pura book ka hidden ya visible content dal sakte ho jisme search chalega
</div>

</body>
</html>

<!-- ================= CHAPTER ================= -->

<!DOCTYPE html>
<html>
<head>
<title>Chapter</title>
<style>
body{font-family:Poppins;background:#111;color:#fff;padding:20px}
.nav{margin-top:30px}
img{width:100%;max-width:500px}
</style>
</head>
<body>

<h1>Chapter 1</h1>
<img src="images/ch1.jpg">
<p>Chapter content yahan likho...</p>

<div class="nav">
<a href="chapter2.html">➡ Next</a> |
<a href="index.html">⬅ Back</a>
</div>

</body>
</html>
