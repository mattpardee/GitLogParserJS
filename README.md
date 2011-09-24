#Git Log Parser in JavaScript

This module takes in the output from a "git log --format=raw -- [file]" operation, parses it and places details into a hash that is then pushed onto an array. This happens for each line.

#Usage

```javascript
var GitLogParser = require("gitlogparser");
var gitLogParser = new GitLogParser();

// Run the git log operation and get a string back

var gLogOut = "[all output]";

gitLogParser.parseLog(gLogOut);

// Get the results of the parsing
var parseResult = gitLogParser.getLogData();
```

From here you can iterate over each item in the array and do something with it.
