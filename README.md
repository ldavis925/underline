# underline

This is a mass file renaming tool:

Syntax:

Normalize all of the file names ending with '.ext'

Sometimes it's worth while to run this command twice, or until it produces no output

_ .ext


All files with 'REMOVE_THIS_STRING' and 'THIS_STRING_TOO' in them will have those strings removed... you can supply an unlimited number of arguments to the "remove" syntax:

_ .ext REMOVE_THIS_STRING THIS_STRING_TOO

Substitute syntax (similar to perl s///)  Note that the "substitute" only modifies the first occurrance, you can stack them to do it multiple times

_ .ext s/substitute-this/for-this/

_ .ext s/_S01/_-_S01/

_ .ext s/_S01/_-_S01/ s/episode/E/


You can combine remove-string and substitute together as well

_ .mp3 DISCO_OF_THE_70S s/_/_-_/

