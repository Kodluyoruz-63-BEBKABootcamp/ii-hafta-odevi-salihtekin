# İnterface ve Abstract Class Arasındaki Farklar

## Abstraction(Soyutlama)

Nesne tabanlı programlama içerisindeki önemli kavramlardan biridir. Amaç, çalışan programların iç detaylarını gizleyerek gerekli işlevlerin görünmesini sağlamaktır. Nesnel programlama dillerinde soyutlama işlemini ise Abstract class ve Interface sağlamaktadır.

## Abstract class 

Abstarct sınıflar  genel olarak temel sınıf oluşturmak için kullanılan ve soyutlama yeteneği kazandıran sınıflardır.Bir sınıfı -n abstrac olması için "abstract"  kelimesi kullanılır.Aslında abstract sınıflar temelde oluşturulan bir sınıfın ait olduğu temel kimliği belirtmek için kullanılır.Örneğin bir kalem sınıfı açtığımızda bu kalem sınıfının özelliklerini belirten bir sınıf açmış oluruz.Bu sınıf içinde kalemi tanımlayıcı özellikler bulunur.Renk, marka, tür gibi. Oluşturulan bu sınıfın altında açılan sınıflar ise bu sınıfın kapsadığı küçük sınıfları belirtir.Örneğin dolma kalem gibi. 



## Interface

Interface, içerisinde sadece kendisinden türeyecek olan sınıfların içini dolduracağı metod tanımlarının bulunduğu ve soyutlama yapmamıza olanak sağlayan bir yapıdır. Bu sınıfı tanımlarken "interface" kelimesi kullanılır.İnterface sınıfından türeyen sınıflar interface içerisinde yer alan tüm sınıfları kullanmaktadır. Temel olarak ınterface sınıf bir sınıfın ne yapması gerektiğini belirtir,nasıl yapması gerektiği ile ilgili bilgi vermez. 



Aslında bu iki sınıf birbirinden çok fazla farklılığa sahiptir. Hatta sadece sınıf olmaları tek benzer noktaları olduğu söylenebilir.Temel faklılık ise abstract class, bir sınıfın ait olduğu kimliği belirtir. İnterface ise sınıfın yapabileceği kabiliyetleri belirtmek için kullanılır.

