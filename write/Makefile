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
		src/harmful.Rmd \
		src/header.html \
		input/hrdag_ID_horiz_w-desc-sdahrj_rgb.png
	-rm src/harmful.html
	Rscript --vanilla -e "rmarkdown::render('$<')"
	mv src/harmful.html $@

# done.
