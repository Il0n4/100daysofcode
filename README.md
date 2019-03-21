# log of 100DaysOfCode_Ruby





## Day 1: 18/03/19 - Basic Concepts


**Today's Progress:** set up log, set up document, re-activate Account for tutorials RUBY
* commenting #, =begin =end, \ 
* puts - die nächste Ausgabe erfolgt in neuer Zeile, print
* principle of variables
* math - Hierachie: Punkt vor Strich
* parallel assignment
* Zeilenumbruch \n




**Thoughts:** Wiederholung des Moduls dauerte am Ende eine Stunde. 

**Link to work:** https://code.sololearn.com/coLyd90VY8g6/#rb


## Day 2: 19/03/19 - Control Structures

**Today's Progress:** 
### Control Strucures
* **boolean values** - in Ruby nur true oder false (2 Möglichkeiten) Only true and false are Booleans. nil is not a Boolean. 0 is not a Boolean. The string "Hello" is not a Boolean. However, in a context where a Boolean is expected, Ruby evaluates them as Boolean (truthy and falsey).
* Vergleich zweier Variablen mit **==, ungleich  !=**
  There is also the **.eql? method**, which results in true only if both arguments have the same type and equal values.</br>
  For example:</br>
  puts 3 == 3.0 # true </br>
  but</br>
  puts 3.eql?(3.0) # false</br>
* größer, kleiner Prinzip funktioniert auch mit strings - Vergleich basiert auf alphabetischer Reihenfolge
* **if** statement: The end keyword is required to indicate the end of the if; es können mehrere Konditionen miteinander verknüpft werden. </br>
  if a<7 </br>
      puts "Yes" </br>
  end </br>
  Conditions können ineinander verschachtelt sein - if im if wird erst dann beachtet, wenn die erste Ebene erfüllt wird. Jedes      if benötigt in eigenes end.
  else ist Teil des if Statements und somit eingebettet und braucht daher kein eigenes end
* **elsif - nur wenn diese Aussage nicht stimmt, dann**
* **unless** - Gegenteil von if, wird nur ausgeführt, wenn Statement falsch ist.
This code before the if executes only if the condition evaluates to true. The code before the unless executes only if the condition is false.
* **logical operators** - um mehr als ein Kriterium zu testen.  **and (&&), or (||), not (!)** (können theoretisch auch ausgeschrieben verwendet werden) 
**or (||)** - beide Aussagen oder mindestens eine Aussage muss wahr sein, damit das Statement als true ausgewertet wird 
You can chain together multiple conditions with the logical operators to check for multiple conditions. Parentheses can be used to group together separate conditions for clarity and to control the order of operations. For example:
(a>b && b < 100) || (a<b && b > 100)
* **case statement** kombiniert mehrere if/else/ifelse, verwendet **when**, parallel testing - zwischen den Werten ein Beistrich
* Case statements allow us to more easily control program flow. If statements should always be used to determine if a conditional is true, and case statements are for when you need to make different decisions based on a value.
* **loops** are used to execute the same block of code a specified number of times.
The **while** loop executes a block of code while its **condition is true**.
The **until** loop is the opposite of a while loop: it will run while its condition is **false**.



**Thoughts:** Die Funtkionen waren einfacher als gedacht. Die Syntax ist noch immer gut klar und übersichtlich <3. unless und elsif sind so Dinge wo ich aufpassen muss, mir nicht falsche Eselsbrücken zu merken.

**Link to work:** https://code.sololearn.com/coLyd90VY8g6/#rb


## Day 3: 20/03/19 - Control Structures und Collections

**Today's Progress:** 
### Control Structures 
* **Ranges** sind Sequenzen von Zahlen. 
**to_a** method is used to convert a range to an array. </br>
c = ("a".."d").to_a</br>
puts c # [a, b, c, d]</br>
''..'' and ''...'' sind die Kommandos. **..** inkludiert alle Werte, **...** schließt den angeführten Maximalwert aus. - funktioniert nicht rückwärts
* **for Loops** füllen eine leere Variable einzeln mit einer Sequenz von Werten </br>
for i in (1..10)</br>
  puts i</br>
end</br>
The for loop is a useful statement when you need to loop over a specific set of values, for example, a range.
The for loop consists of an empty variable and a range. At each iteration of the loop, the empty variable will be assigned the corresponding element of the range.
**The for loop executes a block of code once for each element in the range.**
* **break** statement can be used to stop a loop. </br>
for i in 1..5</br>
  break if i > 3</br>
  puts i</br>
end</br>
* **next** kann mit **for Loop** kombiniert werden und lässt einen Wert überspringen. **redo** lässt eine Iteration des Loops wiederholen, **retry** lässt Loop nochmals von Anfang starten.
* **loop do** It allows code to execute until a break condition is achieved.If we do not include a break condition, the loop will run forever.

### Collections
* **arrays** ist eine Liste nummerierter Items. items = ["Apple", "Orange", "Banana"] - Das array heißt **items** und beinhaltet 3 String. puts items [0] #gibt Apple aus. items Werte können manuell überschrieben werden. A negative index is assumed relative to the end of the array. For example, an index of -1 indicates the last element of the array, -2 is the next to last element in the array, and so on.
Arrays können **alle Formen von Elementen** enthalten.
* zum array hinzufügen: mit **<<** wird ein Element an die letzte Stelle hinzugefügt, **push** fügt Element am Ende des arrays hinzu **arr.push(8)**, **insert** fügt ein Element an einer beliebigen Stelle ein - **arr.insert(2, 8)** #an zweiter Stelle das Element "8"
* Entfernen von Werten mit **pop** - entfernt das letzte Element der Reihe </br>
**arr = [1, 2, 3]</br>
arr.pop**
print arr # [1, 2]</br>
**delete_at** ermöglicht es eine spezifische Position auszuwählen die entfernt wird - </br>
**arr = [2, 4, 6, 8]</br>
arr.delete_at(2)**</br>
print arr # [2, 4, 8]</br>

**Thoughts:** 
Arrays und Logiken machen Spaß. Tolle Gedankenpuzzles. Spannend wird dann der Weg, weg von den isolierten konkreten Rätsellösung hin zur Anwendung.

**Link to work:** 
https://code.sololearn.com/coLyd90VY8g6/#rb

## Day 4: 21/03/19

**Today's Progress:** 
* **arrays kann man miteinander kombinieren/addieren/subtrahieren** aber auch multiplizieren. </br>
a = [1, 2, 3]</br>
b = [4, 5]</br>

res = a + b</br>
print res # [1, 2, 3, 4, 5]</br>

* **boolsche Funktionen** mit **&** werden nur Elemente agerufen, die beide arrays vereinen, mit **|** nur jene Elemente, die nur in je einem array vorkommen.
* **reverse method** kehrt die Reihenfolge der Elemente um. Entweder so angewandt </br>
arr = [5, 3, 8]</br>
res = arr.reverse</br>
print res # [8, 3, 5]</br>

oder: </br>
arr = [1, 2, 3]</br>
print arr.reverse!</br>
(ohne dem Rufzeichen, wird die umgekehrte Abfolge nicht gespeichert und wird nur ein Mal abgerufen)

**array.length or array.size** returns the number of elements in array.</br>
**array.sort** returns a new array with the elements sorted</br>
**array.uniq** returns a new array with duplicate values removed from array.</br>
**array.uniq!** removes duplicates in place.</br>
**array.freeze** safeguards the array, preventing it from being modified.</br>
**array.include?(obj)** returns true if obj is present in array, false otherwise.</br>
**array.min** returns the element with the minimum value.</br>
**array.max** returns the element with the maximum value.</br>
* **hashes** A hash is created with comma separated keys and values inside curly brackets: </br>
ages = { "David" => 28, "Amy"=> 19, "Rob" => 42 } </br>
puts ages["Amy"] </br>
Compared with arrays, hashes have one significant advantage: they can use any object as an index, even an array. For example: { [1,"jan"] => "January" } </br>
es können auch Symbole für das Abrufen von Hashes verwendet werden a = :id - spart for allem Speicher, weil es nur einmal abgerufen wird.</br>
**hash.delete(key**) removes the key-value pair from hash by key. </br>
**hash.key(value)** returns the key for the given value in hash, nil if no matching value is found. </br>
**hash.invert** creates a new hash, reversing keys and values from hash; that is, in the new hash, the keys from hash become values and values become keys. </br>
**hash.keys** returns a new array with keys from hash. </br>
**hash.values** returns a new array containing all the values of hash. </br>
**hash.length** returns the length of hash as an integer. </br>

* 



# outputs 19

**Thoughts:** 

**Link to work:** 


## Day 5: 22/03/19

**Today's Progress:** 

**Thoughts:** 

**Link to work:** 


## Day 6: 23/03/19

**Today's Progress:** 

**Thoughts:** 

**Link to work:** 


## Day 7: 24/03/19

**Today's Progress:** 

**Thoughts:** 

**Link to work:** 


## Day 8: 25/03/19

**Today's Progress:** 

**Thoughts:** 

**Link to work:** 


## Day 9: 26/03/19

**Today's Progress:** 

**Thoughts:** 

**Link to work:** 


## Day 10: 27/03/19

**Today's Progress:** 

**Thoughts:** 

**Link to work:** 


## Day 11: 28/03/19

**Today's Progress:** 

**Thoughts:** 

**Link to work:**


## Day 13: 28/03/19

**Today's Progress:** 

**Thoughts:** 

**Link to work:**


-template-

## Day X: /19

**Today's Progress:** 

**Thoughts:** 

**Link to work:** 



