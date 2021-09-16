# Tugas1ADJ_191402054
Repo untuk tugas 1 mata kuliah Administrasi dan Desain Jaringan

Langkah Langkah Instalasi Docker Toolbox<br>
Karena saya tidak dapat melakukan instalasi menggunakan Docker Desktop maka saya menggunakan Docker Toolbox<br>
1. Pertama install Docker Toolbox di https://github.com/docker/toolbox/releases dan download file executable paling baru
2. Setelah download selesai buka setup, lalu klik next <br>![Screenshot (422)](https://user-images.githubusercontent.com/56826724/133603846-22753158-bdad-45c1-af9e-132a65f7eba5.png)</br>
3. Lalu pilih lokasi instalasi <br>![Screenshot (423)](https://user-images.githubusercontent.com/56826724/133604064-2b59a358-051a-4fd0-87ed-8064a4ea257f.png)</br>
4. Pilih Full Instalation, kemudian klik Next <br>![Screenshot (424)](https://user-images.githubusercontent.com/56826724/133604234-b983995f-e625-4619-aeac-7d4ec7d726ed.png)</br>
5. Lalu pada bagian ini dapat dibiarkan default nya, lalu klik Next <br>![Screenshot (428)](https://user-images.githubusercontent.com/56826724/133604347-e102e198-4390-4b01-805d-2832a99993a5.png)</br>
6. Kemudian klik Install <br>![Screenshot (425)](https://user-images.githubusercontent.com/56826724/133604426-fe0f99e6-a0de-4c59-a72f-9c8779ae5d25.png)</br>
7. Setelah selesai, klik Finish <br>![Screenshot (426)](https://user-images.githubusercontent.com/56826724/133604521-73b82fd5-d959-495b-b536-59025df46dcf.png)</br>
8. Lalu buka Docker Quickstart Terminal kemudian akan muncul seperti ini <br>![Screenshot (430)](https://user-images.githubusercontent.com/56826724/133604933-ab1f54a5-9c94-4488-9cf3-04c6449c968b.png)</br>
9. Lalu tunggu setelah beberapa saat maka akan muncul seperti ini dan instalasi Docker Toolbox selesai <br>![Screenshot (431)](https://user-images.githubusercontent.com/56826724/133605018-2d0139d7-9405-4928-90ac-7abcd485ab1a.png)</br>

Langkah Langkah membuat web statis menggunakan Docker<br>
1. Pertama siapkan file html yang akan digunakan
2. Lalu buat sebuah file tanpa ekstensi dengan nama Dockerfile
3. Lalu pada Dockerfile isinya adalah <br>
FROM nginx:alpine<br>
COPY . /usr/share/nginx/html<br>
4. Masukkan file html tadi beserta file Dockerfile ke satu folder
5. Lalu buat docker image dengan mengetik <br>
$ docker build -t namaimage . <br>
6. Kemudian untuk run docker container ketik <br>
$ docker run -p 80:80 namaimage <br>
contoh :
<br>![Screenshot (421)](https://user-images.githubusercontent.com/56826724/133606618-3b338368-e310-471b-a176-0db24a08af7d.png)</br>
7. kemudian setelah berhasil buka link http://192.168.99.100/ maka web yang telah dibuat akan muncul
<br>![Screenshot (419)](https://user-images.githubusercontent.com/56826724/133606891-e89d5487-55da-4121-bb3d-210b29d3f2ac.png)</br>
