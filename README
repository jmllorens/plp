Plp is a python frontend to gnuplot. It is inspired in the perl frontend created by Michael Sternberg, named `pl`. The main purpose is to quick-look at data from the command line. Say for example that a program has produced a great amountof files named `output_xxx.dat`. A fast way to explore the data would be: `plp output_*.dat`. If the data is in a single file distributed in columns, the command plots assumes the fist column as x and the rest as y. It is also possible to plot just a short range of columns with a given step:

    plp -i 1:2:8:2 output.dat
    
Here, gnuplot will show columns from 2 to 8 every 2. The full help of the command is:

    Usage: plp -n -k -u n1:n2:n3:n4 <first set of data files> ... -u n1:n2:n3:n4 <n-th set of data files> 
           -n Normalize plots wrt to maximum
           -k Show legend
           -l Plot with lines
           -p Plot with points
           -s Show gnuplot script
           -S Smooth with csplines
           -i n Interpolate n points
           -f if "-i n" is present, the interpolated data is dumped to "interp_"+data_file
           -u n1:n2 -> plot column n2 against n1
           -u n1:'(f($n2))' -> plot function f of column n2 against n1
           -u n1:n2:n3 -> plot columns n2 to n3 against n1
           -u n1:n2:n3:n4 -> plot columns n2 to n3 every n4 columns against n1
           if n2 or n3 is negative, the last column of the data file is assumed
           -t <settings_file> Import gnuplot settings
    If -u is absent "-u 1:-1" is assumed
    If -l and -p are absent lines-points style assumed
