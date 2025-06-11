Goal: You are given an integer amount representing a total amount of money and a list of integers coins representing the denominations of coins you have. You need to find the number of combinations of coins that sum up to the given amount. You have an infinite supply of each coin type.
Constraints:
* 0 <= amount <= 5000
* 1 <= coins.length <= 5000
* 1 <= coins[i] <= 5000
* The answer is guaranteed to fit into a signed 32-bit integer.
Input:
* amount: an integer
* coins: a list of integers
Output:
* An integer representing the number of combinations.
Examples:
1. Input: amount = 5, coins = [1, 2, 5] Output: 4 Explanation: There are four ways to make up the amount:
    * 5 = 5
    * 5 = 2 + 2 + 1
    * 5 = 2 + 1 + 1 + 1
    * 5 = 1 + 1 + 1 + 1 + 1
2. Input: amount = 3, coins = [2] Output: 0 Explanation: You can't make the amount 3 with just coins of denomination 2.
3. Input: amount = 10, coins = [10] Output: 1 Explanation: There is only one way to make the amount 10 with a coin of denomination 10.
Instructions for the Candidate:
Please write a Python function coinChange(amount, coins) that returns the number of combinations. Think about how you can build up the solution using the results for smaller amounts.