# Info550Project  
  
 For this project, I am combining three datasets in order to run a regression to assess if the engagement of a student in yoga practice affects their TNF alpha levels.  
 
 Before beginning this project, make sure to download the three datasets (Demographics.csv , Engage.csv , THFalpha.csv ) and the code into the same folder.  
 
 To analyze the data you will need to install some `R` packages. The required packages can be installed using `R` commands.
```{r}
installed_pkgs <- row.names(installed.packages())
pkgs <- c("MASS", "wesanderson")
for(p in pkgs){
	if(!(p %in% install_pkgs)){
		install.packages(p)
	}
}
```

# Execute the code  

To execute the code you can run the following code from the command line while in the working directory with the datasets and the code.  

```{r}
Rscript -e "rmarkdown::render('Code.Rmd')"
```

This will create a file called `Yoga_and_TNFalpha' containing the results.
