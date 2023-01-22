readme content\n

when you go back to the first question, if there is no specific reply as to using the variable, just make it ((vaiable++)). it won't even need to double the variable used because hte for loop itself will reset it back to the next value in the number list

if an if statement is in a wihle loop, it will trigger before the while loop does. if you want something to happen after teh while loop does, make it trigger on the subsequent iteratin of while.

The for loop has two forms to choose from.
it  can be

"
for Variable in list
do
taskToBeDoneInvolvingThatVariable
done
"

or it can be c-style:

"
for ((variable=initialValue; variable binaryOperator endCondition; incriment variable))
do
taskIndependantOfThatVariable
done
"


that second one (c-style) can look like this

"
for ((counter=0;counter>=10; counter++))
do
echo "lol i'm repetitive"
done
"

any of the ocnditions can be left blank in the c-style, adn it will still run, with appropriate consequences.

If "break" (it's its own line) is read at any point within the foor loop (eevn if nested),  the entire For loop ends immediately.
- if "continue" is found, it instead ends the current iteration and moves onto the next

////////////// cut /////////////////
this one can be confusing when searchign to cut out cerrtain cahracters, but yo ucan do it.

when you do
ls | cut -d'deli' -f 2

taht means that in your ls, look for "deli", and anywhere there is one, follow it with a dividing line. the first "field" is the content before the first dividing line. teh secoind field is content between the first and second dividing line." "-f" is how you tell it which fields you want to print. in the above example, it prints field 2,because we put a 2 after it. we could say "-2" for 2 everything up to and incliuding field 2, or we could say "2-" for 2 and everything after it. "2-4" is "2 through 4".