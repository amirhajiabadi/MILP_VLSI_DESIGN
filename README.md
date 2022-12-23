# MIP

We attempted to utilize a framework that is independent of the solvers, as suggested in the description of
the VLSI problem. During our investigation, we encountered Pyomo.
An open-source, Python-based modeling language for optimization with a wide range of optimization
features. Simply modifying the solver's name would be sufficient to solve the problem with another solver.
We tried three different solvers (GLPK, CBC, IPOPT) and compared the result.
We aimed to stabilize the optimization algorithm based on the variables' probable lower and upper bounds

**Results:**
Through trial and error, we spent a lot of time and effort determining the best approach to specify the variables and constraints in the Pyomo framework and addressing the issues. Eventually IPOPT solver showed exceptional performance and solved all 40 samples in 18 seconds.

  
  

**Installation:** 

**Pyomo Using PIP:** pip install pyomo

**GLPK solver:**

1. Download and unzip the file: https://sourceforge.net/projects/winglpk/

2. Move it into Drive C

3. Search for edit the system environment variables, click on environment variables and add that directory to path variable

**IPOPT solver:**

1. Download and unzip the file: https://www.coin-or.org/download/binary/Ipopt/Ipopt-3.11.1-win64-intel13.1.zip

2,3. The same as GLPK

**CBC solver:**

1. Download and unzip the file: https://www.coin-or.org/download/binary/Cbc/Cbc-2.10.5-x86_64-w64-mingw32.zip

2,3. The same as GLPK

