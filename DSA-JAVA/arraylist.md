#  Introduction to Array List in JAVA

>Author : Divyansh Pratap Singh [ Twitter - Handle ](https://twitter.com/dev_pratap3250)




## Difference between ArrayList & Arrays
Arraylist | Array
:-- | --:
They have variable size . | They have fixed size .
non-continous memory allocation | continous memory allocation
can store only objects | can store primitive types ex. int , float and also objects

##  Important Operations to perform on ArrayList : 
1. Add element 
1. delete element
1. display or get element
1. update  element
1. print ArrayList
1. size of ArrayList

##  Defining ArrayList

 Before defining ArrayList we need to import it from the scanner class.

```
import java.util.ArrayList;
```

Complete Code would look like this : 

```
import java.util.ArrayList;
public class  Alst{
    public static void main(String[]args){
        // defining an arraylist
        
        ArrayList<Integer> lst = new ArrayList<Integer>();
        
    }
}

```

## Adding element in ArrayList

To add element in ArrayList we use add( ) function

Syntax : 

```
lst.add(3);

```

>here , lst is the name of the ArrayList which we have defined above

Complete Code : 

```

import java.util.ArrayList;
public class  Alst{
    public static void main(String[]args){
        // defining an arraylist
        
        ArrayList<Integer> lst = new ArrayList<Integer>();
        
        // adding element in ArrayList
        
        lst.add(3);
        lst.add(2);
        lst.add(5);
        lst.add(0);
    }
}

```


#### Adding element at particular position in ArrayList


add( ) function adds an element at the end of the arraylist if we wish to add element at a particular  index position 
we pass 2 parameters in add( <  index position  > < item >)

Syntax  for adding 5 at index position 1 in ArrayList lst defined above

```
lst.add(1,5);

```





##printing entire ArrayList

Syntax for printing ArrayList named lst

```
System.out.println(lst);
```

## printing  particular element of ArrayList

to print a particular element of a ArrayList we use get( ) function
inside the get( ) function we pass the index position of element
```
int i = lst.get(0);

System.out.println(i);
```

## Getting Size of ArrayList

to get the size of the arraylist we use size( ) function

Syntax :
> here  lst is the name of the ArrayList defined above

```

        int i = lst.size();
        System.out.println(i);
        
```


## Deleting an element from ArrayList

to delete a element from ArrayList we use remove()  function and inside this we pass the index position of the element we want to remove

```
lst.remove(0);
```

Complete code would look like this : 

```
import java.util.ArrayList;
public class  Alst{
    public static void main(String[]args){
        // defining an arraylist
        
        ArrayList<Integer> lst = new ArrayList<Integer>();
        
        // adding element in ArrayList
        
        lst.add(3);
        lst.add(2);
        lst.add(5);
        lst.add(0);
        
        // printing arraylist before  deletion
        
        System.out.println(lst);
        
        lst.remove(0); // this removes the element at 0th index position
        
        //  printing  arraylist after deletion
        
        System.out.println("arraylist after  deletion : " + lst);
    }
}

```

##  Updating  an element in arraylist

to update a element  in arraylist we use set( ) function and pass 2  values 
set(< index position of element > < new  value >)

```
lst.set(0,5);
```
above  syntax will change the value at index position 0 from  -> 0 to 5
