Pada copy attempt 2
Model Plain-34 menunjukkan gejala degradasi yang parah: akurasi validasi hanya mencapai ~38%, dengan F1-score makro 0.30. Dua kelas (bakso dan gado-gado) sama sekali tidak terdeteksi, menunjukkan bias ekstrem dan ketidakmampuan model menangkap fitur diskriminatif. Fluktuasi loss validasi (termasuk lonjakan ke 4.77) mengindikasikan instabilitas pelatihan akibat vanishing gradient.

Pada nyoba dengan plain34 residual 
ResNet-34 dengan residual connection menunjukkan peningkatan dramatis dibanding Plain-34: akurasi validasi naik dari ~30% menjadi 56.76%, dan model mampu belajar representasi yang bermakna tanpa mengalami degradasi. Meski masih terjadi overfitting (gap train-val ~18%), stabilitas pelatihan dan kemampuan generalisasi jauh lebih baik. Hasil ini membuktikan bahwa skip connection memungkinkan pelatihan jaringan dalam secara efektif, sesuai prinsip dasar arsitektur ResNet. 


