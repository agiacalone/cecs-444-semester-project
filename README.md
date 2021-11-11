Good evening CECS 444! I have *finally* completed your semester assignment which is to hand-craft the first two major components of a compiler.

Wait...I know what you're thinking right now. Allow me to answer your questions: Yes, this is a difficult task. Yes, I also believe you all can do it. Yes, it will be awesome when you're done. :-)

With the scanner and the parser both created, you should use the scanner's output as the input for the parser. Both pieces should work seamlessly together when the whole thing is done.

Ideally, your scanner/parser system will handle all potential cases in the token and language specifications. I have included a really tough test case which handles a bunch of edge cases so you can thoroughly put your code through the wringer. If you want a "top" grade for the lab assignment, you'll have to make sure your code rigorously handles virtually anything I can throw at it (and I will be tough ;-)  ) If you flawlessly pass the test contained in "hardtestcase.txt", you can be reasonably assured that you've done your job.

*I only have the scanner portion written as of today (Oct 14)*, so the parser requirements will be coming in the following weeks. I will update this document when I have them ready.

The Scanner
-----------

I have included the following files in this section which will serve as the specifications for your project. Included are:

    *   exhaustive unit test <hardtestcase.txt>
    *   tokens <tokens.txt>
    *   reserved words <rwords.txt>
    *   An image of an example log for the scanner <tokenlog.png>

The scanner will need to be verbose in its logging, as I will use the program's logs to verify the successful tokenization of the given input.

Okay, here is what I will require from you for the semester:

**Due by Nov 12**:

1.  Images of your NFA and DFA for all tokens (ideally, in an accessible document)
2.  Your completed scanner, which will include:
    *   an action table
    *   a lookup table
    *   a state table
    *   the executable which reads in a source code file
    *   a screenshot of log output (not a text file)

Of course, your scanner will have to pass the given test in "hardtestcase.txt" for full credit (the A). Anything short of that will receive points based on how closely your scanner meets the specifications.

**Due by Dec 10:**

Your completed parser, which will include:
1.  the parse table
2.  the parser tokens
3.  the parser interpreter runtime file

Like the requirements for the scanner, your parser will be graded on how accurate it handles the requirements given in "grammar.txt".

More details to come soon!