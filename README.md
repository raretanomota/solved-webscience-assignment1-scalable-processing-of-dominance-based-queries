Download Link: https://assignmentchef.com/product/solved-webscience-assignment1-scalable-processing-of-dominance-based-queries
<br>
In this project, you will work with multi-dimensional data. Given a potentially large set of <em>d</em>-dimensional points, where each point is represented as a <em>d</em>-dimensional vector, we need to detect <u>interesting</u> points. The project is based on the concept of <strong>dominance</strong>. We say that a point p dominates another point q, when p is as good as <em>q</em> in all dimensions and it is strictly better in at least one dimension. We will assume that small values are preferable. For example, the point <em>p</em>(1, 2) dominates <em>q</em>(3, 4) since 1 &lt; 3 and 2 &lt; 4. Also, <em>p</em>(1, 2) dominates <em>q</em>(1, 3) since although the have the same <em>x</em> coordinate, the <em>y</em> coordinate of <em>p</em> is smaller than that of <em>q</em>. There are three different tasks you need to complete:

<strong>Task1.</strong> Given a set of <em>d</em>-dimensional points, return the set of points <u>that are not dominated</u>. This is also known as the <strong>skyline</strong> set.

<strong>Task2.</strong> Given a set of <em>d</em>-dimensional points, return the <em>k</em> points with the highest dominance score. The dominance score of a point <em>p</em> is defined as the total number of points dominated by <em>p</em>.

<strong>Task3.</strong>  Given a set of <em>d</em>-dimensional points, return the <em>k</em> points from the skyline with the highest dominance score.

Figure 1. Example of a top-3 dominating query.

An example is shown in Figure 1. The dominating region of the top-1 point is shown gray. Any point that falls inside this region is dominated by top-1. Based on the Figure the top-1 point has a domination score of 8, since it dominates 8 other points.

<h1>Requirements</h1>

Given a dataset of <em>d</em>-dimensional points you should implement scalable and efficient algorithms to solve the aforementioned tasks. Your algorithm must be implemented in the Scala programming language and you should use Apache Spark. Note that the parameter <em>d</em> (number of dimensions) depends on the dataset whereas the parameter <em>k</em> is user-defined and must be given as an input to the algorithm (for Task2 and Task3). The point coordinates in general may be double numbers, so you should treat coordinate values as doubles. You should provide results for different values of <em>k</em>, different dimensionalities, different data distributions and different data cardinalities. (<strong>Tip</strong>: <em>start with a small 2-dimensional dataset in order to be able to check if your algorithm provides the correct results</em>.). Examples of data distributions in the 2-d space are given in Figure 2.

<strong>Figure 2</strong>. Different distributions for 2-d (from left to right): correlated, uniform, normal, anticorrelated.

<h1>Deliverables</h1>

You should deliver the source code of your solution, the code to generate the data distributions and a report describing what you did, in detail. Also, you need to prepare 9-10 slides for the presentation session that will take place at the end of the semester. Note that, the code for data generation can be in another programming language, e.g., Java, Python or anything you prefer. However, the code for your solution must be in Scala over Spark.

<strong>Bibliography </strong><a href="http://www4.comp.polyu.edu.hk/~csmlyiu/journal/vldbj_kdom.pdf">http://www4.comp.polyu.edu.hk/~csmlyiu/journal/vldbj_kdom.pdf </a><a href="http://delab.csd.auth.gr/~apostol/pubs/isps2015_tpm.pdf">http://delab.csd.auth.gr/~apostol/pubs/isps2015_tpm.pdf </a><a href="https://link.springer.com/article/10.1007/s11280-015-0340-6">https://link.springer.com/article/10.1007/s11280-015-0340-6 </a><a href="http://www.cs.ucr.edu/~ravi/CS236Papers/skyline-operator.pdf">http://www.cs.ucr.edu/~ravi/CS236Papers/skyline-operator.pdf </a><a href="https://link.springer.com/article/10.1007/s00778-011-0246-6">https://link.springer.com/article/10.1007/s00778-011-0246-6</a>