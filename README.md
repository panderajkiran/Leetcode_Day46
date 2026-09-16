# Leetcode_Day46
# Day 46 — Best Time to Buy and Sell Stock

**LeetCode Problem:** 121. Best Time to Buy and Sell Stock  
**Difficulty:** Easy  
**Language:** Java

## Problem

Given an array `prices`, where `prices[i]` represents the stock price on the `i`th day, find the maximum profit that can be achieved by buying on one day and selling on a different day in the future.

If no profit is possible, return `0`.

## Example

**Input:**
```text
prices = [7,1,5,3,6,4]
```
Output:

5

Explanation:

Buy at price 1 and sell at price 6.

Profit = 6 - 1 = 5

Approach

I used a single-pass approach.

Keep track of the minimum price seen so far.
For each day's price:
Update the minimum price if the current price is smaller.
Calculate the profit by subtracting the minimum price from the current price.
Keep track of the maximum profit found so far.
Return the maximum profit.

This works because we always buy at the lowest price seen before the current day and sell on the current day.

Complexity
Time Complexity: O(n)
Space Complexity: O(1)
What I Learned

Today I learned how a problem that looks like it requires checking many buy-and-sell combinations can be solved efficiently with just one traversal of the array.

The key idea is to remember the minimum value so far and use it to calculate the best possible profit at each step.

Takeaway

Sometimes we don't need to look back at everything.

Keeping track of just the right information while moving forward can make a solution both simple and efficient.

Another day, another problem solved.
Day 46 of staying consistent with DSA.
