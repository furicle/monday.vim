
created by
Stefan Karlsson
 
script type
utility
 
description
Monday.vim extends the normal-mode commands <ctrl-a> and <ctrl-x> so that they can be applied to the names of months and weekdays. For example, if you are standing on the word "July" and presses <ctrl-a>, the word is replaced by "August".

The script tries to preserve the case of the letters, and can handle the following three variants:

(1) All lower-case ("july" becomes "august").
(2) All upper-case ("JULY" becomes "AUGUST").
(3) First letter upper-case, the rest lower-case ("July" becomes "August").

Todo:

Only English is supported; although it's easy to add any word pairs you want, the script cannot yet handle words that have two or more possible successors/predecessors.  For example, the 4th month is called "April" in both English and Swedish, but its successor is called "May" and "Maj", respectively. So, if you add the Swedish months and then try to increment the word "April", the script won't be able to figure out which word ("May" or "Maj")  it should be replaced with.
 
install details
Just drop the script in your local plugin directory (e.g. ~/.vim/plugin).
 
