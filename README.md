# Методичка по Huetone
## Что такое Huetone
[https://huetone.ardov.me/](https://huetone.ardov.me/)
Это инструмент для создания и тестирований цветовых палитр с учетом требований доступности который разработал Алексей Ардов.
## Возможности Huetone
1. Поддержка цветовых моделей LCH и OkLCH  
2. Поддержка расширенных цветовых пространств (P3 and Rec2020)  
3. Расчеты для всей палитры  
	1. Контраста (WCAG and APCA)  
	2. Цветовой разницы (DeltaE)
4. Экспорт и импорт палитры через JSON
5. Возможность поделится с помощью URL
## Обзор интерфейса
[https://www.youtube.com/watch?v=31mJMMYoKvU](https://youtu.be/31mJMMYoKvU)
## Как производить расчеты и изменения?  
[https://www.youtube.com/watch?v=31mJMMYoKvU](https://youtu.be/31mJMMYoKvU?t=76)
## Автоматизация импорта и экспорта через Json
Важно отметить что Huetone поддерживает только палитры с одинаковым числом плотностей цвета.
Поэтому убедитесь что число плотностей цвета совпадает. Как вариант добавить пустышки.
## Как автоматически работать с палитрой из Figma заданной в стилях?  
### Выгрузка палитры из Figma 
1. В файле Figma запустить плагин **Token Studio**
2. Нажать Styles&Variables - Import Styles
3. Прокрутить и нажать Import all
4. Переключить режим отображения на JSON {}
5. Выделить весь JSON и скопировать
6. Открыть https://colab.research.google.com/drive/1YwrnnrhHAOSRklr67Y3c6EbDn0y8WCrB?usp=sharing
7. Вставить JSON в поле для него
8. Ввести имя палитры
9. Нажать на стрелочку рядом с блоком
10. После завершения обработки перейти по созданной ссылке
### Загрузка палитры в Figma
1. В Huetone в основной части нажать на кнопку "Copy tokens"
2. В Figma открыть плагин **Token Studio**
3. Переключить режим отображения на JSON {}
4. Вставить json
5. Нажать Save Json
6. Нажать Styles&Variables - Export styles & variables to Figma - Подтвердить экспорт
## Как автоматически работать с палитрой из Figma заданной в переменных?  
### Выгрузка палитры из Figma 
1. Запустить плагин Variables Import Export - Export Variables
2. Нажать на Export Variables
3. Выделить JSON нужной коллекции и скопировать
6. Открыть https://colab.research.google.com/drive/1YwrnnrhHAOSRklr67Y3c6EbDn0y8WCrB?usp=sharing
7. Вставить JSON в поле для него
8. Ввести имя палитры
9. Нажать на стрелочку рядом с блоком
10. После завершения обработки перейти по созданной ссылке
### Загрузка палитры в Figma
1. В Huetone в основной части нажать на кнопку "Copy tokens"
2. В любом текстовом редакторе заменить type на $type, value на $value
3. В Figma открыть плагин Variables Import Export - Import Variables
4. Задать имя коллекции
5. Вставить json
6. Нажать Save Json
7. Нажать Styles&Variables - Export styles & variables to Figma - Подтвердить экспорт
8. Открыть плагин Variables Pro для того чтобы заменить текущую коллекцию на импортированную

