---
layout:     post
title:      "RegexGenerator++"
subtitle:   "Automatic Generation of Text Extraction Patterns from Examples"
date:       2015-08-05 15:36:00
author:     "Kumar Ayush"
header-img: "img/dna-image.jpg"
---

<blockquote>
Some people, when confronted with a problem, think<br />
"I know, I'll use regular expressions."<br />
Now they have two problems.<br />
<b>Jamie Zawinski</b>
</blockquote>

<p>A regular expression or regex or regexp is a special text string for describing a search pattern. You are probably familiar with wildcard notations such as *.txt to find all text files ina  file manager. You can think of regular expressions as wildcards on steroids. The regex equivalent is .*\.txt</p>

<p>
But there is so much more you can do with regular expressions. In a text editor like vi or in a specialized text processing tool like grep, you could use the regex \b[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,6}\b to search for an email address. With just a single line of code, a programmer can easily decide if the user entered a valid email address, be it any language he is working with. 
</p>

<p>
  Debating the utility of regex is futile. Another of its applications include parsing HTML or XML. Here is the abstract from Robert Cameron's 1998 article, <i>REX:XML Shallow Parsing with Regular Expressions</i>
</p>
<blockquote>
The syntax of XML is simple enough that it is possible to parse an XML document into a list of its markup and text items using a single regular expression. Such a shallow parse of an XML document can be very useful for the construction of a variety of lightweight XML processing tools. <b>However, complex regular expressions can be difficult to construct and even more difficult to read.</b> Using a form of literate programming for regular expressions, this paper documents a set of XML shallow parsing expressions that can be used a basis for simple, correct, efficient, robust and language-independent XML shallow parsing. Complete shallow parser implementations of less than 50 lines each in Perl, JavaScript and Lex/Flex are also given.
</blockquote>

<p>Pay attention to the text in bold. It represents the major obstacle towards a more popular regex education and usage. Where would you find a solution?</p>

<p>I recently came across a blessing from Genetic Programming. GP is essentially an evolutionary algorithm-based methodology inspired by biological evolution to find computer programs that perform a user-defined task.</p>

<p>Scientists at the <a target = "_blank" href = "http://machinelearning.inginf.units.it">Machine Learning Lab</a>, DIA, University of Trieste, Itlay have come up with an intriguing tool called <a target = "_blank" href = "http://regex.inginf.units.it">RegexGenerator++</a></p>

<h2 class = "section-heading">What does it do?</h2>
<p>
You provide the application with a body of text;perhaps a sample from a large corpus and highlight stuff which fits the pattern you want to search for. If you input two such samples with at least 25 matches (separate highlighted stuff), they claim to generate a regular expression which best describes the pattern in your input matches.
</p>
<p>
This is simply beautiful in my opinion. You don't need to bash your head to find the optimal regular expression or browse the corners of SO for an answer. Do check it out!
</p>
