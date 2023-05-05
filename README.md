Download Link: https://assignmentchef.com/product/solved-csi2120-lab-7-maximum-and-minimum-elements
<br>
Exercise 1: Maximum and Minimum ElementsWrite a Prolog program that finds the maximum and minimum element in a list of numbers. The program should work as follows:

?- maxmin([3,1,5,2,7,3],Max,Min).Max = 7Min = 1

?- maxmin([2],Max,Min).Max = 2Min = 2

Exercise 2: Odd and EvenWrite a Prolog program that processes a list of numbers and outputs another list which consists of a list of the constants odd and even corresponding to the numbers.

?- oddEven([3,1,5,2,7,3],L).L = [odd,odd,odd,even,odd,odd].Exercise 3: List Reversal with Every Second ElementCreate a Prolog program to reverse the order of the elements in a list but also remove every second element. The program should work as follows:

?- reverseDrop([3,1,5,2,7,3],L).L = [ 7, 5, 3 ].

?- reverseDrop([‘world’,’a’,’hello’],L).L = [ ‘hello’, ‘world’ ].Exercise 4: Adding up all the Numbers in a ListComplete the predicate below that is to add up all the numbers in a list but uses an alternating sign. Example:

?- addAlternate([5,6,1],S).S = 0.

?- addAlternate([3,1,5,2,7,3],S).S = 9.

addAlternate(L,S) :- __________________________.

addAlternate(___________________).

addAlternate([H|T],A,p,S) :- !,AA is A + H,addAlternate(T,AA,m,S).

addAlternate([H|T],A,m,S) :- !,AA is A – H,addAlternate(T,AA,p,S).No quiz this week!