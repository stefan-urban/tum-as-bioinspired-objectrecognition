PROJECT(as NONE)
cmake_minimum_required(VERSION 3.0)

INCLUDE(UseLATEX.cmake)

SET(LATEX_OUTPUT_PATH output)

#add_subdirectory(images)

ADD_LATEX_DOCUMENT(
    report.tex
	INPUTS  01_abstract.tex
	        02_content.tex
    BIBFILES mybib.bib
    IMAGES  images/hubel-experiment.png
			images/kolb-2003-howtheretinaworks-p3.pdf
			images/masland-2001-neuron-types.pdf
			images/optic-chiasm.png
			images/riesenhuber-poggio-1999-models-p3.pdf
			images/riesenhuber-poggio-2000-visualpathway.png
			images/serre-appearance-based-model2.pdf
			images/serre-appearance-based-model3.pdf
			images/serre-appearance-based-model.pdf
			images/Simple_and_Complex_Cells.pdf
			images/top-down-model.pdf
			images/Ventral-dorsal-streams.svg
			images/visual-cortex-map.pdf
			images/visual-path-through-brain.png
			images/visualpathways.png
			images/visual-stream2.pdf
			images/visual-stream.pdf
#    DEPENDS overview_pdf
#            software-rpi_pdf
)
