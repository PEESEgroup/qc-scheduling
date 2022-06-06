# qc-scheduling
Hybrid Classical-Quantum Optimization Techniques for Solving Mixed-Integer Programming Problems in Production Scheduling

### Jobshop scheduling
Problem instances for the jobshop scheduling problem are in text format. They are arranged as follows:

***** Start text file *****

J(# jobs) M(# machines)

P(Processing times) : Matrix of dims |J|x|M|

C(Processing costs) : Matrix of dims |J|x|M|

R(Release time) : Vector of dim |J|

D(Due time) : Vector of dim |J|

***** End text file *****



### Multipurpose batch scheduling
Problem instances for the jobshop scheduling problem are provided in the .npz format. These files 
can be read easily with the Numpy library in Python. Data in each instance can be accessed 
with the numpy.load function and the following keywords:

| Data                                    | Keyword |
|-----------------------------------------|---------|
| Tasks                                   | I       |
| Time points                             | N       |
| Chemical material resources | R1     |
| Equipment unit resources | R2      |
| Set of tasks allowed for each equipment | Ir      |
| Set of tasks that consume resources | Ti     |
| Set of tasks that produce resources | To     |
| Rate of generation | rho_I     |
| Rate of consumption | rho_O      |
| Minimum batch size| b_min      |
| Maximum batch size | b_max      |
