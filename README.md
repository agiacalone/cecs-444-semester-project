# CECS 444 Semester Project: Make a Compiler

Good evening CECS 444! I have *finally* completed your semester assignment which is to hand-craft the first two major components of a compiler.

Wait...I know what you're thinking right now. Allow me to answer your questions: Yes, this is a difficult task. Yes, I also believe you all can do it. Yes, it will be awesome when you're done. :-)

With the scanner and the parser both created, you should use the scanner's output as the input for the parser. Both pieces should work seamlessly together when the whole thing is done.

Ideally, your scanner/parser system will handle all potential cases in the token and language specifications. I have included a really tough test case which handles a bunch of edge cases so you can thoroughly put your code through the wringer. If you want a "top" grade for the lab assignment, you'll have to make sure your code rigorously handles virtually anything I can throw at it (and I will be tough ;-)  ) If you flawlessly pass the test contained in [hardtestcase.txt](lexer/hardtestcase.txt), you can be reasonably assured that you've done your job.

## The Scanner/Lexer

I have included the following files in this section which will serve as the specifications for your project. Included are:

* exhaustive unit test: [hardtestcase.txt](lexer/hardtestcase.txt)
* tokens: [tokens.txt](lexer/tokens.txt)
* reserved words: [rwords.txt](lexer/rwords.txt)
* An image of an example log for the scanner: [tokenlog.png](lexer/tokenlog.png)

The scanner will need to be verbose in its logging, as I will use the program's logs to verify the successful tokenization of the given input.

Okay, here is what I will require from you for the semester:

**Due by Nov 19**:

1. Images of your NFA and DFA for all tokens (ideally, in an accessible document)
2. Your completed scanner, which will include:
   * an action table
   * a lookup table
   * a state table
   * the executable which reads in a source code file
   * a screenshot of log output (not a text file)

Of course, your scanner will have to pass the given test in [hardtestcase.txt](hardtestcase.txt) for full credit (the A). Anything short of that will receive points based on how closely your scanner meets the specifications.

## The LL(1) Parser

We will be making a LL(1) parser in this course. Aside from the scanner/lexer that you have created, you will use the grammar specification in [grammar.txt](parser/grammar.txt) to match tokens that your scanner will output.

The grammar will not be enough, however, to fully complete your parser. In addition to the included files, you will need to produce a parse table which takes the grammar and matches statements from your input. Recall our lectures: in order to create the parse table, you will need:

* a left-recursion free grammar (Good news! It's *already* left-recursion free! You can thank me later.)
* the first sets
* the follow sets
* the predict sets
* the final parse table

**Due by Dec 10:**

Your completed parser, which will include:

1. the parse table
2. the sets (first, follow, predict)
3. the parser interpreter runtime file
4. and a test run which shows the successful completion of [hardtestcase.txt](lexer/hardtestcase.txt)

Like the requirements for the scanner, your parser will be graded on how accurate it handles the requirements given in [grammar.txt](parser/grammar.txt).

If you complete all of this, give yourself a strong pat on the back. You've just accomplished *one of the most difficult tasks* in computer science!
