# catatan
catatan cara menggunakan git dengan github
-----------------------------------------------------------
// Perintah Git //

2 #DOWNLOAD DARI GITHUB KE LOCAL KETIKA DI LOCAL BELUM ADA
  #Melakukan cloning ketika di dalam PC belum ada duplikatnya.
  - Pertama kita dowloan repo yang ada di github dengan cara men copy alamat repo nya,
  - Pilih lokasi untuk menempatkan repo tersebut, kemudian buka git bash here,
 #Perintah didalam git nya.
 
 #menghubungkan git dengan github ketika file repo belum ada di komputer local
  - git clone ( paste alamat repositoy )
 #masuk kedalam folder projek/repository
  - cd (nama folder atau projek/repository)
  - git remote              //(untuk mengetahui nama, defaultnya adalah origin)
  - git remote -V           //(untuk mengetahui nama lebih detail)
  - git status              //(untuk mengetahui status)

  - alias graph="git log --all --decorate --oneline --graph"          //( membuat graph commit agar berada di pointer yang sama)
  - graph                                                             //(untuk mengetahui status graph commit)
  - git status                                                        //(untuk melihat status track, jika statusnya untracked file, maka harus di commit)
  - git add .                                                         //(menambahkan file ke staging area), (jika file nya UNTRACKED FILES harus di beri perintah ini dulu)
  - git commit -m "(pesan atau commen deskripsi)"                     //(menambahkan comit baru)
  - git push                                                          //(Mengirim file ke remot/github)
 # Jika di minta melakukan login maka Login masukan email dan password di github nya.
  - git config --list                                                  //(menampilkan status username yang login di github)
  - :q                                                                 //(untuk keluar/log out)
  - git config --global user.name "masukan username"                   //(Memasukan username)
  - git config --global user.email "masukan email"                     //(Memasukan email)


 # Setelah melakukan commit atau edit file atau modifield maka lakukan perintah commit kembali untuk menyamakan dengan repo di github nya
  - git status                                                          //( Untuk melihat status )
  - git commit -am "pesan atau comentar"                                //( menambahkan commit yang di modifield atau edit )
  - git push                                                            //( Untuk mengirim file hasil edit ke remote github )
  --------------------------------///----------------------------------------------------------------------------------------------------------------
  
2 # UPLOAD DARI LOCAL ATAU KOMPUTER KE GITHUB KETIKA DI GITHUB BELUM ADA
  
  #Membuat nama file folder repo baru
  - cd ..                                                               //( Untuk keluar ke direktory utama )
  - mkdir (nama file atau folder direktori baru)                        //( Membuat file repository baru di local )
  - cd (nama folder)                                                    //( Masuk kedalam folder yang telah dibuat )
  - git init                                                            //( Membuat repo git )
  # Setelah project di buat, kemudian kembali lagi ke git bash nya dan upload ke github
  
  - ls                                                                 //(untuk menampilkan list dalam folder)
  - git add .                                                          //(menambahkan file ke staging area), (jika file nya UNTRACKED FILES harus di beri perintah ini dulu)
  - git commit -m "(pesan atau commen deskripsi)"                      //(menambahkan comit baru)
  - graph                                                              //(untuk mengetahui status graph commit)
  # Masuk ke Github nya dan buat REPO baru ( Pada bagian check box yang bertuliskan INITIALISE THIS REPOSITORY nya jangan di centang, biarkan kosong
  ## Maka akan di arahkan ke pilihan perintrah, (membuat file baru seperti cara pertama) atau (meng upload dari local pc ke github yaitu cara kedua ini)
  ## Cara kita tambahkan sebuah remote baru di local kita supaya terhubung ke github. Remotnya yaitu alamat HTTP yang ada di repository github nya.
  
  # copy command perintah sesuai dengan yang ada di petunjuk github nya yaitu :
  - git remote origin (alamat http repo yang ada di github)
  - git push -u origin master            //(membuat kode yang sudah dibuat di local ke github nya ( -u : adalah upstream agar nanti tinggal ketikan git push untuk mengirim) )
 ---------------------------------------------------------------------/////---------------------------------------------------------------------------------------------------
 
 # Jika terjadi error dengan sekenario yaitu ketika di remot github dan di local nya di edit dengan file yang sama atau sama-sama dan terjadi kegagalan maka masukan perintah
  - git fetch         //(Untuk cek sampai mana commit yang ditubah nya)
  - git pull          //(untuk mengambil file nya kedalam codingan kita dan nantinya kita pilih dan edit file mana yang akan kita gunakan kemudian commit kembali)
  - git add .
  - git commit -m "comment/status deskripsi"
  - git push
 
 ---------------------------///////////-------------------------- SELESAI -------------------/////////////-------------------------------------------------------------------
  









