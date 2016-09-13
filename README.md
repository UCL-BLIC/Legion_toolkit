# Legion_toolkit
Misc. scripts which make life easier when working on the Legion cluster at UCL

All scripts should be placed in a "bin" directory in a filesystem which is writeable from the nodes on the cluster. It is suggested that the directory is in "/scratch/scratch/$USER/".

## Contents

+ qclear: Uses the qdel command to remove all jobs in the queue.
+ qdelbyname: Use the qdel command to remove jobs in the queue.
+ qsub1line: Create a generic single-core qsub script and submit this to the queue. The qsub script is based on the file named "qsub1line.template". Usage: 
```
qsub1line "command and arguments to pass to qsub command"
```
+ qwatch: Clear the terminal and watch Legion's queue, refreshing every 120 seconds.
