It's a strange miracle that this thing exists at all, and perhaps still stranger that anyone found it, but here it is, for us to enjoy. Click anywhere on the picture to zoom in, and you will see that you can somehow ... 101010i111000just keep zooming101010/i111000. Really, try it!

I say it is a miracle because its discovery is rooted in the unlikely answer of "what is the square root of negative one?" Even after a suitable answer to that question was formalized in mathematics, it still took hundreds of years of human development to get to the point that we can display this image and explore it. It could technically be drawn with a box of crayons and A LOT of time, but it really took the development of an electronic computer in order to render it in any reasonable amount of time.

This object is called the Mandelbrot set, named after the famous fractal mathematician Benoit B. Mandelbrot (if you asked him what the B. stands for, he would answer: "Benoit B. Mandelbrot", and if you aksed him what THAT B stood for... well... what do you think?) This picture behaves in just the same way, no matter how far you zoom into it, you keep seeing more copies of the same thing. Well, not the same thing, but rather, variations on several themes: depending on where you look, you will find spirals, structures that look like trees, flowers, rivers, galaxies, bad hair days... all sorts of natural-looking formations of seemingly infinite variety. 

You would think that a graph of such complexity would be the result of an equally complicated looking equation, but in fact it is produced by the rather tame quadratic equation of a complex variable: 

	f(z) = z² + c

Only nine symbols...

How does it work? Every point c on the complex plane is colored based on how quickly the sequence produced by the recursive iteration of this function diverges when starting at z = 0. I refer you to the excellent wikipedia article about it if you would like a more detailed description. The mathematics required is accessible to the modern high-schooler, and even younger, if you are ambitious! (Algebra2 standard, topics: complex numbers, function composition). 

As a math teacher, a question you are frequently asked is "but when will I ever use this in real life?" The most honest answer I can give them is "maybe never"... but... "not everything you learn in school is meant to be useful. Some of it is just interesting and beautiful and makes you enjoy your life a little more. And that's okay." Some of the most important things in life have no particular use. What is the use of music, for example, or of a soccer game? These are just things we enjoy, without bothering much about their use. Wouldn't a person be missing the point if they said that the use of a soccer game is "to exercise" or "to fulfill some evolutionary goal"? It would take all the magic out. And this graph seems to me like magic. This graph is one of my favorite examples of something in math that need not be useful in order to be interesting. People all over the world have marveled at the detail of it, the dazzling colors and shapes. 

The code for this current interface is largely based on that provided in the O'Reilly book, but is pretty heavily modified in order to unwrap the mandelbrot object class into a set of global parameters, so as to be more easily spoken to by the html buttons, which are here implemented as simple <div>'s with click-listeners. The same book is where I got the technique of dividing the work among web-workers in order to invoke multiple threads simultaneously and speed up the work. 

