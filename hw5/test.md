Tumor classification from PET images: A company recently developed a new positron emission tomography (PET) radiotracer for the detection of tumor regions in the brain. The PET images are collected after the injection of a radiotracer. The intensity of the pixels in the PET images correspond to the amount of radiotracer absorbed by the tissue. Tumor regions are metabolically more active and hence absorb more radiotracers compared to normal tissue. It is known that the pixel intensities follow an exponential distribution, whose parameter β depends on the uptake of the radiotracer in the specific pixel. Using training data from several subjects and with biopsy as ground truth, the company estimated the β parameters of the likelihood distributions
of the tumor and non-tumor regions using maximum likelihood method.
p(x|normal) ={ 1βnexp(− xβn) if x ≥0
             {  0 else 
p(x|tumor) ={ 1βtexp(−xβt)if x ≥0
            {   0 else with βn = e ≈2.718 and βt = 1. 
In this problem, you can assume the above distributions to be known
and fixed.

a. Plot the two distributions. You may use python to make the plots.
b. Assuming the prior probabilities of the classes to be the same, determine the minimum error classification rule. Plot the decision regions. Check if the answer makes sense by comparing with the plot in (a).
c. Assume that the prior probability of normal tissue to be e1
d. Determine and plot using python the posterior probabilities of the classes.
e. The mis-classification error can be reduced by rejecting regions with posterior probabilities less than 90%. Determine and plot the decision regions with this setting.
f. The physicians assess the risk in mis-classifying a normal pixel as tumor to be $1, while the risk in misclassifying a tumor pixel as normal to be $148.41 ≈ e5, where e ≈ 2.718. With the above information, determine and plot the minimum risk classifier and plot the decision regions. Explain why the shift in the decision region results in a reduction of risk.