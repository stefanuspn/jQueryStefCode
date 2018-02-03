# jQueryStefCode Part II.js
Apa Itu jQueryStefCode Part II.js sebuah plugin jquery yang sederhana untuk mendeteksi user menekan tombol keyboard sesuai pilihan cara penggunaan.<br>

<br>
<br>
Plugin ini di buat oleh Stefanus Prasetyo Nugroho.

## Instalasi
Untuk bisa memakai plugin ini anda membutuhkan jquery terlebih dahulu bebas versi berapa aja, dan anda bisa menginstall jQueryStefPlaySound.js lewat NPM jika komputer anda sudah terpasang node.js dengan cara ketik di command line :<br>



Atau anda juga bisa menggunakan seperti ini menggunakan tag script biasa, contoh:


```javascript
<script
  src="http://code.jquery.com/jquery-3.3.1.min.js"
  integrity="sha256-FgpCb/KJQlLNfOu91ta32o/NMZxltwRo8QtmkMRdAu8="
  crossorigin="anonymous"></script>

<script src="asset/js/jQueryStefCodePartII.js"></script>
```

Anda Bisa mendapatkan jQueryStefPlaySound.JS berikut:<br>
<code>https://raw.githubusercontent.com/stefanuspn/StefPlaySound/master/asset/js/jQueryStefCodePartII.js</code>

### Cara Menggunakan
Siapkan terlebih dahulu file-file yang sudah disebutkan diatas yaitu jquery-3.2.1.min.js dan jQueryStefCodePartII.js :<br>

```html


<script>
  src="http://code.jquery.com/jquery-3.3.1.min.js"
  integrity="sha256-FgpCb/KJQlLNfOu91ta32o/NMZxltwRo8QtmkMRdAu8="
  crossorigin="anonymous"></script>

<script src="asset/js/jQueryStefCodePartII.js.js"></script>

<script>
$(document).ready(function(){
   $(window).stefcode2({
      code : 65 , // menekan fungsi keyboard
       callback: function() {
          swal('Oops!', 'Sorry Gan tombol a Gak Bisa hehe!.', 'error'); setTimeout(1000);
            }
       });
});

$(document).ready(function(){
   $(window).stefcode2({
      ctrlcode : 85 , // menekan fungsi keyboard ctrl+
       callback: function() {
          $(".coba").html("hai");
            }
       });
});

$(document).ready(function(){
   $(window).stefcode2({
      alt : 83 , // menekan fungsi keyboard alt+
       callback: function() {
          $(".coba").html("hai");
            }
       });
});
</script>
```

