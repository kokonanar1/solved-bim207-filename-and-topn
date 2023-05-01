Download Link: https://assignmentchef.com/product/solved-bim207-filename-and-topn
<br>
<ul>

 <li>Your program takes two arguments: filename and topN</li>

 <li>You should read the given text file and preprocess the text according to following order: Tokenize the text by whitespace(not just space character, e.g. more than one space, tab, newline etc.), remove punctuations, and apply the lowercase.</li>

 <li>You are asked to calculate followings:</li>

</ul>

○ <strong>Average Term Length By Initial Character:</strong> For example, If your tokens are [”apple”,”banana”,”avocado”,”blueberry”], then your output should be like

a = 6  b = 7.5

○    <strong>Total Minimum Distance:</strong> For each term pair, calculate the following formula

<em>f</em>(<em>t</em><sub>1</sub>) * <em>f</em>(<em>t</em><sub>2</sub>)

1+<em>ln </em>∑ <em>d</em>(<em>t</em><sub>1</sub>,<em>t</em><sub>2</sub>)

where <em>f(t)</em>​ is the count of the term <em>t</em>​ in the text and <em>d(t</em>​ <sup>​</sup><em><sub>1</sub></em><sub>​</sub><em>,t</em><sup>​</sup><em><sub>2</sub></em><sub>​</sub><em>)</em> gives the minimum distance between <em>t</em>​ <sup>​</sup><em><sub>1</sub></em> and t​2 where <em>t</em>​ <sup>​</sup><em><sub>1</sub></em> is followed by <em>t</em>​ <sup>​</sup><em><sub>2</sub></em><sub>​</sub>. For example, If the text is

”aa bb cc aa cc dd bb” and <em>t</em>​ <sup>​</sup><em><sub>1</sub></em> = aa and <em>t</em>​ <sup>​</sup><em><sub>2</sub></em> = bb, then ∑<em>d</em>(<em>t</em><sub>1</sub>,<em>t</em><sub>2</sub>) = 1+3 = 4. You

should print only topN pairs according to the score.

<strong>Important</strong>​<strong> !</strong>

<strong>Make sure the following commands are running</strong> <strong>mvn clean package </strong>

<strong>java -jar targetbim207hw.jar sampleText.txt 10 </strong>

Sample Output

InitialCharacter            AverageLength

1          3.5 2    2.0 3    5.0

5          1.0

7          4.0

<ul>

 <li>285714285714286</li>

 <li>0</li>

 <li>333333333333333</li>

 <li>0 f 6.0 g 7.125 h 5.375 i   6.0</li>

</ul>

k 9.266666666666667 m 5.857142857142857

o          8.0 p    8.5 r     6.0

s 7.214285714285714 t 6.363636363636363

<ul>

 <li>0</li>

 <li>4285714285714284 y 10.0 z  7.5</li>

</ul>

ç 11.666666666666666 ö 11.090909090909092 ü 12.666666666666666




Pair{t1=’yerleşkesindeki’, t2=’ve’, factor=26.0}

Pair{t1=’ve’, t2=’sayılı’, factor=15.356018837890671}

Pair{t1=’tarih’, t2=’ve’, factor=13.0}

Pair{t1=’donanımlı’, t2=’ve’, factor=13.0}

Pair{t1=’öğrencileri’, t2=’ve’, factor=13.0}

Pair{t1=’söyleşilere’, t2=’ve’, factor=13.0}

Pair{t1=’yaratıcı’, t2=’ve’, factor=13.0}

Pair{t1=’eden’, t2=’ve’, factor=13.0}

Pair{t1=’ve’, t2=’30425′, factor=13.0}

Pair{t1=’kültürel’, t2=’ve’, factor=13.0}


