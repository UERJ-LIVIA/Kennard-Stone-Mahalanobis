# Kennard-Stone-Mahalanobis
Data splitting using Mahalanobis distance can enhance our results significantly when training a neural network in comparison to euclidean distance. Tensorflow doesn't offer Mahalanobis distance for data splitting, thus the need for this simple code that's still under work.

This is an algorithmin for data splitting that takes as input:
DIR           The directory of the samples to be split
HEADER        If your sample file has a header, HEADER = (row of header), usually 0. If not HEADER =None
k             Number of Samples to be sorted
COV           If COV=True , will make a CSV with the covariance matrix
VERBOSE       If VERBOSE = True, will alert you if k>n or k<=2 or n<=2
PRINTRESULTS  If PRINTRESULTS == True, Makes a CSV with Samples on rows and Observations on columns


#References
The method is implemented following the description published in R. W. Kennard & L. A. Stone (1969): Computer Aided Design of Experiments, Technometrics, 11:1, 137-148. https://www.tandfonline.com/doi/abs/10.1080/00401706.1969.10490666

