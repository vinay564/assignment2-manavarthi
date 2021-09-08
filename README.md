# assignment2-manavarthi

## Vinay Manavarthi
### My favorite place is my village which is Jaddangi <br>

My village is a place that I like to visit in my holidays or whenever I feel tired and want to relax. A village is a place that is far away from the __pollution__ and __noise__ of the city. Also, you feel a connection with the soil in a village. Moreover, there are trees, a variety of crops, diversity of flowers, and rivers, etc. Besides all this, you feel the cold breeze at night and a warm but pleasant breeze in the day.

---

## Navigation to my Village

1. Go to Kansas Airport from Maryville.
    1. get the boarding pass.
2. Book flight ticket from  Kansas to Chicago.
    1. Ready to board the flight.
3. and Chicago to London.
    1. London to Dubai.
    2. Dubai to Hyderabad.
    3. Hyderabad to Rajahmundry.
4. travel Rajahmundry to Jaddangi by car.


* Items bought for enjoyment 
    * Playing Cards
    * Drinks
    * Food


[Click here to know About Me](AboutMe.md)

 ---
## Table

Food/Drinks that i recommend someone

| Food/Drink | Location | Money |
| -----------| -------- | ----- |
| Burger | Burgewr King | $3.00 |
|Chicken Burger | McDonald | $2.50 |
| French Fries | McDonald | $1.50 |
| Drink | Sonic | $1.00 |

---

## Quotes

> Winners don't do different things, They do things differently  *Shiva  Khera* 

> No one will believe in you until you believe in you  *Robin Sharma*


---

## Code Fencing

Graphs Flows/Matchings/Misc

>The algorithm takes as input an unweighted graph and the id of the source vertex s. The input graph can be directed or undirected, it does not matter to the algorithm.

>The algorithm can be understood as a fire spreading on the graph: at the zeroth step only the source s is on fire. At each step, the fire burning at each vertex spreads to all of its neighbors. In one iteration of the algorithm, the "ring of fire" is expanded in width by one unit (hence the name of the algorithm).

>More precisely, the algorithm can be stated as follows: Create a queue q which will contain the vertices to be processed and a Boolean array used[] which indicates for each vertex, if it has been lit (or visited) or not.

Breadth-first search algorithm [Reference_link](https://en.wikipedia.org/wiki/Breadth-first_search)

code for Breadth-first search

vector<vector<int>> adj;  // adjacency list representation
int n; // number of nodes
int s; // source vertex

queue<int> q;
vector<bool> used(n);
vector<int> d(n), p(n);

q.push(s);
used[s] = true;
p[s] = -1;
while (!q.empty()) {
    int v = q.front();
    q.pop();
    for (int u : adj[v]) {
        if (!used[u]) {
            used[u] = true;
            q.push(u);
            d[u] = d[v] + 1;
            p[u] = v;
        }
    }

Breadth-first search algorithm [Code_link](https://cp-algorithms.com/graph/breadth-first-search.html)
