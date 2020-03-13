TARGET = short-proposal


SOURCES = *.tex bib.bib


$(TARGET).pdf: $(SOURCES)

	pdflatex -halt-on-error -file-line-error $(TARGET).tex

	bibtex $(TARGET) || echo Suppressed BIBTEX error

	pdflatex -halt-on-error -file-line-error $(TARGET).tex

	bibtex $(TARGET) || echo Suppressed BIBTEX error

	pdflatex -halt-on-error -file-line-error $(TARGET).tex


clean:

	rm -f $(TARGET).ps $(TARGET).dvi

	rm -f $(TARGET).ind $(TARGET).toc $(TARGET).bbl $(TARGET).blg $(TARGET).ilg $(TARGET).idx $(TARGET).log $(TARGET).lot $(TARGET).lfm $(TARGET).out $(TARGET).lof $(TARGET).brf

	rm -f $(TARGET).pdf

	rm -f *.aux

	rm -f *.fls *.fdb_latexmk
