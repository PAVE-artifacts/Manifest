READ ME:

Our repo contains the following directories: 

- paper-formal-artifacts :

      1- Complete fomal models and prooflite scripts of nbench pa-protected code (included in  .pvs files)
      2- proof files ( .prf files)
      3- proofthem proof command : (a script) to load and run the proofs
      4- proveit proof command : (a script) to run the 
      5- all proof summaries (and "grandstotals" files).

Tutorials:

- We encourage people who are interested in the work to watch the tutorial videos.
     1- the chain is running on actual examples ( lifting ) 
     2- provethem command in action (proving)
     3- proof results (proof status (OK vs missed), real time, number of formulas, number PVS files created and verified)

- The formal proofs of the models are ready to be re-produced by just doing the following: 

- Assuming you have PVS7 version 7.1.0 : 
  (if you don't then install from here www.csl.sri.com/~owre/drop/pvs-snapshots/  )  
      choose pvs7.1-0-gbe4ad5c-ix86_64-Linux-allegro.tgz 

     - Clone our repo to your PC 
     - cd to the paper-formal-artifacts directory
     - extract all parts into one directory and copy all files in part-1,2,3,4 and base into into one directory ( myfolder ).  
     - edit the proofthem script the line with your editor (say gedit):
          and put your PVS7 PATH instead. 
     - Add myfolder to your PVSLIBPATH. So PVS can see its libraries directly.       
                  
     - run the command ./proofthem --force <  names.txt  > 

 Example: 
     - (paper-formal-artifacts)$./proofthem --force asl/name-of-any-test-suit-directory/ names.txt
          
For a quick example, use ./proveit filename.pvs (any file name in the directory will do the trick).
 
 Example:
     - (paper-formal-artifacts)$./proveit file-name.pvs )

                           
- Also it contains the source codes of (or links to) the following:

        - Translator( pa-lifter),
        - The binary code of the nebnch-byte benchmark
        - a dis-assembled version of the nbench-byte benchmark code
        - pa-decoder, 
        - pa-verifier
        - ASli-to-PVS7 (Test generator)
        - ARMv8.3 ISA xml files 
        - Many scripts for statistical use on the binary, assembly.
 
 Enjoy! 
