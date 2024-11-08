# Program-4: Trapezoidal rule

## Question:

Evaluate $$\int_0^1 \frac{dx}{1 + x^2} $$ using the trapezoidal rule with $$h = 0.2$$.

## Aim:

To compute given definite integral by using trapezoidal rule

## Algorithm:

Step 1: Define the function $$f(x) = 1 / (1 + x ** 2)$$ 

Step 2: Define the values of a,b,h.

Step 3: Compute n = $$(b - a) / h$$

Step 4: Assign Sum = 0
      - for i = 1 to n
      - $$Sum = sum + f(a + i x h)$$
      - $$trep = h/2 * ( f(n) + f(b) + 2 * sum)$$

Step 5: Print the integral value

## Program:
```
def f(x):
 return 1/(1+x**2)
a=float (input ("Enter the lower limit: "))
b=float (input ("Enter the upperlimit: "))
h=float (input ("Enter the step size: "))
n=int((b-a)/h)
sum=0
for i in range (1, n):
 sum=sum+f(a+i*h)
trap=h/2*(f(a)+f(b)+2*sum)
print ("The Integral value is %.5f"%trap)
```
## Output:

Enter the lower limit: 0

Enter the upperlimit: 1

Enter the step size: 0.2

The Integral value is 0.78373 

## Result:
The value of given definite integeral is obtained
