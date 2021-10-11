# fitbit
Analysis of fitbit data and sleep score

First, you need to download your all-time fitbit data. Go to [www.fitbit.com](www.fitbit.com), and find the Data Export tab in your settings. Choose to request data in Export Your Account Archive, and wait for the download to start (it takes a while, you should receive an email when the data is ready to download). The data comes in a zip folder, MyFitbitData.zip. Move that archive folder in whatever directory you are working in, unzip, and you are ready to explore. 

This jupyter notebook provides an example. It reads various data (sleep, activity, ...), and explore the data. In this particular notebook, I tried to understand what impacts my sleep score the most. Turns out that, unsurprisingly, sleep duration is the most important quantity. My daily physical activity has less of an impact than I expected.

Several regression algorithms are tested to infer sleep score. Because sleep score scales linearly with sleep duration, and because other features are less important, a simple linear regression ends up providing the best fit.
