# Simple-Naive-Bayes-Weather-Prediction
Penerapan Naive Bayes sederhana untuk prediksi cuaca menggunakan python 

Metode Naive Bayes Classifier adalah metode pengklasifikan probabilistik sederhana, dapat diandalkan, mudah, efektif, efesien, dengan menjumlahkan frekuensi dan kombinasi nilai dari dataset. Disini digunakan ntuk memprediksi cuaca dengan parameter suhu udara, kelembapan udara, dan tekanan. Dalam klasifikasi ini menggunakan dataset perkiraan cuaca dengan Outlook: rainy,overcast,sunny. Humidity: high dan normal. Windy: f dan t, Temp:Hot,Mild,Cool, Play: no dan yes

Berikut adalah rumus perhitungannya 
        probability(class) =    How many  times it appears in cloumn
                             __________________________________________
                                  count of all class attribute
        
        Menghitung probabilitas individu
        P(outcome|evidence) =   P(Likelihood of Evidence) x Prior prob of outcome
                               ___________________________________________
                                                    P(Evidence)
                                                    
        Menghitung Kemungkinan Bukti dan mengalikan semua probabilitas individu dengan priori
        (Outcome|Multiple Evidence) = P(Evidence1|Outcome) x P(Evidence2|outcome) x ... x P(EvidenceN|outcome) x P(Outcome)
        scaled by P(Multiple Evidence)                                                   

Berikut adalah perhitungan kondisi probabilitasnya
Priori Values:  {'no': 0.35714285714285715, 'yes': 0.6428571428571429}
{'no': {'Mild': 0.6, 'Normal': 0.4, 'Rainy': 0.8, 't': 0.8},
 'yes': {'Mild': 0.5555555555555556,
         'Normal': 0.7777777777777778,
         'Rainy': 0.3333333333333333,
         't': 0.4444444444444444}}
Result: 
no  ==>  0.05485714285714286
yes  ==>  0.04115226337448559

Pada hasil pengujian dengan tersebut menunjukkan bahwa klasifikasi cuaca menggunakan metode Naive Bayes Classifier memiliki akurasi sebesar dapat ditarik kesimpulan bahwa metode tersebut sangat baik dalam mengklasifikasikan cuaca dengan parameter suhu udara, kelembapan udara, dan tekanan udara.
