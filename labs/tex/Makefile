.PHONY : build move

see : build move

build : research.tex
	pdflatex -shell-escape research.tex
	biber research
	biber research
	pdflatex -shell-escape research.tex
	pdflatex -shell-escape research.tex

move : report.pdf
	-mkdir ../pdf
	mv research.pdf ../pdf/