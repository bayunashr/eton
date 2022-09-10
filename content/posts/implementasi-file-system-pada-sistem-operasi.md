---
title: "Implementasi File-System Pada Sistem Operasi"
date: 2022-09-10T13:43:32+07:00
# weight: 1
tags: ["Sistem Operasi", "Komputer"]
draft: true
showtoc: true
tocopen: true
summary: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus tempor lacus eu faucibus ullamcorper. Aenean nec gravida tellus. Aliquam interdum sem enim, placerat viverra ipsum dignissim sed."
---

## Prolog

Sebuah *file* sebenarnya hanyalah kumpulan informasi. Nah, yang mengatur terkait bagaimana kumpulan informasi itu bisa disimpan di komputer, dimana tempat menyimpannya, dan bagaimana jika kita ingin memanggilnya itu merupakan tugas *file system*.

Seperti yang diketahui, di dalam komputer terdapat 2 jenis ruang penyimpanan atau *storage*, adalah *primary storage* dan *secondary storage*.

### Primary Storage

*Primary storage*, sesuai artinya merupakan ruang penyimpanan utama dalam komputer, contohnya adalah RAM atau *random access memory* yang digunakan untuk menyimpan data sementara dan juga ROM atau *read-only memory* yang jika diartikan ROM hanya menyimpan informasi-informasi yang hanya bisa dibaca, tidak bisa diubah apalagi dihapus, "terus fungsinya apa kalo gabisa diapa-apain?" Pernah kepikiran gak tempat dimana BIOS disimpan? Walaupun komputermu gak ada *hard drive* atau *storage* lain, tapi BIOS masih dapat diakses, itu artinya BIOS tersimpan di dalam sini.

### Secondary Storage

Selanjutnya ada *secondary storage*, ruang penyimpanan cadangan ini fungsinya adalah untuk menyimpan *file-file* jangka panjang cenderung permanen, contohnya adalah semua *storage* yang gak masuk ke kategori *primary*, yaitu *hard disk drive* (HDD), *solid state drive* (SSD), *compact disk* (CD), *digital versatile disk* (DVD), *flashdisk*, dan lain-lain.

Implementasi *file system* akan membahas tentang cara kerja *secondary storage* ini, mulai dari bagaimana struktur file yang tersimpan di media penyimpanan, pengalokasian ruang-ruangnya, mengembalikan ruang tak terpakai, melacak posisi data disimpan, dan lain sebagainya.

## Struktur File-System

otw bro