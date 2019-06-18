# Tracking-using-Event-Based-Cameras

%%%%%%%%%% Steps to Use Ntu Tracker %%%%%%%%%%%%
Add to the path /ntu Tracker , /Minion_Annotations and /minion_
Go to neuromorphic/home_dirs/mohit/ntu_tracker/Updated Code/Tracker_Basuv17_merge_wELM.m
Run the above matlab lab file , this file is The NTU Tracker Code , it will result in a .txt file.
In this file:-
Line 12 => Change the subset for the length of .bin file you want to track.
Line 13 => Add the name of .bin file that you want to run the tracker on.
Line 14 => Recording Type , as mentioned.

%%%%%%%%% Note %%%%%%%
In some cases of LT4 it may throw a error to Tracker_Metrics Evaluation , check that the length of CPP_  and change
Line 192 to  max_time=min(max(annot_GroundTruth.ts),max(annot_cpp.ts));
Delay is set to 0. If needed you change this.

The Tracker Annotation is saved in /neuromorphic/home_dirs/mohit/ntu_tracker/Updated Code/Jun03/tracker_eval/TrackerAnnotations
with a suffix '_tracker' added to its end.

%%%%%% Steps to Plot P-R Curves %%%%%%%%%%%%%%

Open neuromorphic/home_dirs/mohit/ntu_tracker/Updated Code/submission_tracker_evaluation
Run run_batch.m and go through the readme included in the folder.
Update the complete path of the GT and Tracker output files.
GT is saved in /neuromorphic/home_dirs/mohit/ntu_tracker/Updated Code/Jun03 as _SW as 'suffix'.
Tracker output is saved in uromorphic/home_dirs/mohit/ntu_tracker/Updated Code/Jun03/tracker_eval/TrackerAnnotations as _SW_lookprediction_excluded as 'suffix
This code output will be saved as '.mat' file in Jun03.

Run plot_RP.m , and the input to this file will be the '.mat' file obtained from the previous result.
And it will give the result as 2 curves , name same as file , added suffix as 'Precision' and 'Recall', and it will be saved in UpdatedCode.

%%%%%%%% End of the file %%%%%%%%%%%%%
%%%%%%%% For more information contact Mohit Sarin on mohitsarin98@gmail.com %%%%%%%%%
