# kr-compare

This is just a place to store plots that will be publicly accessible.
Descriptions of plots / additional information will be contained in the readme.
Please bother me if anything is missing or unclear.

Current types of plots:
- QXYZ plots. These have names beginning with "QXYZcompare". These plots compare
    various quantities vs x, y, z. The names should look like QXYZcompare\_Q\_Nxy\_Mz\_YYYY-MM-DD.
    Q is the quantity (S2e = S2 energy, N = number of events, etc). Nxy means N x bins and N
    Y bins (so N\*N xy bins). Mz is M zbins. Will always be divided into N\*N different plots,
    each with a curve of Q vs Z for each of several different analysis methods. YYYY-MM-DD is
    the date of creation of the plot.

    The location on the horizontal axis represents the start of the zbin (not the center).
    The names of the analysis methods include kdst (which is the kdst analysis method) and
    json\_\<xymethod\>\_\<zmethod\>\_\<sub\>. xymethod can be xymsipm, xylocit, xyloc for max sipm, local
    center of gravity iterated, and local center of gravity (resp). zmethod can be zgauss
    or zrms, respectively. "sub" indicates whether the prewindow subtraction is being applied
    (if yes, you'll see "\_sub", if not, you'll see nothing).

    For all plots in a given pdf, the x and y axes are always the same, so the axes are only
    shown at the far edges to avoid clutter. 
