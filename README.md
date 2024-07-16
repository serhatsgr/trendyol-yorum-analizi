Türkçe Yorumların Duygu Analizi ve Neo4j İlişkilendirilmesi

Proje Hakkında

Bu proje, Türkçe yorumların duygu analizini yaparak sonuçları Neo4j graf veritabanına yüklemeyi amaçlamaktadır. Proje, kullanıcı yorumlarını toplar, bu yorumların duygu durumlarını analiz eder ve sonuçları kullanıcılar ile üç ana merkez (Olumlu, Olumsuz, Tarafsız) arasında ilişkilendirir.

Kullanılan Teknolojiler ve Araçlar

Makine Öğrenimi ve Doğal Dil İşleme
BERT (Bidirectional Encoder Representations from Transformers): dbmdz/bert-base-turkish-128k-uncased modeli kullanılarak Türkçe metinlerin duygu analizi gerçekleştirilmiştir.
Scikit-Learn: Duygu sınıflandırma modeli olarak MLPClassifier kullanılmıştır.
Veri Toplama ve Ön İşleme
Selenium ve BeautifulSoup: Web scraping işlemi için kullanılmıştır.
Pandas: Veri manipülasyonu ve CSV dosya işlemleri için kullanılmıştır.
Web Uygulaması
Flask: Web arayüzü ve API oluşturmak için kullanılmıştır.
Veri Tabanı
Neo4j: Yorumların duygu durumlarına göre kullanıcılarla ilişkilendirilmesi için graf veritabanı olarak kullanılmıştır.
Py2neo: Python ile Neo4j veritabanı arasında etkileşim kurmak için kullanılmıştır.
Proje Detayları
Veri Toplama: Proje, belirli bir URL'den kullanıcı yorumlarını toplar ve bu yorumları bir CSV dosyasına kaydeder.
Duygu Analizi: Toplanan yorumlar BERT modeli kullanılarak analiz edilir ve Olumlu, Olumsuz, Tarafsız olarak sınıflandırılır.
Neo4j Yükleme: Analiz edilen veriler, kullanıcı yorumları ve duygu durumları Neo4j graf veritabanına yüklenir. Kullanıcılar, rastgele oluşturulan kullanıcı adlarıyla üç ana merkez node (Olumlu, Olumsuz, Tarafsız) ile ilişkilendirilir.
Web Arayüzü: Flask ile oluşturulan web arayüzü, kullanıcıların yorumları girmesine, ilerleme durumunu takip etmesine ve sonuçları görüntülemesine olanak tanır.

Kullanım
Yorumları Topla: Kullanıcılar bir URL girerek yorumları toplar.
Duygu Analizi: Yorumlar analiz edilir ve sonuçlar Neo4j'e yüklenir.
Sonuçları Görüntüle: Web arayüzünden duygu analizi sonuçları ve graf ilişkileri görüntülenir.
Gereksinimler
Python 3.x
Flask
Transformers
Py2neo
Selenium
BeautifulSoup
Neo4j
Kurulum ve Çalıştırma
Gerekli kütüphaneleri yükleyin:

bash
Kodu kopyala
pip install -r requirements.txt
Neo4j veritabanınızı kurun ve çalıştırın.

Web uygulamasını başlatın:

bash
Kodu kopyala
python app.py
Web tarayıcınızdan http://localhost:5000 adresine gidin.

Katkıda Bulunma
Projeye katkıda bulunmak isterseniz, lütfen bir pull request gönderin veya bir issue açın.

Lisans
Bu proje MIT Lisansı ile lisanslanmıştır. Daha fazla bilgi için LICENSE dosyasına bakınız.
