manual.pdf: manual.fvl
	feivel -t manual.fvl | tee error > manual.tex
	pdflatex -interaction=batchmode manual.tex
	pdflatex -interaction=batchmode manual.tex
	rm manual.aux manual.log manual.tex manual.toc error
