# cis-2500-assignment-1--dynamically-allocating-arrays-solved
**TO GET THIS SOLUTION VISIT:** [CIS*2500 Assignment 1- Dynamically Allocating Arrays Solved](https://www.ankitcodinghub.com/product/cis2500-intermediate-programming-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;115153&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CIS*2500 Assignment 1- Dynamically Allocating Arrays Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
&nbsp;

The question

Write a program that takes in a file of words (a regular text file with no punctuation) and prints out all the words from the file that start with ‘A’, all the words that start with ‘B’, etc.

How to write the program

For this assignment, the program has already been analyzed and broken down into the relevant functions (although you are free to create any other supporting functions that you please). Make sure that you create those functions exactly as specified below. In future assignments, you will be given more design latitude.

1. Copy the following function definition into your source code: int file_size(FILE *fp)

{ int sz = 0; fseek(fp, 0L, SEEK_END); sz = ftell(fp); rewind(fp); return sz; }

This function computes the file size (in bytes) of an opened file (see your CIS*1300 notes for opening and closing files).

2. Create a function read_words( ) that takes in one argument, a File pointer, and then reads in words from that file into an array of words.

§ You can assume that the longest word in English has 45 characters in it

(a disease called Pneumonoultramicroscopicsilicovolcanoconiosis)

o The maximum number of words that might be stored in the array of words can be computed from the file size (as opposed to assuming a maximum number as a constant).

§ As there can be no more words in a file then number of bytes in the file, use file_size(fp) to calculate the max number of words possibly in that file

§ note: this is an overestimate; for a single character to be a separate word you need a space or newline after the character … so the maximum word count is actually half the byte size of the file

o The word array should also hold a NULL pointer after the entered words to indicate the end of the word list. o The array of words, once created, should be returned from the function.

3. Create a void function called print_words( ) that takes a NULL terminated array of words and prints out the words, one word per line, stopping when it reaches the NULL pointer. o Make sure you handle the case of no words in the array.

4. Create a function called alphabetical_word_count( ) that takes in the array of words and counts how many words begin with the letter ‘a’ or ‘A’, how many words begin with the letter ‘b’ or ‘B’ etc.

o The results should be stored in a single array of int’s and returned from the function.

5. Create a void function called print_alphabetical_word_count( ) that prints out the array of integers and the letters that each count is associated with. o E.g.

A = 23, B = 12, C = 0, D = 42, … X = 0, Y = 0, Z = 1

6. Create a function called create_alphabetical_array( ) that takes two parameters, a NULL terminated array of words, and the array of starting-letter word counts as returned by the alphabetical_word_count( ) function. The function should:

o Create 26 arrays, each one to stores all the words that start with a particular letter

§ For example, one of the array of words will contain all of the words that start with ‘a’ or ‘A’.

§ There could be any number of words in a list. No maximums should be used.

§ The final element for each of these should be the NULL pointer (not the empty string or the character).

§ If there are no words that start with the letter being considered, the array of words should have one element in it, which should be set to the NULL pointer.

o The 26 arrays should be stored in an array called alphabetical_array, such that alphabetical_array[0] contains the array of all ‘a’ words, alphabetical_array[1] contains the list of all ‘b’ words etc.

§ This array should be the function’s return value

§ You can use this array to store the 26 arrays while they are being created. No need to have separate variable names for each of the 26 word arrays.

7. Create a void function called free_alphabetical_array( ) that takes in a single parameter of the same type and design as alphabetical_array and frees all of the memory in the array (remember to free the words first before freeing the array of words)

8. Create a void function called printWordsAlphabetically that prints out all of the words of alphabetical_array as follows

‘A’

apple Anna apple

‘B’

banana bounce

Basket

‘C’ car chase

castle

‘D’

There are no words that begin with the letter ‘d’

‘E’

elephant easy

etc.

hint: you should use the print_words( ) function that you wrote for step 3

9. Create a main function (in a different file from the other functions so that we can use your functions with our own main()) that uses the above functions to o read in a file called a1_words.txt stored in the same directory as the program o print out the words in the file in the original order, o print out the number of words that start with ‘A’, ‘B’ etc. o print out all the words that start with ‘A’, ‘B’, etc. o read in a second file called a1_moreWords.txt o print out the words in the file in the original order, o print out the number of words that start with ‘A’, ‘B’ etc. o print out all the words that start with ‘A’, ‘B’, etc.

make sure that all malloc’d memory is freed by the end of the program.
