# SearchSnake

### Final project for CSCI 4478 - Artificial Intelligence

*Developed by Ben Greenfield and Ben Placzek*

*Video presentation on this project can be found here:<br>
https://www.youtube.com/watch?v=hrMI7ppUGyU&ab_channel=LazyTech*

*Base code for snake game inspired by FreeCodeCamp.org's example at:<br>
 https://www.youtube.com/watch?v=CD4qAhfFuLo&t=1734s&ab_channel=freeCodeCamp.org*
 
 ### Goal:
 Our objective was to create a game of snake that would be able to play itself intelligently by using
 different search algorithms. We can create a scoring system so that we may analyze the performance of each algorithm.<br>
 **The algorithms we tested were:**
 1. Depth First Search
 2. Breadth First Search
 3. A Star Search
 4. Uniform Cost Search 

### Results:
After testing and compiling data, we found that BFS performed the best overall. This was determined by using our
scoring system which can represented by:
> finalScore = (score / actions) * 100

where score is the number of food eaten and actions is the sum of all actions taken until failure. We wanted
to prioritize score over actions, as an algorithm that gets a higher score shows more success over
basing it just on actions (i.e. DFS generates many actions, but a low score. DFS should be ranked lower
even though it has a lot of actions).

### How-to-use:
After downloading from the git repository, you can:

1. Run main()
	-Can play game of snake 
2. Run showExample()
	-Runs all searches at a slow speed
3. Run runMultiple(times) 
	-Calls runSearch for x times
	-Generates analytics based on every runSearch run
4. runSearch(times)
	-Runs every type of search for 400 iterations or until agent dies
	-Calculates weighted scores
	-Writes to results.txt file
	-Generates a single bar graph with scores
	-Generates 4 line plots with actions vs scores
	

