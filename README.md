# Oriented Trees To Newick

Script to convert oriented trees to newick format. See [Kelleher - ERCS](http://jeromekelleher.github.io/ercs/#oriented-trees-and-forests) for details.

	usage: newick.py [-h] -p PI -t TAU [-b]
	example: python newick.py -b -p [-1,6,6,6,7,7,8,8,0] -t [-1,0.0,0.0,0.0,0.0,0.0,1.0,2.0,4.0]
	output: ((sample3:1.0,(sample1:1.0,sample2:1.0):0.0):3.0,(sample4:2.0,sample5:2.0):2.0);

	optional arguments:
 	 -h, --help         show this help message and exit
  	 -p PI, --pi PI     an array of comma-separated integers encoding the coalescent tree
  	 -t TAU, --tau TAU  an array of comma-separated doubles encoding coalescent times
 	 -b, --bifurcate    output a bifurcating tree by adding zero branch lengths to multifurcating nodes
