# Treasure Islands
You are a treasure hunter with a map of buried treasure on several islands.  You know the value of the treasure on each island, and the cost of travelling between islands like this:

![map](./TreasureIslands.png)

Write a function which takes a list of locations and a list of travel costs, and calculates the maximum profit:

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
    ['Home', 'Monkey Island', 200]
];

calculateProfit(islands, travelCosts); // should calculate the net profit


```



### Notes
- You can visit any location multiple times, but you will only get the treasure for that location once
- You must start and end at the 'Home' location
