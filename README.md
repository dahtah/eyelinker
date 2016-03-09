# Eyelinker: a package for reading Eyelink data

Turns horrible Eyelink .asc files into less horrible R data structures.

	devtools::install_github("dahtah/eyelinker",build_vignettes=TRUE)
	library(eyelinker)
	#Example file from SR research that ships with the package
	fpath <- system.file("extdata/mono500.asc.gz",package="eyelinker")
	dat <- read.asc(fpath)
	plot(dat$raw$time,dat$raw$xp,xlab="Time (ms)",ylab="Eye position along x axis (pix)")
	#For more info:
	vignette("basics",package="eyelinker")
	
Author: Simon Barthelmé, CNRS, Gipsa-lab. See also: [cili](https://github.com/beOn/cili).

