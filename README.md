# Постановка задачи


## Цель индивидуальной работы.
Целью выполнения индивидуальной контрольной работы является закрепление материала теоретического курса. Работа с простыми графическими примитивами и базой данных. 

## Задание
В соответствии с индивидуальным заданием доработать простое игровое   приложение, разработанное в предыдущем контрольном задании №1.
Общее задание для каждого варианта:
Реализовать рейтинг игроков с помощью БД:
- добавить поле в таблице для хранения никнеймов игроков
- добавить поле для хранения результата игры (количество попаданий и т.п.)
- добавить на игровой экран поле для вывода статистики ( например, количество попаданий)
- добавить простую аутентификацию путем ввода никнейма в специальное поле перед началом игры. Если такой никнейм существует, продолжить игру с предыдущим значением очков. Если нет, то отсчет с нуля.
- сделать специальный экран для вывода игроков в порядке убывания рейтинга (использовать sqlite select  с необходимыми параметрами).
- добавить пункт меню для просмотра рейтинга (доступен без аутентификации)
 
#### Фото номера зачётной книжки
![image](https://user-images.githubusercontent.com/75760235/213951763-c13f5647-8742-4e0b-8cae-772631ccdeca.png)

## Запуск
Для запуска достаточно открыть проект в Android Studio последней версии и запустить на AVD.

## Тестирование 

#### Тесты находятся здесь
https://github.com/EugeniyAchinovich/kr2/tree/main/app/src/test/java/com/example/kr2

Для тестирования логики всех 4 классов созданы 4 файла с тестами: 
1)	UserTest.java – тестирование класса, описывающего игрока
2)	DatabaseHelperTest.java – тестирование класса для работы с БД
3)	StartTest.java – тестирование активити главного меню
4)	MainTest.java. – тестирование активити непосредственно игрового процесса

Для тестирования используются ассерты из Junit и фреймворк Mockito.