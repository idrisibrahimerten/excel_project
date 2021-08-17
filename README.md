<img align="left" width="100" height="100" src="img.png">

# RDC+ Eksi Sozluk Scraper
<br>

## Description
* EksiSozlukScraper is an extraction tool for extracting data from EksiSozluk. <br>
Relevant data is stored in Neo4j. <br>
You can follow the steps below to run the program. <br>

## Environment Setup

* You should install the required modules. You can install all of them by using the ```requirements.txt``` file.
```shell
pip install -r requirements.txt
```
* You can also install them by using the commands below. All other required modules will be automatically installed as well. <br>
   * [argparse](https://pypi.org/project/argparse/) &#8594; ```pip install argparse``` <br>
   * [bs4](https://pypi.org/project/bs4/) &#8594; ```pip install bs4``` <br>
   * [selenium](https://github.com/SeleniumHQ/Selenium) &#8594; ```pip install selenium``` <br>
   * [py2neo](https://github.com/py2neo-org/py2neo) &#8594;  ```pip install py2neo```
* Changes that you may need to make in order to run the program. <br>
   * ``` graph = Graph(host="localhost", auth=("xxxx", "xxxx")) ``` <br>
   Edit the code according to the customizations you make in the database. <br>
   Example : ```auth=("neo4j", "123456")```
---
## Yapılması Gereken Düzenlemeler

* Gerekli modül içerisinde bulunan ```Eksi.py``` dosyasına giderek.
    * ```shell
      for topic_id, topic in enumerate(self.topics):
      ```
    * Döngü içirisine ulaşarak,
    * ```shell
            for link in threadList:
                gündemTitle = {"Number": topic_id,
                               "Title": topic.text,
                               "agendaLink": link}
                
                if self.topic_limit > topic_id:
                    #cprint("green", topic_id + 1, "-", end="")
                    #cprint("white", topic.text)
                    print(gündemTitle)
                    break
                else:
                    break
      ```
    * ekleyiniz.
* You should install the required modules. You can install all of them by using the ```requirements.txt``` file.
```shell
pip install -r requirements.txt
```
* You can also install them by using the commands below. All other required modules will be automatically installed as well. <br>
   * [argparse](https://pypi.org/project/argparse/) &#8594; ```pip install argparse``` <br>
   * [bs4](https://pypi.org/project/bs4/) &#8594; ```pip install bs4``` <br>
   * [selenium](https://github.com/SeleniumHQ/Selenium) &#8594; ```pip install selenium``` <br>
   * [py2neo](https://github.com/py2neo-org/py2neo) &#8594;  ```pip install py2neo```
* Changes that you may need to make in order to run the program. <br>
   * ``` graph = Graph(host="localhost", auth=("xxxx", "xxxx")) ``` <br>
   Edit the code according to the customizations you make in the database. <br>
   Example : ```auth=("neo4j", "123456")```
---
## How to Run?

To run the program &#8594; ```python EksiSozlukScraper.py ```

* Gather agenda data for the day you're querying. &#8594; ```main_(**configArgs)```
* Gather detailed information about Ekşi Sözlük user &#8594; <br> ```userArg(username)```
* Collect data on the topic of your choice &#8594; ```threadArg(thread)```
* Gather data on your chosen topic and keyword/hashtag &#8594; ```threadKeywordArg(thread,keyword/hashtag)```

**************************************************************
#### Türkçe 
                         
## Proje hakkında bilgi

Projemiz sosyal medya aracı olan "Ekşi Sözlük" üzerinden detaylı bilgi toplaması yapması için
geliştirilmiştir. Projemiz topladığı verileri "Neo4j" veri tabanı üzerine kayıt işlemi gerçekleştirmektedir.
Projemizi çalıştırmak için kod bloğunun ilgili alanındaki fonksiyonları aktif hale getirmeniz yeterlidir.

## Kurulum

*  ```requirements.txt``` dosyasını kullanarak gerekli modül kurulumlarını yapın.
```shell
pip install -r requirements.txt
```
* Aşağıdaki kodları çalıştırarak da gerekli kurumları yapabilirsiniz.<br>
   * [argparse](https://pypi.org/project/argparse/) &#8594; ```pip install argparse``` <br>
   * [bs4](https://pypi.org/project/bs4/) &#8594; ```pip install bs4``` <br>
   * [selenium](https://github.com/SeleniumHQ/Selenium) &#8594; ```pip install selenium``` <br>
   * [py2neo](https://github.com/py2neo-org/py2neo) &#8594;  ```pip install py2neo```
* Programın çalışması için ```graph``` objesini kendi veritabanınıza göre ayarlayın. <br>
   * ``` graph = Graph(host="localhost", auth=("xxxx", "xxxx")) ``` <br>
   Örnek : ```auth=("neo4j", "123456")```
---
## Nasıl Çalıştıracağız?

Programı çalıştırmak için &#8594; ```python EksiSozlukScraper.py ```

* Sorguladığınız gün için gündem verilerini toplayın. &#8594; ```main_(**configArgs)```
* Aradığınız Ekşi Sözlük kullanıcısına ait detaylı veri toplayın &#8594; <br> ```userArg(username)```
* Aramak istediğiniz konu başlığı üzerine veri toplayın &#8594; ```threadArg(thread)```
* Seçtiğiniz konu ve anahtar kelime/hashtag hakkında veri toplayın &#8594; ```threadKeywordArg(thread,keyword/hashtag)```


					######################################################
					####          RDC+ Eksi Sozluk Scraper            ####
					######################################################
					#         RDC+ Data Team Eksi Sozluk Scraper.        #
					#      RDC+ Veri Ekibi Eksi Sozluk Veri Toplayıcı.   #
					#                                                    #
					#                   August - 2021                    #
					#                  Ağustos - 2021                    #
					#                                                    #
					######################################################
