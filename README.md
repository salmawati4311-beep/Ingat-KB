<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>INGAT KB</title>
</head>
<body>
 <h1>INGAT KB</h1>
<p>Website Pengingat Jadwal Kunjungan KB</p>
<form id="formKB">
<label for="jenis">Pilih jenis KB:</label>
<select id="jenis" name="jenis" required>
<option value="">Pilih jenis KB</option>
<option value="suntik1">Suntik 1 Bulan</option>
<option value="suntik3">Suntik 3 Bulan</option>
<option value="pil">Pil KB</option>
<option value="implan">Implan</option>
<option value="iud">IUD</option>
</select>
<br><br>
<label for="tanggal">Tanggal terakhir KB:</label>
<input type="date" id="tanggal" name="tanggal" required>
<br><br>
<button type="submit">Hitung Jadwal</button>
</form>
<p id="hasil"></p>
<script>
const form = document.querySelector("#formKB");
form.addEventListener("submit", function(event) {
event.preventDefault();
const jenis = document.querySelector("#jenis").value;
const tanggal = document.querySelector("#tanggal").value;
const hasil = document.querySelector("#hasil");
if (!jenis || !tanggal) {
hasil.textContent = "Silakan lengkapi semua data.";return; }
hasil.textContent ="Data berhasil dimasukkan. Silakan konfirmasi jadwal kunjungan berikutnya kepada bidan."; });
</ script>
</body>
</html>
