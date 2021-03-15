### Introduction
  he AWK language is a data-driven scripting language consisting of a set of actions to be taken against streams of textual data – either run directly on files or used as part of a pipeline – for purposes of extracting or transforming text, such as producing formatted reports. The language extensively uses the string datatype, associative arrays (that is, arrays indexed by key strings), and regular expressions. While AWK has a limited intended application domain and was especially designed to support one-liner programs, the language is Turing-complete, and even the early Bell Labs users of AWK often wrote well-structured large AWK programs


### Baics

<details>
<summary>Display file</summary>
Print the content of the file to the screen.
<pre>
eg: 
  awk "{print}" fileName
  awk "{print}" file1 file2
  awk "{}1" fileName
</pre>
</details>

<details>
<summary>Insert string </summary>
Insert string to every line of the file
<pre>
  awk '{printf "String\t"}{print}' fileName
</pre>
Insert string only to the beginning of the file
<pre>
  awk 'BEGIN{printf "Beginning"}{print}' fileName
</pre>
Append string only to the end of the file
  awk 'END{printf "Ending"}{print}' fileName
<pre>
  awk '{printf "String\t"}{print}' fileName
</pre>
</details>
