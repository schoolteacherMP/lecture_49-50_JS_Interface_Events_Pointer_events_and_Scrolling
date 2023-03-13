## Задача 1.   
### Наводим указатель  
Напишите функцию `changeBackgroundColor`, которая изменяет цвет фона элемента при наведении курсора на него.   
PS: воспользуйтесь `mouseove`r и `mouseout` или `pointermove`, `pointerover`      
 HTML код:  
 `<div id="myElement"></div>`  
 CSS код:  
 `#myElement {`  
  `width: 200px;`  
  `height: 200px;`  
  `background-color: yellow;`  
 `margin: 50px auto;`  
`}`  

## Задача 2.   
### Изменяем дочерний div   
Есть родительский и дочерний div. При нажатии на дочерний div мышкой и удерживать нажатие он должен изменить размер (width: 200px; height: 200px;) и цвет фона(green). 
При отпускании клавиши мышки вернуть в исходное состояние.  
PS: воспользуйтесь `mousedown`, `mouseup` или  pointerdown, pointerup.  
HTML код:  
`<div class="parent">`  
  `<div class="child"></div>`  
`</div>`    
CSS код:  
  `.parent {`  
  `width: 300px;`  
  `height: 300px;`  
  `background-color: #ccc;`  
  `display: flex;`  
  `justify-content: center;`  
  `align-items: center;`  
`}`  
`.child {`  
  `width: 100px;`  
  `height: 100px;`  
  `background-color: #f00;`  
`}`  
  

## Задача 3.   
### Меняем текст  
При наведении курсора мыши на div, текст внутри него должен измениться на: "Оно живое! (c) Франкенштейн" и цвет фона на красный.  
Как только указатель мыши покидает приделы div, все должно вернуться в исходное состояние.  
PS: воспользуйтесь mouseenter, mouseleave или pointerenter, pointerleave. 	
HTML код:  
`<div id="box">Наведите курсор на меня</div>`   
CSS код:  
`#box {`  
  `width: 400px;`  
  `height: 200px;`  
  `background-color: gray;`  
  `margin: 50px auto;`  
  `text-align: center;`  
  `line-height: 200px;`  
  `font-size: 24px;`  
  `color: white;`  
`}`  


## Задача 4.   
### Вам нравится ваш преподаватель?  
При нажатии мышкой на div с зеленым фоном должен вызываться alert с текстом 'Правильный ответ!'.  
При наведении курсора мыши на div с красным фоном, он должен изменять свое позицционирование в пределах родительского div.  
1. Необходимо добавить обработчик события mouseenter на дочерний элемент, который будет вызывать функцию, изменяющую позицию дочернего элемента внутри родительского элемента.  
2. Эта функция должна выбирать случайную позицию в пределах родительского элемента (новые случайные координаты для дочернего элемента) и задавать ее в качестве новой позиции для дочернего элемента(новые значения CSS-свойств "top" и "left).  
Пример новых координат 'top':  
`const newTop = Math.floor(Math.random() * (parent.clientHeight - childDiv.clientHeight));`  
`childDiv.style.top = ${newTop}px;`  
Ознакомьтесь с: [clientHeight](https://developer.mozilla.org/ru/docs/Web/API/Element/clientHeight)   и [clientWidth](https://developer.mozilla.org/ru/docs/Web/API/Element/clientWidth)  
4. Добавление обработчика события "click" для элемента #btnYes.  

В результате мы получаем дочерний элемент "childDiv", который будет перемещаться по родительскому элементу при наведении курсора мыши на него, и элемент "childDiv2", который будет выводить сообщение "Правильный ответ!" в диалоговом окне при нажатии на него.  

https://user-images.githubusercontent.com/113675674/224688495-e032e303-745e-4e47-be67-b0fd9a7e0b4b.mp4  

HTML код:  
 `<div id="parent">`  
    `<h2>Вам нравится ваш преподаватель?</h2>`  
    `<div id="child">НЕТ</div>`  
    `<div id="btnYes">ДА</div>`  
  `</div>`  
  CSS код:  
`#parent {`  
  `width: 400px;`  
  `height: 400px;`  
  `background-color: gray;`  
  `position: relative;`  
`}`  
`#child {`  
  `background-color: red;`  
  `position: absolute;`  
  `top: 55%;`  
  `left: 70%;`  
  `transform: translate(-50%, -50%);`  
`}`  
`#btnYes {`  
  `background-color: green;`  
  `position: absolute;`  
  `top: 50%;`  
  `left: 20%;`  
`}`  
`#child,`  
`#btnYes {`  
  `width: 100px;`  
  `height: 40px;`  
  `display: flex;`  
  `justify-content: center;`  
  `align-items: center;`  
  `cursor: pointer;`  
`}`  



## Задача 5.   
### 

## Задача 6.   
### 

## Задача 7.   
### 

## Задача 8.   
### 

## Задача 9.   
### 

## Задача 10.   
### Наводим указатель 2 
Напишите функцию `changeBackgroundColor`, которая изменяет цвет фона элемента при наведении курсора на него. Функция должна принимать два аргумента: идентификатор элемента и цвет, на который нужно изменить фон при наведении курсора.  
Например, при вызове функции `changeBackgroundColor('myElement', 'red')`, цвет фона элемента с идентификатором myElement должен измениться на красный при наведении курсора.  
