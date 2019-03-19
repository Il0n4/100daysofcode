# log of 100daysofcode



-template-

## Day X: /19

**Today's Progress:** 

**Thoughts:** 

**Link to work:** 



## Day 1: 18/03/19


**Today's Progress:** set up log, set up document, re-activate Account for tutorials RUBY
* commenting #, =begin =end, \ 
* puts - die nächste Ausgabe erfolgt in neuer Zeile, print
* principle of variables
* math - Hierachie: Punkt vor Strich
* parallel assignment
* Zeilenumbruch \n




**Thoughts:** Wiederholung des Moduls dauerte am Ende eine Stunde. 

**Link to work:** https://code.sololearn.com/coLyd90VY8g6/#rb


## Day 2: 19/03/19

**Today's Progress:** 
* **boolean values** - in Ruby nur true oder false (2 Möglichkeiten) Only true and false are Booleans. nil is not a Boolean. 0 is not a Boolean. The string "Hello" is not a Boolean. However, in a context where a Boolean is expected, Ruby evaluates them as Boolean (truthy and falsey).
* Vergleich zweier Variablen mit **==, ungleich  !=**
  There is also the **.eql? method**, which results in true only if both arguments have the same type and equal values.
  For example:
  puts 3 == 3.0 # true 
  but
  puts 3.eql?(3.0) # false
* größer, kleiner Prinzip funktioniert auch mit strings - Vergleich basiert auf alphabetischer Reihenfolge
* **if** statement: The end keyword is required to indicate the end of the if; es können mehrere Konditionen miteinander verknüpft werden. 
  if a<7 
      puts "Yes" 
  end 
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



**Thoughts:** 

**Link to work:**


## Day 3: 20/03/19

**Today's Progress:** 

**Thoughts:** 

**Link to work:** 

