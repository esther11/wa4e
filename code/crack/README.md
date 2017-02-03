The Reverse Hash Application
============================
This application is adapted from Dr. Charles Sevenrance's
two-lower-case-character cracker.
You can play with his original application at:
http://www.wa4e.com/code/crack

This application uses a very simple brute force attack to 
"reverse" an MD5 hash.  It is really not reversing the hash
at all as that would be impossible.  Instead it knows that 
the original pre hash text was a four digit string with 
exactly four characters.

So the application uses two nested loops and tests all 
10*10*10*10 combinations of four numbers, and computes the
hashes of those values and checks to see if the computed hash
matches.

This is a lesson in how easy it is to crack short passwords
with limited numbers.  While this works well to crack 
very short passwords it is not practical as password 
length grows.