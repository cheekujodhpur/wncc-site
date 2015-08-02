---
layout:     post
title:      "[ISoC] True Friends"
subtitle:   "Institute Summer of Code"
date:       2015-05-13 13:00:00
author:     "Ranveer Aggarwal"
header-img: ""
---
<b>Level:</b> Moderate
<br />

<h4 class = "section-heading">Problem</h4>
<p>
  You are given a string array representing Known people. Known[i][j]='Y' if i knows j.<br />
  <b>Friends:</b> A is a friend of B if B knows A or B has a friend who knows A.<br />
  <b>True friends:</b> A and B are true friends if A is a friend of B and B is a friend of A.<br />
  <b>Group:</b> Everyone in a Group must be true friends to each other. Your task is to find the number of Groups from the given list of Known people. It can be proved that there is exactly only one possible way for forming the groups.
</p>

<h4 class="section-heading">Input</h4>
<p>
  The first line consists of and integer t, the number of test cases. For each test case, you are given an array of strings representing Known people. Known is of size NxN where N is the total number of people.
</p>

<h4 class="section-heading">Output</h4>
<p>
For each test case, print the number of Groups
</p>

<h4 class = "section-heading">Input Constraints</h4>
<p>
1<=t<=1000<br />
1<=N<=100<br />
Known[i][j] is either 'Y' or 'N'
Known[i][i]='N' (No one is known to themselves)
</p>

<h4 class = "section-heading">Sample Input</h4>
<blockquote>
3<br />
3<br />
NYN<br />
NNY<br />
YNN<br />
7<br />
NNYNNNN<br />
NNNYYYN<br />
NNNNNNN<br />
YNNNNNN<br />
NNNYNNN<br />
NNNNNNN<br />
NNNNNYN<br />
7<br />
NNNNYYN<br />
NNNNNNN<br />
NNNNNYN<br />
NYNNNYY<br />
NNNYNNN<br />
NNYNNNY<br />
NNNYNNN<br />
</blockquote>

<h4 class = "section-heading">Sample Output</h4>
<blockquote>
1<br />
7<br />
3<br />
</blockquote>

<h4 class = "section-heading">Explanation</h4>
<p>
<b>Case 1:</b> All the friends are true friends to each other<br />
<b>Case 2:</b> No two true friends exist<br />
<b>Case 3:</b> There are 3 groups of true friends. {0},{1},{2,3,4,5,6}
</p>

<b>Source</b>: <a href = "http://www.spoj.com/problems/TFRIENDS/">TFRIENDS</a>
