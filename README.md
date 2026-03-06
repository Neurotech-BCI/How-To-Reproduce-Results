## How to Reproduce Results
With relevant links from the example of [Chavarriaga et al., 2010](https://drive.google.com/file/d/1uxEamO9PvZj2BkqvQEPetc-48vVGhNLS/view?usp=share_link), where the researchers tried to create an ErrP detection tool. 

Reproducing the results of a paper is an excellent way to dive very deep into the paper, and gain a thorough understanding of what the researchers were trying to do, what they did, what data they collected, and what they didn’t report. It gains you a better understanding of what the data in a specific field or type of study looks like (e.g. what ErrP data looks like, how its processed, how ErrPs are detected), which will help you have a deeper understanding of other, similar papers you read.
### One
The first step of reproducing results is to have a high level of understanding of the paper.
* What had previous studies done?
* What gap in the literature did the researchers identify?
* What did they do (what was their procedure)? What were their aims?
* What results did they get?
* What did they conclude?

Your first step should be to read the paper. Everyone reads papers differently. Some read the discussion first and then read the rest; others read it from start to finish. Some leave the methods to the end. Do what works for you.
### Two
Find their experimental procedure and download their data. Look through the data a bit– is it formatted? Some datasets will be ready for processing out-the-box, while others will make you work a little bit. Authors will often have their code available or some sort of supplementary document detailing how they preprocessed their data. Try to follow their steps. Often, datasets themselves will have README files. Many of them will tell you what the data looks like.

In the example of Chavarriaga et al., this [document](https://lampx.tugraz.at/~bci/database/013-2015/description.pdf) describes [the dataset](https://bnci-horizon-2020.eu/database/data-sets) (#22 on there). One thing the researchers did was to have two sessions for each participant, in order to see how well the signal holds up over time. In our case, we don’t care much about this, so you can just download the first sessions for each participant.

We will do all of our data analysis in Python, although many datasets (like the Chavarriaga one) will be pre-formatted for Matlab. Scipy has a “loadmat” function that you can use to load .mat (Matlab) files.

See the Jupyter notebook I sent you (chavWalkthrough.ipynb) for the coding side!