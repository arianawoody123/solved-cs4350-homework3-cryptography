Download Link: https://assignmentchef.com/product/solved-cs4350-homework3-cryptography
<br>
Assignment  3The science of writing secret codes is called cryptography.  For thousands of years cryptography has made secret messages that only the sender and recipient could read, even if someone captured the messenger and read the coded message. A secret code system is called a cipher.   In cryptography, we call the message that we want to be secret the plaintext.  The plaintext could look like this:Hello there! The keys to the house are hidden under the flower pot.Converting the plaintext into the encoded message is called encrypting   the plaintext. The plaintext is encrypted into the ciphertext.       The ciphertext looks like random letters, and we cannot   understand what the original plaintext was just by looking at the ciphertext.

Here is the previous example encrypted into ciphertext:

Yvccf kyviv! Kyv bvpj kf kyv yfljv riv yzuuve leuvi kyv wcfnvi gfk.

But if you know about the cipher used to encrypt the message, you can decrypt the ciphertext back to the plaintext. (Decryption is the opposite of encryption.)

CS  4350  –  Unix  Systems  ProgrammingSpring  2020  –  Husain  Gholoom  –  Senior  Lecturer  in  Computer  Science   Page  2Many ciphers also use keys. Keys are secret values that let you decrypt ciphertext that was encrypted using a specific cipher.

Think of the cipher as being like a door lock. You can only unlock it with a particular key.

encrypt a message by taking each letter in the message (in cryptography, these letters are called symbols because they can be letters ( A-Z) ( a-z ), numbers( 0-9 ) , all symbols and replacing it with a “shifted” letter.

Using letters are , If you shift the letter A by one space, you get the letter B. If you shift the letter A by two spaces, you get the letter C. For example , this is a picture of some letters shifted over by three spaces.

<img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2020/05/161.png?w=980&amp;ssl=1" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2020/05/161.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript>

<img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2020/05/180.png?w=980&amp;ssl=1" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2020/05/180.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript>

The number of spaces you shift is the key in the Cipher. The example above shows the letter translations for the key 3. If you encrypt the plaintext “Howdy” with a key of 3, then:

• The “H” becomes “K”. • The letter “o” becomes “r”. • The letter “w” becomes “z”. • The letter “d” becomes “g”. • The letter “y” becomes “b”.

The ciphertext of “Howdy” with key 3 becomes “Krzgb”.

We will keep any non-letter characters the same. To decrypt “Krzgb” with the key 3, we go from the bottom boxes back to the top:

• The letter “K” becomes “H”. • The letter “r” becomes “o”. • The letter “z” becomes “w”. • The letter “g” becomes “d”. • The letter “b” becomes “y”.

You will write a C program that accept a message and the word encrypt , decrypt , or exit ( not case sensitive ) . The program then will do the following :

– Encrypt a message – Enter a key and :

a. Count and display number of capital letters , Small letters , digits and symbols in the message. b. Count number of characters in the message. c. Convert all small characters to capital letters and vice versa the display the message. d. Encrypt the original message e. Concatenate the encrypted message with the original message

– Decrypt a message – Enter a key and :

f. Count and display number of capital letters , Small letters , digits and symbols in the message. g. Count number of characters in the message. h. Convert all small characters to capital letters and vice versa then Display the message. i. Decrypt the original message. j. Concatenate the decrypted message with the original message

– Exit the program. Terminate the program.

Guideline:     1) Must  use  2  dimensional      array

2) key  number  must  be  between  1  and  93.  Anything   else  should  be  rejected.

3) Must  have  one  function  for  populating  the  2d       array  and  encrypting  the  message  and  all  other   functions.

4) Must  have  one  function  for  populating  the  2d   array  and  perform  the  decrypting  the  message   and  all  other  functions.

5) Must  pass  parameters  (  message  and  the  key  )  to   encrypt  or  decrypt  functions  .

6) Must  have  one  function  to  perform  the  validation   (  encrypt  ,  decrypt  ,  exit    and  the  key  number  ).

7) You    may  use  the  functions  that  are  provided  by  C     libraries  when  writing  this  program.

8)  Your    encryption  /    decryption    arrays  will  contain  the   following  characters  and  numbers  in  the  that  sequence.       A  –  Z      followed  by

a    -­    z    followed  by

0 -­    9        followed  by  the  following  symbols  in!   (exclamation  mark)

”   (Quotation  mark)

#   (Number  sign)

$   (Dollar  sign)

%   (Percent  sign)

&amp;   (Ampersand)

‘   (Apostrophe)

(   (round  brackets  or  parentheses)

)   (round  brackets  or  parentheses)

*   (Asterisk)

+   (Plus  sign)

,   (Comma)

-­‐ (Hyphen

.   (Full  stop,  dot)

/   (Slash)

:   (Colon)

;   (Semicolon)

&lt;   (Less-­than  sign)

=   (Equals  sign)

&gt;   (Greater-­than  sign;  Inequality)

?   (Question  mark)

@   (At  sign)

[   (square  brackets  or  box  brackets)

   (Backslash)

]   (square  brackets  or  box  brackets)

^   (Caret  or  circumflex  accent)

_   (underscore,  understrike,  underbar  or  lowline)

`   (Grave  accent)

{   (curly  brackets  or  braces)

-­   (vertical  bar,  vbar,  vertical  line  or  vertical  slash)

}   (curly  brackets  or  braces)

~   (Tilde;  swung  dash)

9  )    Must    place  the  following  information  on  top  left  of   the  first  page  of  your  assignment  as  comments