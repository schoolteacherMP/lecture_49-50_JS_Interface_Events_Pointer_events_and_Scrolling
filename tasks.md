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
### 

## Задача 4.   
### 

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
