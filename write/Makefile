#
# Authors:     TS
# Maintainers: TS
# Copyright:   2019, HRDAG, GPL v2 or later
# =========================================
# /Users/tshah/git/rproj-harmful/write/Makefile

.PHONY: all clean

all: output/harmful.html

clean: 
		-rm -r output/*

output/harmful.html: \
		src/harmful.Rmd
	-rm src/harmful.html
	Rscript --vanilla -e "rmarkdown::render('$<')"
	mv src/harmful.html $@

# done.
