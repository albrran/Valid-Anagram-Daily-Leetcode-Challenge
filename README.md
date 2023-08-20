# Valid-Anagram-Daily-Leetcode-Challenge
![1_OathM0PWiIfPfFuJ3wv87A](https://github.com/albrran/Valid-Anagram-Daily-Leetcode-Challenge/assets/120284166/4d831238-d99d-4762-93b5-6311438f469d)
<br>
<h2>Problem: Given two strings s and t, return true if t is an anagram of s, and false otherwise. An <b>Anagram</b> is a word or phrase formed by rearranging the letters of a different word or phrase, typically using all the original letters exactly once.</h2>

<h2>Example 1:</h2>
    <p>
        Input: s = "anagram", t = "nagaram"<br>
        Output: true
    </p>
    <h2>Example 2:</h2>
    <p>
        Input: s = "rat", t = "car"<br>
        Output: false
    </p>
    <h2>Constraints:</h2>
    <ul>
        <li>1 <= s.length, t.length <= 5 * 10^4</li>
        <li>s and t consist of lowercase English letters.</li>
    </ul>
<br>
<h1>Solution 1: Compare using Char Array</h1>
<p>Imagine that we've received two packages of computer mouse and we want to determine that both packages have the same exact kinds of mouse. We peer through each box simultaneously and take out a mouse at random, then compare them to each other, but what good would that do? What if we emptied each box and sorted the mice based on size, and then compared them simultaneously? That would allow us to tell if both packages have the same exact kinds of mouse and the same number of mouse. </p>
    
<br>
<h3>Lets break it down into steps</h3>
<ol>
    <li>Determine if the length of the given strings are the same since an anagram can exist only if both strings are of the same length, if not return false</li>
    <li>Convert each string into a char array.</li>
    <li>Sort each char array.</li>
    <li>Loop through an array (doesn't matter which one) while comparing index values only breaking the loop and returning false if the values are not the same</li>
</ol>
<p>Time Complexity: O(nlogn). We're using the ".sort()" which is log(n) and a for loop which is n. Therefore the time complexity is nlogn</p>
<p>Space Complexity: O(n). We are iterating to the length of n, the given string's length</p>
