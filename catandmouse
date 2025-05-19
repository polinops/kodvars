function catMouse(map,moves){
if (!map.includes('C') || !map.includes('m')) {
return "boring without two animals";
}
const rows = map.split('\n'); //Разбиваем строку на массив строк
for (let i = 0; i < rows.length; i++) {//проходим по каждой строке
for (let j = 0; j < rows[i].length; j++) {//проходим по элементу каждой строки
if (rows[i][j] === 'C') {//если элемент определенной сироки равен с то опеределяем его координаты
catRow = i;
catCol = j;
} else if (rows[i][j] === 'm') {
mouseRow = i;
mouseCol = j;
}
}
}
const distance = Math.abs(catRow - mouseRow) + Math.abs(catCol - mouseCol);//определяем кратчайшее расстояние от кошки до мышки
if (distance <= moves) {//сравниваем с заданным количеством шагов
return "Caught!";
} else {
return "Escaped!";
}
}
