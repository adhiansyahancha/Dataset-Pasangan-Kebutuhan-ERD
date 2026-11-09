# Teks deskripsi

Hotel memiliki setidaknya satu atau beberapa kamar, dan setiap kamar pada gilirannya merupakan bagian dari tepat satu hotel. Setiap kamar memiliki nomor kamar. Tamu dapat menginap di hotel dan memesan satu atau beberapa kamar. Sebaliknya, sebuah kamar pada gilirannya dapat dipesan oleh nol atau lebih tamu.

# ERD Acuan

```uml
@startchen

entity Tamu {
}
entity Kamar {
NomorKamar
}
entity Hotel {
}
relationship memesan {
}
relationship memiliki {
}

Tamu -1- memesan
memesan -N- Kamar

Hotel -1- memiliki
memiliki -N- Kamar

@endchen
```

# Lisensi

[EMISAJ - International Journal of Conceptual Modeling](https://emisa-journal.org/emisa/article/view/318) mengizinkan di bawah [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/ )
