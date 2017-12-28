# My CV in Latex
This is my CV in LaTeX. I am new to LaTeX, but I use it here because it offers some nice typesetting options and automation features for plain text documents.

For example, you can integrate LaTeX with Python via [PythonTex package][pythontex]. This package is super helpful for executing Python code within your LaTeX document. For my CV, I used PythonTex to query the NIH web API for the [iCite Database][rcr-nih] containing the Relative Citation Ratio (RCR) for papers in PubMed. The RCR is a new citation metric that quantifies an article's influence relative to articles in its field. The authors of the RCR delineate an article's field using its co-citation network. For more details, see the original paper in [PLoS Biology][rcr-pub].

There are a few packages for creating CVs/resumes in LaTeX, but I opted for a template created Dario Taraborelli, which can be found on his [website][dar-url] and on his [GitHub][dar-git]. Although it should work for any LaTeX compiler, I have been using TeXShop and the [MacTeX distribution][mactex]. You may need to install the [Academicons package][academicons] and the [FontAwesome package][font]. You may also need to install other fonts, including [Libertine][lib-font].

Steps for compiling:
1) xelatex smith_cv.tex
2) pythontex smith_cv.tex
3) xelatex smith_cv.tex

Please note that this work is licensed under a [CC BY-SA 3.0 License][cc-sa].

[lib-font]: https://sourceforge.net/projects/linuxlibertine/files/latest/download
[dar-url]: http://nitens.org/taraborelli/cvtex
[dar-git]: https://github.com/dartar/cvtex
[rcr-nih]: https://icite.od.nih.gov
[pythontex]: https://github.com/gpoore/pythontex
[rcr-pub]: https://www.ncbi.nlm.nih.gov/pubmed/27599104
[academicons]: https://github.com/diogo-fernan/academicons
[font]: http://fontawesome.io
[cc-sa]: http://creativecommons.org/licenses/by-sa/3.0/
[mactex]: http://tug.org/mactex/
