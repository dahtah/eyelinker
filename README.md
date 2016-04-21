[![CRAN Version](http://www.r-pkg.org/badges/version/eyelinker)](https://cran.rstudio.com/web/packages/eyelinker)

# Eyelinker: a package for reading Eyelink data

Turns horrible Eyelink .asc files into less horrible R data structures.

	install.packages("eyelinker")
	library(eyelinker)
	#Example file from SR research that ships with the package
	fpath <- system.file("extdata/mono500.asc.gz",package="eyelinker")
	dat <- read.asc(fpath)
	plot(dat$raw$time,dat$raw$xp,xlab="Time (ms)",ylab="Eye position along x axis (pix)")
	#For more info:
	vignette("basics",package="eyelinker")
	
Author: Simon Barthelmé, CNRS, Gipsa-lab. See also: [cili](https://github.com/beOn/cili).

