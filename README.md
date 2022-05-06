# Groove Rivercrossing
This project contains a solution for the missionary and cannibal problem. It was implemented by using [Groove](https://sourceforge.net/projects/groove/).

### Missionary and cannibal problem
Three missionaries and three cannibals are standing next to a river. They want to get all to the other side, but they always need someone that can row. All three missionaries are able to row. There is also one cannibal that is able to row. Cannibals are actually pretty friendly people, but if there are more cannibals than missionaries on one side their hunger overcomes their rationality.

### Solution
The following table describes a possible solution with the applied grammar-rules.  
🧙‍♂️ = Missionary, 🧟‍♂️ = Cannibal, 🚣‍♂️ = Cannibal that can row

| 🔄 | 👈 | ⛵ | 👉 | 🧾
| :---: | :---: | :---: | :---: | :---: |
| 0 | 🧙‍🧙‍🧙‍🧟‍🧟‍🚣‍ |  |  | load |
| 4 | 🧙‍♂️🧙‍🧟‍🚣‍♂️ | 🧙‍🧟‍♂️ |  | unload-two |
| 8  |🧙‍♂️🧙‍🧟‍🚣‍♂️ |  | 🧙‍🧟‍ | load |
| 14 |🧙‍♂️🧙‍🧟‍🚣‍♂️  |🧙‍♂️ | 🧟‍ | unload-one |
| 21 |🧙‍♂️🧙‍♂️🧙‍🧟‍🚣‍♂️ |  | 🧟‍ | load |
| 30 |🧙‍♂️🧙‍♂️🧙‍ | 🧟‍🚣‍  | 🧟‍ | unload-two |
| 33 |🧙‍♂️🧙‍♂️🧙‍ |  |  🧟‍♂️🧟‍♂️🚣 | load |
| 35 |🧙‍♂️🧙‍♂️🧙‍ | 🚣‍♂️ | 🧟‍🧟‍ | unload-one |
| 36 |🧙‍♂️🧙‍♂️🧙‍🚣‍♂️ |  |  | load |
| 38 |🧙‍🚣‍♂️ | 🧙‍🧙‍ | 🧟‍🧟‍  | unload-two |
| 41 |🧙‍🚣‍♂️ |  | 🧙‍🧙‍🧟‍🧟‍  | load |
| 45 |🧙‍🚣‍♂️  | 🧙‍♂️🧟‍♂️ | 🧙‍🧟‍♂️ | unload-two |
| 46 |🧙‍🧙‍🧟‍♂️🚣‍  |  | 🧙‍🧟‍♂️ | load  |
| 49 |🧙‍🧟‍♂ |🧙‍♂️🚣 | 🧙‍🧟‍♂️ | unload-two |
| 54 |🧙‍🧟‍♂ |  |🧙‍♂️🧙‍🧟‍♂️🚣‍ | load |
| 62 |🧙‍🧟‍♂ |🧙‍🧟‍♂   |🧙‍♂️🚣‍  | unload-two |
| 67 |🧙‍🧙‍🧟‍🧟‍ |  | 🧙‍♂️🚣‍  | load |
| 72 |🧟‍🧟‍  |🧙‍♂️🧙‍♂️  |🧙‍♂️🚣‍  | unload-two |
| 74 |🧟‍♂️🧟‍♂️  |  |🧙‍♂️🧙‍♂️🧙‍🚣‍♂️  | load |
| 78 |🧟‍🧟‍ | 🚣‍ |🧙‍🧙‍🧙‍  | unload-one |
| 80 |🧟‍🧟‍🚣‍  |  |🧙‍🧙‍🧙‍  | load |
| 81 |🧟‍  |🧟‍🚣‍   |🧙‍🧙‍🧙‍    | unload-two |
| 83 |🧟‍   |  |🧙‍🧙‍🧙‍🧟‍🚣‍ | load |
| 84 |🧟‍    | 🧙‍♂️ | 🧙‍🧙‍🧟‍♂️🚣‍  | unload-one |
| 90 |🧙‍🧟‍♂️    |  |🧙‍🧙‍🧟‍♂️🚣‍   | load |
| 92 |  |🧙‍🧟‍♂️   |🧙‍🧙‍🧟‍♂️🚣‍  | unload-two |
| 96 |  |  |🧙‍♂️🧙‍♂️🧙‍🧟‍🧟‍🚣‍♂️ | final |
