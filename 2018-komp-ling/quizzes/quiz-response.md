1. Which problems does maxmatch suffer from? (Choose all that apply.)

Answer: 

a) requires comprehensive dictionary

b) is computationally expensive  (it can be computationally expensive only in term of using dictionary, because every time we need to loop over dict to find the word(if it exists), but the type of algorithm is greedy, therefore, all in all, we can say that it is not com. expensive)

d) constructs non-grammatical sentences

2. Write a perl/sed substitution with regular expressions that adds whitespace for segmentation around "/" in "either/or" expressions but not around fractions "1/2":

 "either/or" -> "either / or"
 "1/2"       -> "1/2"

Answer:  sed -e 's/\([a-z]\+\)\/\([a-z]\+\)/\1 \/ \2/g' < exemple_for_reg_exp.txt

3. the text mentions several times that machine learning techniques produce better segmentation than rule-based systems; what are some downsides of machine learning techniques compared to rule-based?

Answer: In many cases after using machine learning techniques it is difficult to direct influence on the algrithm to avoid concrete mistackes in parsing. Overvise rule-based system easily can be changed according to result it produced. It allows us fast find causes of mis-spliting. 

4. write a sentence (in English or in Russian) which maxmatch segments incorrectly.

Answer: 

correct - "Это, на самом неделе, не хороший, а плохой человек"

maxmatch - "Это, на самом деле, нехороший, а плохой человек"


5. what are problems for sentence segmentation? provide one example in English or Russian for each that applies.

Answer:
a) ambiguous abbrevations with punctuation

"А.С.Пушкин - солнце русской поэзии"

b) sentences containing symbols '!' and '?'

"Алексей, это ты?" - спросила девушка взволнованно.
"Господи!" - вскрикнул жандарм.

c) sentences lacking separating punctuation

Он был там в 1996 г. Тогда-то и произошли эти события.

d) sentences not separated by whitespace

Он был специалист.Таких еще поискать.
