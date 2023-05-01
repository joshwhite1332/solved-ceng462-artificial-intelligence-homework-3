Download Link: https://assignmentchef.com/product/solved-ceng462-artificial-intelligence-homework-3
<br>
<strong>1      Objectives</strong>

This assignment aims to assist you to expand your knowledge on First Order Predicate Logic.

<h2>2       Problem Definition</h2>

In this assignment, you are going to implement a function called theorem prover in python as a theorem prover for First Order Predicate Logic by using <em>Resolution Refutation </em>technique and <em>Set of Support </em>strategy with <em>Breadth-First </em>order. This function gets two lists of clauses, namely the list of base clauses and the list of clauses obtained from the negation of the theorem.

Your program has to eliminate

<ul>

 <li>tautologies</li>

 <li>subsumptions</li>

</ul>

The function detects whether the theorem is derivable or not. Then, it returns the result as a tuple. First element of this tuple will be <strong>“yes” </strong>or <strong>“no” </strong>according to derivability of the theorem. The second element will be:

<ul>

 <li><strong>list of resolutions </strong>which contribute to the proof of the theorem, if it is derivable.</li>

 <li><strong>an empty list</strong>, if the theorem is not derivable.</li>

</ul>

<h2>3      Specifications</h2>

<ul>

 <li>By the convention we follow in FOPL; variables, predicate and function names start with with a lower case letter, while the constants with an upper case letter.</li>

 <li>In the given clauses; “+” and “∼” signs will be used for disjunction and negation respectively.</li>

 <li>Each resolution in the return value must be given in “<em>&lt; clause</em>1 <em>&gt; </em>$ <em>&lt; clause</em>2 <em>&gt; </em>$ <em>&lt; resolvent &gt;</em>” form <strong>without using any space character</strong>.</li>

 <li>The “empty” string must be used for empty clause in the return value.</li>

</ul>

1

<h2>4        Sample Function Calls</h2>

<table width="673">

 <tbody>

  <tr>

   <td width="673"><em>&gt;&gt;&gt; </em>theorem_prover ([ ”p(A, f ( t ) )” , ”q(z)+˜p(z , f (B) )” , ”˜q(y)+r (y)” ] ,[ ”˜r (A)” ])( ’ yes ’ , [ ’˜r (A)$˜q(y)+r (y)$˜q(A) ’ , ’˜q(A)$q(z)+˜p(z , f (B) )$˜p(A, f (B) ) ’ , ’˜p(A, f (B) ) $p(A, f ( t ) )$empty ’ ])<em>&gt;&gt;&gt; </em>theorem_prover ([ ”p(A, f ( t ) )” , ”q(z)+˜p(z , f (B) )” , ”q(y)+r (y)” ] ,[ ”˜r (A)” ]) ( ’no ’ , [ ] )</td>

  </tr>

 </tbody>

</table>

<h2>5      Regulations</h2>

<ol>

 <li><strong>Programming Language: </strong>You must code your program in Python <strong>7</strong>. Your submission will be tested in inek machines. So make sure that it can be executed on them as below.</li>

</ol>

<table width="634">

 <tbody>

  <tr>

   <td width="397">Python 2.7.15+ ( default , Oct 7 2019 ,                                          17:39:04)[ GCC 7.4.0] on linux2Type ”help” , ”copyright” , ” credits ” or ” license ”<em>&gt;&gt;&gt; </em>import e1234567_hw3<em>&gt;&gt;&gt; </em>e1234567_hw3 . theorem_prover ( . . . )</td>

   <td width="31">for</td>

   <td width="207">more information .</td>

  </tr>

 </tbody>

</table>

<ol start="2">

 <li><strong>Implementation: </strong>You have to code your program by only using the functions in standard module of python. Namely, you <strong>cannot </strong>import any module in your program.</li>

 <li><strong>Late Submission: </strong>No late submission is allowed. No correction can be done in your codes after deadline.</li>

 <li><strong>Cheating: We have zero tolerance policy for cheating</strong>. People involved in cheating (any kind of code sharing and codes taken from internet included) will be punished according to the university regulations.</li>

 <li><strong>Discussion: </strong>You must follow the OdtuClass for discussions and possible updates on a daily basis.</li>

 <li><strong>Evaluation: </strong>Your program will be evaluated automatically using “black-box” technique so make sure to obey the specifications. A reasonable timeout will be applied according to the complexity of test cases in order to avoid infinite loops due to an erroneous code.</li>

</ol>


