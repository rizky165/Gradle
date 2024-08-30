**Proyek Gradle Greeting**
==========================
Tugas ini bertujuan untuk membuat sebuah proyek Gradle sederhana yang memiliki tugas khusus untuk menerima parameter dari Command Line Interface (CLI) dan mencetak pesan ucapan

Kriteria:
=========
- Membuat Gradle sederhana untuk menerima parameter CLI dan mencetaknya dengan pesan ucapan
- Proyek skrip Gradle harus dibuat di repositori yang berbeda dan dorong ke GitHub

Langkah-langkah
=============
Buka file build.gradle di direktori root proyek dan tambahkan kode berikut

Run command :
```
task greetingTask {
    doLast {
        String nama = project.hasProperty('nama') ? project.property('nama') : 'Gradle User'
        println "Hello, $nama! Welcome to Gradle World!"
    }
}
```
Langkah selanjutnya tambahkah pustaka dengan menggunakan fitur bawaan gradle
