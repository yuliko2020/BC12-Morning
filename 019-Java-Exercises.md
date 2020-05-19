# Задачи на закрепление всех основных конструкций. Пауза перед массивами

1. The parameter weekday is true if it is a weekday, and the parameter vacation is true if we are on vacation. We sleep in if it is not a weekday or we're on vacation. Return true if we sleep in.
    ```
    sleepIn(false, false) → true
    sleepIn(true, false) → false
    sleepIn(false, true) → true
    ```
2. Given an int n, return the absolute difference between n and 21, except return double the absolute difference if n is over 21.
    ```
    diff21(19) → 2
    diff21(10) → 11
    diff21(21) → 0
    ```
3. Given an int n, return true if it is within 10 of 100 or 200. Note: Math.abs(num) computes the absolute value of a number.
   ```
   nearHundred(93) → true
   nearHundred(90) → true
   nearHundred(89) → false
   ```
4. Given a non-empty string and an int n, return a new string where the char at index n has been removed. The value of n will be a valid index of a char in the original string (i.e. n will be in the range 0..str.length()-1 inclusive).
    ```
    missingChar("kitten", 1) → "ktten"
    missingChar("kitten", 0) → "itten"
    missingChar("kitten", 4) → "kittn"
    ```
5. Given a string, take the last char and return a new string with the last char added at the front and back, so "cat" yields "tcatt". The original string will be length 1 or more.
    ```   
   backAround("cat") → "tcatt"
   backAround("Hello") → "oHelloo"
   backAround("a") → "aaa"
   ```
6. Given a string, return true if the string starts with "hi" and false otherwise.
    ```
    startHi("hi there") → true
    startHi("hi") → true
    startHi("hello hi") → false
    ```
7. We'll say that a number is "teen" if it is in the range 13..19 inclusive. Given 3 int values, return true if 1 or more of them are teen.
    ```
    hasTeen(13, 20, 10) → true
    hasTeen(20, 19, 10) → true
    hasTeen(20, 10, 13) → true
    ```
8. Return true if the given string begins with "mix", except the 'm' can be anything, so "pix", "9ix" .. all count.
    ```
    mixStart("mix snacks") → true
    mixStart("pix snacks") → true
    mixStart("piz snacks") → false
    ```
9. Given 2 int values, return whichever value is nearest to the value 10, or return 0 in the event of a tie. Note that Math.abs(n) returns the absolute value of a number.
    ```
    close10(8, 13) → 8
    close10(13, 8) → 8
    close10(13, 7) → 0
    ```
10. Return true if the given string contains between 1 and 3 'e' chars.
    ```
    stringE("Hello") → true
    stringE("Heelle") → true
    stringE("Heelele") → false
    ```
11. Given a non-empty string and an int N, return the string made starting with char 0, and then every Nth char of the string. So if N is 3, use char 0, 3, 6, ... and so on. N is 1 or more.
    ```
    everyNth("Miracle", 2) → "Mrce"
    everyNth("abcdefg", 2) → "aceg"
    everyNth("abcdefg", 3) → "adg"
    ```
12. We have two monkeys, a and b, and the parameters aSmile and bSmile indicate if each is smiling. We are in trouble if they are both smiling or if neither of them is smiling. Return true if we are in trouble.
    ```
    monkeyTrouble(true, true) → true
    monkeyTrouble(false, false) → true
    monkeyTrouble(true, false) → false
    ```
13. We have a loud talking parrot. The "hour" parameter is the current hour time in the range 0..23. We are in trouble if the parrot is talking and the hour is before 7 or after 20. Return true if we are in trouble.
    ```
    parrotTrouble(true, 6) → true
    parrotTrouble(true, 7) → false
    parrotTrouble(false, 6) → false
    ```
14. Given 2 int values, return true if one is negative and one is positive. Except if the parameter "negative" is true, then return true only if both are negative.
    ```
    posNeg(1, -1, false) → true
    posNeg(-1, 1, false) → true
    posNeg(-4, -5, true) → true
    ```
15. Given a string, return a new string where the first and last chars have been exchanged.
    ```
    frontBack("code") → "eodc"
    frontBack("a") → "a"
    frontBack("ab") → "ba"
    ```
16. Return true if the given non-negative number is a multiple of 3 or a multiple of 5. Use the % "mod" operator -- see Introduction to Mod
    ```
    or35(3) → true
    or35(10) → true
    or35(8) → false
    ```
17. Given two temperatures, return true if one is less than 0 and the other is greater than 100.
    ```    
    icyHot(120, -1) → true
    icyHot(-1, 120) → true
    icyHot(2, 120) → false
    ```
18. We'll say that a number is "teen" if it is in the range 13..19 inclusive. Given 2 int values, return true if one or the other is teen, but not both.
    ```    
    loneTeen(13, 99) → true
    loneTeen(21, 19) → true
    loneTeen(13, 13) → false
    ```
19. Given a string, return a string made of the first 2 chars (if present), however include first char only if it is 'o' and include the second only if it is 'z', so "ozymandias" yields "oz".
    ```
    startOz("ozymandias") → "oz"
    startOz("bzoo") → "z"
    startOz("oxx") → "o"
    ```
20. Given 2 int values, return true if they are both in the range 30..40 inclusive, or they are both in the range 40..50 inclusive.
    ```
    in3050(30, 31) → true
    in3050(30, 41) → false
    in3050(40, 50) → true
    ```
21. Given two non-negative int values, return true if they have the same last digit, such as with 27 and 57. Note that the % "mod" operator computes remainders, so 17 % 10 is 7.
    ```
    lastDigit(7, 17) → true
    lastDigit(6, 17) → false
    lastDigit(3, 113) → true
    ```