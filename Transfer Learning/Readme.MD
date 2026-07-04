# Tugas #


Pada Fase 2 fine-tuning, model ResNet18 mencapai kondisi seimbang dengan rata-rata gap Train-Val sebesar +0.05, jauh di bawah ambang overfitting (0.10). Train Accuracy naik progresif hingga 98.09% sementara Val Accuracy stabil di kisaran 88–91%, menandakan model berhasil belajar tanpa menghapal data training.

Pada test set, model mencapai Test Accuracy 89.06% — peningkatan signifikan dibanding CNN scratch (~68.5%) — dengan performa terbaik pada kelas paper (F1=0.94) dan cardboard (F1=0.92). Kelas trash masih menjadi kelemahan (F1=0.71) akibat jumlah sampel yang sangat sedikit dibanding kelas lain. 

Secara keseluruhan, Transfer Learning dengan ResNet18 terbukti efektif meningkatkan akurasi klasifikasi sampah secara substansial, dengan teknik regularisasi Dropout, BatchNorm, dan Weight Decay yang berhasil menjaga model tetap generalizable.
