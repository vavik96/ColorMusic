![PROJECT_PHOTO](https://github.com/AlexGyver/ColorMusic/blob/master/proj_img.jpg)
# Светомузыка на Arduino и WS2812b
* [Описание проекта](#chapter-0)
* [Папки проекта](#chapter-1)
* [Схемы подключения](#chapter-2)
* [Материалы и компоненты](#chapter-3)
* [Как скачать и прошить](#chapter-4)
* [FAQ](#chapter-5)
* [Полезная информация](#chapter-6)
[![AlexGyver YouTube](http://alexgyver.ru/git_banner.jpg)](https://www.youtube.com/channel/UCgtAOyEQdAyjvm9ATCi_Aig?sub_confirmation=1)

<a id="chapter-0"></a>
## Описание проекта
Крутейшая свето- цветомузыка на Arduino и адресной светодиодной ленте WS2812b  
Управление:
- Однократное нажатие кнопки: смена режима
- Удержание кнопки: калибровка нижнего порога шума

Режимы работы (переключаются кнопкой):
- VU meter (столбик громкости): от зелёного к красному
- VU meter (столбик громкости): плавно бегущая радуга
- Светомузыка по частотам: 5 полос симметрично
- Светомузыка по частотам: 3 полосы
- Светомузыка по частотам: 1 полоса

Особенности:
- Плавная анимация (можно настроить)
- Автонастройка по громкости (можно настроить)
- Фильтр нижнего шума (можно настроить)
- Автокалибровка шума при запуске (можно настроить)
- Поддержка стерео и моно звука (можно настроить)
- Подробности в видео: https://youtu.be/nu31By9Phdc

<a id="chapter-1"></a>
## Папки
**ВНИМАНИЕ! Если это твой первый опыт работы с Arduino, читай [инструкцию](#chapter-4)**
- **libraries** - библиотеки проекта. Заменить имеющиеся версии
- **colorMusic** - прошивка для Arduino, файл в папке открыть в Arduino IDE ([инструкция](#chapter-4))
- **schemes** - схемы подключения

<a id="chapter-2"></a>
## Схемы
### Обычная
![SCHEME](https://github.com/AlexGyver/ColorMusic/blob/master/schemes/scheme2.jpg)
### С микрофоном
![SCHEME](https://github.com/AlexGyver/ColorMusic/blob/master/schemes/scheme3.jpg)

<a id="chapter-3"></a>
## Материалы и компоненты
### Ссылки оставлены на магазины, с которых я закупаюсь уже не один год
* Arduino NANO с ногами http://ali.ski/kJHHnL http://ali.ski/OnjivR
* Arduino NANO без ног http://ali.ski/SK0PW http://ali.ski/GAq_mq
* Адресная лента http://ali.ski/CjdQCL
	- Black PCB / White PCB - цвет подложки ленты, чёрная / белая. В видео была чёрная
	- 1m/5m - длина ленты в метрах (чтобы заказать 2 метра, берите два заказа 1m, очевидно)
	- 30/60/74/96/100/144 - количество светодиодов на 1 метр ленты. В видео использовалась лента 60 диодов на метр
	- IP30 лента без влагозащиты (как на видео)
	- IP65 лента покрыта силиконом
	- IP67 лента полностью в силиконовом коробе
	- **Лента как на видео: Black PCB 5m 60 IP30**
* Понижайка для автомобиля http://ali.ski/T5TpbR  http://ali.ski/yLUrOg
* Блок питания 5V 2A http://ali.ski/I6Djw  http://ali.ski/6agpb
* Адаптер питания 5.5х2.1 http://ali.ski/UWjFu
* Аудио гнездо http://ali.ski/OBCRvl
* Разветвитель наушников http://ali.ski/LuAcL  http://ali.ski/gjhGIB
* Звук через микрофон
	+ Микрофон модуль http://ali.pub/2cd5qr  http://ali.pub/2cd5th  http://ali.pub/2cd5un
* Звук по FM радио
	+ Передатчик FM  http://ali.ski/29sic  http://ali.ski/lklMs
	+ Передатчик "сделай сам" http://ali.ski/YsmHW  http://ali.ski/wmNkEX
	+ Приёмник FM из видео http://ali.ski/VsnK0  http://ali.ski/uVp3_
	+ Понижайка 3.3V http://ali.ski/ftSy1x  http://ali.ski/acDEN
	+ Приёмник "сделай сам" http://ali.ski/26e_Jh
* Звук по Bluetooth
	+ Передатчик Bluetooth http://ali.ski/_94Dig
	+ Приёмник "свисток" http://ali.ski/Rkuyvl
	+ Ещё приёмник http://ali.ski/QyigGj
* Кнопки, конденсаторы и крутилки ищите в любых магазинах для радиолюбителей, так как у китайцев можно купить только мешок 50 штук!
* Алик
	+ Куча резисторов http://ali.ski/FcTn6
	+ Куча кнопок http://ali.ski/EBLzU
	+ Куча конденсаторов http://ali.ski/_ARA6v
	+ Куча потенциометров http://ali.ski/fAJrzc
	+ Куча конденсаторов для микрофона http://ali.ski/eqALT
* ЧипДип (Россия)
	+ Резистор https://www.chipdip.ru/product0/27226
	+ Кнопка https://www.chipdip.ru/product/tyco-2-1825910-7-fsm14jh
	+ Конденсатор 10нф https://www.chipdip.ru/product0/42179
	+ Конденсатор для микрофона https://www.chipdip.ru/product0/9000261766
	+ Потенциометр https://www.chipdip.ru/product/r-0901n-b20k

## Вам скорее всего пригодится
* [Всё для пайки (паяльники и примочки)](http://alexgyver.ru/all-for-soldering/)
* [Недорогие инструменты](http://alexgyver.ru/my_instruments/)
* [Все существующие модули и сенсоры Arduino](http://alexgyver.ru/arduino_shop/)
* [Электронные компоненты](http://alexgyver.ru/electronics/)
* [Аккумуляторы и зарядные модули](http://alexgyver.ru/18650/)

<a id="chapter-4"></a>
## Как скачать и прошить
* [Первые шаги с Arduino](http://alexgyver.ru/arduino-first/) - ультра подробная статья по началу работы с Ардуино, ознакомиться первым делом!
* Скачать архив с проектом
> На главной странице проекта (где ты читаешь этот текст) вверху справа зелёная кнопка **Clone or download**, вот её жми, там будет **Download ZIP**
* Установить библиотеки в  
`C:\Program Files (x86)\Arduino\libraries\` (Windows x64)  
`C:\Program Files\Arduino\libraries\` (Windows x86)
* Подключить Ардуино к компьютеру
* Запустить файл прошивки (который имеет расширение .ino)
* Настроить IDE (COM порт, модель Arduino, как в статье выше)
* Настроить что нужно по проекту
* Нажать загрузить
* Пользоваться  

### НАСТРОЙКА НИЖНЕГО ПОРОГА ШУМА (строки 65-71)
- Ручная: выключаем AUTO_LOW_PASS и EEPROM_LOW_PASS, настраиваем LOW_PASS и SPEKTR_LOW_PASS вручную
- При запуске: включаем AUTO_LOW_PASS. При подаче питания музыка должна стоять на паузе!
- По кнопке: при удерживании кнопки 1 секунду настраивается нижний порог шума (музыку на паузу!)
- Из памяти (ЛУЧШИЙ ВАРИАНТ): выключаем AUTO_LOW_PASS и включаем EEPROM_LOW_PASS
  * Включаем систему
  * Ставим музыку на паузу
  * Удерживаем кнопку 1 секунду
  * Значения шумов будут записаны в память и САМИ загружаться при последующем запуске! Всё!

## Настройки в коде
    // лента
    #define NUM_LEDS 120        // количество светодиодов
    #define BRIGHTNESS 230     // яркость (0 - 255)
    
    // пины
    #define SOUND_R A2         // аналоговый пин вход аудио, правый канал
    #define SOUND_L A1         // аналоговый пин вход аудио, левый канал
    #define SOUND_R_FREQ A3    // аналоговый пин вход аудио для режима с частотами (через кондер)
    #define BTN_PIN 3          // кнопка переключения режимов (PIN --- КНОПКА --- GND)
    #define LED_PIN 12         // пин DI светодиодной ленты
    #define POT_GND A0         // пин земля для потенциометра

    // настройки радуги
    #define RAINBOW_SPEED 6    // скорость движения радуги (чем меньше число, тем быстрее радуга)
    #define RAINBOW_STEP 6     // шаг изменения цвета радуги
    
    // отрисовка
    #define MODE 0              // режим при запуске
    #define MAIN_LOOP 5         // период основного цикла отрисовки (по умолчанию 5)
    #define SMOOTH 0.5          // коэффициент плавности анимации VU (по умолчанию 0.5)
    #define SMOOTH_FREQ 0.8     // коэффициент плавности анимации частот (по умолчанию 0.8)
    #define MAX_COEF 1.8        // коэффициент громкости (максимальное равно срднему * этот коэф) (по умолчанию 1.8)
    #define MAX_COEF_FREQ 1.2   // коэффициент порога для "вспышки" цветомузыки (по умолчанию 1.5)
    
    // сигнал
    #define MONO 1              // 1 - только один канал (ПРАВЫЙ!!!!! SOUND_R!!!!!), 0 - два канала
    #define EXP 1.4             // степень усиления сигнала (для более "резкой" работы) (по умолчанию 1.4)
    
    // нижний порог шумов
    int LOW_PASS = 100;         // нижний порог шумов режим VU, ручная настройка
    int SPEKTR_LOW_PASS = 40;   // нижний порог шумов режим спектра, ручная настройка
    #define AUTO_LOW_PASS 0     // разрешить настройку нижнего порога шумов при запуске (по умолч. 0)
    #define EEPROM_LOW_PASS 1   // порог шумов хранится в энергонезависимой памяти (по умолч. 1)
    #define LOW_PASS_ADD 13     // "добавочная" величина к нижнему порогу, для надёжности (режим VU)
    #define LOW_PASS_FREQ_ADD 3 // "добавочная" величина к нижнему порогу, для надёжности (режим частот)
    
    // режим цветомузыки
    #define LOW_COLOR RED       // цвет низких частот
    #define MID_COLOR GREEN     // цвет средних
    #define HIGH_COLOR YELLOW   // цвет высоких
    
<a id="chapter-5"></a>
## FAQ
### Основные вопросы
В: Как скачать с этого грёбаного сайта?  
О: На главной странице проекта (где ты читаешь этот текст) вверху справа зелёная кнопка **Clone or download**, вот её жми, там будет **Download ZIP**

В: Скачался какой то файл .zip, куда его теперь?  
О: Это архив. Можно открыть стандартными средствами Windows, но думаю у всех на компьютере установлен WinRAR, архив нужно правой кнопкой и извлечь.

В: Я совсем новичок! Что мне делать с Ардуиной, где взять все программы?  
О: Читай и смотри видос http://alexgyver.ru/arduino-first/

В: Компьютер никак не реагирует на подключение Ардуины!  
О: Возможно у тебя зарядный USB кабель, а нужен именно data-кабель, по которому можно данные передавать

В: Ошибка! Скетч не компилируется!  
О: Путь к скетчу не должен содержать кириллицу. Положи его в корень диска.

В: Сколько стоит?  
О: Ничего не продаю.

### Вопросы по этому проекту

<a id="chapter-6"></a>
## Полезная информация
* [Мой сайт](http://alexgyver.ru/)
* [Основной YouTube канал](https://www.youtube.com/channel/UCgtAOyEQdAyjvm9ATCi_Aig?sub_confirmation=1)
* [YouTube канал про Arduino](https://www.youtube.com/channel/UC4axiS76D784-ofoTdo5zOA?sub_confirmation=1)
* [Мои видеоуроки по пайке](https://www.youtube.com/playlist?list=PLOT_HeyBraBuMIwfSYu7kCKXxQGsUKcqR)
* [Мои видеоуроки по Arduino](http://alexgyver.ru/arduino_lessons/)