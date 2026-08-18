TALK = talk

all: $(TALK).pdf

$(TALK).pdf: $(TALK).tex asc-theme.sty
	lualatex -interaction=nonstopmode $(TALK).tex
	lualatex -interaction=nonstopmode $(TALK).tex

clean:
	rm -f $(TALK).aux $(TALK).log $(TALK).nav $(TALK).out $(TALK).snm $(TALK).toc $(TALK).vrb

distclean: clean
	rm -f $(TALK).pdf

.PHONY: all clean distclean
