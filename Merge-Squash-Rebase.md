# MERGE COMMİTS İŞLEMİ

## Merge komutuna daha yakın bir bakış

Git merge işlemini gerçekleştirmeden önce aşağıdaki üç commit'i tespit eder.

* **İki branch'in ortak commit'i:** İki branch'in de tarihçesini daha yakından incelediğinizde bu branch'lerin zamanın bir noktasında ortak bir commit'e sahip olduklarını görürüz. Bu anda her iki branch'in de içeriği bire bir aynıdır.
* **Branch'lerin son commit'leri:** Her iki branch için de yapılan son commit'ler

## Fast-Forward ve Merge Commit

Basit bazı durumlarda branch'lerden bir tanesinde herhangi bir değişiklik yapılmamıştır ve bu branch'in yukarıdaki bölümde belirttiğimiz ortak commit'i ve son commit'i aynıdır. Bu durumda merge işlemi çok basitleşir ve git diğer branch'in tüm commit'lerini ortak commit'in üzerine ekleyerek merge işlemini yapar. Bu özel duruma Git terminolojisinde **"Fast-Forward Merge"** denir ve her iki branch'in tarihçesi de ortaktır.

Fakat çoğu zaman her iki branch'de birbirinden bağımsız olarak değişikliğe uğrar ve tarihçe açısından birbirinden uzaklaşırlar. Bu durumda merge işlemini yapmak için Git'in her iki branch arasındaki değişiklikleri içeren otomatik bir commit oluşturması gerekir. Oluşturulan bu commit'e Git terminolojisinde **"Merge Commit"** denir.

## Rebase ile değişiklikleri entegre etmek

Bazı takımlar iki branch'i yukarıda anlattığımız otomatik merge commit'ler yerine **rebase** ile entegre etmeyi tercih edebilir. Rebase sonrasında projenizin iki farklı branch'i olduğuna dair herhangi bir tarihsel iz oluşmaz.



# Git Merge ve Git Rebase arasındaki önemli farklılık

**Git merge** ile yaptığımız birleştirmede yeni bir commit yaratacak ve yeni branch’deki tüm history tarafını kaybetmeden birleştirme işlemi gerçekleşmiş olcaktır.

**Git rebase** ile birleştirdiğimizde ise branch deki commit’lerimizi tek tek alıp istediğmiz branch üzerine ekleyecektir. Böylelikle tek bir history oluşturacak ve istenmeyen history ortadan kalkacaktır.



## Git Squash nedir?



Öncelikle git squash nedir buradan başlayalım, git squash komutu aslında farklı bir rebase kullanımı olarak değerlendirmek daha doğru olacaktır. Geçmişte atılan commit’leri yeniden düzenlemek, isimlendirmek veya birleştirmek için kullanıyoruz.