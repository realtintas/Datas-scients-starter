# Genel Hatları İle Veri Bilimi

## Veri Bilimi ve Makine Öğrenmesi

Makine öğrenmesi veri yapılarının belli modellemeler doğrultusunda bilgisayara öğretilmesi ile gerçekleşen yapıya söylenir.
2 farklı şekilde olur denetimli veya denetimsiz.

Burada ki ***denetimsiz*** kısmından kasıt aslında bir denetim olmaması anlamına gelmemekte. Çünkü aslın denetimsiz makine öğrenmesi mümkün olmamaktadır.Denetimsiz yerine bu yazımızda az denetimli dememiz daha doğru bir bilgi olacaktır.

Denetimli makine öğrenmesi etiketlenmiş veriler ile eğitilmiş etiketli veriler kadar kapsayıcı olan makine öğrenmesi türüdür. Denetimsiz(az denetimli) makine öğrenmesinde ise olay etiketli verilerin öğretilmesinden daha çok kavranma mantığı ile açıklanır. Nasıl ki kavranacak şeylerin sonsuzluğu gibi bir durum var ise herşeyi kavranması veya bu kavranacak şeylerin tamamen bilgisayara bırakılması durumu mümkün değildir.

## Verilerin Classification ve Regresion Şeklinde Ayrımı

Classification adından da anlaşılacağı gibi ***sınıflandırma*** olarak ele alınabilir.İşleyiş olarak alınacak verilerin sınıflandırılması ve bu sınıflandırmaların model içinde değerlendirilmesi ile test edilecek verinin hangi sınıfa ait olacağı gibi durumlar belirlenir.

Peki Regresion nedir? Regresion tahmin ve mantık yürütme becerisidir.Classificationa benzer gibi görünse de aslında bu sınıflandırmanın yanı sıra önceki verilerden yola çıkarak bir sonraki verilerin veya durumların tahmini üzerine gider,verileri bu şekilde değerlendirir ve tahmin algoritmasını oluşturur.

## Ele Alınan Verilerin Verimli Şekilde Kullanılması

Elimizde bir veri seti var gibi düşünelim. Bunu bir torbadaki bilyelere benzetebiliriz. Bilyelerin hepsini tek seferde gösterdiğimizde bu tahminden veya sınıflandırmadan daha çok makineye ezber yaptırmak olur çünkü zaten göreceği tüm verileri görmüştür ve ilerleyen zamanlarda modelin patlayacağının birazda sinyalidir.

Bu durumda ne yapacağız. Veriden bir kısmı kenara alsak ve bunu test için tutsak. O zaman öğrenme yaptıktan sonra makinenin göremediği verileri makineye göstermek için bir fırsatımız olacaktır ve bu şekilde modelin işlevselliğini kontrol için bir fırsatımız olur. Daha sonradan test sonuçlarının doğruluğunu arttırmak için modelimiz üzerinde değişiklikler yapabiliriz. Bu durumda yine kısmi olarak yine ezberletmiş sayılıyoruz.
Peki daha iyi bir hale getirebilir miyiz?

Validation tam burda ortaya çıkıyor.Veri setimizi 2 yerine 3 parçaya bölerek validation kısmını yaratmış oluyoruz. İlk bölümü ile makine eğitimi yapıyoruz.Daha sonra ikinci kısım ile test ediyoruz fakat bu kısım test kısmı değil validation kısmı. Sonra validation kısmına göre modelimizde düzenlemeler yapıyoruz ve tahmini değerimiz ile reel değer arasındaki farkını (hata payı) azaltıyoruz.En son kısımda 3. parçamızı test olarak sunuyoruz ve modelimizin daha önce görmediği verilerde nasıl davrandığını inceliyoruz.

 # Resul Ekrem Altıntaş