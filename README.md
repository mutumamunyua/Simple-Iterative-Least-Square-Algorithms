# Simple-Iterative-Square-Algorithms
Simple Iterative Square Algorithms with two unknown variables in the same equation

Given Equation (1) and data with variables y, d and m, I want to estimate α(αis between 0 and 1) through iterative square approach because β  in Equation (2) also contains the unknown estimate α
	 		log(y)=c-βlog⁡(d+2αm/(1-α))
Where  
            2)        β=2/(1-α)

Steps for solving Iterative Square approach algorithms are,
	Starts with an initial guess of  α,e.g.,(α_0).
	Regress (1) with initial(α_0)  in place to get the parameter estimate β that is used to calculate a new (α_1).
	Use estimate βon (2) to calculate a new (α_1)
	Use α_1as the “new guess” and repeat steps 2 and 3 until the initial and new αconverge.

I develop the following R-code that follows the 4 steps. However, I would like to loop in steps 2 and 3 and stop the process after convergence (or near convergence-a little tolerance lance levels)  
