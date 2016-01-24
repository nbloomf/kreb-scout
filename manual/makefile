manual.pdf: FORCE
	feivel -t manual.fvl | tee error > manual.tex
	pdflatex -interaction=batchmode manual.tex
	pdflatex -interaction=batchmode manual.tex
	rm manual.aux manual.log manual.tex manual.toc manual.out error
	@echo "Done!" | doppler lightgreen

FORCE:
