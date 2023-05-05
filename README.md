Download Link: https://assignmentchef.com/product/solved-cse111-lab-7
<br>
<h1>Task 1 (length())</h1>

Take a string as input from the user and print the length of the string (Remember that you cannot use any string class methods other than <em>toCharArray () </em>

<h1>Task 2 (charAt ())</h1>

Take a string as input from the user … then take a position <em>n</em> as input. “n” must be a valid index (which is an integer) less than the length of the String (Refer to Task1 on how to find the length). If n is invalid, then print “Invalid index”, otherwise print the character at that index/position.

<h1>Task 3 (startsWith ())</h1>

Take two Strings as input from the user … check if the second String is a prefix of the first String. If yes, print “true” else print “false”. Please ensure your program works for empty string inputs, as in it shouldn’t crash if the first or second or both of the strings are empty: P

<em>Remember that you cannot use any String class methods here, hence character by character comparison will be required.  </em>

<h1>Task 4 (endsWith () )</h1>

Take two Strings as input from the user … check if the second String is a suffix of the first String. If yes, print “true” else print “false”. Please ensure your program works for empty string inputs, as in it shouldn’t crash if the first or second or both of strings are empty: P

<h1>Task 5 (replaceFirst(char,char))</h1>

Take a String as input from the user. Then take in two more characters, oldChar and newChar (Read in as string and then convert to charArray and the save first index to a char variable). Replace the first occurrence of oldChar with newChar .. You are not permitted to modify the original character array …: P  <strong><u>Task 6 (replaceAll(char,char))</u></strong>

Take a String as input from the user. Then take in two more characters, oldChar and newChar (use the same method as Task 5). Replace all occurrences of oldChar with newChar ..you are not permitted to modify the original character array.

<strong> </strong>

<strong> </strong>

<h1>Task 7 (replaceLast(char,char))</h1>

Take a String as input from the user. Then take in two more characters, oldChar and newChar (use the same method as Task 5 and 6). Replace the last occurrence of oldChar with the newChar… you are not permitted to modify the original character array.




<strong><u>Task 8 (toLowerCase())</u></strong>

Take a String as input from the user. Convert all uppercase to lowercase.




<strong><u>Task 9 (toUpperCase())</u></strong>

Take a String as input from the user. Convert all lowercase to uppercase.

<strong><u>Task 10(equals())</u> </strong>

Take two Strings as input; if they are equal print “true”, else print “false”.

<strong><u>Task 11(equalsIgnoreCase()</u></strong>

Take two Strings as input; if they are equal regardless of the case, print “true”, else print “false”.

<h1>Task 12(compareTo())</h1>

Take two String as input. Print 0 if the Strings are equal. If the second string is lexicographically before the first one, returns a negative value, else returns a positive value. This task should behave the same as the compareTo() method in the String class, so look at the method definition in java doc for String.

<h1>Task 13(compareToIgnoreCase())</h1>

Take two String as input. Print 0 if the Strings are equal. If the second string is lexicographically before the first one, returns a negative value, else returns a positive value, regardless of the case. This task should behave the same as the compareToIgnoreCase() method in the String class, so look at the method definition in java doc for String.

<h1>Task 14(substring (int))</h1>

Take a String as input, and then an integer. If the integer is within the valid range, then find the substring starting with that integer till the end

<h1>Task 15(substring (int,int))</h1>

Take a String as input, and then two integers. If the integers are within the valid range, then find the substring starting with the character at the position of the first value and ending at the position of the last character.

<strong> </strong>

<strong> </strong>

<h1>Task 16(indexOf(char))</h1>

Take a String as input and then take a character as input (Same method as in Task 5/6). If the character exists in the String, print the location of the first occurrence of the character. If the character is not found, print -1.

<h1>Task 17(lastIndexOf(char))</h1>

Take a String as input and then take a character as input (Same method as in Task 5/6). If the character exists in the String, print the location of the last occurrence of the character. If the character is not found, print -1.

<h1>Task 18(indexOf(char,int))</h1>

Take a String as input and then a character and a number as input. Check the string from location indicated by the integer value, and print the location of the first occurrence of the character. If not found, print -1.

<h1>Task 19(lastIndexOf(char,start))</h1>

Take a String as input and then a character and a number as input. Check the string from location indicated by the integer value, and print the location of the last occurrence of the character. If not found, print -1.

<h1>Task 20(concat())</h1>

Take two strings as input and create a new character array that contains all characters of the first String followed by all characters of the second string. Print the new array and verify.











































<table width="0">

 <tbody>

  <tr>

   <td width="628"><strong>Lab 6 </strong><strong><u>Task 1</u></strong>Implement a <strong>MyString</strong> ADT.<strong>Elements</strong>An empty array of characters.<strong>Structure of the Elements</strong>A collection of characters. The characters in a string are in sequential (or linear) order – that is, the characters follow one after the other from the beginning of a string to its end. The character positions are numbered beginning with zero. A word, phrase, or sentence is some examples of strings.The characters in the instance of MyString will be stored in an array. <strong><u>CONSTRUCTORS</u></strong> <strong>MyString ( )</strong> Precondition:None.Postcondition:This is the default constructor. It creates an empty MyString object (just a MyString reference).Example:  … main ( ){ …MyString a = new MyString( );…} </td>

  </tr>

 </tbody>

</table>




<table width="0">

 <tbody>

  <tr>

   <td width="628"><strong>MyString (char[ ] charSeq)</strong>  Precondition:An array of characters charSeq will be given to create the constructor.Postcondition:It creates a new MyString object with a character sequence identical to the character array charSeq.Example: … main ( ){ …MyString a = new MyString(c); // c is a character array…} <strong>MyString (String str)</strong> Precondition:A String str will be given to create the constructor. Postcondition:This creates a new MyString object whose contents are equivalent to the String str. Example: … main ( ){ … </td>

  </tr>

 </tbody>

</table>




<table width="0">

 <tbody>

  <tr>

   <td width="628">MyString a = new MyString(“cat”);…} <strong><u>METHODS</u></strong><strong>[Some of the more commonly used String class methods-but you <u>CANNOT</u> use the String class methods here. You have to implement these methods on your own.]</strong> <strong>int length ( )</strong> Precondition:None. Postcondition:Returns the number of characters in the MyString object. <strong>char charAt ( int n )</strong> Precondition:“<em>n</em>” must be a valid String index (which is an integer) less than the length of the MyString object where you invoke this method (check the validity for <em>n</em>, e. g., <em>n</em> is an integer, non-negative and less than the length of the String). Postcondition:Returns the <em>n</em><sup>th</sup> character in the MySrting object.<strong>boolean startsWith (MyString prefix)</strong></td>

  </tr>

 </tbody>

</table>




<table width="0">

 <tbody>

  <tr>

   <td width="628"> Precondition:A MyString object <em>prefix</em> that is not null. Postcondition:Returns true if the MyString object starts with “<em>prefix</em>”. Otherwise, returns false. <strong>boolean startsWith (String prefix)</strong> Precondition:A String object <em>prefix</em> that is not null. Postcondition:Returns true if the MyString object starts with “<em>prefix</em>”. Otherwise, returns false. <strong>boolean endsWith(MyString suffix)</strong> Precondition:A MyString object <em>suffix</em> that is not null. Postcondition:Returns true if the MyString object ends with “<em>suffix</em>”. Otherwise, returns false. <strong>boolean endsWith(String suffix)</strong> Precondition:A String object <em>suffix</em> that is not null.


    <table width="0">

     <tbody>

      <tr>

       <td width="628"> Postcondition:Returns true if the MyString object ends with “<em>suffix</em>”. Otherwise, returns false. <strong>MyString replaceFirst(char oldChar, char newChar)</strong> Precondition:Two valid characters “<em>oldChar</em>” and “<em>newChar</em>”.Postcondition: Returns a new MyString resulting from replacing the first occurrence of the <em>oldChar</em>in this string with the <em>newChar</em>.<strong>MyString replaceAll(char oldChar, char newChar)</strong> Precondition:Two valid characters “<em>oldChar</em>” and “<em>newChar</em>”. Postcondition: Returns a new MyString resulting from replacing all occurrences of the <em>oldChar</em> in this string with the <em>newChar</em>.<strong>MyString replaceLast(char oldChar, char newChar)</strong> Precondition:Two valid characters “<em>oldChar</em>” and “<em>newChar</em>”. Postcondition:Returns a new MyString resulting from replacing the last occurrence of the <em>oldChar</em>in this string with the <em>newChar</em>.<h2>MyString toLowerCase ( )</h2> Precondition:None. Postcondition:Returns the invoking MyString object if all its characters are already lowercase. Otherwise, returns a new MyString object in which all characters have been converted to lowercase. <h2>MyString toUpperCase ( )</h2> Precondition:None. Postcondition:Returns the invoking MyString object if all its characters are already uppercase. Otherwise, returns a new String object in which all characters have been converted to uppercase.<h2>boolean equals ( MyString rightStr )</h2> Precondition:A MyString object <em>rightStr</em> and <em>rightStr</em> is not null. (check validity of <em>rightStr</em>) Postcondition:


        <table width="0">

         <tbody>

          <tr>

           <td width="628">It returns true if the invoking MyString object and rightStr have the same value (i.e, identical). Otherwise, returns false. <strong>boolean equalsIgnoreCase ( MyString rightString )</strong> Precondition:A MyString object <em>rightStr</em> and <em>rightStr</em> is not null. (check validity of <em>rightStr</em>) Postcondition:It returns true if the invoking MyString object and <em>rightString</em> are identical not considering the case (uppercase or lowercase) to each character. Otherwise, returns false.<strong>int compareTo ( MyString str )</strong> Precondition:A MyString object <em>str</em>. <em>Str</em> is not null. (check validity of <em>str</em>) Postcondition:Returns a value indicating if the invoking MyString object is lexicographically before (returns a negative value), equal to (returns 0), or after (returns a positive value) the MyString str. Example: … main ( ){ … a.MyString(b); // a and b are instances of MyString Class</td>

          </tr>

         </tbody>

        </table>


        <table width="0">

         <tbody>

          <tr>

           <td width="628">…} [This method returns 0 if a and b are identical, returns negative value if a&lt;b and returns positive value if a &gt; b.] <strong>int compareTo (String str )</strong> Precondition:A String object <em>str</em> and <em>Str</em> is not null. (check validity of <em>str</em>) Postcondition:Returns a value indicating if the invoking MyString object is lexicographically before (returns a negative value), equal to (returns 0), or after (returns a positive value) the String str. Example: … main ( ){ …a.MyString(“book”); // a is an instances of MyString Class…}<strong>int compareToIgnoreCase(MyString str)</strong> Precondition:A MyString object <em>str</em> where <em>str</em> not null (check validity of <em>str</em>). </td>

          </tr>

         </tbody>

        </table>


        <table width="0">

         <tbody>

          <tr>

           <td width="628">Postcondition:Returns a value indicating if the invoking MyString object is lexicographically before (returns a negative value), equal to (returns 0), or after (returns a positive value) the MyString <em>str</em>, if both are not case sensitive.<strong>int compareToIgnoreCase(String str)</strong> Precondition:A String object <em>str</em> where <em>str</em> not null (check validity of <em>str</em>). Postcondition:Returns a value indicating if the invoking MyString object is lexicographically before (returns a negative value), equal to (returns 0), or after (returns a positive value) the String <em>str</em>, if both are not case sensitive.<strong>MyString substring (int start)</strong> Precondition:The argument “<em>start</em>” must be a nonnegative String index and is not greater than the length of the MyString object. Postcondition:Returns a new MyString object containing the substring from the index “<em>start</em>” to the end of the invioking MyString object. <strong>MyString substring (int start, int end)</strong> Precondition:</td>

          </tr>

         </tbody>

        </table>


        <table width="0">

         <tbody>

          <tr>

           <td width="628">The “<em>start</em>” and “<em>end</em>” must be nonnegative String indices and are not greater than the length of the MyString. Moreover, “<em>start”</em> must not be greater than “<em>end”</em>. (check validity) Postcondition:Returns a new MyString object containing the substring starting at position “<em>start</em>” through position “<em>end</em>” of the invoking MyString object. [Here, a total of “<em>end</em> –<em>start</em> + 1” characters are copied into the new MyString object].<strong>int indexOf (char ch)</strong> Precondition:A character “<em>ch</em>”, where “<em>ch</em>” is not null. (check validity of “ch”) Postcondition:Returns the position within the invoking MyString object at which the first (the leftmost) occurrence of the character “<em>ch</em>” is located. If “<em>ch</em>” is not found, -1 is returned. <strong>int lastIndexOf (char ch)</strong> Precondition:A character “<em>ch</em>”, where “<em>ch</em>” is not null. (check validity of “<em>ch</em>”) Postcondition:Returns the index within this Mystring object of the last (rightmost) occurrence of the specified character “ch”. If “ch” is not found, -1 is returned.<strong>int indexOf ( char ch, int start )</strong> </td>

          </tr>

         </tbody>

        </table>


        <table width="0">

         <tbody>

          <tr>

           <td width="628">Precondition:A character “<em>ch</em>”, where “<em>ch</em>” is not null. (check validity of “<em>ch</em>”) and the starting position “<em>start</em>” to start searching within the MyString object. Postcondition:Returns the position within the invoking MyString object at which the first (the leftmost) occurrence of the character “<em>ch</em>” is located, with “start” specifying the position at which to begin the search. If “<em>ch</em>” is not found, then -1 is returned. <strong>int lastIndexOf (char ch, int start)</strong> Precondition:A character “<em>ch</em>”, where “<em>ch</em>” is not null. (check validity of “<em>ch</em>”) and the starting position “<em>start</em>” to start searching within the MyString object. Postcondition: Returns the index within this string of the last occurrence of the specified character, searching from the position “<em>start</em>”. If “<em>ch</em>” is not found, -1 is returned.<strong>int indexOf ( MyString str)</strong> Precondition:A MyStrjng object <em>str</em> that is not null. (check validity of <em>str</em>) Postcondition:Returns the position within the invoking MyString object at which the first (the leftmost) occurrence of the MyString str is located. If “<em>str</em>” is not found, then -1 is returned.</td>

          </tr>

         </tbody>

        </table>


        <table width="0">

         <tbody>

          <tr>

           <td width="628"> <strong>int lastIndexOf (MyString str)</strong> Precondition:A MyStrjng object <em>str</em> that is not null. (check validity of <em>str</em>) Postcondition:Returns the position within the invoking MyString object at which the last (the righttmost) occurrence of the MyString str is located. If “<em>str</em>” is not found, -1 is returned. <strong>int indexOf (String str)</strong> Precondition:A Strjng object <em>str</em> that is not null. (check validity of <em>str</em>) Postcondition:Returns the position within the invoking MyString object at which the first (the leftmost) occurrence of the String <em>str</em> is located. If “<em>str</em>” is not found, then -1 is returned.<strong>int lastIndexOf (String str)</strong> Precondition:A Strjng object <em>str</em> that is not null. (check validity of <em>str</em>) Postcondition:Returns the position within the invoking MyString object at which the last (the rightmost) occurrence of the String <em>str</em> is located. If “<em>str</em>” is not found, -1 is returned.</td>

          </tr>

         </tbody>

        </table>


        <table width="0">

         <tbody>

          <tr>

           <td width="628"><strong>MyString concat (MyString str)</strong> Precondition:A MyString object <em>str</em>. The object <em>str</em> is not null (check validity of <em>str</em>). Postcondition: This Returns a new MyString object that containins the MyString object that invoked this method with <em>str</em>, added to it at the end. Example: string1.concat(string2);// string 1 and string2 are instances of MyString class.<strong>MyString concat (char[ ] charSeq)</strong> Precondition:A character array. Postcondition: This Returns a new MyString object that containins the MyString object that invoked this method with <em>charSeq</em>, added to it at the end. <strong>MyString concat (String str)</strong></td>

          </tr>

         </tbody>

        </table> Precondition:A String <em>str</em>. The object <em>str</em> is not null. (check validity of <em>str</em>) Postcondition: This Returns a new MyString object that containins the MyString object that invoked this method with a string <em>str</em>, added to it at the end.      </td>

      </tr>

     </tbody>

    </table></td>

  </tr>

 </tbody>

</table>