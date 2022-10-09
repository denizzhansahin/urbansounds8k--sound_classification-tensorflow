# urbansounds8k--sound_classification-tensorflow
UrbanSound8K veri seti ile TensorFlow kullanılarak ses verilerinin sınıflandırılması üzerine yapılmış bir çalışmadır.  CNN algoritmaları ile ses verilerini öğrenme ve işleme yapılmıştır. Python dilinde yazılan bu projede ilk veri ön işleme ile klasörler içindeki ses verilerine ulaşılmıştır, daha sonra ses verileri görüntü verisine Librosa kütüphanesi aracılığıyla dönüştürülmüştür, görüntü grafikleri Matplotlib ile oluşturulmuştur. Görüntü verileri, OpenCV kütüphanesi aracığıyla grayscale, resize ve normalization görüntü işleme çalışmaları yapılmıştır. Görüntüler kaydedildikten sonra ilgili etiketleri ile bir liste haline getirilmiştir. Oluşturulan liste sırası ile x_train, x_test, y_train ve y_test kümelerine bölünmüş ve bu kümeler yeniden boyutlandırılmıştır. İlgili kümeler Pickle kütüphanesi aracığıyla kullanılabilecek formata dönüştürülüp kaydedilmiştir. TensorFlow kütüphanesi ile birlikte evrişimsel sinir ağının(CNN) sırası ile giriş katmanı, gizli katmanı ve sonuç katmanları olşturulmuştur. Veri kümeleri eğitim için epoch=100 olacak şekilde eğitilmiş olmakla birlikte Matplotlib kütüphanesi ile eğitim grafikleri oluşturulmuştur.
Kullanılan kütüphaneler:
Matplotlib, ses veri grafiği ve eğitim modelinin  oluşturulması.
OS, sistem üzerinde klasör oluşturma.
Librosa, ses verilerinin görüntüye dönüştürme, spektrumlarını bulma.
OpenCV, görüntüler üzerinde görüntü işleme yapma.
Pandas ve Numpy, matematikse ve matrix işlemleri yapma.
TensorFlow, derin öğrenme için evrişimsel sinir ağları(CNN) oluşturma ve model eğitimi.
Pickel, model ve veri kümelerinin kaydedilmesi.

Proje dosyası, Jupiter Notebook dosyası olduğu için içinde Linux sistemine ait komutlar çalıştırılmıştır. Bu proje Google Colab aracığıyla toplamda 2300 dosya ile yapılmıştır. UrbanSound8K veri seti, toplamda 8000 dosyaya sahiptir. GPU ile yapılan işlemler CPU'ya göre hızlıdır. CNN model eğitimi ve eğitim için veri hazırlamada RAM ve dahili hafıza tüketimi fazla olmaktadır. Bu durum kullanmak isteyeceğiniz dosya sayısına göre değişiklik göstermektedir.
