### Questions
These are a collection of questions asked in TCS Code Vita 2019 (28-29th June 2019). Please go through these and try to solve these and push into the `Competitive coding` folder inside the language folders.

> ## Distribute Books :

**Problem Description**

For enhancing the book reading, school distributed story books to students as part of the Children’s day celebrations.

To increase the reading habit, the class teacher decided to exchange the books every weeks so that everyone will have a different book to read. She wants to know how many possible exchanges are possible.

If they have 4 books and students, the possible exchanges are 9. Bi is the book of i-th student and after the exchange he should get a different book, other than Bi.

```
B1 B2 B3 B4 - first state, before exchange of the books

B2 B1 B4 B3

B2 B3 B4 B1

B2 B4 B1 B3

B3 B1 B4 B2

B3 B4 B1 B2

B3 B4 B2 B1

B4 B1 B2 B3

B4 B3 B1 B2

B4 B3 B2 B1

```
Find the number of possible exchanges, if the books are exchanged so that every student will receive a different book.

**Constraints**

1<= N <= 1000000

**Input Format**

Input contains one line with N, indicates the number of books and number of students.

**Output
**
Output the answer modulo 1000000007.

**Test Case**

Input

4

Output

9

> ## Philaland Coin :

**Problem Description**

The problem solvers have found a new Island for coding and named it as Philaland.

These smart people were given a task to make purchase of items at the Island easier by distributing various coins with different value.

Manish has come up with a solution that if we make coins category starting from $1 till the maximum price of item present on Island, then we can purchase any item easily. He added following example to prove his point.

Lets suppose the maximum price of an item is 5$ then we can make coins of {$1, $2, $3, $4, $5} to purchase any item ranging from $1 till $5.

Now Manisha, being a keen observer suggested that we could actually minimize the number of coins required and gave following distribution {$1, $2, $3}. According to him any item can be purchased one time ranging from $1 to $5. Everyone was impressed with both of them.

Your task is to help Manisha come up with minimum number of denominations for any arbitrary max price in Philaland.

**Constraints**

1<=T<=100

1<=N<=5000

**Input Format**

First line contains an integer T denoting the number of test cases.

Next T lines contains an integer N denoting the maximum price of the item present on Philaland.

**Output**

For each test case print a single line denoting the minimum number of denominations of coins required.

**Test Case**

```
Input

2

10

5

Output

4

3

```
**Explanation**

For test case 1, N=10.

According to Manish {$1, $2, $3,... $10} must be distributed.

But as per Manisha only {$1, $2, $3, $4} coins are enough to purchase any item ranging from $1 to $10. Hence minimum is 4. Likewise denominations could also be {$1, $2, $3, $5}. Hence answer is still 4.

For test case 2, N=5.

According to Manish {$1, $2, $3, $4, $5} must be distributed.

But as per Manisha only {$1, $2, $3} coins are enough to purchase any item ranging from $1 to $5. Hence minimum is 3. Likewise denominations could also be {$1, $2, $4}. Hence answer is still 3.

> ## Market Survey :

**Problem Description**

Market Research firm is carrying out a survey regarding popular brands. The person who has the best pulse of the survey population will be rewarded by the firm.

The survey comprises of N questions was taken by M participants, not at the same time but one after the other. Clearly, there is no correct answer since it is a survey of brands. Each question can have only four options (1,2,3,4). Most expected answers to different questions is used as a template to measure brand popularity. Think of this as a default answer sheet where the question paper is the Survey.

'0' represents no answer to a question. Thus it means that the participant has skipped answering that question.

Right Answer:

For a particular question, the highly chosen option till that point of time is treated as the correct answer. If multiple options have the same count, then out of those options the one which was chosen recently is treated as the right answer.

Score of a Participant:

One point will be awarded for each right answer. No negative points for wrong answers.

Instant Result:

This is shared to the Participant instantly after completion of his/her exam. (this is equal to number of right answers)

Final Result:

Only the final top scorer(TOPPER) is announced along with his score.

Note:

At the end of all M Participants completing the exam, the final right answers gets decided.

Based on these answers score of each candidate gets recalculated and the one with highest score is the TOPPER!!!

If more than one Participant gets the top score then the one among them who attempted the exam first, is treated as TOPPER.

**Constraints**

1 <= N,M <= 1000

**Input Format**

First line contains N (number of questions)

Second line contains M (number of Participants)

Third line contains N integers separated with space (default answers)

Next M lines contains N integers separated with space (response of M participants)

**Output**

First M lines showing the instant results of each Participant.

Last line containing the TOPPER’s id and his score

(assume id’s start with 1)

**Test Case**

```
Input

10

2

1 2 3 4 1 2 3 4 1 2

1 2 4 4 3 2 3 1 1 3

2 3 4 4 1 2 3 1 1 2

Output

6

6

1 8

```
**Explanation**

Number of questions = 10

Number of Participants = 2

Default answers : 1 2 3 4 1 2 3 4 1 2

(Latest Key is same as Default answers)

First Participant answers : 1 2 4 4 3 2 3 1 1 3

Right answers : 6 (= Instant result of first Participant)

Latest Key : 1 2 4 4 3 2 3 1 1 3

Second Participant’s answers : 2 3 4 4 1 2 3 1 1 2

Right answers : 6 (= Instant result of second Participant)

Latest Key : 1 2 4 4 1 2 3 1 1 2

Final key : 1 2 4 4 1 2 3 1 1 2

(Final Key is same as Latest Key at the end of all Participants completing the exam)

Right answers of Participant1 = Right answers of Participant2 = 8.

So topper is first Participant with score 8.

> ## Coins Required

**Problem Description**

Find minimum number of coins required to form any value between 1 to N, both inclusive. Cumulative value of coins should not exceed N. Coin denominations are 1 Rupee, 2 Rupee and 5 Rupee.

Lets understand the problem using the following example.

Consider value of N is 13, then the minimum number of coins required to formulate any value between 1 and 13, is 6. One 5 Rupee, three 2 Rupee and two 1 Rupee coins are required to realize any value between 1 and 13. Hence this is the answer.

However, if one takes two 5 Rupee coins, one 2 rupee coin and two 1 rupee coin, then too all values between 1 and 13 are achieved. But since the cumulative value of all coins equals 14, i.e., exceeds 13, this is not the answer.

**Constraints**

0 < n < 100000

**Input Format**

A single integer value.

**Output**

Four space separated integer values.

1st – Total number of coins.

2nd - number of 5 Rupee coins.

3rd – number of 2 Rupee coins.

4th – number of 1 Rupee coins.

**Test Case**

```
Input

13

Output

6 1 3 2

```
**Explanation**

The minimum number of coins required is 6 with in it:

minimum number of 5 Rupee coins = 1

minimum number of 2 Rupee coins = 3

minimum number of 1 Rupee coins = 2

Using these coins, we can form any value with in the given value and itself, like below:

Here the given value is 13

For 1 = one 1 Rupee coin

For 2 = one 2 Rupee coin

For 3 = one 1 Rupee coin and one 2 Rupee coins

For 4 = two 2 Rupee coins

For 5 = one 5 Rupee coin

For 6 = one 5 Rupee and one 1 Rupee coins

For 7 = one 5 Rupee and one 2 Rupee coins

For 8 = one 5 Rupee, one 2 Rupee and one 1 Rupee coins

For 9 = one 5 Rupee and two 2 Rupee coins

For 10 = one 5 Rupee, two 2 Rupee and one 1 Rupee coins

For 11 = one 5 Rupee, two 2 Rupee and two 1 Rupee coins

For 12 = one 5 Rupee, three 2 Rupee and one 1 Rupee coins

For 13 = one 5 Rupee, three 2 Rupee and two 1 Rupee coins

> ## Glass Piece

**Problem Description**

A square glass sheet of size 'S' cm fell down and broken down into N+1 pieces.

A man collected the broken pieces and he is trying to arrange the pieces to get the original shape. He found that exactly one piece is missing. To find the exact position of the missing piece, he noted down all (x,y) coordinates of each broken piece. Please help him to find the coordinates of the missing piece.

Note 1 : The input order of corners of known glass pieces are in the clockwise direction starting from the corner having least X value. If more than one corners having the same least X value, then start from the corner having least X and least Y value.

Note 2 : The corners of missing glass piece should output in the clockwise direction starting from the corner having least X value. If more than one corners have same least X value, then start from the corner having least X and least Y value.

**Constraints**

1 < S <= 1000.

1 < N <= 50.

**Input Format**

First line contains an integer, S, size of Glass Sheet.

Second line contains an integer, N.

Next N lines contain set of space separated integers indicates the details of N known glass pieces as follows:

First number indicates total corners of that glass piece - say i, followed by 2 * i integers denotes X and Y coordinates of i corners, delimited by space.

**Output**

Coordinates of missing piece in (X,Y) format separated by spaces.

**Test Case**
```
Input

400

3

5 0 0 200 0 400 200 100 250 0 250

3 200 0 400 0 400 200

4 100 250 400 200 400 400 200 400

Output

(0,250) (100,250) (200,400) (0,400)

```

> ## Home Lighting :

**Problem Description**

You are moving to a new apartment and want to plan your total lighting cost for the next 2 years which includes the cost of bulb procurement and cost of electricity consumption. Three types of bulbs are available in the market.

1. Regular bulbs, which cost C1, have a warranty of M1 hours, and have a running cost of R1 per hour. 
2. CFL bulbs, which cost C2, warranty M2 hours, running, cost R2 per hour. 
3. LED bulbs, which cost C3, warranty M3 hours, running cost R3 per hour  C1 < C2 < C3 and R1 > R2 > R3, nothing can be said about M1, M2, and M3. 
You have a plan for 1 bulb in the kitchen at H1 hours per day, 2 bulbs per room across 3 rooms at H2, H3, H4 hours per day per room per bulb, 1 bulb for bathroom at H5 hours per day. 
When you prepare your budget you assume that it will last only till the warranty period. 
Given the above requirements, come up with a bulb procurement plan that incurs least cost over 2 years - where cost includes procurement and running cost. In case warranty expires, in your model assume that the bulb will need to be replaced. Also assume that you will move out after 2 years, and so you are not concerned about stretching the life of bulbs beyond that time. Assume that there are 365 days in each year.

**Constraints**

C1 < C2 < C3

R1 > R2 > R3

0<= Fixed Cost <=1000

0<= Warranty<=150

0<= Running cost <=30000

0<= H1,H2,H3,H4,H5<=24

Input Format

The first three lines contains three integers denoting Fixed cost, Warranty and running cost of regular bulb, CFL and LED respectively.

The next five lines contain one integer each denoting usage hours of rooms (H1, H2, H3, H4, H5)

Output

Minimum cost to light the house.

**Test Case**

```
Input

50 1500 16

100 8000 14

400 25000 1

1

2

8

14

2

Output

38500

```

> ## Television Sets :

**Problem Description** 

Dr. Vishnu is opening a new world class hospital in a small town designed to be the first preference of the patients in the city. Hospital has N rooms of two types - with TV and without TV, with daily rates of R1 and R2 respectively. 

However, from his experience Dr. Vishnu knows that the number of patients is not constant throughout the year, instead it follows a pattern. The number of patients on any given day of the year is given by the following formula – 

`(6-M)^2 + |D-15|` ,

where M is the number of month (1 for jan, 2 for feb ...12 for dec) and D is the date (1,2...31).

All patients prefer without TV rooms as they are cheaper, but will opt for with TV rooms only if without TV rooms are not available. Hospital has a revenue target for the first year of operation. Given this target and the values of N, R1 and R2 you need to identify the number of TVs the hospital should buy so that it meets the revenue target. Assume the Hospital opens on 1st Jan and year is a non-leap year. 

**Constraints**

Hospital opens on 1st Jan in an ordinary year

5 <= Number of rooms <= 100

500 <= Room Rates <= 5000

0 <= Target revenue < 90000000

**Input Format**

First line provides an integer N that denotes the number of rooms in the hospital

Second line provides two space-delimited integers that denote the rates of rooms with TV (R1) and without TV (R2) respectively

Third line provides the revenue target

**Output**

Minimum number of TVs the hospital needs to buy to meet its revenue target. If it cannot achieve its target, print the total number of rooms in the hospital.

**Test Case**

_Example-1 :_
```
Input

20

1500 1000

7000000

Output

14 
```
**_Explanation_**

Using the formula, number of patients on 1st Jan will be 39, on 2nd Jan will be 38 and so on. Considering there are only twenty rooms and rates of both type of rooms are 1500 and 1000 respectively, we will need 14 TV sets to get revenue of 7119500. With 13 TV sets Total revenue will be less than 7000000

_Example-2 :_

```
Input

10

1000 1500

10000000

Output

10
```
**_Explanation_**

In the above example, the target will not be achieved, even by equipping all the rooms with TV. Hence, the answer is 10 i.e. total number of rooms in the hospital.

> ## War Companion

**Problem Description**

Infinity War is Over. Thanos has successfully collected all the Infinity Stones and wiped out half the population of the universe. Now the world depends on the remaining Avengers to bring back their loved ones.

To get a last chance of defeating Thanos, the Avengers has put together a team of its best warriors to try to steal the Infinity Gauntlet and restore order to the universe. The warriors must be put in pairs into its warships and sent out. Obviously, the team size is even.

Each warrior in the warship needs to work well with his partner in the warship, and chemistry between them is important. Hence the Supreme Commander has requested all the warriors to give a list of the remaining warriors in the team in the order of their preferring to work with them.

Using these lists the Supreme Commander needs to create a set of suitable pairs of warriors, with each warrior getting a partner. A set of pairings of warriors is not suitable if two warriors exist who both prefer each other more than their existing partner. The Supreme Commander recognizes that there can be more than one set of suitable pairs of warriors. He ranks the warriors in descending order of competence, so that the most competent are at the top. He has directed you, his chief analyst, to create a suitable set of pairings that lets the most competent warrior to partner someone as high in list of preferences as possible, and then the next most competent warrior to work with as high a person on his list as possible, and so on.

Please write a program to create a suitable set of pairings that meets the Supreme Commander’s directions. If no such pairing exits, indicate that.

**Constraints**

N <= 10

**Input Format**

First line contains the number of warriors (N).

Next N lines contain the preference list of N warriors, where the first word in the line is the warrior and the next (N-1) words are the warriors in the preference order.

The N lines give the warriors in order of decreasing competence

**Output**

A set of suitable pairs as directed by the Supreme Commander. If no suitable sets exist, output “No Suitable Pairs.”.

**Test Case**

_Example-1 :_

```
Input

6

Ironman Thor Blackwidow Hawkeye Hulk Captainamerica

Thor BlackwidowCaptainamerica Hawkeye Ironman Hulk

Hulk BlackwidowCaptainamerica Hawkeye Ironman Thor

Blackwidow Hawkeye Hulk Ironman Captainamerica Thor

Captainamerica Hawkeye Hulk Blackwidow Thor Ironman

Hawkeye Ironman Thor Blackwidow Hulk Captainamerica

Output

Ironman,Hawkeye

Thor,Captainamerica

Hulk,Blackwidow
```
_**Explanation**_

This is a suitable set of pairs. If we take a pair of warriors, say Thor and Blackwidow,though Thor prefers Blackwidow to his current partner (Captainamerica), Blackwidow prefers the current partner(Hulk) to Thor. Similarly all other pairs of warriors can be checked to see that this is a suitable set of pairings.

_Example-2 :_

```
Input

4

Charles Wolverine Jean Deadpool

Wolverine Jean Charles Deadpool

Jean Charles Wolverine Deadpool

Deadpool Charles Wolverine Jean

Output

No Suitable Pairs.
```
**_Explanation_**

It can be seen that there is no suitable set of pairings. If Deadpool is paired with say Charles, and the other two paired with each other, consider the warriors Charles and Jean. Charles prefers Jean to his current partner, Deadpool, and Jean prefers Charles to the current partner, Wolverine. Hence this is not a suitable pairing. Similarly, Deadpool cannot be paired with anyone else to form a suitable set. Thus the output is “No Suitable Pairs”