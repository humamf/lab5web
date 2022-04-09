# Praktikum 5

## Profil
| | Biodata |
| -------- | --- |
| **Nama** | Humam Fathurrahman |
| **NIM** | 312010389 |
| **Kelas** | TI.20.A2 |
| **Mata Kuliah** | Pemrograman Web |

## **Langkah-langkah Praktikum**

Membuat dokumen HTML dengan nama file **lab5_javascript.html** .

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mengenal Javascript</title>
</head>
<body>
    <h1>Pengenalan Javascript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
        document.write("Hello World");
        console.log("Hello World");
    </script>
</body>
</html>
```

Tampilannya seperti berikut.

![PengenalanJS](img/pengenalanjs.png)

## **Javascript Dasar**

### **1. Pemakaian Alert sebagai property window**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alert Box</title>
</head>
<body>
    <script language = "javascript">
        <!--
        window.alert("ini merupakan pesan untuk anda")
        //-->
    </script>
</body>
</html>
```

Tampilannya seperti berikut. 

![AlertBox](img/alertbox.png)

### **2. Pemakaian method dalam objek**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Skrip Javascript</title>
</head>
<body>
Percobaan memakai Javascript: <br>
    <script language = "javascript">
        <!--
        document.write("selamat mencoba javascript <br>")
        document.write("semoga sukses")
        //-->
    </script>
</body>
</html>
```

Tampilannya seperti berikut.

![SkripJS](img/skripjs.png)

### **3. Pemakaian Prompt**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Skrip Javascript</title>
</head>
<body>
Percobaan memakai Javascript: <br>
    <script language = "javascript">
        var nama  = prompt("siapa nama anda?", "masukkan nama anda");
        document.write("hai, " + nama);
    </script>
</body>
</html>
```

Tampilannya seperti berikut. 

![Prompt](img/prompt.png)

### **4. Pembuatan fungsi dan cara pemanggilannya**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh program Javascript</title>
    <script language = "javascript">
    function pesan(){
        alert ("memanggil javascript lewat body onload")
        }
    </script>
</head>
<body onload=pesan()>
</body>
</html>
```

Tampilannya seperti berikut.

![FungsidancaraMemanggil](img/memanggil.png)

## Dasar Pemrograman Di Javascript

### **1. Operasi dasar arimatika**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh program Javascript</title>

    <script language = "javascript">
    function test (val1,val2)
    {
        document.write("<br>"+"perkalian : val1*val2 "+ "<br>")
        document.write(val1*val2)
        document.write("<br>"+"pembagian : val1/val2 "+ "<br>")
        document.write(val1/val2)
        document.write("<br>"+"penjumlahan : val1+val2 "+ "<br>")
        document.write(val1+val2)
        document.write("<br>"+"pengurangan : val1-val2 "+ "<br>")
        document.write(val1-val2)
        document.write("<br>"+"modulus : val1%val2 "+ "<br>")
        document.write(val1%val2)
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="arithmetic" onclick=test(9,4)>
</body>
</html>
```

Tampilannya seperti berikut.

![Aritmatika](img/aritmatik.png)

### **2. Seleksi kondisi (if,else)**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh if-else</title>
</head>
<body>
    <script language = "javascript">
    <!--
    var nilai = prompt("nilai (0-100): ", 0);
    var hasil = "";
    if (nilai >= 60)
    hasil = "lulus";
    else 
    hasil = "tidak lulus";
    document.write("hasil: "+ hasil);
    //-->
    </script>
</body>
</html>
```

Tampilannya seperti berikut.

![Contohifelse](img/contohifelse.png)

### **3. Penggunaan operator switch untuk seleksi kondisi**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh program javascript</title>

    <script language = "javascript">
    function test ()
    {
        val1=window.prompt("input nilai (1-5):")
        switch (val1)
        {
            case "1" :
                document.write("bilangan satu")
                break
            case "2" :
                document.write("bilangan dua")
                break
            case "3" :
                document.write("bilangan tiga")
                break
            case "4" :
                document.write("bilangan empat")
                break
            case "5" :
                document.write("bilangan lima")
                break
            default :
                document.write("bilangan lainnya")
        }
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
```

Tampilannya seperti berikut.

![Switch](img/switch.png)

## **Pembuatan Form**

### **1. Form input**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh program javascript</title>

    <script language = "javascript">
    function test ()
    {
        var val1=document.kirim.T1.value
        if (val1%2==0)
            document.kirim.T2.value="bilangan genap"
        else
            document.kirim.T2.value="bilangan ganjil"
    }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20">
        MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
        <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
    </form>
</body>
</html>
```

![FormInput](img/forminput.png)

### **2. Form button**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Objek document</title>
</head>
<body>
    <script language = "javascript">
    <!--
    function ubahWarnaLB(warna) {
        document.bgColor = warna;
    }
    function ubahWarnaLD(warna) {
        document.fgColor = warna;
    }
    //-->
    </script>

    <h1>tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
        <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
    </form>
    <script language = "javascript">
    <!--
    document.write("Dimodifkasi terakhir pada" + document.lastModified);
    //-->
    </script>
</body>
</html>
```

Tampilannya seperti  berikut.

![FormButton](img/formbutton.png)

## **HTML DOM**

### **Pilihan menggunakan checkbox dengan perhitungan otomatis**

```html
<!DOCTYPE html>
<!--File: daftar_menu.html//-->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
                total = (total ? parseInt(total) : 0);

            if (ele.checked) {
                harga = ele.value;
                total += parseInt(harga);
            }
            else {
                harga = ele.value;
                if (total > 0)
                    total -= parseInt(harga);
            }

            document.getElementById('total').value = total;
        }
    </script>
</head>
<body>
    <h1>Daftar Menu Makanan</h1>
    <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);" /> Ayam Goreng Rp. 5.000</label><br />
    <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);" /> Tempe Goreng Rp. 500</label><br />
    <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);" /> Telur Dadar Rp. 2.500</label><hr />
    <strong>Total Bayar : Rp <input id="total" type="text" /></strong>
</body>
</html>
```

Tampilannya seperti berikut. 

![HTMLDOM](img/checkbox.png)

## **Pertanyaan dan Tugas**

### 1. Buat script untuk melakukan validasi pada isian form.

**HTML**
```html
<!DOCTYPE html>
<!--File: daftar_menu.html//-->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form</title>
    <link rel="stylesheet" href="style.css">
    <script type="text/javascript">
        function validasiform() {
            var nama = document.getElementById("nama").value;
            var email = document.getElementById("email").value;
            var alamat = document.getElementById("alamat").value;
            if (nama != "" && email != "" && alamat != ""){
                return true;
            } else {
                alert('Isi Dengan Lengkap !');
                return false;
            }
        }
    </script>
</head>
<body>
    <div id="container">
    <h2>Validasi Data Diri</h2>
        <form action="#" method="POST" onSubmit="return validasiform()">
            <div class="data">
                <div>
                    <label for="name">Nama :</label>
                    <input type="text" name="name" id="nama">
                </div>
                <div>
                    <label for="email">Email :</label>
                    <input type="email" name="email" id="email">
                </div>
                <div>
                    <label for="alamat">Alamat :</label>
                    <textarea name="alamat" id="alamat" cols="30" rows="7"></textarea>
                </div>
                <input type="submit" name="button1" id="button">
            </div>
        </form>
    </div>
</body>
</html>
```

**CSS**
```css
*{
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}

body {
    background-color: rgb(0, 57, 143);
}

#container {
    width: 50%;
    margin: 0 auto;
    border-radius: 4px;
    background-color: #fff;
}

h2 {
    padding-top: 20px;
    text-align: center;
}

label {
    margin: 10px 0;
}

#nama, #email, #alamat {
    margin: 5px 0 ;
    width: 95%;
}

.data {
    font-size: 10pt;
    padding: 10px 0;
    display: block;
    margin: 10px;
    box-sizing: border-box;   
}

#button {
    margin: 10px 0;
    padding: 10px;
    color: white;
    background-color: rgb(0, 101, 253);
}
```

Tampilannya seperti berikut.

![Tugas](img/tugas.png)
