*number- extra informations/how i solved the problem- description below

Shortly about:
Project based on MVC architecure. 
Program reads the special GameOfLife models from files using boost library- filesystem.
Position of alive and dead cells is coded*1, so i've implemented special functions for encoding it.
Model supports 5 options: Play, Pause, NextStep, PreviousStep*2 and Set FPs. GUI implemented in SFML


What could i do more or better:
a) add a multimethreading in the future- in the time of writing the program it was to hard to me
b) make classes more friendly
c) make code cleaner
d)use more move semantics- it would speed up my program, also use unique_ptr




#1 Patterns are encoded using RLE encoding, there is a webpage where there is a lot of beautiful and interesting patterns to dowload
coded this way.
#2 Game of Life is not a deterministic problem, so i've implemented a mechanism to store 1000 last alive cells, so you can
make step back and get all the alive cells from iteration as long as they're in there. I havent implemented the mechanism
which will react where you make more stepbacks then memory stores, so the program will crush after that

It was my first bigger project, where i've learned some technics from new standards (i know there's no plenty of them in
the code)

