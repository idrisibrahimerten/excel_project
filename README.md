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

## Information about the project

Our project to collect detailed information via "Instagram", which is a social media tool
have been developed. Our project records the data collected on the "Neo4j" database.
Just activate the functions in the corresponding area of the code block to run our project.

## How to Run?

### Actions that must be performed to make the project work without errors:
Note: <br>
	Code work that you work in a file <code>"user.py"</code> note that it is.
	
* Install the required database. <br>
	1- [neo4j](https://neo4j.com/download/) : Neo4j you do the installation.

* Install the required modules. <br>
	1- [py2neo](https://github.com/py2neo-org/py2neo) : pip install py2neo <br>
	2- [instaloader](https://instaloader.github.io/installation.html) : pip3 install instaloader
	
* Changes that you need to make in the code. <br>
	1- ```graph = Graph(host="localhost", auth=("xxxx", "xxxx"))``` <br> 
	edit the code according to the customizations you make in the database. <br>
	Example : ```auth=("neo4j", "123456")```
	
	2- ```L.login('username', 'password')``` <br>
	enter your "Instagram" username and password in the Code Section.

### Running the project:

* For running the project <code>"user.py"</code> perform the following steps in. <br>
	
	ATTENTION! <br>
		Before Instagram starts collecting data ```User('username')``` by running the function
		in the data base are to be used for process control.
		
	1- To collect detailed profile data of the user name entered, <br>
	```User('username')``` <br>
	"usurname" run the function by entering the user name of the person you are looking for in the section.
	
	2- To determine the followers/followers of the user name from which you received the data, <br> 
	```get_user_followers_followees('username')``` <br>
	activate the function.
	
	3- To access information about the posts that the user from whom you received the data sent, <br>
	```user_posts('username')``` <br>
	activate the function.
	
	4- For detailed HASHTAG and keyword search, <br>
	```get_hashtags("hashtag/keywords", count)``` <br>
	activate the function.

## -----------------------------------------TO TURKISH-----------------------------------------

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
	
### Projenin çalıştırılması işlemi:

* Projenin çalıştırılması için <code>"user.py"</code> içerisinde aşağıdaki adımları uygulayın. <br>
	
	DİKKAT! <br>
		Instagram veri toplama işlemine başlamadan önce ```User('username')``` fonksiyonunu çalıştırarak
		veri tabanında kontrol işlemini yapınız.
		
	1- Girilen kullanıcı adının detaylı profil verisini toplamak için, <br>
	```User('username')``` <br>
	"usurname" kısmına aradığınız kişinin kullanıcı adını girerek fonksiyonu çalıştırınız.
	
	2- Verisini aldığınız kullanıcı adının takipçi/takip ettiklerini tespit etmek için, <br> 
	```get_user_followers_followees('username')``` <br>
	fonksiyonunu aktif hale getiriniz.
	
	3- Verisini aldığınız kullanıcının attığı gönderilere (POST) bilgisine erişmek için, <br>
	```user_posts('username')``` <br>
	fonksiyonunu aktif hale getiriniz.
	
	4- Detaylı HASHTAG ve anahtar kelime araması için, <br>
	```get_hashtags("hashtag/keywords", count)``` <br>
	fonksiyonunu aktif hale getiriniz.
	
