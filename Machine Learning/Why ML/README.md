# Why Machine Learning?

**Why we are looking into machine learning in such details?**

Because data analytics in particular data mining is machine learning. BUT applied to very large data set, very noisy data set and real data sets.

Classicaly machine learning has been more concerned with getting accurate parameter estimates from small volumes of data and trying to best what we could do with little data. but now with very large volumes of data available some of the focus is moving away from handling small data to things like how do we make sure that our algorithm will finish running in few weeks. So looking in to scaling issues etc so all of these issues have come forward now. So when we are working with these kinds of domain we call it data mining and if we go back and look at specific algorithms, error measures and we call it machine learning.

**Core of data mining is machine learning applied to :-**
 - Large data sets
   - Scaling issues
     - Architechture aware algo's
     - External memory algo's
   - Data Selection
   - Feature Selection
   - Database design
 - Noisy Datasets
   - Data cleaning
   - Robustness
   - Missing values
 - Real datasets
   - Real data typically doesnot satisfy some of the nice theoratical assumptions of many of the machine learning algorithms were operating under several decades. typically the assumption is that the data is independent but its not likely true fro example if my friend bought a laptop and i also need a laptop than i will probably buy the laptop too. here is the influencing factor. So indeoendent assumptions are not valid.
   - Class imbalance (If we look into medical domain, the fraction of people who are sick is very small thankfully).
   - Stringent performance measures ( Medical data)
   - Resource contraints
     - Produce answers on realtime
     - Limited computational power
