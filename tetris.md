Notation B-PSU-200 tetris 2017

# Basic tests

* Debug Mode - Read Tetriminos : Subject sample - 1 test
  * Normal
* Display help - 2 tests
  * ./tetris --help
  * cp tetris mytetris ; ./mytetris --help

# Advanced tests
* Bad parameter : - 4 tests
  * ./tetris --key-left=
  * ./tetris -l z -d e -a f
  * ./tetris -l=r
  * ./tetris key-left
* Debug Mode - Read Tetriminos - 17 tests
  * Big Tetrimino
  * Empty Tetrimino
  * Error Tetrimino 1
  * Error Tetrimino 2
  * Error Tetrimino 3
  * Error Tetrimino 4
  * Error Tetrimino 5
  * Error Tetrimino 6
  * Filename of Tetrimino : .h.tetrimino
  * Filename of Tetrimino : .tetrimino
  * Filename of Tetrimino : .tetrimino.tetrimino
  * Filename of Tetrimino : a.tetrimino.b.tetrimino
  * Mix Files
  * Only 1 Tetrimino
  * Only 1 Tetrimino without EOF newline
  * Without Tetriminos Directory
  * Without Tetriminos files
* Debug Mode - Read capacities - 6 tests
  * TERM='' ./tetris -D
  * TERM=vt200 ./tetris -D
  * TERM=vt52 ./tetris -D
  * TERM=vterm ./tetris -D
  * TERM=xterm ./tetris -D
  * env -i ./tetris -D
* Testing Parameters - 4 tests
  * Change many sequence - evil test
  * Change many sequence with special char
  * change left and map size
  * change pause, left, ...
