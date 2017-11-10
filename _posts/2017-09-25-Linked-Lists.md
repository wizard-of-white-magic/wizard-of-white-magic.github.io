# Linked Lists
> Linked list is in a way a strange datastructure, think of it as a one handed knight who is trying to save the world. There is no question of doubt as to whether linked lists have actually saved the world or not... You will understand it in a while. 
> Below you would see `Spoiler Alert`'s , here I would try to explain a concept using some real world analogies or some tv series analogy.
> So, if you dont need spoilers you can skip it. I would use `Spoiler Alert` only if I'm using a Tv Series example :)
### Analogy: *(Spoiler Alert)*
> But for now, think of Linked List as Jaime Lannister (Any `GOT` fans reading this blog... ? No, Linked List has no sisters....)
> FYI, Jaime Lannister is a one handed knight in one of the TV series. If you dont know, dont worry, nothing related to Linked Lists.
>
>To actually understand linked list better or to appreciate linked lists better, we have to look at how Arrays were causing a problem in the first place.

### What are Arrays?
Arrays are kind of data structure that can store a `fixed-size`,  `sequential` collection of elements of the `same type`.

**Declaration Syntax** : `Java Syntax` int[] arr = new int[n]

**Fixed Size** - 
So, what does it mean when we tell Arrays are `fixed size`? If you have hands on experience with programming, you would already know that you will have to declare the size of an array while initializing it before hand, meaning you would have to somehow through `black magic` (magic need not be black all the time, but just taking it up like that) know that the application your building would exactly use `n` (n being the size of the array) amount of space and you would declare an array of size `n` and give it to the application. But there is a catch here isn't it? The catch is, all of us are not talented enough to perform `black magic` :( or are we? Well `Linked Lists` is a work around to solve this, so consider implementing a linked list itself as `black magic` :D 

**Sequential** - Arrays store the data in contiguos memory locations. Well in the text books and many websites you would see the below diagram.

<!--![Array](http://wizard-of-white-magic.github.io/img/array.png)
-->

<img src="http://wizard-of-white-magic.github.io/img/array.png" width="500">


<!--
what are these locations exactly? What does `contiguos/sequential` mean? It means, that the `compiler` would in advance request for the `n` amount of space in `main memory` (RAM - Random Access Memory) `FYI RAM is the place, where all the programs at runtime runs or are executed` and the Operating System, in-turn being the `resource manager` allocate the requested `n` amount of space in the `main memory` here, the operating system makes sure that the space it is allocating for the program is all continous, next to each other, the boxes in the above diagram represent continous/contiguos blocks/chunks of memory in `RAM` hope this rings some bells, but what would Operating System do, if `n` amount of space we requested for is not availabe in the `main memory`? Operating System would just throw an `Insufficient Memory Exception` Exceptions are nothing but errors, but there are many differences to exceptions as compared to errors, but that is for another post, for now think of it as, the operating system would just throw an error at us. Even though the required `n` amount of space is present in RAM, but all spread out across the RAM and not continous, still we would not be able to utilize the space as it is not present continously. Now, isn't this in efficient usage of Main Memory??


**Same Type** - As shown in the above syntax example, the array `arr` can hold only integers, the type of elements this array can hold is fixed at the time we declare an array for use itself. Well, most of the programming languages today provide us with the freedom to store data of varied types today, but still it would not cover up the draw back of an array. This can be stored with LinkedLists, but with some work around, which would become too complex for now, just remember that it can be solved using Linked Lists.

Well enough of digging `Array's Grave`, Arrays' have some advantages too,

###Advantages of Arrays
**Fast** - Arrays' are fast... Now, that's what I'm talking about! Speeeeeed!

Think of it, since the compiler already knows the type of data you would be storing in an array and how much data (`n`) you'd be storing, it need not worry about finding the *type* of the value or the the *location* at which you'll have to store this data at run time. All it cares about is, whether the value your trying to store is the *same type* as of the array or not and whether or not there is still *allocated* space left next to it or not. That is it. Other than this, it does not give a damn! It just blindly throws an exception if you try to insert data of different *type* or try to insert *data* when there is no space left.

**Random Acess** - Arrays provide `Random Access`, since arrays store the data in contiguous memory locations, each `unit` of data it stores, it backs it up with an index, like in the above shown array diagram. 0....4 are indices of that array. (psss... Don't see flash, he's not an array, above him please...) Now, what exactly I mean by random access? If I have to access the `3rd` element of an array, I need not go to the `1st` element and then `2nd` element and then to `3rd` element, this would become sequential access, if the array variable is `arr` I could directly access `arr's` `3rd` value as `arr[3]` and ola! I would get it.  

***Think Of It..***

Why are RAMs(Random Access Memories) named Random Access Memory?? Does it have something to do with Arrays?? I dont know... Research it...
Now that you know about Arrays, lets see what's under LinkedList's Hood!-->