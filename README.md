Download Link: https://assignmentchef.com/product/solved-coptimzation-problem-set-3
<br>



<strong>Convex Optimization</strong>




<strong>Problem 1. </strong>A Boolean linear program is an optimization problem of the form,

Minimize <em>c<sup>T</sup>x</em>

Subject to <em>Ax </em>= <em>b</em>

<em>x<sub>i </sub></em>∈ {0<em>,</em>1}

In general, such problems are very difficult to solve, even though the feasible set is finite.

<ul>

 <li>In a general method called relaxation, the constraint that <em>x<sub>i </sub></em>be zero or one is replaced with the linear inequalities 0 ≤ <em>x<sub>i </sub></em>≤ 1:</li>

</ul>

Minimize <em>c<sup>T</sup>x</em>

Subject to <em>Ax </em>= <em>b</em>

0 ≤ <em>x<sub>i </sub></em>≤ 1

We refer to this problem as the LP relaxation of the Boolean LP. The LP relaxation is far easier to solve than the original Boolean LP. Show that the optimal value of the LP relaxation is a lower bound on the optimal value of the Boolean LP. What can you say about the Boolean LP if the LP relaxation is infeasible?

<ul>

 <li>The Boolean LP can also be reformulated as the problem</li>

</ul>

Minimize <em>c<sup>T</sup>x</em>

Subject to <em>Ax </em>= <em>b</em>

<em>x<sub>i</sub></em>(1 − <em>x<sub>i</sub></em>) = 0

Find the Lagrange dual of this problem. The optimal value of the dual problem (which is convex) gives a lower bound on the optimal value of the Boolean LP. This method of finding a lower bound on the optimal value is called Lagrangian relaxation

<ul>

 <li>Show that the lower bound obtained via Lagrangian relaxation in part (b), and via the LP relaxation in part (a), are the same. Derive the dual of the LP relaxation.</li>

 <li>Can you describe an application for Boolean linear program?</li>

</ul>

<strong>Problem 2. </strong>Consider a quadratic programming (QP) described by,

Minimize

Subject to <em>Ax </em>≤ <em>b</em>

Assume that the matrix <em>P </em>is subject to errors, and the other parameters (<em>q,r,A,b</em>) are exactly known. The optimization problem with unknown matrix <em>P </em>is defined as,

Minimize sup                                                    (1)

Subject to <em>Ax </em>≤ <em>b</em>

where E is the set of possible matrices P.

<ul>

 <li>Let E be a finite set of matrices: E = {<em>P</em><sub>1</sub><em>, P</em><sub>2</sub><em>, …P<sub>k</sub></em>} with. Express the optimization problem (1) as an standard QCQP.</li>

 <li>Let E be described bywith Express the optimization problem</li>

</ul>

(1) as an standard QP.

<strong>Problem 3. </strong>The relative entropy between two vectors is defined as

This is a convex function, jointly in <em>x </em>and <em>y</em>. In the following problem we calculate the vector <em>x </em>that minimizes the relative entropy with a given vector <em>y</em>, subject to equality constraints on <em>x</em>:

Minimize

Subject to

<em>.</em>

The parameters  and <em>b </em>∈ R<em><sup>m </sup></em>are given. Derive the Lagrange dual of this problem and simplify it to get,

Maximize<em>,                                                          </em>(2)

where <em>a<sub>k </sub></em>is the <em>k</em>th column of <em>A</em>.

<strong>Problem 4. </strong>Source localization from range measurements: A signal emitted by a source at an unknown position <em>x </em>∈ R<em><sup>n </sup></em>(n = 2 or n = 3) is received by <em>m </em>sensors at known positions <em>y</em><sub>1</sub><em>,…y<sub>m </sub></em>∈ R<em><sup>n</sup></em>. From the strength of the received signals, we can obtain noisy estimates <em>d<sub>k </sub></em>of the distances k<em>x </em>− <em>y<sub>k</sub></em>k<sub>2</sub>. We are interested in estimating the source position <em>x </em>based on the measured distances <em>d<sub>k</sub></em>. In the following problem the error between the squares of the actual and observed distances is minimized:

Minimize

Introducing a new variable <em>t </em>= <em>x<sup>T</sup>x</em>, we can express this as

Minimize                                                     (3)

Subject to <em>t </em>= <em>x<sup>T</sup>x.</em>

Although this problem is not convex, it can be shown that strong duality holds. The objective of this problem is to solve (3) for an example with <em>m </em>= 5,

<em>,</em>

and

2

<strong>(a) </strong>To solve the problem, you can note that <em>x<sup>? </sup></em>is easily obtained from the KKT conditions for (3) if the optimal multiplier <em>ν<sup>? </sup></em>for the equality constraint is known. Derive the dual problem, express it as an SDP, and solve it using CVX (CVX can be downloaded from www.cvxr.com). <strong>(b) </strong>Reduce the KKT conditions to a nonlinear equation in <em>ν</em>, and pick the correct solution <strong>(c) </strong>Compare the results in part (a) and (b).

<h1>Matlab Assignment</h1>

<strong>Problem 5.</strong>

<ul>

 <li>Generate random instances of the problem 1 in part (a) and solve it using CVX for different values of <em>n</em>. Comment on the computational time varying <em>n</em>.</li>

 <li>Generate random instances of the problem 1 in part (b) and solve it using CVX for different values of <em>n</em>. Comment on the computational time varying <em>n</em>.</li>

</ul>

3