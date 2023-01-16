redirection assignment content.
 notes go here (if I can remember to put them here.)

tail deafaults to last 10 lines.


cat, head, and tail can take multiple arguments, and will display the relevnet lines in sequence, without a newline between them.

" | " is used to feed the instructions of one thing into another.
for example cat fileName | head -n -6 | tail -n -4
will print all of fileName to head,which will prnt all of fileName except the heading 6 (because we aid minus 6) lines to tail, which will print all but the last 4 (because we negatived 4) lines of fileName.
Essentially, fileName without the first 6 or last 4.
positive (no + symbol) arugments in head/tail just print the first n lines instead