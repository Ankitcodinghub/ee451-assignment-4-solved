# ee451-assignment-4-solved
**TO GET THIS SOLUTION VISIT:** [EE451 Assignment 4 Solved](https://www.ankitcodinghub.com/product/ee451-assignment-4-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;100472&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EE451 Assignment 4 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
1. Examples

Copy example files to your home directory.

1. Login to HPC 2. Copy

cp -r /project/xuehaiqi_652/examples .

3. Goto examples cd examples

The openmp_example.c contains the OpenMP implementation of matrix vector multi- plication.

<ol>
<li>Login to HPC</li>
<li>Compile
gcc -O3 -fopenmp openmp_example.c
</li>
<li>Run
The option -c specifies the number of CPUs allocated for a task. By default, the value is 1. For OpenMP program, the number of threads should equal the number of CPUs.
</li>
</ol>
The mpi_examples folder includes the source codes used in discussions. To run an mpi program, for example, the ‘scatter.c’, follow the steps:

</div>
</div>
<div class="layoutArea">
<div class="column">
srun -c8 ./a.out

</div>
</div>
<div class="layoutArea">
<div class="column">
1. Login to HPC

2. Setup MPI toolchain:

3. Compile

mpicc -O3 scatter.c

4. Run

</div>
</div>
<div class="layoutArea">
<div class="column">
module purge

module load intel/19.0.4 intel-mpi

</div>
</div>
<div class="layoutArea">
<div class="column">
srun –exclusive –mpi=pmi2 -n4 ./a.out

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
The option -n specifies the number of tasks (processes). By default, the value is 1. There is 1 task per node (machine), but note that the -c option will change this default.

2. Parallel Matrix Multiplication

Parallelize the naive matrix multiplication which you implemented in PA 1 using

OpenMP. Name the program as openmp.c. Take a screenshot.

<ul>
<li>The matrix size is 4K × 4K. Print out the execution time and the value of
C[100][100] in your program.
</li>
<li>Pass the number of threads p as a command line parameter [1].</li>
<li>Report the execution time for p = 1, 2, 4.
3. Pass Message in a Ring [50 points]

Write an MPI program that passes a value around 4 processes using the following steps.

Name this program as mpi.c. Take a screenshot.

<ol>
<li>Process 0 initializes Msg = 451 and prints value of Msg</li>
<li>Process 0 sends the value of Msg to Process 1</li>
<li>Process 1 receives the value of Msg, increases it by 1, prints the value and sends the current value of Msg to Process 2</li>
<li>Process 2 receives the value of Msg, increases it by 1, prints the value and sends the current value of Msg to Process 3</li>
<li>Process 3 receives the value of Msg, increases it by 1, prints the value and sends the current value of Msg to Process 0</li>
<li>Process 0 receives the value of Msg from Process 3 and prints the value</li>
</ol>
The output messages look like (Note that your code is still correct if the order of messages
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
is different):

• Process 0: Initially Msg = 451 • Process 1: Msg = 452

• Process 3: Msg = 454

• Process 2: Msg = 453

• Process 0: Received Msg = 454. Done!

</div>
</div>
</div>
