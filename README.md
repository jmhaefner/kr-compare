# kr-compare

This is just a place to store plots that will be publicly accessible.
Descriptions of plots / additional information will be contained in the readme.
Please bother me if anything is missing or unclear.

Different types of plots are stored in different directories.

Current types of plots:
- QXYZcompare plots. These have names beginning with "QXYZcompare". These plots compare
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
- DistXYZ plots. These plots look at a single quantity, generally a difference between kdst and json,
    binned in X and Y. Instead of each plot having several curves vs Z for each XY bin, the full distribution
    is shown for each XYZ bin. The panels are still XY bins, the Z bin is indicated in the legend. The name
    is similar to QXYZcompare, and is of the form DistXYZ\_Q\_\specifics\_Nxy\_Mz\_YYYY-MM-DD. All of this is
    the same as form QXYZcompare, except for the specifics. If the Q is dx, you need additional info about
    which x determination algorithm we are using. This is specified in the specifics, and could be kdst-jsonsipm,
    kdst-jsonloc, kdst-jsonlocit, etc. Hopefully the additional info here is self explanatory, but as always,
    let me know if it is unclear.
