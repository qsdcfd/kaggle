<img width="758" alt="스크린샷 2022-05-06 오후 2 03 33" src="https://user-images.githubusercontent.com/86671456/167070247-81361bb0-8a27-4408-980f-417268013502.png">

Results

After all that work, we can say that including the extra information did improve performance! The model is definitely not optimized to our data, but we still had a noticeable improvement over the original dataset when using the calculated features. Let's officially summarize the performances:

Experiment	Train AUC	Validation AUC	Test AUC
Control	0.815	0.760	0.745
Test One	0.837	0.767	0.759
Test Two	0.826	0.765	0.753


(Note that these scores may change from run to run of the notebook. I have not observed that the general ordering changes however.)

All of our hard work translates to a small improvement of 0.014 ROC AUC over the original testing data. Removing the highly collinear variables slightly decreases performance so we will want to consider a different method for feature selection. Moreover, we can say that some of the features we built are among the most important as judged by the model.

In a competition such as this, even an improvement of this size is enough to move us up 100s of spots on the leaderboard. By making numerous small improvements such as in this notebook, we can gradually achieve better and better performance. I encourage others to use the results here to make their own improvements, and I will continue to document the steps I take to help others.
