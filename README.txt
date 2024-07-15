MODULAR LATEX DOCUMENT:

https://en.wikibooks.org/wiki/LaTeX/Modular_Documents

================================================================
================================================================
1. INCLUDING FILES:

To include sections use \input{filename} or \include{filename}:
compiling your main doc.tex will insert the "filename" in its place. So formatting will happen in the main doc.tex while the written text can be organized in different "filenames".
- input:
	+ can be nested.
	+ doesn't force page break.
	+ .tex filename extension is optional.

- include:
	+ cannot be nested with more include.
	+ can be nested with input.
	+ forces a page break.
	+ .tex filename extension has to be avoided.

================================================================
================================================================
2. FILE PATHS:

By default the "filename" will be searched in the same directory as the main doc.tex

________________________________________________________________
Asolut Path:
otherwhise you can give the ABSOLUT path of the file:
/home/.../filename.tex
	+ only useful for global files which are not saved within the doc directory

________________________________________________________________
Relativ Path:
to include your written files use RELATIV paths, refering to the current directory(dir of main doc.tex):
./"..."/filename.tex
	+ so in our case: ./tex/.../filename.tex

!!! Do note, however, that LaTeX uses forward slashes / even on Microsoft Windows platforms, which use backslashes \ in pathnames. !!!

================================================================
================================================================
3. COMPILING SELECTED SECTIONS

Using \includeonly{filename1,filename2,...} before \begin{document} in the main doc.tex will only include the explicitly named files WITHOUT .tex extension. "filename" will be the relativ path in our case

================================================================
================================================================
4. IMPORT PACKAGE

http://ctan.org/pkg/import



