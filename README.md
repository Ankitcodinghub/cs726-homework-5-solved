# cs726-homework-5-solved
**TO GET THIS SOLUTION VISIT:** [CS726 Homework #5 Solved](https://www.ankitcodinghub.com/product/cs-726-homework-5-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117549&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS726 Homework #5 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
Please typeset or write your solutions neatly! If we cannot read it, we cannot grade it.

Note: You can use the results we have proved in class – no need to prove them again. To implement Euclidean projections onto simplex, you can use the provided ProjectOntoSimplex.m and ProjectOntoEllOneBall.m files (available under ’Files’ on Canvas). If you are coding in Python, you can find similar implementations online (for example, take a look at https://gist.github.com/daien/1272551/edd95a6154106f8e28209a1c7964623ef8397246).

The same rules as in previous homework assignments regarding the use of Python for coding apply.

Your code needs to compile without any errors to receive any points. You need to justify all your answers.

Q 1 (The importance of choosing the appropriate geometry). In this question, you are asked to implement Projected Gradient Descent and Mirror Descent to solve the following problem:

, (P)

where X = {x ∈ Rn : x ≥ 0, 1Tx = 1} is the probability simplex and f is defined by:

, (1)

where zi are independent Rademacher vectors. Namely, ∀i,j ∈ {1,…,n}, zji = +1 with probability and zji = −1 with probability , independently over i,j ∈ {1,…,n}.

Is (P) a convex optimization problem? Justify your answer.

What is the Lipschitz constant M2 of f with respect to k·k2? What is the Lipschitz constant M1 of f with respect to k · k1? (We will accept answers that just bound one of the subgradients at each of the possible query points, in the appropriate norm.) What is D2 = maxx,y∈X kx − yk2? What is D1 = maxx,y∈X kx − yk1?

The variant of Mirror Descent you should implement will use the negative entropy regularizer

(see the previous homework assignment for the definition of Mirror Descent). Note that this ψ(x) is 1-strongly convex with respect to the `1 norm (you don’t need to prove this). Note also that the iterates of the Mirror Descent algorithm can be written in closed form for this choice of ψ. Write the formula for the iterates xk+1 of Mirror Descent explicitly as a function of the step size ak, previous iterate xk, and a subgradient gxk of f at xk. Prove that the formula for xk+1 is invariant to translation of akgxk, meaning that it gives the same result for akgxk and akgxk + C1, for any constant C ∈ R. This is important for numerical stability of your algorithm – for the algorithm not to encounter numerical issues, you will want to compute xk+1 using akgxk + C1, with C = −ak min1≤i≤n(gxk)i.

You should initialize both methods at x . What is maxu∈X Dψ(u,x0)?

To implement the methods, you should take√ n = 500 and run them for K = 2000 iterations. Your step sizes should

be ai = 1/(M i), where M ∈ {M1,M2} is the appropriate Lipschitz constant for each of the two methods. Your code should output two plots, comparing the function values of the two methods aginst the iteration count. The first plot should use function evaluations at individual iterates/query points of the algorithms xi. The second plot should use function evaluations at the algorithm’s output points . Discuss your results. What can you conclude from the first plot? Now observe the second plot. Which algorithm is faster? Use the theoretical results we derived in the last homework and in class to explain why.

Q 2 (Comparing Frank-Wolfe and PGD). In this question, you are asked to compare the Frank-Wolfe method we saw in class to Projected Gradient Descent, on the following problem instance:

,

1

where X = {x ∈ Rn : kxk1 ≤ 1} is the `1 ball and is a quadratic function defined by: (i) B, an p × n matrix whose entries are i.i.d. Gaussian with mean zero and variance one, where n = 200 and p = 10; and (ii) b ∈ Rp is the vector of all 1’s.

What are the vertices of X? How do you compute vk = argminu∈X{h∇f(xk),u − xki}? Write it in closed form. For PGD, you can use the provided code to implement projections onto X.

Run both algorithms 30 times for 300 iterations. You should initialize both algorithms at x0 = e1, where e1 is the first basis vector. Your code should output a plot that shows against the iteration count for PGD and the

Frank-Wolfe algorithm averaged over 30 independent runs. Discuss the results. Do you see what you expect from the theoretical results we derived in class?

You should also consider, for each of the algorithms, the solution points at the first iteration for which

10−1. Your code should output the average sparsity (number of nonzero elements) of these points for both algorithms, over 30 independent runs. Which of the two algorithms constructs sparser solutions (solutions with fewer nonzero elements)? Can you explain why?

Q 3 (First-order methods in the presence of gradient noise). In this question, you should implement three algorithms: (i) Nesterov’s AGD, (ii) standard gradient descent with step size√ 1/L, and (iii) (projected) stochastic gradient descent

with averaging (from class) with the step size ak = 1/(L k). Your algorithms should not work with the exact gradients; instead, you should implement them with “noisy” gradient oracles g(x,ξ) = ∇f(x) + εξ, where ξ are vectors with i.i.d. mean-zero variance-one Gaussian elements, and ε is an algorithm parameter.

The problem instance is Mx − bTx, where M ∈ Rn×n is a tridiagonal matrix with 2’s on the main diagonal and -1’s on the remaining two diagonals (as in previous problem sets) and b = e1. Your algorithms should all be initialized at x = 0.

Your code should output three plots, produced for three different values of ε : (i) ε = 10−5, (ii) ε = 10−3, and (iii) ε = 10−1. In all the plots, n = 200. Each plot should show the optimality gap (on a log scale) against the iteration count, for all three algorithms.

Discuss your results. What do you observe? Which algorithm is fastest? Which one is the most stable? Which one would you use in practice, under what circumstances, and why?

2
