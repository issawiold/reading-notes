**importing in java**

importing a package or library in java is similar to calling a professional person to do a specific operation , asking that person to stand on the side until his name is called and they are asked to do something specific , the reason we do that is to ensure that our program is not heavy.

 by keeping all that specialized code stored in libraries that you can  import, we make sure to keep the program light, and all you have to do whenever you need one is to import them and call them as you use them .

 keeping all the libraries loaded inside your program is similar to having over a thousand people inside the second floor of a building that the building is going to fall and collapse , or inside a vehicle which would either crash it or it would move very slowly and we don't want those two outcomes .

**loops in java**

loops in java are very similar to those from javascript with the exception of for-each

*for: for (initialization; Boolean-expression; step)\
  statement;*

*while: while (Boolean-expression)\
    statement;*

*do-while: do {\
    statement;\
} while (Boolean-expression);*

only for statement contains a counter and  the difference between while and do-while is the placement of the code block , one places it before the condition(do-while) while the other afte the condition (while)

**arrays in Java**

you can declare an array in java using one of three ways

datatype [ ] arrayname = new datatype [arraysize];

datatype [ ] arrayname={elements}

datatype arrayname [ ] = new datatype [arraysize];

and you can either decide the array size by the number of elements you place in the array on initiation , or also by initiating it using size

**three methods for arrays**

mismatch(arr1,arr2)=> find the first mismatched element inside the two arrays .

compare(arr1,arr2)=>compare the elements of two arrays .

setAll(arr,function)=> generate the elements of the array using a generator function .