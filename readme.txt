Bu projede, cilt kanserinde dermatologların kullandığı ABCD yöntemi matematiksel işlemlerle desteklenerek 
bilgisayarın anlayacağı hale getirilmiştir. Elimizde bulunan veri setindeki 10 farklı konumdan alınan 
verilerin sonuçlarının ortalamasına göre başarı durumu yorumlanmıştır.

Bu çalışmada lezyonun hastalıklı veya sağlıklı olduğunu tespit etmek için KNN en yakın komşu algoritmasına 
verilecek veriler için merkezden sınıra olan düzensiz uzunluklara ait nokta sayısı, 
türev ile bulunmuş sınırdaki yüksek sıçrama yapan nokta sayısı, lezyon renginin standart sapması, 
çapı, benzerlik oranı, kontur sayısı gibi öznitelikler kullanılmıştır.

Tek başına doğruluk (accuracy) oranı yetersiz kalmaktadır. Bu nedenle, kesinlik yani 
hastalıklı tahmin edilenlerin kaçının hastalıklı olduğu, duyarlılık yani hastalıklı olanların 
doğru tespit oranı ve f1 score hassasiyeti ile sağlamlık oranı belirlenmiştir. 


Projenin Çalıştırılması:

1) Lezyon bölgelerine ait görüntüler "foto" klasörüne eklenir.
2) Hair_Filtering.py dosyası çalıştırılarak görüntüler üzerinde işlem yapılarak  "foto2" klasörüne kaydedilir.
3) Main.py dosyası çalıştırılarak "foto2" klasöründeki fotoğrafların öznitelikleri lezyon.csv dosyasına yazılır.
4) knn.py dosyası çalıştırılarak lezyon.csv dosyasından veriler ile knn algoritması tahmin yapmaktadır. 