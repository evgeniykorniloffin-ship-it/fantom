# fantom
chess with gui, win64, winboard chess engine + winboard.exe


## Приятной игры с ШАХМАТАМИ.


### О программе FANTOM.

Это 0x88 движок с интерфейсом WinBoard. Написан в 2006 году и немного модифицирован 2026г.
Чтобы запустить программу, надо кликнуть мышью по start.cmd.
Основные эвристики поиска:
1. Генетичекое сокращение глубины поиска - выбирается случайная точка разделения.
   после точки разделения глубина сокращается (шахи взятия и первый легальный - исключения).
2. Перед поиском запускаются случайные розыгрыши монте-карло для упорядочивания таблицы истории.

```
evgeniy-korniloff@yandex.ru
+79119389756
*Free Soft Spb Ltd, 2026*
GNU GENERAL PUBLIC LICENSE
Version 3, 29 June 2007


```




### compiler:

```
  clang -O3 -m64 *.c -o fantom.exe    
  cl /D_CRT_SECURE_NO_WARNINGS -O1 *.c /Fe:fantom.exe
  gcc -O2 *.c -o fantom.exe
  
```

### platform:
  windows-linux-...


### Run:

```

 windows:
  winboard.exe   /fcp  fantom.exe
     OR
  start.cmd

 linux:
  xboard -fcp  ./fantom&

```




