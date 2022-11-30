# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init* в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов

### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*
 
 ### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Ветки в Git

### Создание ветки

Для того,чтобы создать ветку, используется команда *git branch*


## Слияние веток

Для того,чтобы добавить ветку в текущую ветку используется команда *git merge <name branch>*


# Блочные элементы

## Параграфы и разрывы строк
Для того, чтобы создать параграф с использованием синтаксиса языка Markdown, достаточно отделить строки текста одной (или более) пустой строкой (пустой считается всякая строка, которая не содержит в себе ничего, кроме пробелов и символов табуляции). Для того, чтобы вставить видимый перенос строки (элемент <br/>) необходимо окончить строку двумя пробелами и нажатием клавиши «Enter». Многие элементы синтаксиса Markdown выглядят и работают гораздо лучше в случае, когда их форматируют с помощью «жесткого перевода строк» (разделение строк, осуществленное самим пользователем, а не программой автоматически). К таким элементам относятся цитаты, списки и пр.

## Заголовки
Язык разметки Markdown поддерживает 2 стиля обозначения заголовков: подчеркивание и выделение символом («#»). Выделение заголовков с помощью подчеркивания производится знаками равенства («=») в случае, если заголовок первого уровня, и дефисами («-») в случае, если заголовок второго уровня. Количество знаков подчеркивания не ограничивается. При выделении заголовков с помощью символа («#») используется от одного до шести данных символов, которые устанавливаются в начале строки (перед заголовком). В данном случае количество символов соответствует уровню заголовка. Кроме того, заголовок возможно снабдить закрывающимися символами («#»), хотя это и не является обязательным. Количество закрывающихся символов не обязано соответствовать количеству начальных символов. Уровень заголовка определяется по количеству начальных символов.

Заголовки первого и второго уровней, выполненные с помощью подчеркивания, выглядят следующим образом:

Заголовок первого уровня
========================
Заголовок второго уровня
-------------------------
Заголовки первого, третьего и шестого уровней, выполненные с помощью символа («#»), выглядят следующим образом:
#  Заголовок первого уровня
### Заголовок третьего уровня
###### Заголовок шестого уровня



## Цитаты
Для обозначения цитат в языке Markdown используется знак «больше» («>»). Его можно вставлять как перед каждой строкой цитаты, так и только перед первой строкой параграфа. Также синтаксис Markdown позволяет создавать вложенные цитаты (цитаты внутри цитат). Для их разметки используются дополнительные уровни знаков цитирования («>»). Цитаты в Markdown могут содержать всевозможные элементы разметки. Цитаты в языке Markdown выглядят следующим образом:

>Это пример цитаты,
>в которой перед каждой строкой
>ставится угловая скобка.

>Это пример цитаты,
в которой угловая скобка
ставится только перед началом нового параграфа.
>Второй параграф.

Вложение цитаты в цитату выглядит следующим образом:
> Первый уровень цитирования
>> Второй уровень цитирования
>>> Третий уровень цитирования


## Списки
Markdown поддерживает упорядоченные (нумерованные) и неупорядоченные (ненумерованные) списки. Для формирования неупорядоченный списков используются такие маркеры, как звездочки, плюсы и дефисы. Все перечисленные маркеры могут использоваться взаимозаменяемо. Для формирования упорядоченных списков в качестве маркеров используются числа с точкой. Важной особенностью в данном случае является то, что сами номера, с помощью которых формируется список, не важны, так как они не оказывают влияния на выходной HTML код. Как бы ни нумеровал пользователь список, на выходе он в любом случае будет иметь упорядоченный список, начинающийся с единицы (1, 2, 3…). Эту особенность стоит учитывать в том случае, когда необходимо использовать порядковые номера элементов в списке, чтобы они соответствовали номерам, получающимся в HTML. Упорядоченные списки всегда следует начинать с единицы. Маркеры списков обычно начинаются с начала строки, однако они могут быть сдвинуты, но не более чем на 3 пробела. За маркером должен следовать пробел, либо символ табуляции. При необходимости в список можно вставить цитату. В этом случае обозначения цитирования ( «>» ) нужно писать с отступом. Упорядоченные списки выглядят следующим образом:
1.	Проводник
2.	Полупроводник
3.	Диэлектрик
Неупорядоченные списки выглядят следующим образом:
* Проводник
* Полупроводник
* Диэлектрик
Или
- Проводник
- Полупроводник
- Диэлектрик
Или
+ Проводник
+ Полупроводник
+ Диэлектрик

Цитата, вставленная в список, выглядит следующим образом:

1. Элемент списка с цитатой:

    > Это цитата
    > внутри элемента списка.

2. Второй элемент списка

В результате на экран выводится следующее:
1.	Элемент списка с цитатой:
Это цитата внутри элемента списка.
2.	Второй элемент списка

При вставке цитат в элементы списка важно учитывать, что элементы списка должны находиться на одном уровне, а цитаты должны указываться с отступом. В случае, если правило с единым уровнем списка не соблюдается, следующий после цитаты элемент списка будет автоматически нумероваться цифрой «1.». Кроме того, при необходимости в список можно вставить исходный код. В этом случае его нужно писать с двойным отступом – 8 пробелов или 2 символа табуляции.

## Блоки кода
Отформатированные блоки кода используются в случае необходимости процитировать исходный код программ или разметки. Для создания блока кода в языке Markdown необходимо каждую строку параграфа начинать с отступа, состоящего из четырех пробелов или одного символа табуляции. Блок кода продолжается до тех пор, пока не встретится строка без отступа (или конец текста). Внутри блока кода амперсанды («&») и угловые скобки («<» и «>») автоматически преобразуются в элементы HTML разметки. Кроме того, следует отметить, что внутри блоков кода обычный синтаксис Markdown не обрабатывается. Блок кода в Markdown выглядит следующим образом:

Это обычный параграф:
Это блок кода

Для оформления блока кода используется обратный апостроф ` вокруг кода. Три символа для многострочного кода и один для однострочного:

Пример:

```
$a = 5; 
$b = 3; 
$c = $a + $b; 
``` 

`echo $c;`


## Горизонтальные линии (разделители)
Для того чтобы создать горизонтальную линию с использованием синтаксиса языка Markdown, необходимо поместить три (или более)дефиса или звездочки на отдельной строке текста. Между ними возможно располагать пробелы. Горизонтальные линии в Markdown выглядят следующим образом:
Первая часть текста, который необходимо разделить
***
Вторая часть текста, который необходимо разделить
Или
Первая часть текста, который необходимо разделить

---

Вторая часть текста, который необходимо разделить
В результате на экран выводится следующее:
Первая часть текста, который необходимо разделить
________________________________________
Вторая часть текста, который необходимо разделить
При использовании данного инструмента важно помнить, что после первой части текста и перед второй необходимо оставлять пустую строку. Данное правило необходимо соблюдать только при использовании дефисов. Если его не соблюдать, на экран будет выведен заголовок второго уровня и строка обычного текста. При использовании символа звездочки данным правилом можно пренебречь


# Строчные элементы

## Ссылки
Markdown поддерживает два стиля оформления ссылок:
•	Гиперссылка, с немедленным указанием адреса (внутритекстовая);
•	Гиперссылка, подобная сноске.
Подразумевается, что помимо URL-адреса существует еще текст ссылки. Он заключается в квадратные скобки. Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо поместить URL-адрес. В них же возможно расположить название, заключенное в кавычки, которое будет отображаться при наведении, но этот пункт не является обязательным.
  [пример](http://example.com/ "Необязательная подсказка")
В результате на экран выводится следующее: пример При ссылке на локальную директорию возможно использование относительного пути (от текущей страницы, сайта и т.п.)
При создании сносной гиперссылки вместо целевого адреса используется вторая пара квадратных скобок, внутри которых помещается метка, идентификатор ссылки (id).
[пример][id]:
Также, можно использовать пробел, чтобы отделять 2 пары квадратных скобок:
[пример] [id]: 
В этом случае возможно определить идентификатор в любом месте документа:
[id]: http://example.com/ "Необязательная подсказка"
В результате на экран выводится следующее: [пример] [id] [id]: http://example.com/ "Необязательная подсказка" Иными словами, она состоит из следующих элементов:
•	Идентификатор ссылки, окружённый квадратными скобками (которым может предшествовать необязательный отступ от одного до трёх пробелов);
•	Двоеточие;
•	Один или несколько пробелов (или символов табуляции);
•	URL гиперссылки;
•	Необязательный заголовок (подсказка к изображению, которая всплывает при наведении на него) гиперссылки, заключённый либо в двойные или одиночные кавычки, либо в скобки.
Идентификаторы ссылок могут состоять из букв, цифр, пробелов и знаков пунктуации, однако они не чувствительны к регистру. То есть эти два варианта эквивалентны:
[текст ссылки][a]
[текст ссылки][A]
Markdown позволяет также использовать неявно выраженный идентификатор (сокращенный). В этом случае метка не приводится, вместо неё текст гиперссылки используется и в качестве её имени, а вторая пара квадратных скобок остаётся пустою. Например, чтобы сделать слово «Example» гиперссылкой, ведущей на сайт http://example.com/, достаточно написать:
[Example][]
и затем определить гиперссылку:
[Example]: http://example.com/
В результате на экран выводится следующее: [Example][] [Example]: http://example.com/

## Кодовые фрагменты строк
Чтобы отметить фрагмент строки, содержащий код, необходимо окружить его обратными апострофами «`». При использовании кодовых фрагментов строк текст будет отображаться в виде моноширинного шрифта. В отличие от блоков кода, кодовый фрагмент позволяет поместить код внутрь обычного абзаца текста. Кодовый фрагмент строки в языке Markdown выглядит следующим образом:
Используйте оператор if

## Изображения
В Markdown существует 2 способа вставки изображений в документ:
a. С помощью непосредственного указания URL-адреса изображения. Синтаксис данной команды выглядит следующим образом:
![Альтернативный текст](/путь/к/изображению.jpg)
или
![Альтернативный текст](/путь/к/изображению.jpg "Подсказка")
Иными словами, он состоит из следующих элементов:
•	восклицательный знак;
•	квадратные скобки, в которых указывается альтернативный изображению текст (он станет содержимым атрибута в элементе img);
•	круглые скобки, содержащие URL-адрес или относительный путь изображения, а также (необязательно) всплывающую подсказку, заключённуе в двойные или одиночные кавычки.
b. С помощью метки-идентификатора. Синтаксис данной команды записывается следующим образом:
![Альтернативный текст][id]
где «id» — имя определённой метки изображения. Метки изображений определяются при помощи синтаксиса, совершенно идентичного меткам гиперссылок:
[id]: путь/к/изображению "Необязательная подсказка"
Важной особенностью является то, что Markdown не позволяет задать размеры изображения (ширину, высоту).

# Дополнительные элементы

## Обратный слеш
Может употребляться в Markdown перед специальными символами для того, чтобы они воспринимались в их буквальном (а не служебном) значении. Полный список данных символов приводится ниже:
«\» - слеш;
«`» - обратный апостроф;
«*» - звездочка;
«_» - символ подчеркивания;
«{}» - фигурные скобки;
«[]» - квадратные скобки;
«()» - круглые скобки;
«#» - символ решетки;
«+» - плюс;
«-» - минус (дефис);
«.» – точка;
«!» - восклицательный знак.

## Автоматические ссылки

Markdown поддерживает упрощённый порядок автоматического создания ссылок для URL-адресов и адресов электронной почты. Для этого достаточно поместить URL-адрес или почтовый адрес в угловые скобки, и Markdown сделает его гиперссылкой. В отличие от вышеописанных стилей, в данном случае сам же URL-адрес или почтовый адрес становится и текстом гиперссылки. Автоматические ссылки на адреса электронной почты работают аналогично.

 Автоматические ссылки в языке Markdown выглядят следующим образом:

<http://example.com/>

В результате на экран выводится следующее: http://example.com/

Автоматическая ссылка на адрес электронной почты в Markdown выглядит следующим образом
<address@example.com>

В результате на экран выводится следующее:  address@example.com

## Специальные символы HTML

В языке HTML существует два символа, требующих специального рассмотрения: это символы («<») и («&»). Левая угловая скобка используется как начало тэга; амперсанды применяются для обозначения специального символа HTML. Для того чтобы использовать эти символы в их буквальном смысле, необходимо заменить их элементами HTML, а именно &lt; и &amp; соответственно.

При использовании Markdown подобных действий совершать не нужно. Он позволяет использовать эти символы в исходном виде. В случае если амперсанд используется как часть спецсимвола HTML, он останется неизменным. В противном случае Markdown преобразует его в &amp;.



# Работа с удаленным репозиторием

Коммит, созданный нами, хранится в репозитарии, привязанном к конкретной папке на нашем компьютере, т.е. является локальным. Это полезно, если мы работаем над проектом самостоятельно. Однако в большинстве случаев возникает необходимость обеспечить доступ к результатам работы или доставить код на сервер, где он будет выполняться.

## Как подключиться к удаленному репозитарию?


Для загрузки данных в удаленный репозитарию сначала нужно к нему подключиться. В нашем примере мы используем адрес https://github.com/tutorialzine/awesome-project, однако пользователь может создать собственный удаленный репозитарий на GitHub, BitBucket или другом подобном сервисе. Это занимает некоторое время, однако в дальнейшем полностью себя оправдывает, тем более, что подобные службы имеют пошаговые инструкции для правильно выполнения нужных действий.

Для того, чтобы связать созданный нами локальный репозитарий с удаленным, выполним такую команду:

"This is only an example. Replace the URI with your own repository address".

$ git remote add origin https://github.com/tutorialzine/awesome-project.git

Первая строка напоминает нам, что URI репозитария, который приведен в примере, нужно изменить на свой.

Иногда бывает так, что проект имеет несколько удаленных репозитариев – в таком случае каждому из них присваивается собственное имя. Главный репозитарий принято называть origin.


## Как отправить изменения в удаленный репозитарий?


Теперь, когда у нас в локальном репозитарии создан коммит и мы подключились к удаленному, можем отправить его на сервер. Мы это будем делать каждый раз, когда хотим обновить данные в удаленном репозитарии.

Отправка коммита осуществляется с помощью команды push, которая имеет два параметра - имя удаленного репозитория (в нашем случае origin) и ветку, в которую необходимо внести изменения (master — это ветка по умолчанию для всех репозиториев).


$ git push origin master
Counting objects: 3, done.
Writing objects: 100% (3/3), 212 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/tutorialzine/awesome-project.git
* [new branch] master -> master


Если мы все сделали правильно, то отправленный файл hello.txt на удаленном сервере мы можем увидеть с помощью браузера. Важный момент – некоторые сервисы для отправки изменений могут требовать дополнительной аутентификации.


## Как клонировать удаленный репозитарий?

Если у других пользователей возникла необходимость клонировать удаленный репозитарий, они могут получить полностью работоспособную копию при помощи команды clone:

$ git clone https://github.com/tutorialzine/awesome-project.git

GitHub автоматически создаст новый локальный репозитарий в виде удаленного на собственном сервере.


