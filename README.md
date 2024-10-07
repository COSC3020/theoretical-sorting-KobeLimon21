# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

This seems like it would be quite the generational find if this is possible. I would use the black box to test a variety of different cases such as reverse sorted, empty and a wide variety of different inputs. On the same note on inputs, I would run the same input various times to ensure consistency and as well as using large inputs to see how it performs on a large scale. I would also incorporate a graph and compare it with the speeds of our other algorithms as it should surpass our known fast algorithms such as quicksort or mergesort. Also within our graph, we would expect the the execution time to grow linearly as the input size increases where our very large inputs in the blackbox would make or break this. 

I don't believe this is possible since from what we discussed in class as our lower bound for these algorithms is O(nlogn). This is because we sort two objects at once when we use these algorithms, this can be modeled like the tree in the slides where we have a "choice point" for the two elements. The tree must be able to account for all the leafs possible in array n, or else the algorithm would not be able to sort as the height of tree would be atleast log(n!). This algorithm suggests that it would be able to sort it without having to go through the minimum "choice points" to reach a sorted array. 

Sources:
slides from powerpoint

"I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice."



Add your answers to this markdown file.
