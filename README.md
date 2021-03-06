# Groove Rivercrossing
This project contains a solution for the missionary and cannibal problem. It was implemented by using [Groove](https://sourceforge.net/projects/groove/).

### Missionary and cannibal problem
Three missionaries and three cannibals are standing next to a river. They want to get all to the other side, but they always need someone that can row. All three missionaries are able to row. There is also one cannibal that is able to row. Cannibals are actually pretty friendly people, but if there are more cannibals than missionaries on one side their hunger overcomes their rationality.

### Solution
The following table describes a possible solution with the applied grammar-rules.  
๐งโโ๏ธ = Missionary, ๐งโโ๏ธ = Cannibal, ๐ฃโโ๏ธ = Cannibal that can row

| ๐ | ๐ | โต | ๐ | ๐งพ
| :---: | :---: | :---: | :---: | :---: |
| 0 | ๐งโ๐งโ๐งโ๐งโ๐งโ๐ฃโ |  |  | load |
| 4 | ๐งโโ๏ธ๐งโ๐งโ๐ฃโโ๏ธ | ๐งโ๐งโโ๏ธ |  | unload-two |
| 8  |๐งโโ๏ธ๐งโ๐งโ๐ฃโโ๏ธ |  | ๐งโ๐งโ | load |
| 14 |๐งโโ๏ธ๐งโ๐งโ๐ฃโโ๏ธ  |๐งโโ๏ธ | ๐งโ | unload-one |
| 21 |๐งโโ๏ธ๐งโโ๏ธ๐งโ๐งโ๐ฃโโ๏ธ |  | ๐งโ | load |
| 30 |๐งโโ๏ธ๐งโโ๏ธ๐งโ | ๐งโ๐ฃโ  | ๐งโ | unload-two |
| 33 |๐งโโ๏ธ๐งโโ๏ธ๐งโ |  |  ๐งโโ๏ธ๐งโโ๏ธ๐ฃ | load |
| 35 |๐งโโ๏ธ๐งโโ๏ธ๐งโ | ๐ฃโโ๏ธ | ๐งโ๐งโ | unload-one |
| 36 |๐งโโ๏ธ๐งโโ๏ธ๐งโ๐ฃโโ๏ธ |  |  | load |
| 38 |๐งโ๐ฃโโ๏ธ | ๐งโ๐งโ | ๐งโ๐งโ  | unload-two |
| 41 |๐งโ๐ฃโโ๏ธ |  | ๐งโ๐งโ๐งโ๐งโ  | load |
| 45 |๐งโ๐ฃโโ๏ธ  | ๐งโโ๏ธ๐งโโ๏ธ | ๐งโ๐งโโ๏ธ | unload-two |
| 46 |๐งโ๐งโ๐งโโ๏ธ๐ฃโ  |  | ๐งโ๐งโโ๏ธ | load  |
| 49 |๐งโ๐งโโ |๐งโโ๏ธ๐ฃ | ๐งโ๐งโโ๏ธ | unload-two |
| 54 |๐งโ๐งโโ |  |๐งโโ๏ธ๐งโ๐งโโ๏ธ๐ฃโ | load |
| 62 |๐งโ๐งโโ |๐งโ๐งโโ   |๐งโโ๏ธ๐ฃโ  | unload-two |
| 67 |๐งโ๐งโ๐งโ๐งโ |  | ๐งโโ๏ธ๐ฃโ  | load |
| 72 |๐งโ๐งโ  |๐งโโ๏ธ๐งโโ๏ธ  |๐งโโ๏ธ๐ฃโ  | unload-two |
| 74 |๐งโโ๏ธ๐งโโ๏ธ  |  |๐งโโ๏ธ๐งโโ๏ธ๐งโ๐ฃโโ๏ธ  | load |
| 78 |๐งโ๐งโ | ๐ฃโ |๐งโ๐งโ๐งโ  | unload-one |
| 80 |๐งโ๐งโ๐ฃโ  |  |๐งโ๐งโ๐งโ  | load |
| 81 |๐งโ  |๐งโ๐ฃโ   |๐งโ๐งโ๐งโ    | unload-two |
| 83 |๐งโ   |  |๐งโ๐งโ๐งโ๐งโ๐ฃโ | load |
| 84 |๐งโ    | ๐งโโ๏ธ | ๐งโ๐งโ๐งโโ๏ธ๐ฃโ  | unload-one |
| 90 |๐งโ๐งโโ๏ธ    |  |๐งโ๐งโ๐งโโ๏ธ๐ฃโ   | load |
| 92 |  |๐งโ๐งโโ๏ธ   |๐งโ๐งโ๐งโโ๏ธ๐ฃโ  | unload-two |
| 96 |  |  |๐งโโ๏ธ๐งโโ๏ธ๐งโ๐งโ๐งโ๐ฃโโ๏ธ | final |
