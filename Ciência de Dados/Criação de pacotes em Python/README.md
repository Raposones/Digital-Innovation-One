# Romania Search

Romania Search is a college project for Artificial Intelligence subject, where you do a given search method to find and print the way the method goes through two cities in the Romania contry.

The start city is given by the user, but the destination is always Bucharest. You can use the following methods:

	- Breadth-first search
	- Depth-first search
    - Uniform-cost search
    - Greedy search
    - A* search

This project is based on this Romania map:

![rom_map](images/romania_map.png)

<br>

Also, for heuristic search purposes, we also have information based on this table, which shows us an approximate distance from Bucharest to a city:

![heuristic](images/h_dist.png)

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install romania_search

```bash
pip install romania_search
```

## Usage

Import **RomaniaMap.py** and use the *search* method, giving as parameters start city, search method. Additionally, you can use a third parameter as a boolean to determine if a colorful full path will be printed. Otherwise, only total distance will be displayed.

```python
from romania_search.romania_map import RomaniaMap

#Do a greedy search between Arad and Bucharest and print everything
RomaniaMap.search('Arad', 'greedy', True)

#Do a depth-first search through Zerind and Bucharest and print only total distance
RomaniaMap.search('Zerind', 'dfs')
```

Each search has it own string, so change the search parameter as follows:

	- Breadth-first search - 'bfs'
	- Depth-first search - 'dfs'
    - Uniform-cost search - 'c_unif'
    - Greedy search - 'greedy'
    - A* search - 'star'

## Author
Raphael Garcia

## License
[MIT](https://choosealicense.com/licenses/mit/)