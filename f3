=IFERROR(
    SUMIFS(Data!$AA:$AA, Data!$V:$V, 'Work sheet'!$A58, Data!$T:$T, 'Work sheet'!$B$1, Data!$P:$P, 'Work sheet'!$B$2, Data!$W:$W, 'Work sheet'!$B$3, Data!$U:$U, 'Work sheet'!$B$5) /
    SUMIFS(Data!$S:$S, Data!$V:$V, 'Work sheet'!$A58, Data!$T:$T, 'Work sheet'!$B$1, Data!$P:$P, 'Work sheet'!$B$2, Data!$W:$W, 'Work sheet'!$B$3, Data!$U:$U, 'Work sheet'!$B$5),

    IF(
        ISERROR(OFFSET(INDIRECT(ADDRESS(ROW(), COLUMN())), -1, 0)),
        AVERAGE(OFFSET(INDIRECT(ADDRESS(ROW(), COLUMN())), -1, 0), OFFSET(INDIRECT(ADDRESS(ROW(), COLUMN())), -2, 0)),
        OFFSET(INDIRECT(ADDRESS(ROW(), COLUMN())), -1, 0)
    )
)
