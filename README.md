# SIMULATION-OF-MEAN-AND-VARIANCE-USING-SCILAB

## AIM:
To write a program for mean, variance and cross correlation in SCILAB and verify the output.
## EQUIPMENTS Needed

•	Computer with i3 Processor
•	SCI LAB

# Algorithm

1.	Define	the	Function:	Specify the	function	you	want	to	simulate.	For	example, f(x)=sin⁡(x)f(x) = \sin(x)f(x)=sin(x) or any other function.
2.	Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.
3.	Evaluate the Function: Compute the function values at each of these sample points.
4.	Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.
5.	Display Results: Output the computed mean variance and Cross Correlation 
# PROCEDURE
•	Refer Algorithms and write code for the experiment.
•	Open SCILAB in System
•	Type your code in New Editor
•	Save the file
•	Execute the code
•	If any Error, correct it in code and execute again
•	Verify the generated results
# PROGRAM
```
clear;
clc;
clear;
function X=f(x)
    z=3*(2-x)^2
    X=x*z
endfunction
a=0;
b=1;
EX=intg(a,b,f);
function Y=c(y)
    z=3*(2-y)^2
    Y=y*z
endfunction
EY=intg(a,b,c);
disp(EX,"i)Mean of X=")
disp(EY,"Mean of Y=")
function X=g(x)
    z=3*(2-x)^2
    X=x^2*z
endfunction
a=0;
b=1;
EX2=intg(a,b,g);
function Y=h(y)
    z=3*(2-y)^2
    Y=y^2*z
endfunction
EY2=intg(a,b,h);
vX2=EX2-(EX)^2;
vY2=EY2-(EY)^2;
disp(vX2,"ii) Variance of X");
disp(vY2,"Variance of Y");
x=[1 3 4 6 7 2 9 8];
y=[2 5 8 4 6 1 7 3];
n1=max(size(y))-1;
n2=max(size(x))-1;
r=corr(x,y,n1);
plot2d3('gnn',r);

```
# TABULATION
<img width="982" height="1600" alt="image" src="https://github.com/user-attachments/assets/ffff3d73-55de-4281-89bc-4ee0d9dd692f" />

# CALCULATION
<img width="1600" height="1508" alt="image" src="https://github.com/user-attachments/assets/c827e94b-d5ef-44e0-b3e5-b535b018c76e" />
<img width="988" height="1600" alt="image" src="https://github.com/user-attachments/assets/955a551a-99e2-4ac3-b7a9-3b7244008496" />

# OUTPUT

<img width="1064" height="1533" alt="image" src="https://github.com/user-attachments/assets/32d00d8b-31a4-4065-a582-1760e69abb6e" />

# RESULT

Thus, the mean , variance and cross correlation are executed in scilab sucessfully.


