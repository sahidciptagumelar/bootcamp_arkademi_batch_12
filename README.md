  # bootcamp_arkademi_batch_12
  Jawaban soal bootcamp arkademi batch 12

  1. function getProfile() {
      return {
      name: 'SAHID CIPTA GUMELAR',
      age: 24,
      address: 'Kosan Bintang Berlian (Kosan 23) Jl. Johar Baru Utara 6 Gg.7 RT.08 RW.05 Kel. Johar Baru Kec. Johar Baru 
      Jakarta Pusat',
      hobbies: ['Programming', 'GameOnline'] //Array,
      is_married: false //Boolean,
      list_school: [{
        name: 'SDN 3 Ciseureuh',
        year_in: 2001,
        year_out: 2007,
        major: 'MTK'
      },{
        name: 'MTSN Purwakarta',
        year_in: 2007,
        year_out: 2010,
        major: 'IPA'
      },{
        name: 'SMAN 1 Campaka',
        year_in: 2011,
        year_out: 2014,
        major: 'IPA'
      },{
        name: 'Universitas Bina Sarana Informatika',
        year_in: 2015,
        year_out: 2018,
        major: 'PHP'
      }] // Array Of Object
      skills: [{
        skill_name: 'PHP Framework CI',
        level: 'advanced'
      },{
        skill_name: 'HTML',
        level: 'advanced'
      }] // Array Of Object
      interest_in_coding: true //Boolean,
      }
      }
  //fungsi dari JSON dari web API tapi pada dasarnya sangat sederhana yaitu sebagai format untuk mentransmisikan (mengirim dan menerima) data dari web API (server) ke client atau sebaliknya.

  2. function is_username_valid(username) {
    // Huruf dari a sampai z
    var lowercaseRe = /[a-z]/g;
    var uppercaseRe = /[A-Z]/g;
    var numberRe = /[0-9]/g;

    // check panjang string dan memastikan karater yang ditemukan sama dengan panjang string

    if(username.length >= 5 && username.length <=9 
             && username.match(lowercaseRe).length 
             && username.match(uppercaseRe).length 
             && username.match(numberRe).length == username.length) {
        return true;
      }
      return false;
      }

      function is_password_valid(password) {
      // huruf keci a sampai z
    var lowercaseRe = /[a-z]/g;

      // huruf besar A sampai Z
         var uppercaseRe = /[A-Z]/g;

      // angka dari 0 sampai 9
         var numberRe = /[0-9]/g;

      // karater unik _@$= atau %
         var specialRe = /[_@$%=]/g;

        if(password.length == 8
           && lowercaseRe.test(password)
           && uppercaseRe.test(password)
           && numberRe.test(password)
           && specialRe.test(password)) {
             return true;
           }

           return false;
           }

  3. public class JavaApplication {

      public static void main(String[] args) {
          int n = 11;
          for (int i = 0; i <= n; i++) {
              String bintang = "*";
              for (int j = 0; j < i; j++) {
                  bintang = bintang + "*";
              }
              System.out.println(bintang);
          }
         }
       }

  4. <?php

      $a = '00000004523423400023402340240';
      $b = str_replace("0", "", "0001")
      echo $b;
      ?>

  5.  public class Main {
      public static void main(String[] args){
          String text = "Belajar Pemrograman Java String Split";

          String[] kata = text.split("\\s+");

          for(String result : kata){
              System.out.println("Text = "+result);
                }

            }
        }

    6. $query=mysqli_query($conn,"SELECT name.*, work.name, salary.salary 
                              FROM name, work, salary 
                              WHERE name.id_work = work.id_work 
                              AND name.id_salary = salary_id_salary  
                              ORDER BY id DESC");

       Untuk pembuatan website menggunakan framework CI
       Cara membuka file di localhost adalah http://localhost/ci_datatable/
       Database sudah ada di direktori CI dengan nama bootcamp_arkademia
