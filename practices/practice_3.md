1. Create a list called "lista" with the elements "red", "white", "black"
```Scala
val list = List("red", "white", "black")
print(list)
```

2. Add 5 more items to "list" "green" ,"yellow", "blue", "orange", "pearl"
```Scala
list = list :+ "green" :+"yellow":+ "blue":+ "orange":+ "pearl"
print(list)
```
3. Bring the items from "list" "green", "yellow", "blue"
```Scala
list slice(3,6)
print(list slice(3,6))
```

4. Create an array of numbers in the range 1-1000 in steps of 5 at a time
```Scala
val arr = Array.range(1,1000,5)
for(i<-arr){
    println(i)
}
```

5. What are the unique elements of the list List(1,3,3,4,6,7,3,7) use conversion to sets
```Scala
val list = List(1,3,3,4,6,7,3,7)
print(list.toSet.filter (i => list.indexOf (i) == list.lastIndexOf (i)))
```

6. Create a mutable map named names containing the following
     "Jose", 20, "Luis", 24, "Ana", 23, "Susana", "27"
     ```Scala
     val names = collection.mutable.Map(("Jose", 20), ("Luis", 24), ("Ana", 23),("Susana", 27))
    ```
   6 a . Print all the keys on the map
        
             ```Scala
            print(names.keys)
            ```
   6 b . Add the following value to the map("Miguel", 23)
             ```Scala
            names += ("Miguel" -> 23)
            print(names)  
            ```