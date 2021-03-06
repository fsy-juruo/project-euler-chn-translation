### [683. The Chase II](https://projecteuler.net/problem=683)

Consider the following variant of "The Chase" game. This game is played between $n$ players sitting around a circular table using two dice. It consists of $n-1$ rounds, and at the end of each round one player is eliminated and has to pay a certain amount of money into a pot. The last player remaining is the winner and receives the entire contents of the pot.

At the beginning of a round, each die is given to a randomly selected player. A round then consists of a number of turns.

During each turn, each of the two players with a die rolls it. If a player rolls a 1 or a 2, the die is passed to the neighbour on the left; if the player rolls a 5 or a 6, the die is passed to the neighbour on the right; otherwise, the player keeps the die for the next turn.

The round ends when one player has both dice at the beginning of a turn. At which point that player is immediately eliminated and has to pay $s^2$ where $s$ is the number of completed turns in this round. Note that if both dice happen to be handed to the same player at the beginning of a round, then no turns are completed, so the player is eliminated without having to pay any money into the pot.

Let $G(n)$ be the expected amount that the winner will receive. For example $G(5)$ is approximately 96.544, and $G(50)$ is 2.82491788e6 in scientific notation rounded to 9 significant digits.

Find $G(500)$, giving your answer in scientific notation rounded to 9 significant digits.

### 683. 追逐游戏 2

以下描述的是追逐游戏的一个变种，$n$ 位玩家围坐圆桌边，通过掷骰子来玩这个游戏。这个游戏共分 $n-1$ 轮，每一轮结束后，将由一名玩家被淘汰，并且需要向奖池里投入一定量的钱。存活到最后的人获胜，达到奖池里的所有钱。

每一轮开始时，两个骰子将分别随机分配给一名玩家。每一轮又由若干次操作组成。每次操作时，两名手持骰子的玩家掷出手里的骰子，如果掷出 1、2，这名玩家就将骰子传给他左边的玩家；如果掷出 5、6，这名玩家就将骰子传给他右边的玩家；否则这名玩家需要将骰子留着。

如果一名玩家同时持有两颗骰子，本轮结束，这名玩家被淘汰，并且需要向奖池内投入 $s^2$ 元，其中 $s$ 是这一轮的操作数。如果一名玩家太非了，在一轮开始时就拿到两颗骰子，那这名玩家即刻淘汰，并且一分钱也不用出。

令 $G(n)$ 为玩家数量为 $n$ 时，胜者从奖池内得到的钱的期望值。$G(5)$ 约等于 96.544，$G(50)$ 在科学计数法下保留 9 位有效数字时，等于 2.82491788e6。

求出 $G(500)$，将你的答案用科学计数法表示，保留 9 位有效数字。
