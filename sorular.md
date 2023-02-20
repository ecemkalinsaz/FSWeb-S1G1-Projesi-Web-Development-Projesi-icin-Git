## Araştırma Soruları

Şimdi görevi gerçekleştirmek için hazırsınız. Şimdi biraz daha kullandığımız araçları anlama zamanı. Bu dokümanı güncelleyerek, aşağıdaki soruları cevaplayınız. Git'e biraz daha aşina olmaya başladığınızı göreceksiniz. 

Soruları cevaplamak için [GitHub docs](https://docs.github.com/en)'u kullanabilirsiniz. Docs, (ingilizce documentation'ın kısaltılmış halidir) bir programı veya dilin nasıl kullanılacağını anlatan dokümandır. Yazılım dünyasında sıkça kullanılır. Bir yazılımcı olarak zamanınızın büyük çoğunluğu da bu tarz dokümanları okumakla ve üzerinde çalışmakla geçer.

Eğer aradığınız soruların cevapları GitHub docs'ta yok ise Google'lama becerileriniz size yardımcı olacaktır :)

1. Git nedir?
2. Git ile GitHub arasında ne fark var?
3. Neden bir branch oluşturuyoruz? 
4. Pull Request'in amacı nedir?
5. Bir Branchten diğerine geçmek için kullanıdığımız KOMUT nedir? Örneğin ADINIZ-SOYADINIZ branch'inde çalıştığınızı hayal edin ve main branch'ine geçmek istiyorsunuz.
6. `git fetch`, `git merge` ve `git pull` arasındaki farklıarı açıklayınız. Bu konutlar ne yapar açıklayınız.
7. Merge conflict nedir?
8. Merge conflict'i nasıl çözeriz?

## Cevaplar 

1. Git, yazılım kodlarındaki değişikliklerin takip edilmesini sağlayan bir versiyon kontrol sistemidir. Projelerin yerel bilgisayarlarda depolanmasını ve yönetilmesini sağlar. Bu sayede projelerin önceki sürümlerine geri dönülebilir veya değişiklikler karşılaştırılabilir. 

2. GitHub, Git ile yönetilen projelerin bulut tabanlı olarak depolanması ve paylaşılması için kullanılan bir platformdur. Yazılım geliştiriciler, GitHub üzerinden projelerini paylaşarak diğer geliştiricilerin kolayca katkıda bulunmasını ve hataların düzeltilmesini sağlayabilirler. Örneğin, ekip arkadaşlarımızla bir projede çalışırken projeyi Git kullanarak takip edebiliriz. Herhangi bir değişiklik yaparken, Git değişiklikleri takip eder ve önceki sürüme geri dönmek istediğimizde bize yardımcı olur. Ayrıca, GitHub'da projemizin bir kopyasını saklayabiliriz. Bu sayede, birlikte aynı projede çalışırken, kodlarımızı kolayca paylaşabilir ve çalışmaları takip edebiliriz. Başka bir örnek olarak, açık kaynaklı bir projede çalışabilir ve projeyi GitHub'a yükleyerek tüm dünya ile paylaşabiliriz. GitHub, projemizi kolayca saklamamızı ve düzenlememizi sağlar. Diğer insanlar da projeye katkıda bulunabilir ve GitHub sayesinde birbirimizle iletişim kurabiliriz. Özetle, Git projelerin yönetimi için bir araçken, GitHub bu projelerin depolanması ve paylaşılması için bir arayüz sağlar.

3. Bir branch, yazılım geliştirme sürecinde projenin ana dalından ayrılarak farklı özellikler veya hatalar üzerinde çalışmayı mümkün kılan bir araçtır. Bu sayede, geliştiriciler farklı özellikler üzerinde aynı anda çalışabilirler ve projenin ana dalı etkilenmez, daha düzenli ve güvenli bir çalışma ortamı sağlanır. Örneğin, bir e-ticaret web sitesi geliştirirken, sepete ürün ekleme işlevselliğini eklemek istiyoruz. Ancak, aynı zamanda ödeme işlevselliğini de eklemek isteyen bir başka geliştirici de var. Bu durumda, her birimiz kendi branch'imizde çalışabiliriz. Böylece, sepete ürün ekleme işlevselliği için yapılan değişiklikler, ödeme işlevselliğini etkilemez ve ödeme işlevselliği için yapılan değişiklikler de sepete ürün ekleme işlevselliğini etkilemez. 

4. Pull Request (PR), yazılım geliştirme sürecinde değişiklikleri inceleme ve onaylama, projeye dahil etme ve farklı branch'lerin birleştirilmesini kolaylaştırma amacıyla kullanılan bir araçtır. Örneğin, açık kaynak bir projeye özellik eklemek istiyorsak, öncelikle bir branch açarak değişiklikler yaparız. Değişiklikleri tamamladıktan sonra PR oluştururuz. PR, projenin yöneticilerine veya geliştiricilerine, yaptığımız değişiklikleri inceleme ve onaylama fırsatı verir. Yaptığımız değişikliğin proje ile uyumlu olduğundan emin olmak için kod incelemesi yapılabilir. Eğer yöneticiler veya geliştiriciler değişikliği onaylarsa, değişiklikler ana branch'e birleştirilir. Bu, değişikliklerin proje ile uyumlu olmasını sağlar ve hataların önlenmesine yardımcı olur.

5. Branch'ten diğerine geçmek için kullanılan komut "git checkout" komutudur. Örneğin, ADINIZ-SOYADINIZ branch'inden main branch'ine geçmek istiyorsak, “git checkout main” komutunu kullanırız.

6. - `git fetch`: Remote repository'deki değişiklikleri lokal repository'ye çeker ancak değişiklikleri otomatik olarak birleştirmez. Lokal repository'deki branch'leri remote repository ile senkronize etmek için kullanılır. Remote repository'deki değişiklikleri lokal repository'ye yalnızca indirir.
- `git merge`: Bu komut, değişikliklerin birleştirilmesi için kullanılır. İki farklı branch arasındaki farkları birleştirerek tek bir commit oluşturur.
- `git pull`: Fetch ve merge komutlarını birleştirir. Remote repository'den değişiklikleri çeker (fetch) ve daha sonra lokal branch ile merge eder. Yani, pull komutu, fetch komutunu çalıştırır ve ardından merge komutunu otomatik olarak uygular. Bu komutların farkları şu şekildedir:
git fetch komutu, remote repository'deki değişiklikleri yalnızca indirirken, git pull komutu, remote repository'deki değişiklikleri indirir ve lokal branch ile birleştirir. git merge komutu, yerel repository'de yapılan değişiklikleri birleştirmek için kullanılır. Yani özet olarak, git fetch komutu sadece değişiklikleri indirir, "git merge", yerel repository'de yapılan değişiklikleri birleştirmek için kullanılır, "git pull", yerel repository'deki değişiklikleri uzaktaki değişikliklerle birleştirmek için kullanılır. "Git pull" işlemi, "git merge" işlemini içerir.

7.  Merge conflict, birden fazla kişinin aynı dosyaları değiştirdiği ve değişikliklerin birleştirilirken çakıştığı durumlarda ortaya çıkan bir hatadır. Örneğin, iki kişi aynı satırları değiştirdiğinde çakışma meydana gelebilir. Bu durumda, Git dosyayı birleştiremez ve kullanıcıların manuel olarak çözümlemeleri gerekir. Kullanıcılar, çakışan bölümleri düzenleyerek ve Git'e göndererek birleştirme işlemini tamamlayabilirler.

8. Merge conflict'i çözmek için aşağıdaki adımları izleyebiliriz:
İlk olarak, çakışan dosyaları düzenlemek için VS Code açılır.
VS Code, Git'in hangi değişiklikleri yaptığını gösterir ve bu değişiklikleri kabul etmek veya reddetmek için seçenekler sunar (Accept Current Change | Accept Incoming Change | Accept Both Changes).
- Değişiklikler yapılır ve kaydedilir.
- Değişiklikleri eklemek ve işaretlemek için Git kullanarak dosyalar işaretlenir (add).
- Son olarak, birleştirme işlemini tamamlamak için birleştirme işlemi onaylanır (commit).
- Eğer farklı bir remote repository'den bir değişiklik alıyorsak ve conflict çıkıyorsa, öncelikle diğer değişiklikleri içe aktarmak için git fetch veya git pull komutlarını kullanmamız gerekebilir.