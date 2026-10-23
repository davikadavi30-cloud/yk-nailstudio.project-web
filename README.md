
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>YK Nailstudio | Nail Art & Nail Care</title>
<meta name="description" content="YK Nailstudio menyediakan layanan nail art, manicure, dan perawatan kuku. Pesan jadwalmu melalui WhatsApp.">
<style>
*{box-sizing:border-box}
body{margin:0;font-family:Arial,sans-serif;background:#fffaf9;color:#493b3e}
header{padding:20px 7%;display:flex;justify-content:space-between;align-items:center;background:#fff;position:sticky;top:0;z-index:5;border-bottom:1px solid #f3e4e5}
.logo{font-size:23px;font-weight:bold;color:#a96f7c;letter-spacing:1px}
nav a{color:#59464b;text-decoration:none;margin-left:15px;font-size:14px}
.hero{text-align:center;padding:75px 20px;background:linear-gradient(140deg,#f8e6e9,#fff7f3)}
.tag{letter-spacing:3px;font-size:12px;color:#a56c79}
h1{font-family:Georgia,serif;font-size:clamp(38px,8vw,62px);font-weight:normal;line-height:1.15;margin:18px 0}
.hero p{line-height:1.8;color:#79676b;max-width:470px;margin:0 auto 25px}
.btn{display:inline-block;padding:14px 23px;border-radius:30px;background:#ad7481;color:white;text-decoration:none;border:none;font-size:15px;cursor:pointer}
section{padding:55px 7%}
.heading{text-align:center;font-family:Georgia,serif;font-size:34px;font-weight:normal;margin:0 0 12px}
.sub{text-align:center;color:#89777b;line-height:1.7;margin-bottom:30px}
.services{display:grid;grid-template-columns:repeat(auto-fit,minmax(190px,1fr));gap:16px}
.service{background:#fff;border:1px solid #f0e0e3;border-radius:17px;padding:25px 20px;text-align:center}
.emoji{font-size:35px}
.service h3{font-family:Georgia,serif;font-size:22px;font-weight:normal}
.service p{color:#89777b;font-size:14px;line-height:1.7}
.booking{background:#f8e9eb}
form{max-width:540px;margin:auto;background:#fff;padding:25px;border-radius:18px}
label{display:block;font-size:14px;margin:15px 0 7px}
input,select,textarea{width:100%;padding:13px;border:1px solid #e5d5d9;border-radius:9px;background:#fffaf9;font-size:15px;color:#493b3e}
textarea{min-height:100px;resize:vertical}
form .btn{width:100%;margin-top:22px}
.note{text-align:center;color:#89777b;font-size:13px;line-height:1.7}
footer{text-align:center;padding:28px 15px;background:#493b3e;color:#fff0f1;font-size:13px;line-height:1.8}
</style>
</head>
<body>
<header>
<div class="logo">YK Nailstudio</div>
<nav><a href="#layanan">Layanan</a><a href="#booking">Booking</a></nav>
</header>

<main>
<section class="hero">
<div class="tag">BEAUTY • CARE • CONFIDENCE</div>
<h1>Your Nails,<br>Your Elegance.</h1>
<p>Rawat dan percantik kukumu dengan sentuhan nail art yang elegan, detail, dan istimewa.</p>
<a class="btn" href="#booking">Reservasi Sekarang ↗</a>
</section>

<section id="layanan">
<h2 class="heading">Layanan Kami</h2>
<p class="sub">Sentuhan cantik untuk setiap detail kukumu.</p>
<div class="services">
<div class="service">
<div class="emoji">💅🏻</div>
<h3>Nail Art</h3>
<p>Desain kuku cantik dan personal sesuai gaya serta keinginanmu.</p>
</div>
<div class="service">
<div class="emoji">🌸</div>
<h3>Manicure</h3>
<p>Perawatan kuku dan tangan agar tampak bersih, rapi, dan terawat.</p>
</div>
<div class="service">
<div class="emoji">✨</div>
<h3>Nail Treatment</h3>
<p>Perawatan kuku untuk membantu menjaga penampilan kuku tetap indah.</p>
</div>
</div>
</section>

<section class="booking" id="booking">
<h2 class="heading">Book Your Appointment</h2>
<p class="sub">Isi formulir berikut untuk mengirim permintaan booking.</p>
<form id="bookingForm">
<label for="nama">Nama lengkap *</label>
<input id="nama" name="nama" required placeholder="Masukkan nama kamu">

<label for="layananPilihan">Pilih layanan *</label>
<select id="layananPilihan" name="layanan" required>
<option value="">Pilih layanan</option>
<option>Nail Art</option>
<option>Manicure</option>
<option>Nail Treatment</option>
<option>Nail Art + Manicure</option>
<option>Layanan lainnya</option>
</select>

<label for="tanggal">Tanggal booking *</label>
<input id="tanggal" name="tanggal" type="date" required>

<label for="jam">Waktu yang diinginkan</label>
<select id="jam" name="jam">
<option value="">Pilih waktu</option>
<option>09.00–11.00</option>
<option>11.00–13.00</option>
<option>13.00–15.00</option>
<option>15.00–17.00</option>
<option>17.00–19.00</option>
</select>

<label for="detail">Detail kebutuhan</label>
<textarea id="detail" name="detail" placeholder="Contoh: desain kuku, warna, panjang kuku, atau pertanyaan lainnya"></textarea>

<button class="btn" type="submit">Kirim Pesanan via WhatsApp ↗</button>
<p class="note">WhatsApp akan terbuka agar kamu bisa memeriksa dan mengirim pesan booking.</p>
</form>
</section>
</main>

<footer>
<strong>YK Nailstudio</strong><br>
Nail Art • Manicure • Nail Treatment<br>
Made with love for your beauty ♡
</footer>

<script>
document.getElementById("bookingForm").addEventListener("submit",function(e){
e.preventDefault();
const nama=document.getElementById("nama").value.trim();
const layanan=document.getElementById("layananPilihan").value;
const tanggal=document.getElementById("tanggal").value;
const jam=document.getElementById("jam").value||"Belum ditentukan";
const detail=document.getElementById("detail").value.trim()||"Tidak ada";
const pesan="Halo YK Nailstudio, saya ingin booking.\n\nNama: "+nama+"\nLayanan: "+layanan+"\nTanggal: "+tanggal+"\nWaktu: "+jam+"\nDetail kebutuhan: "+detail+"\n\nMohon informasi ketersediaan jadwal. Terima kasih.";
const url="https://wa.me/6288706509767?text="+encodeURIComponent(pesan);
window.location.href=url;
});
</script>
</body>
</html>
