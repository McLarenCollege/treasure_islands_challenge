# Treasure Islands
You are a treasure hunter with a map of buried treasure on several islands.  You know the value of the treasure on each island, and the cost of travelling between islands.  The net profit is the total treasue minus the total cost of travel.

Note:
- **You must start and end at the 'Home' island**
- Travel costs are bi-directional.  ie. The cost of travelling directly from island `A` to island `B` is the same for `B` to `A`
- You can visit any location multiple times, but you will only get the treasure for that location once
- It may be that staying Home produces the maximum net profit (ie. all routes give negative profit)

Write a function `calculateProfit` which takes a list of locations and a list of travel costs, and calculates the maximum profit.

For example:

![map](./Treasure%20Islands.png)

Your code should look like this:

```js

let islands = [
    ['Kong Island', 800],
    ['Scar Island', 600],
    ['Home', 0],
    ['Isle of the Dead', 500],
    ['Monkey Island', 400]
];

let travelCosts = [
    ['Kong Island', 'Scar Island', 700],
    ['Kong Island', 'Isle of the Dead', 250],
    ['Isle of the Dead', 'Monkey Island', 250],
    ['Home', 'Isle of the Dead', 500],
    ['Scar Island', 'Monkey Island', 200],
    ['Home', 'Scar Island', 200],
    ['Home', 'Monkey Island', 300]
];

calculateProfit(islands, travelCosts); // should calculate the net profit


```



