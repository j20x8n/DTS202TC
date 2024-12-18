java c

Module code and Title 
DTS202TC Foundation of Parallel Computing 
School Title 
School of AI and Advanced Computing 
Assignment Title 
Individual Assessment 2 
Submission Deadline 
Friday Dec. 20th, 2024 @ 11:59pm 
Final Word Count 
N/A 
DTS202TC Foundation of Parallel Computing 
Individual Coursework   2 
Assessment Overview The   purpose of   this   assignment   is   to   provide   hands-on   experience with   parallel   programming   and   performance   analysis. You   are   expected   to implement   two   C programs   that   apply   a blur   effect   to   a   grayscale image using two distinct parallelism techniques.   The goal is to understand the   differences   between   the   techniques   in   terms   of   implementation   complexity, execution speed, and scalability.   Through this exercise, you   will develop skills   in   writing   parallel code, optimizing algorithms   for   parallel execution, and analyzing the   performance gains achieved   by   parallelizing computational   tasks.
Learning Outcomes 
.      C. Devise and implement parallel   algorithms
.   D. Acquire basic   software development   skill using MPI
.   E.      Analyze and implement common parallel algorithm patterns in a parallel programming   model   such as   CUDA.
.   F. Design experiments to analyze the performance bottlenecks in their   parallel   code.
.      G. Apply common parallel techniques to improve performance given hardware   constraints.
.   H. Use a parallel debugger to identify and repair code defects; Use a parallel   profiler   to   identify   performance bottlenecks in their code.
.   J.   Demonstrate   understanding   of   the   major   types   of   hardware   limitations   that   limit   parallel   program performance.
Avoid Plagiarism 
.   Do not submit work from   others.
.   Do not share code   or work   to   other   students.
.   Do not read   code   or work   from   others,   discussions between   teams   should be   limited   to   high   level   only.
.   Do not use open-source   code.
Tasks Image blurring is one of the   most   common   image   processing algorithms (right plot).   A   simplest way   to blur   an   image   is   to   set   each   pixel   to   the   mean   of   its   neighbour   pixels.         One of   the   problems of   this algorithm is that   the   effect may   not be visible   for    large    images, to solve this, we can repeat   the   process   multiple   times.    For   our   coursework,   please repeat the mean process 20 times.
Reading and Writing Image You   will   need   to   read   a   PGM   image,   process   the   blurring,   then   write   the   blurred   PGM   image   back   to the file system. Plain PGM format is a simple grayscale graphic image format, each pixel is   represented by its grey value number, with   0 being black   and   Maxval   (defined   in   the   PGM   file)   being   white.   The below image.pgm is given as an example,   more   deta代 写DTS202TC Foundation of Parallel ComputingR
代做程序编程语言il   pgm   specifications   can be   found   athttp://davis.lbl.gov/Manuals/NETPBM/doc/pgm.html
image.pgm
P2
24 7
15
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
0 3 3 3 3 0 0 7 7 7 7 0 0 11 11 11 11 0 0 15 15 15 15 0
0 3 0 0 0 0 0 7 0 0 0 0 0 11 0 0 0 0 0 15 0 0 15 0
0 3 3 3 0 0 0 7 7 7 0 0 0 11 11 11 0 0 0 15 15 15 15 0
0 3 0 0 0 0 0 7 0 0 0 0 0 11 0 0 0 0 0 15 0 0 0 0
0 3 0 0 0 0 0 7 7 7 7 0 0 11 11 11 11 0 0 15 0 0 0 0
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
1       Parallel implementations (25 points for each implementation) Each   student is required to implement two different parallel   programs:   one using   MPI   and   the   other   using a different parallel technique such   as   Pthreads,   OpenMP,   or   CUDA.   It   is   important   to   note   that   you only need to focus on   optimizing the   core   algorithm for   speedup.
2 Performance analysis (30 points) 
Analyse   the   performances   of   two   parallel   implementations,   including   speedup   and   efficiencies   (15 points).
You should provide line plots to represent the results, including   serial runtime, runtime   of   different   processes, speedup and   efficiencies.   (5 points).Compare   and   contrast   the   two implementations   (Performance Metrics, Hardware limitation, Ease   of   Debugging   and   Testing,   Communication   and   Synchronization,   or   any   other   aspects   you   can   think   of), choose your preferred parallel technique and justify your choice (10 points).
3 Reflection (10 points) 
Did you face any challenges during the   implementation?   How   did you   solve   them?
4 Submission (10 points) 
You   should   submit the following files   in   a   zip:
. blur_mpi/pthread/openmp.c Your parallel implementations.
.   A Makefile that will compile your code, make   sure the   output   executable names   are   correct.
.   A pdf file   contains   all   the   source   code   and   the   report,   you   should   put   the Cover Page in   the   first page of   the   report.
Once you have all the files, please put them in a single directory (named A2) and compress it   to a zip file.   You must follow the following   structure:

The      assignment must be submitted via Learning Mall to the correct drop box. Only    electronic   submission   is   accepted   and   no   hard   copy   submission.    All   students   must   download   their   file   and check that it is viewable after   submission.   Documents may become   corrupted   during   the uploading   process   (e.g.    due   to   slow   internet   connections).    However,   students   themselves   are   responsible   for   submitting a functional and correct   file   for   assessments. 
Please   note   that   quality   of   report   and   correctness   of   submission will   also be   marked   (10 points,    5   points for the quality of report,   5 points for   the   correctness   of   submission).         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
