# Integration By Part D-I Method
> 如果你还在为 by part integration 分部积分烦恼，觉得 Math AA data booklet 上面给的公式是一坨的话，赶紧快来尝试一下由油管数学博主 blackpenredpen 发明的 D-I 表格 By part 法吧!  
> 原视频:  
>https://www.youtube.com/watch?v=2I-_SV8cwsw&ab_channel=blackpenredpen

Integration by parts 分部积分原公式:  
$$\int u\frac{dt}{dx}dx=ut-\int \frac{du}{dx}tdx$$

## D-I Method 解题过程
以下面的积分式为例:  
$$\int x^2\text{sin}(3x)dx$$
首先我们需要画 D-I 表格，然后分别将积分式拆成两个部分，优先将易于求导的部分放在 $D(\text{Differentiation})\space\text{column}$ 求导列, 并将另外一个部分放在 $I(\text{Integration})\space\text{column}$ 积分列。 我们还需要在表格左侧添加正负号，且正负交替出现 (第一行是正号) 。  
||$D(\text{Differentiation})$|$I(\text{Integration})$|
|---|---|---|
|$+$|$x^2$|$\text{sin}(3x)$|
|$-$|||
|$+$|||
|$-$|||

随后，开始运算，对左列部分一直求导，对右列部分一直积分，将求导与积分出来的结果填入表格中的下一行。重复运算直到最新运算出的一行里的求导与积分部分满足[三个终止情况](#three-stop-cases-三个终止情况)。  

||$D(\text{Differentiation})$|$I(\text{Integration})$|
|---|---|---|
|$+$|$x^2$|$\text{sin}(3x)$|
|$-$|$2x$|$-\frac{1}{3}\text{cos}(3x)$|
|$+$|$2$|$-\frac{1}{9}\text{sin}(3x)$|
|$-$|$0$ *(meets the first "STOP" case)*|$\frac{1}{27}\text{cos}(3x)$|

然后，从第一列开始，到倒数第二列，将 $D$ 求导列部分***乘左侧符号***与***下一行***的 $I$ 积分列部分相乘，并将所有积相加。  
$$(x^2)(-\frac{1}{3}\text{cos}(3x))+(-1)(2x)(-\frac{1}{9}\text{sin}(3x))+(2)(\frac{1}{27}\text{cos}(3x))$$
我们就可以得出这个积分的最终答案了！
$$\int x^2\text{sin}(3x)dx=-\frac{1}{3}x^2\text{cos}(3x)+-\frac{2}{9}x\text{sin}(3x))+\frac{2}{27}\text{cos}(3x)+C$$

## Three "STOP" cases 三个终止情况
1. The latest part of the ***D column*** *(differentiation part)* is ***zero***  
  在D列 (求导部分) 计算出来的部分等于零

2. The ***product*** of *differentiation part* and *integration part* in the ***same row*** can be ***"easily"*** integrated   
  同一行的求导部分与积分部分的积可以被“轻易”积分

3.  The ***product*** of *differentiation part* and *integration part* in the ***same row*** equals to the ***original expression times negative one***  
  同一行的求导部分与积分部分的积等于原式乘负一



