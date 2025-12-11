# Ayarlanabilir PWM Tetikleyici

<img width="1603" height="1451" alt="Devre Tasarimi" src="https://github.com/user-attachments/assets/26b9a9c8-3730-417f-9240-853d1dce58a9" />

## Devre Açıklaması ve Malzemeler

| Parçalar | Parçalar|
| ------------- |-------------|
| 1-) Esc nin sinyal bacağı| 6-) 8.2k veya 9.1k direnç|
| 2-) Esc nin Vcc yani (+) bacağı| 7-) 1k direnç.|
| 3-) Esc nin Gnd yani (-) bacağı| 8-) 10k Pot (Preset Pot olursa daha hassas olabilir)|
| 4-) 10uf kapasitör minimum 6v| 9-) IRFZ44N mosfet.|
| 5-) 10k direnç| 10-) LM358 (LM358N veya LM358P de olabilir)| 
|| 11-) Giriş (ek besleme) ve çıkış hattı.| 

> **1000-2000us pwm sinyalleri için geçerlidir, birçok rc alıcı devresi 1000-2000us arası pwm üretmektedir, eski tip alıcı kullanıyorsanız devrenin 8 nolu pot devresinin girişine direkt 5v verebilirsiniz. LM358 aynı anda 2 kanal kontrolü yapabilir LM358 in (2-3 ve 5-6 aynı görevi yapar 2-3 ün çıkışı 1 nolu pin,  5-6 nın çıkışı 7 nolu pin dir) son olarak 10k pot (preset) türünde olursa daha ince ayar yapılabilir ve gaz veya direksiyon tetiğinin sonuna yada başına gelince tetiklensin diyebilirsiniz.

> **Not : Eğer motorunuz reverse ise ya da örnek olarak gaz kolunun tersi işlem yapılacak ise LM358 in 2. ve 3. pinlerini yer değiştirerek çözebilirsiniz, daha hızlı tetik tepkimesi isterseniz 10uf yi düşürebilirsiniz ama unutmayın buda pot yani tetiklenme konum hassasiyetini etkileyecektir.
