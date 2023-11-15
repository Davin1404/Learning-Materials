# People and Hat Problem 

e.g.  

Sophie and Ella play a game. They each have five cards showing roman numerals I, V, X, L, C. Sophie lays her cars face up on the table in order I, V X, L, C.  

Ella shuffles her cards and lays them face down on the table. She then turns them over one by one see if her card matches with Sophie's 4 card directly above. Sophie wins if nomatches occur; otherwise Ella wins.  

Shwo that the probability that Sophie wins the game is $\frac{11}{30}$.  

$$\text{Recursive formula: }$$  

$$F(n)=n!-\sum ^{n-1}_{i=0} \binom {n}{n-i}F(i)$$  

$$\text{terminal condition: }F(0)=1$$

$$P(n)=\frac{F(n)}{n!}$$  

The number of combinations with no matches between 2 sets of $n$ cards is denoted by $F(n)$.  
