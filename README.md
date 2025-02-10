# Implementasi Artificial Intelligence
Implementasi Decision Tree, Random Forest, SVM, KNN, dan Naive Bayes untuk Diagnosis Diabetes berdasarkan Demografi dan Pola Hidup Asia 2024

**Dataset:** https://www.kaggle.com/code/ahmadreginald/diabetes-predictive-analytics/notebook (Diabetes Predictive Analytics)

**by:** Ahmad Reginald Syahiran

Dengan dataset ini, kami mengembangkan model prediksi **diabetes yang ada di wilayah Asia pada tahun 2024 menggunakan Supervised Learning dengan pendekatan Klasifikasi yang menggunakan lima algoritma** diantaranya:
1. Decision Tree
2. Random Forest
3. Support Vector Machine (SVM)
4. K-Nearest Neighboard (K=3)
5. Naive Bayes 

Selain itu, **metode penelitian** yang kami guna terdiri dari tiga tahapan diantaranya:

*1. Identifikasi Masalah*
Dengan mengidentifikasikan masalah lalu mencari studi literatur baik dari makalah maupun jurnal terkait penyakit diabetes dan machine learning.

*2. Analsis Kebutuhan dan Perancangan* 
Dimulai dengan pengumpulan data yang kami temmukan melalui lama kaggle yang berjudul Diabetes Predictive Analytics.

Selanjutnya kami melakukan pre-processing untuk memastikan dataset yang kami gunakan sudah sesuai dengan kebutuhan dengan tiga tahapan yaitu:

**a. Exploration Data**, untuk memastikan tidak ada data yang null atau duplikat, sekaligus memahami karakteristik dan tipe data yang digunakan secara mendalam.

**b. Cleaning Data,** dalam proses penelitian ini, terdapat beberapa atribut yang dianggap kurang relevan karena tidak berhubungan langsung dengan patogenesis diabetes,seperti patient ID, educational level, heavy metals exposure, occupational exposure chemicals, water quality, dan doctor in charge.

**c. Selection Data,** Atribut “ethnicity” untuk menyaring pasien yang hanya berasal dari negara-negara di kawasan Asia (2) yang menyisakan 206 data point untuk diolah lebih lanjut. Langkah akhir dalam pre-processing adalah menentukan label berupa atribut “diagnosis”, yang menunjukkan apakah seorang pasien terdiagnosis diabetes (1) atau tidak (0).

Setelah itu, kami melakukan klasifikasi data dengan **membangun machine learning melalui lima algoritma** diatas yang diawali dengan pembagian dataset, pelatihan dataset, hingga pengujian dataset.

**a. Pembagian Dataset**
Dataset yang telah diolah kemudian dibagi menjadi dua bagian melalui metode train-test split, sebuah fitur unggulan yang disediakan oleh pustaka scikit-learn. Dataset dibagi secara proporsional, dengan sebagian besar data dialokasikan sebagai data latih (training set) untuk membantu model memahami pola, dan sisanya digunakan sebagai data uji (testing set) guna mengukur performa model. Pendekatan ini memastikan bahwa evaluasi terhadap kinerja model dilakukan secara objektif dan akurat. Pembagian dataset dilakukan dalam pembagian 80% data latih dan 20% data uji dengan parameter random_state=42 untuk memastikan bahwa pembagian dataset dilakukan secara konsisten setiap kali kode dijalankan

**b. Pelatihan dan Pengujian Dataset**
Melatih model menggunakan data latih. Dalam pelatihan ini, model mempelajari hubungan antara fitur dan label target, membangun fungsi atau aturan matematis
- Decision Tree: menggunakan algoritma DecisionTreeClassifier dari scikit-learn
- Random Forest: menggunakan algoritma RandomForestClassifier dari scikit-learn
- SVM: menggunakan algoritma SVC dari scikit-learn
- K-Nearest Neighboard: menggunakan algoritma KNeighborsClassifier dari scikit-
- Naive Bayes: menggunakan algoritma GaussianNB dari scikit-learn
Setelah pelatihan selesai, model diuji menggunakan data uji untuk mengevaluasi kinerjanya

Tahap metode yang ketiga yaitu *Implementasi dan Hasil.*
Dalam implementasi ini, kami membangun **model machine learning** dari lima algoritma diatas untuk memprediksi diagnosis diabetes seseorang di wilayah Asia pada tahun 2024. Setelah itu, kami evaluasi dilakukan dengan menggunakan metrik evaluasi yang paling umum digunakan yaitu **accuracy, precision, recall, dan F1-score.**

Sehingga, hasil analisis menunjukkan bahwa **Decision Tree dan Random Forest menjadi algoritma paling optimal dalam mendeteksi diabetes dibandingkan metode lainnya.** Kedua algoritma ini menunjukkan akurasi tinggi dan keseimbangan prediksi yang lebih baik, menjadikannya pilihan unggul untuk diagnosis diabetes di wilayah Asia pada tahun 2024.

