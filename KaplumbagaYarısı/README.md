# Turtle_Race_game

**is_race_on** adında bir boolean değişkeni False değeri ile başlatılır. Bu değişken, yarışın devam edip etmediğini kontrol etmek için kullanılacaktır.
**screen** adında bir Screen objesi oluşturulur ve ekranın boyutu 500x400 piksel olarak ayarlanır.
**user_bet** adında bir kullanıcı girişi alınır. Kullanıcı hangi renkteki kaplumbağanın kazanacağına bahis yapabilir.
**colors** ve **y_postions** adında iki liste tanımlanır. colors liste, kaplumbağaların renklerini içerir ve y_postions liste, kaplumbağaların başlangıç yatay konumlarını belirler.
**all_turtles** adında bir liste oluşturulur. **colors** ve **y_postions** listeleri kullanılarak, her renkte bir kaplumbağa oluşturulur, rengi, başlangıç yatay konumu ve liste içine eklenir.
Eğer kullanıcı bahis yapmışsa (**user_bet** değeri True ise), **is_race_on** değişkeni True olarak güncellenir ve yarış başlar.
while döngüsü, **is_race_on** değişkeni True olduğu sürece devam eder.
**all_turtles** listesindeki her bir kaplumbağa için, rastgele bir mesafe seçilir (**rand_distance**) ve kaplumbağa bu mesafeyi ileri doğru hareket eder.
Herhangi bir kaplumbağa ekranda belirli bir yatay konumu (230 birim) geçerse, yarış sona erer **(is_race_on** değeri False olarak güncellenir).
Kazanan kaplumbağanın rengi (**turtle.pencolor**()) winner_color değişkenine atanır.
Eğer kazanan kaplumbağanın rengi, kullanıcının bahis yaptığı renkle aynı ise, kullanıcı kazanmıştır ve bir mesaj yazdırılır. Aksi takdirde, kullanıcı kaybetmiştir ve kaybetme mesajı yazdırılır.
**screen.exitonclick()** metodu ile kullanıcının ekrana tıklaması beklenir ve program sonlanır.