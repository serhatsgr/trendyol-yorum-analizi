TÜRKÇE YORUMLARIN DUYGU ANALİZİ VE NEO4J İLİŞKİLENDİRMESİ

PROJE HAKKINDA

Bu proje, Türkçe yorumların duygu analizini yaparak sonuçları Neo4j graf veritabanına yüklemeyi amaçlamaktadır. Proje, kullanıcı yorumlarını toplar, bu yorumların duygu durumlarını analiz eder ve sonuçları kullanıcılar ile üç ana merkez (Olumlu, Olumsuz, Tarafsız) arasında ilişkilendirir.

KULLANILAN TEKNOLOJİLER VE ARAÇLAR

Makine Öğrenimi ve Doğal Dil İşleme

BERT (Bidirectional Encoder Representations from Transformers): dbmdz/bert-base-turkish-128k-uncased modeli kullanılarak Türkçe metinlerin duygu analizi gerçekleştirilmiştir.<br>
Scikit-Learn: Duygu sınıflandırma modeli olarak MLPClassifier kullanılmıştır.

Veri Toplama ve Ön İşleme

Selenium ve BeautifulSoup: Web scraping işlemi için kullanılmıştır.<br>
Pandas: Veri manipülasyonu ve CSV dosya işlemleri için kullanılmıştır.<br>

Web Uygulaması
Flask: Web arayüzü ve API oluşturmak için kullanılmıştır.<br>

Veri Tabanı<br>
Neo4j: Yorumların duygu durumlarına göre kullanıcılarla ilişkilendirilmesi için graf veritabanı olarak kullanılmıştır.<br>
Py2neo: Python ile Neo4j veritabanı arasında etkileşim kurmak için kullanılmıştır.<br>

PROJE DETAYLARI

Veri Toplama: Proje, belirli bir URL'den kullanıcı yorumlarını toplar ve bu yorumları bir CSV dosyasına kaydeder.<br>

Duygu Analizi: Toplanan yorumlar BERT modeli kullanılarak analiz edilir ve Olumlu, Olumsuz, Tarafsız olarak sınıflandırılır.<br>

Neo4j Yükleme: Analiz edilen veriler, kullanıcı yorumları ve duygu durumları Neo4j graf veritabanına yüklenir. Kullanıcılar, rastgele oluşturulan kullanıcı adlarıyla üç ana merkez node (Olumlu, Olumsuz, Tarafsız) ile ilişkilendirilir.<br>

Web Arayüzü: Flask ile oluşturulan web arayüzü, kullanıcıların yorumları girmesine, ilerleme durumunu takip etmesine ve sonuçları görüntülemesine olanak tanır.



KULLANIM


Yorumları Topla: Kullanıcılar bir URL girerek yorumları toplar. <br>
<br>


![agprojeEkran](https://github.com/user-attachments/assets/c008715b-1ed3-4c5d-8a52-4f03e1bb21c6) <br>
<br>
<br>
<br>


Duygu Analizi: Yorumlar analiz edilir ve sonuçlar Neo4j'e yüklenir. <br>

![trendyolgraf1](https://github.com/user-attachments/assets/26d13cf9-13af-4305-9744-8997ecdbeae6)<br>
<br>
<br>
<br>


Sonuçları Görüntüle: Web arayüzünden duygu analizi sonuçları görüntülenir.<br>


![agProjeEkran2](https://github.com/user-attachments/assets/a0a4b933-7757-48fa-92c2-604f830021cd)<br>
<br>
<br>
<br>




PROJE AFİŞİ<br>


![TRENDYOL ÜRÜN YORUMLARININ ÇEKİLEREK DUYGU ANALİZİ YAPILIP GÖRSELLEŞTİRİLMESİ (1)](https://github.com/user-attachments/assets/49b265d4-b0dc-4eb5-89c2-13cdd952ed72)<br>




GEREKSİNİMLER

Python 3.x
Flask
Transformers
Py2neo
Selenium
BeautifulSoup
Neo4j


KURULUM VE ÇALIŞTIRMA

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









