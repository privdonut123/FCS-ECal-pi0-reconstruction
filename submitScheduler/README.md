Instruction on running schuduler job submit for pi0 reconstruction.

0) Make sure the path in the scripts are correct for your working folder.


1) For each iteration: 

	 1.0) (For the second and further iteration) Before you start a new iteration, please make sure the previous iteration analysis is completed and the fcsgaincorr.txt is updated to the gain correction result from the previous calculation.

	 1.1) open submit_event_scheduler_fcsgain.pl file , go to line 7 and change the run number to the one that you need.

	 1.2) run command "perl submit_event_scheduler_fcsgain.pl" , wait until the scheduler submit is completed.

	 1.3) open submit_event_scheduler_fcsgain.pl file again, go to line 7 and change the run number to another run number that you need.

	 1.4) run command "perl submit_event_scheduler_fcsgain.pl" again , wait until the scheduler submit is completed.

ps: Depending on the fit result of each tower invariant mass, you might need about 2 or 3 iterations to get most of the tower invariant mass close to pi0 invariant mass.


2) For each iteration, you need to wait until all the jobs are completed to go to the next step (back to README.md in the main working folder)






