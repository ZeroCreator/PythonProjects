Задание 10.
> Лабиринт может быть представлен двухмерной матрицей, где нули представляют области, по которым можно ходить,
а единицы - стены. Вы начинаете движение с верхнего левого угла, а выход находится в самой нижней правой ячейке.
Создайте функцию, которая возвращает истину, если вы можете пройти от одного конца лабиринта до другого.
Двигаться можно только вверх, вниз, влево и вправо. По диагонали двигаться нельзя.
___
Примеры:
```python
can_exit([
  [0, 1, 1, 1, 1, 1, 1],
  [0, 0, 1, 1, 0, 1, 1],
  [1, 0, 0, 0, 0, 1, 1],
  [1, 1, 1, 1, 0, 0, 1],
  [1, 1, 1, 1, 1, 0, 0]
]) ➞ true

can_exit([
  [0, 1, 1, 1, 1, 1, 1],
  [0, 0, 1, 0, 0, 1, 1],
  [1, 0, 0, 0, 0, 1, 1],
  [1, 1, 0, 1, 0, 0, 1],
  [1, 1, 0, 0, 1, 1, 1]
]) ➞ false # В этом лабиринте одни тупики!

can_exit([
  [0, 1, 1, 1, 1, 0, 0],
  [0, 0, 0, 0, 1, 0, 0],
  [1, 1, 1, 0, 0, 0, 0],
  [1, 1, 1, 1, 1, 1, 0],
  [1, 1, 1, 1, 1, 1, 1]
]) ➞ false # Выход так близко, но недостижим!

can_exit([
  [0, 1, 1, 1, 1, 0, 0],
  [0, 0, 0, 0, 1, 0, 0],
  [1, 1, 1, 0, 0, 0, 0],
  [1, 0, 0, 0, 1, 1, 0],
  [1, 1, 1, 1, 1, 1, 0]
]) ➞ true
```