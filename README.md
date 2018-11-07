# circus_plot
Make a circus plot of pvalues by calling the function plot_circus_plot(...)

# example
Just source the file and call the function test_circus_plot()

This will plot a circus plot with 60 variables, grouped in 3 classes. The family variable is the class indicator.
```
  M = 20 
  N = M*3
  family=rep(c(1,2,3),each=M)   # group the pvalues in 3 clusters
  labels=paste0("label",1:N)    # labels for each pvalue (variable names)
  pvalues=1/(.01+1:N)           # make pvalues
  guides = c(.01,.05,.1,.25,.5) # set chart guide lines
  myP=plot_circus_pvalues(family, labels, (pvalues), (guides) ) 
  print(myP)
```  
