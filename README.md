	######################################################
	####          RDC+ Instagram Scraper              ####
	######################################################
	#   RDC+ Data Team Instagram Scraper.                #
	#   RDC+ Veri Ekibi Instagram Veri Toplayıcı.        #
	#                                                    #
	#   August - 2021                                    #
	#   Ağustos - 2021                                   #
	#                                                    #
	######################################################

# RDC+ Instagram Scraper

## Proje hakkında bilgi

Projemiz sosyal medya aracı olan "Instagram" üzerinden detaylı bilgi toplaması yapması için
geliştirilmiştir. Projemiz topladığı verileri "Neo4j" veri tabanı üzerine kayıt işlemi gerçekleştirmektedir.
Projemizi çalıştırmak için kod bloğunun ilgili alanındaki fonksiyonları aktif hale getirmeniz yeterlidir.

## Proje nasıl çalışır?

### Projenin hata almadan çalışması için yapılması gereken işlemler:
Not: <br>
	Dosya içerisinde çalıştığınız kod çalışmasının <code>"user.py"</code> olduğuna dikkat ediniz.

* Gerekli veri tabanının kurulumunu yapınız. <br>
	1- [neo4j](https://neo4j.com/download/) : Neo4j kurulumunu yapınız.
	
* PİP install işlemlerini yapınız. <br>
	1- [py2neo](https://github.com/py2neo-org/py2neo) : pip install py2neo <br>
	2- [instaloader](https://instaloader.github.io/installation.html) : pip3 install instaloader
	
* Kod içerisinde yapmanız gereken düzenlemeler. <br>
	1- ```graph = Graph(host="localhost", auth=("xxxx", "xxxx"))``` <br> 
	kod içerisindeki düzenlemenizi veri tabanında yaptığınız özelleştirmelere göre yapınız. <br>
	Örnek : ```auth=("neo4j", "123456")```
	
	2- ```L.login('username', 'password')``` <br>
	kod kısmında "Instagram" kullanıcı adı ve şifrenizi giriniz. 
