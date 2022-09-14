## CS150 Assignment 2

A Mortgage Calculator

**Points:** 25

**This is an individual assignment.**

**Goals:**

1.  Use relational and arithmetic operators appropriately

2.  Program conditionally using a single-alternative if and nested ifs

3.  Introduce built-in functions from the cmath library

If you run into any problems with this assignment, it is important that
you come and see me or a TA early so that we can help. Also, it
is very important for you to do this assignment on your own. Every
assignment you will be doing from now on will require the techniques you
learned in class and in the lab.

**Information on buying a house**

Many believe that one of the best investments that anyone can make is
buying a house. Houses in general will appreciate and the interest on
the loan is tax deductible. Unfortunately, most of us become so mind
boggled when presented with all of the paperwork for buying a house that
we really don\'t understand much of what went on (trust me on this). For
this problem, I want to concentrate on the mortgage loan.

Before you go out looking at houses, you need to have a price range in
mind. That price range is based on how much the monthly payment is going
to be. A monthly payment consists of principal, interest, taxes, and
insurance (PITI). The principal is a portion of the actual loan that is
being paid back. The interest is what you are paying as interest on the
remainder of the loan each month. Taxes refer to property taxes and
insurance is self-explanatory. The majority of the monthly payment is
made up of (PI) which is principal and interest.

In order to figure out how much house we can buy, we need to know what
the monthly payment is going to be. To figure out the monthly payment,
we must do a what-if analysis. That is, for instance, what-if we are
looking at an \$87,000 house. Further, we must do a what-if on the
interest rate. As an example, presently the interest rate is somewhere
in the range of 3.0% to 3.5% (fixed).

Here is the formula for finding the monthly payment for any loan:

P = L\[m(1 + m)<sup>n</sup>\]/\[(1 + m)<sup>n</sup> - 1\], where

**L** is the loan amount in dollars

**m** is the monthly interest rate (the yearly interest rate will be
entered as example, 6.0,\
meaning 6%, so m would need to be .06 / 12 or .005 for the above formula
to work)

**n** is the number of months the loan is for

**Here is the problem that you are to solve**

You are to write a complete C++ program fully documented that allows the
user the ability to enter a loan amount in dollars (e.g. 115000.00), a
down payment (e.g. 15000.00), a yearly interest rate (e.g. 3.5), and a
number of years the loan is for (e.g. 30). You must then calculate the
monthly payment that will be paid each month for the duration of the
loan, the monthly mortgage insurance payment, and the total interest
paid on the loan over that same period of time. Anyone unable to put a
20% down payment of the purchase price, must pay mortgage insurance. The
mortgage insurance rate is calculated based on the amount of the down
payment and a credit rating. For this assignment, the mortgage insurance
for the year will be 1% of the loan amount and paid monthly.

Here is exactly what your program is to output (asterisks and all), and
user input is in **bold**:

<pre>
*******************
Mortgage Calculator
*******************

Enter Purchase Price: $<b>115000.00</b>
Enter Down Payment: $<b>15000.00</b>
Enter Interest Rate: %<b>3.5</b>
Enter Number Of Years: <b>30</b>

**************************************
Loan Amount: $100000
Monthly Mortgage Payment: $449.045
Monthly Mortgage Insurance: $83.3333
Total Interest Paid: $61656.1
**************************************
</pre>

**Note1:** Each inputted value is to be \> 0.0. If an inputted value is
entered incorrectly, output the message "Incorrect Input -- Terminating
Program" Here is an example. You are to terminate the program
immediately when an illegal input occurs. **Further, there is to be only
one return statement at the end of your program.**

<pre>
*******************
Mortgage Calculator
*******************

Enter Purchase Price: $<b>115000.00</b>
Enter Down Payment: $<b>15000.00</b>
Enter Interest Rate: %<b>-1.0</b>
Incorrect Input - Terminating Program
</pre>

**Note2:** Do not use any C++ constructs not introduced in the class
thus far.**\
**

You will need to use the pow function. In order to use the pow function,
you will need to include the library cmath by using the preprocessor
directive #include \<cmath>. The pow function accepts two doubles and
returns a double. As an example,

cout \<\< pow (2.0, 3.0); // outputs 8.0 because 2.0<sup>3.0</sup> equals 8.0

**To complete this assignment you must submit the following:**

1.  **An electronic Solution of your program on GitHub**

    a.  You are to click on the Assign02 Link on Moodle to accept this
        assignment as we've done in lab. Once accepted, code up a
        complete solution to the above assignment specification. Your
        complete solution is to be pushed to GitHub no later than the
        date and time specified above for your specific section. I will
        only grade your solution from the proper location on GitHub.

    b.  Pay attention to the example output above. Your program's output
        must look **exactly** like the example output! The spacing and
        newlines in your output must match exactly.

    c.  Make sure that your program compiles and runs correctly with no
        errors and no warnings. If you get any errors, double check that
        you typed everything correctly. Be aware that C++ is
        case-sensitive.

2.  **An electronic copy of your program is to be placed on Moodle**

    a.  See Lab01 for producing a pdf of your complete program. Once you
        have produced the pdf of your program and named the pdf your
        **punetid**, drop the pdf in the Assign02 folder on Moodle.

    b.  The pdf must be in the drop folder on Moodle by the time and day
        specified above. Anything submitted after that will be
        considered late.

> **Good luck! And remember, if you have any problems, come and see
> straight away. **
