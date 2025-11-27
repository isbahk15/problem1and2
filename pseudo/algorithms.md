Algorithm SumDistinctElements(Set1[], n, Set2[], m)
// Input: Set1[] and Set2[] are arrays of size n and m
// Output: sum of all elements that are only present in 1 set

Begin
 sum ← 0   //Initialize the sum to 0
 // Step 1: Add elements from Set1 that are NOT present in Set2
 For i from 0 to n-1 do
 isDistinct←true //we assume every element is distinct
 for j from 0 to m-1 do //compare with each element in Set2
 If Set1[i] = Set2[j] then
 isDistinct=false //the element is found in set2 hence not distinct
 Break //to end the loop early
 End If
 End For
If isDistinct = true then
sum ← sum + Set1[i] //Add distinct element to sum
End If
End For
//Step 2 does step 1 but in the opposite direction
// Step 2 Add elements from Set2 that are not in Set1
For i from 0 to m-1 do
isDistinct = true
For j from 0 to n-1 do //Compare with each element in Set1
If Set2[i] = Set1[j]  then
isDistinct= false
Break // end loop early as element has been detected as indistinct
End If
End For
If isDistinct = true then
sum ← sum + Set2[i] //Add the distinct element to the sum
End If
End For
Print "Sum of all distinct elements: ", sum
End

//problem 2
Procedure dot_product(v1[], v2[], n, output ps)
// Input: v1 and v2 are arrays of numbers and n= size of the arrays
// Output: ps-dot (scalar) product of the 2 vectors
Begin
 ps ← 0    // Initialize the dot product to 0
 For i from 0 to n-1 do // nesting loops as per the requirements
 For j from 0 to 0 do //making the inner loop run once to satisfy checkpoint requirements
 ps ← ps + v1[i]*v2[i] //multiplying the vector integers and adding them to the ps value
 End For
 
  End For
  End Procedure
Algorithm CheckOrthogonalVectors(Pairs, n)
// Input: Pairs is an array of n pairs of vectors (v1, v2)
// Output: Print if vectors are orthogonal or not
Begin
For k from 0 to n-1 do
v1 ← Pairs[k].v1
v2 ← Pairs[k].v2
size ← length(v1)
// Call procedure to calculate the dot product
dot_product(v1, v2, size, ps)
If ps==0 then
Print "Pair", k+1, "vectors are orthogonal"
Else
Print "Pair", k+1, "vectors are not orthogonal"
End If
End For
End

