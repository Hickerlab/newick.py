# Oriented Trees To Newick

Script to convert oriented trees to newick format. See [Kelleher - ERCS](http://jeromekelleher.github.io/ercs/#oriented-trees-and-forests) for details.

	usage: newick.py [-h] -p PI -t TAU [-b]
	example: python newick.py -b -p [-1,4,4,5,5,0] -t [-1,0.0,0.0,0.0,30441.57,46750.11]
	output: (sample5:200.0,((sample1:100.0,sample2:100.0):100.0,sample4:200.0):0.0);

	optional arguments:
 	 -h, --help         show this help message and exit
  	 -p PI, --pi PI     an array of comma-separated integers encoding the coalescent tree
  	 -t TAU, --tau TAU  an array of comma-separated doubles encoding coalescent times
 	 -b, --bifurcate    output a bifurcating tree by adding zero branch lengths to multifurcating nodes