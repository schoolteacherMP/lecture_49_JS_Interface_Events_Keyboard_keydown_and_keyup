# lecture_49_JS_Interface_Events_Keyboard_keydown_and_keyup

#  [Задачи ](https://github.com/schoolteacherMP/lecture_49_JS_Interface_Events_Keyboard_keydown_and_keyup/blob/main/tasks.md)  

Нажатие клавиши всегда генерирует клавиатурное событие, будь то буквенно-цифровая клавиша или специальная типа `Shift` или `Ctrl` и т.д. Единственным исключением является клавиша `Fn`, которая присутствует на клавиатуре некоторых ноутбуков. События на клавиатуре для неё нет, потому что она обычно работает на уровне более низком, чем даже ОС.  

**События клавиатуры:**  

**keydown** – при нажатии на клавишу (если клавиша остаётся нажатой, происходит автоповтор),   
**keyup** – при отпускании клавиши.  

**Главные свойства для работы с клавиатурными событиями:**    

**code** – «код клавиши» ("KeyA", "ArrowLeft" и так далее), особый код, привязанный к физическому расположению клавиши на клавиатуре.  
**key** – символ ("A", "a" и так далее), для не буквенно-цифровых групп клавиш (таких как `Esc`) обычно имеет то же значение, что и code.  

В прошлом события клавиатуры иногда использовались для отслеживания ввода данных пользователем в полях формы. Это ненадёжно, потому как ввод данных не обязательно может осуществляться с помощью клавиатуры. Существуют события `input` и `change` специально для обработки ввода (рассмотренные позже в лекции _События: change, input, cut, copy, paste_). Они срабатывают в результате любого ввода, включая Копировать/Вставить мышью и распознавание речи.  

События клавиатуры же должны использоваться только по назначению – для клавиатуры. Например, чтобы реагировать на горячие или специальные клавиши.  
