## Primitives vs. Objects

there are two types of data in java

*primitive* or  *objects* ,

*primitive* data types are declared with small letters taken word in java , such as int , char , etc,,,,

there is a limited number of the primitive data types , this data type refers to it's own value

this type takes a very small place in the memory , and is stored in a stack which means it's faster to access

*Objects* data types declaration begins with a capital letter in java such as String , there is infinite number of them since you can create your very own data type . this data type refers to a certain address inside the

this type of data takes a bigger place inside the memory when compared to primitives, and is stored in a heap , which means it's much slower to access especially when it's compared with primitive

memory Explain the difference between an “int” and an “Integer” in Java?
int is a primitive data type while ineger is an object data type ,int takes 32 bits while integer 128 bits , int is called from a stack while integer is called from a heap.

What is the default value for ints? Integers?
default value for int =0
default value for integer=NULL

What is autoboxing? Unboxing?
autoboxing is changing the type of a veriable from primitive to object , while unboxing is the opposite to change a variable type from object to primitive
examples :
autoboxing Integer j = 1;
unboxing int j=new Integer (1);

## Exceptions in Java

 they are the cases where something not accounted for happens usually a good programmer would be able to use a try catch finally statement to incoaprate those statements into the code .

 List the three basic categories of exceptions ?
 the checked exception, the error exception the runtime exception

What type of statement can you use to handle an exception?
 throw and try statements obviously
 try{ code that's volatile and might cause error }
 catch(error-type e){
    something
 }
 catch(error-type2 e){
    something
 }
 finally{
    code
 }
 if the code in try fails it will excute the code inside catch depending on the error type
 if it doesn't it will execute the code inside try
 and in all the cases the code inside finally will be executed

## Using Scanner to read in a file in Java

 an extremely usefull ability since we can get data from a json file or csv file or something , we could use it to check how many times a certain words have been mentioned inside a book , or to track certain dangerous words online to check if anyone is planning something bad
 we could use it to create a language algorithem by checking
 what word is most likely to come after a certain word which allows us to create pridicting algorthems for texts
 or the frequancy of a certain word in a certain language
 we could use it to import data or to cut a file of txt into
 smaller files

What is input from a Scanner broken down into?
tokens

