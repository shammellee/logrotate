# logrotate
Simple file logger with built-in file-size-based archiving

* **Organization** [Karbon Industries][companyURL]
* **Author** [Shammel Lee][authorURL]
* **Start Date** Mon Dec  1 06:04:29 EST 2014

[companyURL]: http://www.karbonindustri.es/
[authorURL]: http://www.shammellee.com/

## usage
	$ <command> | logrotate <logFile> [<maxFileSizeBytes>=10000]

## examples
	$ echo foo | logrotate log.txt // archive log.txt and create a new file every 10KB
	$ echo foo | logrotate log.txt 56000 // archive log.txt and create a new file every 56KB