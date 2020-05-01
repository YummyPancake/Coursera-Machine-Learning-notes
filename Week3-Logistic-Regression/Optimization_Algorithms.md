## Apply Optimization Algorithms to minimize the cost function <img src="http://latex.codecogs.com/gif.latex?J(\theta)" />

* Write a function to calculate <img src="http://latex.codecogs.com/gif.latex?J(\theta)" /> and <img src="http://latex.codecogs.com/gif.latex?\frac{\partial}{\partial\theta_i}J(\theta)" />

See the example in the costFunction.m

* Then use octave's 'fminunc()' optimization algorithm and the 'optimset()' function that creates an object containing the options sent to "fminunc()".

>options = optimset('GradObj', 'on', 'MaxIter', 100);  
>initialTheta = zeros(2,1)  
>[optTheta, functionVal, exitFlag] = fminunc(@costFunction, initialTheta, options)  

Then, you get this result:
![Image of result]
()
