#Day11 of My LeetCode Journey — Problem: Best Time to Buy and Sell Stock (Easy)

Today’s LeetCode challenge was all about maximizing profit in a stock trading scenario 📈

🧩 Problem Summary:
You're given an array prices where prices[i] represents the price of a stock on day i.

🎯 Goal:
 Pick a day to buy and a later day to sell, such that you maximize your profit.
 If no profit can be made, return 0.

🧠 My Approach:
This is a one-pass greedy algorithm:
Track the minimum price seen so far while iterating through the list.
At each day, calculate the potential profit if you sold on that day.
Update the maximum profit if this potential profit is greater than the previously recorded one.
This avoids checking all pairs (O(n²)) and instead runs in O(n) time and O(1) space ✅
🧮 Sample Test Case:
📥 Input: [7,1,5,3,6,4]
 ✅ Output: 5
 📈 Explanation: Buy at 1 (day 2), sell at 6 (day 5) → 6 - 1 = 5

💡 Key Takeaways:
Greedy problems can be optimized with a "track-as-you-go" mindset.
Keep track of min so far and max difference — a powerful pair.
Don’t overthink — brute force isn't always needed!
