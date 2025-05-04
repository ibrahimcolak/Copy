CyberShield AI - Antivirüs ve Dosya İzleme Sistemi
CyberShield AI, bilgisayarınızdaki dosyaları otomatik olarak izler ve potansiyel virüsleri, truva atlarını tespit edip karantinaya alır. Bu sistem, ClamAV kullanarak dosya taraması yapar ve herhangi bir zararlı yazılım tespit ettiğinde dosyayı güvenli bir şekilde karantinaya alır. Ayrıca, sistemin aktif/pasif durumunu belirlemek için bir yapılandırma dosyası (config.txt) kullanılır.

Özellikler
Gerçek Zamanlı İzleme: Sistem, belirli bir dizindeki tüm dosya değişikliklerini izler.

ClamAV Taraması: ClamAV kullanarak her dosya taranır ve zararlı yazılım olup olmadığı kontrol edilir.

Karantinaya Alma: Tespit edilen zararlı dosyalar karantinaya alınır.

Loglama: Yapılan tüm işlemler detaylı bir şekilde cyberlog.txt dosyasına kaydedilir.

Kolay Yapılandırma: config.txt dosyası ile sistemin aktif veya pasif durumunu ayarlayabilirsiniz.

Başlangıç
Gereksinimler
Python 3.8 veya daha yeni bir sürüm

ClamAV (Antivirüs Yazılımı): ClamAV İndirme

watchdog Python Kütüphanesi:


pip install watchdog
Kurulum
ClamAV Kurulumu:

Windows için ClamAV’ı buradan indirip kurun.

ClamAV’ı kurduktan sonra, clamscan.exe yolunu not alın ve Python scriptinde belirtilen yere ekleyin.

/ Python Scripti: /

Proje dosyasındaki cybershield.py dosyasını çalıştırarak antivirüs ve dosya izleme sistemini başlatabilirsiniz.

/ Yapılandırma /
config.txt dosyasındaki değeri "aktif" olarak ayarlayarak sistemi başlatabilirsiniz.

Eğer sistemin pasif olmasını isterseniz, "pasif" olarak değiştirebilirsiniz.

/ Çalıştırma /
Projeyi çalıştırmak için:

python cybershield.py
Windows üzerinde arka planda çalıştırmak için:

start /min pythonw cybershield.py

Bu komut, programı arka planda çalıştıracak ve herhangi bir ekran çıktısı olmayacaktır.


//Loglar ve Karantina//
cyberlog.txt: Tüm işlemler burada kaydedilir.

quarantine/: Zararlı olarak tespit edilen dosyalar burada saklanır.

İleri Seviye Özellikler
VirusTotal Entegrasyonu: Çevrimiçi virüs kontrolü eklenebilir.

Yapay Zeka Destekli Dosya Tespiti: Dosyaların içeriği hakkında daha akıllı analizler yapmak için yapay zeka entegrasyonu düşünülebilir.

