
Overleaf: How to Cite Papers Using et al. Style

This article shows you how to cite papers with three or more authors using et al. style. The example is for jpe bib style, but the method should apply to other citation styles as well.

    Step 1: before \begin{document}, add \immediate\write18{cp `kpsewhich jpe.bst` .} (the space before . cannot be missing) to tell the shell to copy the “jpe.bst” file to your Overleaf project.
    Step 2: To the right of the Recompile button, you can find Logs and output files, click on this button and go to the bottom right, from Other logs and files, find “jpe.bst”, click to download.
    Step 3: rename the downloaded file to “myjpe” and upload it to your Overleaf project.
    Step 4: open the “myjpe.bst” file on Overleaf and find FUNCTION {format.lab.names}, under this section, change numnames #3 > and to numnames #2 > and, that is, for papers with number of authors names over 2 (3 or more), use “et al.” style.
    Step 5: change the \bibliographystyle{jpe} to \bibliographystyle{myjpe}.
    Step 6: recompile.

References:

    [1] To find the bst file: https://tex.stackexchange.com/questions/553385/where-to-find-apacite-bst-file-to-change-bibliography-style
    [2] To locate the format section: ChatGPT
    [3] Original Idea: https://xiao-ying-liu.github.io/mywebsite/overleaf_et_al_citation.html
