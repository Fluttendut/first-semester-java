# Variables, operators and expressions



Today we will be working with operators and variables. 



## Variables

A variable is a container for some value (data). As the image shows below we can save the number 22 (value) in a variable we call `x`. In Java that would look like this:

```java
int x = 22;
```



![Variables are like boxes (from Khan Academy)](https://github.com/HackYourFuture-CPH/JavaScript/raw/master/javascript1/week1/assets/box.png)



Lets disect the above code example:

- `int` is the **type** of the variable
- `x` is the **name** of the variable
- `22` is the value we **assign** to the variable called `x`



Let's make a more real world scenario:

```java
int salary = 400000;
```

In this example we assign the value of `400000` to a variable called `salary`. The type of `salary` is `int`

![Screenshot 2021-05-04 at 13.06.40](../../assets/variable-type-name-value.png)



### Types

In Java it's very important that the type of the variable is specified. Not all programming languages are like that but Java is **very** strict with this!

There are lots of different types in Java. Let's have a look at some of them:

- `int` - Stores integers. Integers are whole numbers. That means `2`, `-344` or `6000` but not `2.2` or `3.1415`
- `double` - Stores numbers with decimal. Fx `2.2` or `3.1415`
- `char` - Stores a single character. Fx the character `a` or the character `y`. `char` have single quotation around them `'a'` or `'y'`
- `string` - Stores text. So if i wanted to store my name or the the city Copenhagen. String are stored with double quotation around them `"Benjamin"`, `"Copenhagen"`

You can read up on more more Java types here: https://www.w3schools.com/java/java_data_types.asp dont get too frightened we will learn the types as we progress with the language. One thing at a time 😄

![Screenshot 2021-05-31 at 15.10.22](../../../third-semester/assets/variable-types.png)





### Print out your variables

To see the value of your variables we print the value to the console. Now what does that mean? 

The console you can see as way for us developers to know how our program is doing. A console can help us write correct code. In the console fx we can see errors  that were thrown or warnings. 

To print something to the variable write the following:

```java
System.out.println(23);
```

This will print `23` to the console. We can print whatever we want to fx

```java
int salary = 400000;
System.out.println(salary);
```

Now `400000` will be printed to the console!



#### Where to find the console

When you run your Java application the console should appear in the bottom of the IDE!



![Console](../../assets/console.png)



### Some more code examples

When i write `//` in Java that means a comment. A comment is invicible to Java and will not be seen

```java
// variable declaration but no assignment
int pages;
// assignment happens later!
pages = 456;
// the variable called pages can be reassigned (changed)
pages = 455;

// lets try and declare and assign a string
String bookTitle = "To the sea";
// lets try and change that!
bookTitle = "From the sea";
```



### Exercise 1

Create a new Java class called `Person.java`. Use the code below as a start

```java
public class Person {
    public static void main(String[] args) {
				// Write your code here
    }
}
```

Do these steps one step at a time! Think about what type of data should be stored in the different variables

1. Create a variable called `age` (no assignment!)
2. Create another variable called `height`
3. Assign `age` to be your age
4. assign `height` to be your height in meter
5. Create the variable `showSize` and assign it to be your showsize
6. Create a variable called `name` and assign this to your name

*Remember to compile at each step!*



## Operators and expressions

> An expression is a simple value or a set of operations that produce a value



The simplest expression is just a value fx `55.9` but if we go a bit more advanced we can do things like addition:

```java
3 + 5
```

Here `+` is called the operator. Lets take a look at some more operators



### Arithmetic Operators

- `+` - Addition
- `-` - Subtraction
- `*` - Multiplication
- `/` - Division
- `%` - Modulus



## More complex expressions

It is possible to create more complex expressions:

````java
result = 3 * 5 / 5 + 1 // will this java code run??
````



![Expression](../../assets/expression.png)



### Order op operations

![Order of operations](../../assets/order-of-operations.png)



### Exercise 1.1

In what order will Java calculate these different expressions?

```java
int result = 100 * 100 / 5 + 200 * 3 / 2;
double result = radius * 3.14 * 0.1;
double profit = salesPrice - purchasePrice * 0.8;
int result = 2 + 3 * 4 + 10 / 5 * 2 – 1 + ;
int modulus = 10 % 3;
```



### Exercise 2

Convert 100 Fahrenehit to the same amount in Celcius



### Exercise 3

Print the following message, with the same format:

````
Software development
The best subject ev-er
Learning ”Java” is the most fun you can have
2 + 2 = 5;
````



### Exercise 4

Compute and print the result of `(9.5 * 4.5 - 2.5 * 3) / (45.5 - 3.5)`



### Exercise 5

A mile is 1.609 kilometers. Compute the result of 19 kilometers



### Exercise 6

Write variables to represent a rectangle:

- Width of 5.5

- Height of 8.5

Compute the area and the perimeter of the rectangle and print the results



### Exercise 7

Write a variable to represent a circle

- Radius of 16

Compute the area & perimeter of the circle and print the results.





## Homework

1. Skriv en klasse der hedder Kage, med en main-metode, gem, compiler og kør (intet sker!). 

2. Gå på nettet og find en kageopskrift – frit valg af yndlingskage 

3. Lav en variabel for hver af ingredienserne i kagen, med et passende navn og type (fx `int gramSugar`,  `int teaspoonsVanilla` eller `int numberOfEggs`).  

4. Tildel variablene den værdi der er i opskriften (fx `int gramFlour = 250;`) 

5. Udskriv hver af variablene pænt ovenover hinanden så det ligner en opskrift, a la: 

```
Sukker 200 g
Mel 250 g
```



6. Lav en variabel der hedder `totalIngredientsGrams`. I alle efterfølgende opgaver laver du variable efter behov, som du selv navngiver meningsfuldt. 

7. Regn ud hvor meget alle ingredienser i kagen vejer tilsammen (hvis det er skefulde, så søg på nettet hvor meget en skefuld af ingrediensen ca. vejer, eller gæt!) og tildel denne værdi til `totalIngredientsGrams`. 

8. Udskriv variablen `totalIngredientsGrams`, samt en lille forklaring på hvad tallet betyder (fx ”Ingredienserne til kagen vejer 740 gram”, hvor 740 er værdien af variablen). 

9. Vi regner med at en færdigbagt kage vejer 10 % mindre end ingredienserne – hvor meget vejer den færdige kage? Udskriv resultatet af beregningen. 

10. Gå på nettet og find en energifordeling for hver af ingredienserne (dvs hvor mange gram protein, kulhydrat osv. pr 100 g, og hvor mange kalorier ). 

11. Udregn og udskriv hvor mange gram protein der er i hver ingrediens i den mængde kagen indeholder, med en lille forklaring, som fx `Protein fra æg: 23 g`

12. Udskriv hvor mange gram protein der samlet er i kagen. 

13. Find energifordelingstabellen igen, og beregn hvor mange kalorier der er i hver ingrediens i kagen, i den mængde der er brugt (kalorier i tabellen er typisk angivet i kalorier pr 100 gram). Udskriv resultatet af beregningen, fx ”Energi fra sukker: 146 kcal”. 

14. Hvor mange kalorier er der i alt i kagen? Udskriv resultatet af beregningen. 

15. Søg på nettet hvor meget hver ingrediens koster (fx en bakke med 10 æg, 22 kr). Beregn pris pr ingrediens i den mængde der bruges i kagen (fx giver 2 æg 4,4 kr). Beregn kagens samlede pris og udskriv resultatet. 





**HVORNÅR SKAL VI SNAKKE SCOPE??? Loops, conditionals, methods**