# TSP-2-Approximation-Visualization

## What?
We do know 2 things for sure: 
  * TSP (the travelling salesman problem) is np complete
  * there exists a polynomial 2-approximation (the approximation is max. twice as long)
  
What I didn't know: How well is the approximation on average or compared to a random choice?


## Quick results
### Approximation-Visualization
The image below shows the optimal solution for this metric tsp-input-problem along with the 2-approximation path.
![input](/Results/city9.png)


### Performance
We can compare the time differences between the optimal finder (expon.) and the approximtion (polyn.):

![input](/Results/time_optimal.png)
![input](/Results/time_approx.png)

For each city-size I repeated the computation 10 times and drew the curves for the results on average, for the best-, median- and worst-round.


### Error
Below are the error rates for each of the 10 input sizes (each repeated 10 times at random).

![input](/Results/cost_approx.png)
![input](/Results/cost_guess.png)

In my experiment, on 10 nodes we're still as good as the optimal solution, if we repeat the computation 10 times. On average, we have a 15% error rate. 

For comparision, I also plotted the results for just guessing a route (right): We optain a around 80% longer route on average (and the route can be longer as 2x optimum).
