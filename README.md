# Spriter

## Usage

    var Spriter = require('./Spriter');

    var options = {
    	outputDir: 		    "path/to/output",   //required
    	outputDirForCss:	"path/for/css",     //required
    	inputPath: 		    "path/to/input",    //required
    	sassPath: 		    "path/to/_map.scss",//required
    	svgMode:			"view",             //optional, default "css", see https://github.com/jkphl/svg-sprite
    	svgLayout:		    "diagonal"          //optional, default "packed", see https://github.com/jkphl/svg-sprite
    	padding:			"0"                 //optional, default 2 for png and 0 for svg
        algorithm:		    "binary-tree"       //optional, default binary-tree, see https://github.com/Ensighten/spritesmith#algorithms
    }

    var spriter = new Spriter(options);
    spriter.Run();