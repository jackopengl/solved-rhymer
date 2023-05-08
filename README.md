Download Link: https://assignmentchef.com/product/solved-rhymer
<br>
<a href="https://www.youtube.com/playlist?list=PLhOuww6rJJNPNn2qa5ATHJ0qd-JUgM_s0" rel="nofollow">https://www.youtube.com/playlist?list=PLhOuww6rJJNPNn2qa5ATHJ0qd-JUgM_s0</a>

Write a program that will create rhyming words for a given word by removing the initial consonant sounds and substituting other sounds. Note that the given word should not appear in the output, so “cake” will be omitted from this run:

<pre><code>$ ./rhymer.py cake | headbakeblakebrakechakeclakecrakedakedrakefakeflake</code></pre>

The rhyming words will be created by adding all the consonants plus the following consonant clusters:

<pre><code>bl br ch cl cr dr fl fr gl gr pl pr sc sh sk sl sm sn sp st sw th tr tw thw wh wr sch scr shr sph spl spr squ str thr</code></pre>

The output should be sorted alphabetically. If there is no initial consonant sound, then apply all the consonant sounds to the given word:

<pre><code>$ ./rhymer.py apple | tailthwappletrappletwapplevapplewapplewhapplewrapplexappleyapplezapple</code></pre>

If provided no arguments, the program should print a short usage:

<pre><code>$ ./rhymer.pyusage: rhymer.py [-h] strrhymer.py: error: the following arguments are required: str</code></pre>

And a longer usage for <code>-h</code> or <code>--help</code>:

<pre><code>$ ./rhymer.py -husage: rhymer.py [-h] strMake rhyming "words"positional arguments:  str         A word to rhymeoptional arguments:  -h, --help  show this help message and exit</code></pre>

Run the test suite to ensure your program is correct:

<pre><code>$ make testpytest -xv test.py============================= test session starts ==============================...collected 7 itemstest.py::test_exists PASSED                                              [ 14%]test.py::test_usage PASSED                                               [ 28%]test.py::test_take PASSED                                                [ 42%]test.py::test_chair PASSED                                               [ 57%]test.py::test_chair_uppercase PASSED                                     [ 71%]test.py::test_apple PASSED                                               [ 85%]test.py::test_no_vowels PASSED                                           [100%]============================== 7 passed in 0.47s ===============================</code></pre>