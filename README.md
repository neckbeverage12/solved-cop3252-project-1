Download Link: https://assignmentchef.com/product/solved-cop3252-project-1
<br>
This assignment should help you gain practice with basic Java syntax using procedural programming, functions, arrays, and console I/O.

<h1>Task</h1>

Do the following three exercises each in a different file. Your filenames should be

<ul>

 <li>java</li>

 <li>java</li>

 <li>java</li>

</ul>

<strong>Each file should have a comment including your name at the top of the file. Each file should also have appropriate comments throughout the program.</strong>

To do the console input for these exercises, use the java.util.Scanner class. For random numbers in the last exercise, you may use the <a href="https://docs.oracle.com/javase/7/docs/api/java/util/Random.html">java.util.Random </a>class.

Declare any methods you write to be public and static. You may also use the java.lang.Math class if you need it. You may assume correct user input in these problems.

<h1>Exercise 1</h1>

Filename: Pi.java

Calculate the value of <em>π </em>from the infinite series:

<em>π </em>= 4 − 4<em>/</em>3 + 4<em>/</em>5 − 4<em>/</em>7 + 4<em>/</em>9 − 4<em>/</em>11 + <em>…</em>

Print a table that shows the value of <em>π </em>approximated by computing one term of the series, approximated by two terms, three terms, and so on. Use default precision for output (do <strong>not </strong>set any decimal precision).

Start by asking the user how many terms to compute to and then let the user enter the information. Use this to print a table of the first <em>N </em>terms of the series (where <em>N </em>is the data entered by the user). Assume the user’s input will be a non-negative integer. Try to match my sample output as closely as you can. Be aware that the default precision of System.out.print is different from that of System.out.printf, so if your precision does not match my output exactly, it is okay as long as you are using the default for whichever printing function you are using (I used System.out.printf).

<strong>Sample Run</strong>

(Sample user input is underlined)

Compute to how many terms of the series? <u>20 </u>terms            PI approximation

<ul>

 <li>000000</li>

 <li>666667</li>

 <li>466667</li>

 <li>895238</li>

 <li>339683</li>

 <li>976046</li>

 <li>283738</li>

 <li>017072</li>

 <li>252366</li>

 <li>041840</li>

 <li>232316</li>

 <li>058403</li>

 <li>218403</li>

 <li>070255</li>

 <li>208186</li>

 <li>079153</li>

 <li>200366</li>

 <li>086080</li>

 <li>194188</li>

 <li>091624</li>

</ul>

<h1>Exercise 2</h1>

Filename: Reverse.java

Write a static method called reverseDigits that takes a long integer value and returns that number with its digits reversed. For example, given the value 1459, the method should return the value 9541 as a long integer.

Write a main() method that enters a loop in which the user is prompted and allowed to enter any long integer (0 to exit the loop) and the reverseDigits method is used to compute and return the reversed number. Print this from the main routine.

You may assume the user inputs a positive integer. Try to match the sample run exactly.

<strong>Sample Run</strong>

(Sample user input is underlined)

Please enter a long integer (0 to quit): <u>123456</u>

The number reversed is: 654321

Please enter a long integer (0 to quit): <u>4837946852</u>

The number reversed is: 2586497384

Please enter a long integer (0 to quit): <u>2345678</u>

The number reversed is: 8765432

Please enter a long integer (0 to quit): <u>123456789012345678</u>

The number reversed is: 876543210987654321

Please enter a long integer (0 to quit): <u>234005700</u>

The number reversed is: 7500432 Please enter a long integer (0 to quit): <u>0 </u>Goodbye!

<h1>Exercise 3</h1>

Filename: DiceStats.java

Write a program that does the following:

<ol>

 <li>Ask the user to enter how many dice will constitute a roll (Some games require different numbers of dice per turn. Yahtzee takes 5, Monopoly takes 2, etc.).</li>

 <li>Ask the user to enter how many rolls they would like to simulate.</li>

 <li>Create and use an array to keep track of how many times each possible dice sum appears. Basically, it is a bunch of counters and how many you need depends on how many dice are rolled per ”turn.”

  <ul>

   <li>Hint: The idea is that this array is a frequency array like the example we went over in class (number 7.7 from the array lecture)</li>

   <li>Hint: You determine how many counters you will need based on the number of dice rolled per turn. The lowest possible total is all 1s, so the number of dice rolled. The highest possible total is all 6s, so it is (6 * number of dice). Use this to determine the size of your array.</li>

  </ul></li>

 <li>Use a loop to roll the specified number of dice the desired number of times (and calculate the sum of each roll). Use the array to keep track the number of times each possible sum appears.</li>

 <li>Display the results in a table with 3 columns:

  <ul>

   <li>the die total</li>

   <li>the number of times that total appeared</li>

   <li>the percentage of the total rolls that this sum appeared (print the percentage to 2 decimal places)</li>

  </ul></li>

</ol>

Try to match the sample runs as closely as possible. Since randomness is involved, the number of times each sum appears (and the matching percentages) will be different, but if you use the same number of dice they should be similar to the sample run values (if you roll 2 dice at a time, you should not get a sum of 12 8% of the time, for example). If you get unexpected values, you may want to try to run it a few more times to make sure you did not just get unlucky (as any distribution is theoretically possible).

<strong>Sample Run 1</strong>

(user input is underlined)

How many dice will constitute one roll? <u>2</u>

How many rolls? <u>100000</u>

Sum                  <em># of times                        Percentage</em>

<ul>

 <li>2741 74 %</li>

 <li>5540 54 %</li>

 <li>8404 40 %</li>

 <li>11228 23 %</li>

 <li>13835 84 %</li>

 <li>16662 66 %</li>

 <li>13827 83 %</li>

 <li>10989 99 %</li>

 <li>8538 54 %</li>

 <li>5480 48 %</li>

 <li>2756 76 %</li>

</ul>

<strong>Sample Run 2</strong>

(user input is underlined)

How many dice will constitute one roll? <u>4</u>

How many rolls? <u>100000</u>

Sum                  <em># of times                        Percentage</em>

<ul>

 <li>66 07 %</li>

 <li>312 31 %</li>

 <li>773 77 %</li>

 <li>1512 51 %</li>

 <li>2633 63 %</li>

 <li>4313 31 %</li>

 <li>6312 31 %</li>

 <li>8096 10 %</li>

 <li>9660 66 %</li>

 <li>10831 83 %</li>

 <li>11179 18 %</li>

 <li>10720 72 %</li>

</ul>

<table width="239">

 <tbody>

  <tr>

   <td width="191">16                  9654</td>

   <td width="48">9.65 %</td>

  </tr>

  <tr>

   <td width="191">17                  7938</td>

   <td width="48">7.94 %</td>

  </tr>

  <tr>

   <td width="191">18                  6158</td>

   <td width="48">6.16 %</td>

  </tr>

  <tr>

   <td width="191">19                  4406</td>

   <td width="48">4.41 %</td>

  </tr>

  <tr>

   <td width="191">20                  2658</td>

   <td width="48">2.66 %</td>

  </tr>

  <tr>

   <td width="191">21                  1613</td>

   <td width="48">1.61 %</td>

  </tr>

  <tr>

   <td width="191">22                  781</td>

   <td width="48">0.78 %</td>

  </tr>

  <tr>

   <td width="191">23                  304</td>

   <td width="48">0.30 %</td>

  </tr>

  <tr>

   <td width="191">24                 81</td>

   <td width="48">0.08 %</td>

  </tr>

 </tbody>

</table>

<h1>Compiling</h1>

Remember that the compile command is javac at the unix command prompt. Compile your code on linprog.cs.fsu.edu and run your program with the java command.


