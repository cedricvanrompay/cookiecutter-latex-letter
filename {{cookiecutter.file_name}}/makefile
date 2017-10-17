LATEX_COMPILER = lualatex
LATEX_OPTS = -output-directory .latex

# for use with "LaTeX Workshop" extention for MS VSCode
# https://github.com/James-Yu/LaTeX-Workshop
LATEX_OPTS +=  -interaction=nonstopmode -file-line-error


pdf/{{cookiecutter.file_name}}.pdf: dirs main.tex
	$(LATEX_COMPILER) $(LATEX_OPTS) main.tex
	mv .latex/main.pdf pdf/{{cookiecutter.file_name}}.pdf

dirs:
	mkdir -p .latex pdf

.PHONY: dirs
