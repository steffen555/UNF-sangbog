# To compile

1. Compile unf-sangbog.pdf using pdflatex
2. Run mksbtdx.
3. Compile unf-sangbog.pdf using pdflatex

Since the table of contents was created without the table of contents, the page numbers are probably off, so:

4. Run mksbtdx again. Change hardcoded pagenumbers and \TeX commands in .tocx and .tdx. Add headers in .tocx.
5. Compile unf-sangbog.pdf using pdflatex

Adding headers might make the list longer and fill more pages. Iterate as needed.

# To add a song
Make a copy of the template file in the songs folder and follow the instrucions in the comments. Add the song to the main file using \include{songs/filename}