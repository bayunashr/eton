---
title: "Struktur Data Stack"
date: 2022-09-11T12:26:08+07:00
# weight: 1
tags: ["Struktur Data", "Komputer"]
draft: false
summary: "Stack, salah satu jenis struktur data dengan konsep LIFO (last in first out)."
---

## Prolog

*Stack* adalah salah satu jenis struktur data dengan konsep tumpukan atau LIFO (*last in-first out*, terakhir masuk-keluar pertama). Sederhananya, dalam *stack*, hanya elemen yang berada di paling atas-lah yang dapat keluar, karena jika ada dibawah, elemen itu akan tertindih elemen diatasnya.

![Konsep Stack](https://i.ibb.co/XZk7hkx/konsep-stack.png)

## Operasi Dasar dalam Stack

Dalam *stack*, ada beberapa operasi untuk memanipulasi isi dari *stack*.

- **push** &rarr; Meletakkan elemen di bagian atas *stack*.
- **pop** &rarr; Mengambil elemen paling atas *stack*.
- **top** &rarr; Menampilkan nilai elemen paling atas *stack*.
- **isEmpty** &rarr; Memeriksa apakah *stack* kosong.
- **isFull** &rarr; Memeriksa apakah *stack* penuh.

### Push

*Push* meletakkan elemen di bagian atas *stack*, jika *stack* dalam kondisi *isFull*, maka kondisi ini dinamakan **Overflow**.

![Stack Push](https://i.ibb.co/BKcYWh7/stack-push.png)

```
start
    if stack isFull
        write "Overflow"
    else
        top + 1
        stack[top] = value
    endif
end
```

### Pop

*Pop* mengambil elemen paling atas *stack*, jika *stack* dalam kondisi *isEmpty*, maka kondisi ini dinamakan **Underflow**.

![Stack Pop](https://i.ibb.co/yndGFkL/stack-pop.png)

```
start
    if stack isEmpty
        write "Underflow"
    else
        top - 1
    endif
end
```

### Top

*Top* menampilkan nilai elemen paling atas *stack*.

![Stack Top](https://i.ibb.co/nLgY42s/stack-top.png)

```
start
    write stack[top]
end
```

### isEmpty

*IsEmpty* memeriksa apakah *stack* kosong.

```
start
    if top < 1
        write "Stack is Empty"
    else
        write "Stack is not Empty"
    endif
end
```

### isFull

*IsFull* memeriksa apakah *stack* penuh.

```
start
    if top >= stack[max]
        write "Stack is Full"
    else
        write "Stack is not Full"
    endif
end
```

## Sumber Pustaka

- [Stack Data Structure (Introduction and Program)](https://www.geeksforgeeks.org/stack-data-structure-introduction-program/)