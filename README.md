# PraktikumWEB1
## HTML
HTML (Hyper Text Markup Language) merupakan bahasa markup standar untuk membuat halaman Web. HTML terdiri dari serangkaian elemen yang memberi tahu browser cara menampilkan konten. Elemen juga memberi label pada bagian konten seperti "Hello World!", "ini adalah judul", dll.
### Contoh dokumen HTML sederhana
```
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>

```
Memiliki output sebagai berikut:

<img width="227" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/34eda089-e811-4fb3-8833-b7aeb36772ed">

* Deklarasi < !DOCTYPE html > mendefinisikan bahwa dokumen ini adalah dokumen HTML5
* Elemen < html > adalah elemen akar dari halaman HTML
* Elemen tersebut head berisi informasi meta tentang halaman HTML
* Elemen < title > menentukan judul untuk halaman HTML (yang ditampilkan di bilah judul browser atau di tab halaman)
* Elemen body mendefinisikan badan dokumen, dan merupakan wadah untuk semua konten yang terlihat, seperti judul, paragraf, gambar, hyperlink, tabel, daftar, dll.
* Elemen < h1 > mendefinisikan judul besar
* Elemen < p > mendefinisikan paragraf
### HTML Dasar
Semua dokumen HTML harus dimulai dengan deklarasi tipe dokumen: < !DOCTYPE html >. Deklarasi ini < !DOCTYPE > tidak membedakan huruf besar-kecil. Bagian yang terlihat dari dokumen HTML adalah antara < body > dan < /body >.
```
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

<h1>This is heading 1</h1>
<h2>This is heading 2</h2>
<h3>This is heading 3</h3>
<h4>This is heading 4</h4>
<h5>This is heading 5</h5>
<h6>This is heading 6</h6>

<p>This is a paragraph.</p>
<p>This is another paragraph.</p>

<h2>HTML Links</h2>
<p>HTML links are defined with the a tag:</p>

<a href="https://www.w3schools.com">This is a link</a>

<h2>HTML Images</h2>
<p>HTML images are defined with the img tag:</p>

<img src="Screenshot 2024-03-19 051922.png" alt="W3Schools.com" width="200" height="120">


</body>
</html>
```
Memiliki output sebagai berikut:
* Heading (Judul) HTML ditentukan dengan tag < h1 > sampai < h6 >. < h1 > mendefinisikan judul yang terpenting sedangkan h6 mendefinisikan judul yang tidak terlalu penting.

  <img width="208" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/7a5fdb53-c780-446d-9142-557c1415d413">
* Paragraf HTML didefinisikan dengan tag p.

  <img width="158" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/2351de73-4f8f-4279-982a-336ea7f0c63a">
* Tautan HTML ditentukan dengan tag a. Tujuan tautan ditentukan dalam atribut href. Atribut digunakan untuk memberikan informasi tambahan tentang elemen HTML.

  <img width="214" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/85468680-0537-4622-a0e4-745880efbe26">
* Gambar HTML ditentukan dengan tag img. File sumber ( src), teks alternatif ( alt), width, dan height disediakan sebagai atribut.

  <img width="238" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/4437bb69-1b85-4c40-b04b-0ac8bab7c4b7">

### Tabel HTML
Setiap sel tabel ditentukan oleh tag < td > dan < /td > sedangkan setiap baris tabel dimulai dengan < tag > tr dan < /tr > . Segala sesuatu di dalam tag tersebut merupakan konten sel tabel.
```
<!DOCTYPE html>
<html>
<head>
<style>
table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

td, th {
  border: 1px solid grey;
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {
  background-color: #dddddd;
}
</style>
</head>
<body>

<h2>HTML Table</h2>

<table>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>SM Entertainment</td>
    <td>Lee Sooman</td>
    <td>South Korea</td>
  </tr>
  <tr>
    <td>YG Entertainment</td>
    <td>Yang Hyunsuk</td>
    <td>South Korea</td>
  </tr>
  <tr>
    <td>JYP Entertainment</td>
    <td>Park Jinyoung</td>
    <td>South Korea</td>
  </tr>
  <tr>
    <td>Yorozuya Gin-san</td>
    <td>Sakata Gintoki</td>
    <td>Japan</td>
  </tr>
  <tr>
    <td>Ghibli Studio</td>
    <td>Totoro</td>
    <td>Japan</td>
  </tr>
</table>

</body>
</html>
```
Memiliki output sebagai berikut:

<img width="919" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/a8bcd8e6-e3b5-4cc4-9273-13973487c782">

### Elemen Div HTML
Elemen ini < div > secara default adalah elemen blok, artinya elemen ini mengambil semua lebar yang tersedia, dan dilengkapi dengan jeda baris sebelum dan sesudahnya. Elemen tersebut < div > tidak memiliki atribut yang diperlukan, tetapi style, classdan id bersifat umum.
```
<!DOCTYPE html>
<html>
<style>
.div1 {
  background-color: #FFF4A3;
}

.container {
  background-color: #FFF4A3;
}

.element {
  width: 300px;
  margin: auto;
  background-color: #FFF4A3;
}

.float {
  width:100%;
  overflow:auto;
}
.float div {
  width:33%;  
  float:left;
}

.ib {
  width:30%;  
  display:inline-block;
}

.flex {
  display: flex;
}
.flex > div {
  width:33%;
}

.grid-container {
  display: grid;
  grid-template-columns: 33% 33% 33%;
}
</style>
<body>

<h1>HTML DIV Example</h1>

Lorem Ipsum <div class="div1">I am a div</div> dolor sit amet.

<p>The yellow background is added to demonstrate the footprint of the DIV element.</p>


<div class="container">
    <h2>London</h2>
    <p>London is the capital city of England.</p>
    <p>London has over 13 million inhabitants.</p>
  </div>
  
  <p>The yellow background is added to demonstrate the footprint of the DIV element.</p>

  <h1>Center align a DIV element</h1>

<div class="element">
  <h2>London</h2>
  <p>London is the capital city of England.</p>
  <p>London has over 13 million inhabitants.</p>

<h1>Aligning div elements side by side</h1>
</div>
<h2>Float</h2>
  <div class="float">

    <div style="background-color:#FFF4A3;">
      <h2>London</h2>
      <p>London is the capital city of England.</p>
      <p>London has over 13 million inhabitants.</p>
    </div>
    
    <div style="background-color:#FFC0C7;">
      <h2>Oslo</h2>
      <p>Oslo is the capital city of Norway.</p>
      <p>Oslo has over 600.000 inhabitants.</p>
    </div>
    
    <div style="background-color:#D9EEE1;">
      <h2>Rome</h2>
      <p>Rome is the capital city of Italy.</p>
      <p>Rome has almost 3 million inhabitants.</p>
    </div>
  
  </div>


    <h1>Flexbox Example</h1>

<p>Align three DIV elements side by side.</p>

<div class="flex">

  <div style="background-color:#FFF4A3;">
    <h2>London</h2>
    <p>London is the capital city of England.</p>
    <p>London has over 13 million inhabitants.</p>
  </div>
  
  <div style="background-color:#FFC0C7;">
    <h2>Oslo</h2>
    <p>Oslo is the capital city of Norway.</p>
    <p>Oslo has over 600.000 inhabitants.</p>
  </div>
  
  <div style="background-color:#D9EEE1;">
    <h2>Rome</h2>
    <p>Rome is the capital city of Italy.</p>
    <p>Rome has almost 3 million.</p>
  </div>

</div>


<h1>Grid Example</h1>

<p>Align three DIV elements side by side.</p>

<div class="grid-container">

<div style="background-color:#FFF4A3;">
  <h2>London</h2>
  <p>London is the capital city of England.</p>
  <p>London has over 13 million inhabitants.</p>
</div>

<div style="background-color:#FFC0C7;">
  <h2>Oslo</h2>
  <p>Oslo is the capital city of Norway.</p>
  <p>Oslo has over 600.000 inhabitants.</p>
</div>

<div style="background-color:#D9EEE1;">
  <h2>Rome</h2>
  <p>Rome is the capital city of Italy.</p>
  <p>Rome has almost 3 million inhabitants.</p>
</div>

</div>

</body>
</html>
```

<img width="909" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/e5fa1582-20a3-46ab-9d33-540bec766b57">


* Div sebagai wadah
  
  Elemen ini < div > sering digunakan untuk mengelompokkan bagian-bagian halaman web menjadi satu.

  <img width="911" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/9ee04f7e-6aee-4853-b994-6cf1805eca84">

* Elemen < div > Rata Tengah

  Jika terdapat < div > elemen yang lebarnya tidak 100%, setel margin properti CSS ke auto agar dapat meratakannya di tengah.

  <img width="919" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/95988e84-fec6-40e2-89eb-353025846762">

* Menyelaraskan elemen < div > secara berdampingan dengan Float

  Properti CSS float digunakan untuk memposisikan dan memformat konten serta memungkinkan elemen melayang bersebelahan, bukan di atas satu sama lain.

  <img width="905" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/310e5000-bb98-475f-b72a-7ddeb57b564c">

* Menyelaraskan elemen < div > secara berdampingan dengan Flex

  Modul Tata Letak CSS Flexbox diperkenalkan untuk memudahkan merancang struktur tata letak responsif yang fleksibel tanpa menggunakan float atau positioning. Agar metode fleksibel CSS berfungsi, kelilingi < div > elemen dengan < div > elemen lain dan berikan status sebagai wadah fleksibel.

  <img width="907" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/f32838ba-f301-4aff-8bc2-2cd05d93d9cb">

* Menyelaraskan elemen < div > secara berdampingan dengan Grid

  Modul Tata Letak Grid CSS menawarkan sistem tata letak berbasis grid, dengan baris dan kolom, sehingga memudahkan mendesain halaman web tanpa harus menggunakan float dan positioning.

  Kedengarannya hampir sama dengan flex, namun memiliki kemampuan untuk menentukan lebih dari satu baris dan memposisikan setiap baris secara individual.

  Metode grid CSS mengharuskan Anda mengelilingi < div > elemen dengan < div > elemen lain dan memberikan status sebagai wadah grid, dan Anda harus menentukan lebar setiap kolom.

<img width="892" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/cfcf3ca7-81ba-47b5-bdcc-fcd40af8aded">

## CSS
CSS (Cascading Style Sheet) menjelaskan bagaimana elemen HTML ditampilkan di layar. CSS menghemat banyak pekerjaan dengan mengontrol tata letak beberapa halaman web sekaligus. Stylesheet eksternal disimpan dalam file CSS.
### Contoh CSS
```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: lightblue;
}

h1 {
  color: white;
  text-align: center;
}

p {
  font-family: verdana;
  font-size: 20px;
}
</style>
</head>
<body>

<h1>CSS Home Example</h1>
<p>Ikan hiu makan tomat</p>
<p>I love u tomat</p>

</body>
</html>
```
Memiliki output sebagai berikut:

<img width="918" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/9480b283-04e0-4d9a-84f0-2a990ebcb3d2">

### Cara Menambahkan CSS
* CSS Eksternal
  Dengan style sheet eksternal, Anda dapat mengubah tampilan seluruh situs web hanya dengan mengubah satu file!

Setiap halaman HTML harus menyertakan referensi ke file style sheet eksternal di dalam elemen < link >, di dalam bagian head.

  <img width="349" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/0963b589-2c9a-4fd9-800d-e8841be7010a">

<img width="305" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/5beb503a-e654-4414-9198-69f32b74a3b3">

  Memiliki output sebagai berikut:

  <img width="239" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/0ea68f7c-3544-4cc3-af7c-e141bea82005">

* CSS Internal
  Lembar gaya internal dapat digunakan jika satu halaman HTML memiliki gaya yang unik. Gaya internal didefinisikan di dalam elemen < style >, di dalam bagian head.

<img width="271" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/a555d22f-ba15-4601-b2fb-3f4f3a397566">


  Memiliki output sebagai berikut:

  <img width="295" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/4b14778b-3c8b-4a48-b0c4-4b0982bc1bcc">

* CSS Inline
  Gaya inline dapat digunakan untuk menerapkan gaya unik pada satu elemen. Untuk menggunakan gaya sebaris, tambahkan atribut style ke elemen yang relevan. Atribut style dapat berisi properti CSS apa pun.

  <img width="469" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/b7c4b886-6e76-455f-ae8c-6b6bdd9c3f73">


Memiliki output sebagai berikut:

<img width="922" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/d89dafa5-1ffa-41b0-b13f-0ba23da219f7">


## Javascript
JavaScript adalah bahasa pemrograman Web paling populer di dunia. JavaScript dapat mengubah konten HTML. Salah satu dari banyak metode JavaScript HTML adalah getElementById().
```
<!DOCTYPE html>
<html>
<body>

<h2>What Can JavaScript Do?</h2>

<p id="demo">JavaScript can change HTML content. Let's try it by clicking the button below.</p>

<button type="button" onclick='document.getElementById("demo").innerHTML = "Hello JavaScript!"'>Click Here!</button>


<h2>What Can JavaScript Do?</h2>

<p id="demo2">JavaScript can change the style of an HTML element. JavaScript accept both double and single quotes</p>

<button type="button" onclick="document.getElementById('demo2').style.fontSize='35px'">Click Me!</button>



<h2>What Can JavaScript Do?</h2>

<p>JavaScript can change HTML attribute values.</p>

<p>In this case JavaScript changes the value of the src (source) attribute of an image.</p>

<button onclick="document.getElementById('myImage').src='https://www.w3schools.com/js/pic_bulbon.gif'">Turn on the light</button>

<img id="myImage" src="https://www.w3schools.com/js/pic_bulboff.gif" style="width:100px">

<button onclick="document.getElementById('myImage').src='https://www.w3schools.com/js/pic_bulboff.gif'">Turn off the light</button>


<h2>What Can JavaScript Do?</h2>

<p id="demo3">JavaScript can hide HTML elements.</p>

<button type="button" onclick="document.getElementById('demo3').style.display='none'">Click Me!</button>


<h2>What Can JavaScript Do?</h2>

<p>JavaScript can show hidden HTML elements.</p>

<p id="demo4" style="display:none">Hello JavaScript!</p>

<button type="button" onclick="document.getElementById('demo4').style.display='block'">Click Me!</button>

</body>
</html>
```
Memiliki output sebagai berikut:
* JavaScript Dapat Mengubah Konten HTML

  <img width="428" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/01e6361a-cac3-444d-8386-dd61d3295b0d">

  <img width="311" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/faa24b1b-488b-4243-9900-d6c31f62aa26">

* JavaScript Dapat Mengubah Nilai Atribut HTML
  
  Dalam contoh ini JavaScript mengubah nilai src atribut (sumber) dari  sebuah < img > tag:

  <img width="438" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/922b5f53-6f70-4685-8627-7d266a8907b5">

  <img width="450" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/a06e0a55-e292-44f2-afe1-5c34eae2823b">

* JavaScript Dapat Mengubah Gaya HTML (CSS)
  
  Mengubah gaya elemen HTML, merupakan varian dari mengubah atribut HTML:

<img width="544" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/2d080c95-30d0-4fdf-b289-8182ed54a286">

<img width="905" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/de36a3a2-e0c2-4b60-b58b-b07d6a995c15">

* JavaScript Dapat Menyembunyikan Elemen HTML
  
  Menyembunyikan elemen HTML dapat dilakukan dengan mengubah display gaya:

<img width="245" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/d5481f22-1a89-4e97-9520-b6f3ec7d8139">

<img width="236" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/04024e95-2b2d-4c89-9b33-b1213192f932">

* JavaScript Dapat Menampilkan Elemen HTML
  
  Menampilkan elemen HTML tersembunyi juga dapat dilakukan dengan mengubah display gaya:

<img width="236" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/79c84b80-ea9b-4260-8357-2dd763d724e5">

<img width="241" alt="image" src="https://github.com/adzaniard/PraktikumWEB1/assets/152271194/dcc71bc6-c5b7-40d2-b46c-a9a11ffb7ece">

















 
