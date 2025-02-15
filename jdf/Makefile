# Tools
LATEXMK = latexmk
RM_CMD = rm -f

# Project-specific settings
DOCNAME = jdf-example

# Targets
all: doc
doc: pdf
pdf: $(DOCNAME).pdf

# Rules
%.pdf: %.tex
	$(LATEXMK) -pdf -M -MP -MF $*.d $*

clean:
	$(LATEXMK) -silent -c
	$(RM) *.bbl
	$(RM) *.d
ifeq ($(doc), true)
	$(LATEXMK) -silent -C
	$(RM) *.run.xml *.synctex.gz
endif

cleanall: clean
	@echo "Running cleanall target"


.PHONY: all clean doc mostlyclean pdf

# Include auto-generated dependencies
-include *.d
