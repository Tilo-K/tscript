
all: singlefile multifile

JSFILES := ../source/codemirror.js \
	../source/codemirror-activeline.js \
	../source/codemirror-dialog.js \
	../source/codemirror-search.js \
	../source/codemirror-searchcursor.js \
	../source/codemirror-jumptoline.js \
	../source/codemirror-comment.js \
	../source/codemirror-scroll.js \
	../source/codemirror-unindent.js \
	../source/codemirror-tscriptmode.js \
	../source/tscript.js \
	../source/tgui.js \
	../source/interact.min.js \
	../source/search.js \
	../source/doc.js \
	../source/def-concepts.js \
	../source/def-ide.js \
	../source/def-language.js \
	../source/def-stdlib.js \
	../source/def-examples.js \
	../source/def-errors.js \
	../source/def-cheatsheet.js \
	../source/def-legal.js \
	../source/ide.js \

CSSFILES := ../source/codemirror.css \
	../source/tgui.css \
	../source/ide.css \
	../source/documentation.css \

singlefile:
	rm -f index.html
	rm -f index.html.zip
	cat start ${JSFILES} middle ${CSSFILES} end > index.html
	zip index.html.zip index.html

multifile:
	rm -f tscript.css
	rm -f tscript.js
	cat ${CSSFILES} > tscript.css
	cat strict ${JSFILES} > tscript.js

clean:
	rm -f index.html
	rm -f index.html.zip
	rm -f tscript.css
	rm -f tscript.js
