Bu projede UAV ve bazı endüstriyel uygulamalarda kullanılması için IMU tasarlanmıştır. Projede amaç, tek PCB düzlemi ile FOG IMU (Fiber Optik Jiroskop İzleme Ünitesi) performansına yakın, ultra yüksek doğruluğa sahip bir MEMS IMU tasarlamaktır.
Projenin şematik tasarımı tamamlanmış olup PCB tasarımı devam etmektedir.
Projede 3 eksende ivmeölçer, jiroskop ve manyetik sensör bulunmaktadır. 

Projede ; 

a) Cortex®-M7 çekirdeğine sahip olması,

b) M7 çekirdeğinin ARM tarafından sensör füzyonu algoritmaları için  optimize edilmiş olması , 

c) Dahili cache, ram ve hafızasının sensör füzyonu algoritmaları için yeterli boyuta sahip olması,

d) İçerisinde ekstra güvenlik için kripto şifreleme motoruna sahip olması sebebiyle STM32F777VIT6 MCU modeli tercih edilmiştir.

IMU ±14g arası ölçüm yapıp RS232 ile haberleşme sağlamaktadır. Sensörler SPI üzerinden MCU ile haberleşmektedir.Güç kaynağında yüksek PSRR (Güç Kaynağı Reddetme Oranı) ve düşük Voltage Dropout sahip Analog Devices LDO' ları tercih edilmiştir. Devrede ters bağlantı koruması ve kısa devre koruması için PTC sigorta kullanılmıştır. 

Devrede ki kompanentler seçilirken tek bir tedarikçiden temin edilebilimesine dikkat edilmiştir.

ŞEMATİK TASARIM
![IMU_SCH](https://github.com/sezear07/INTERNAL_MEASUREMENT_UNIT/assets/167361624/1fe740c9-da74-46e7-9002-64d0913661ff)

PCB KATMANLARI
1. SIG/PWR
2. GND
3. SIG
4. PWR
5. GND
6. SIG/PWR
![layer](https://github.com/sezear07/INTERNAL_MEASUREMENT_UNIT/assets/167361624/a17d24f7-0b99-41d2-962f-8e0748af0b21)

3D MODEL
![3D_IMU](https://github.com/sezear07/INTERNAL_MEASUREMENT_UNIT/assets/167361624/3d4d433d-3d14-44a5-8485-8eb2bf3dccf6)



