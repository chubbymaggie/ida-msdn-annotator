# ida-msdn-annotators
Add MSDN annotations to IDA imported functions and structures

---------------------------------------------------------------------------------------------------------------------

This work is almost based on Moritz Raabe and William Ballenthin's work at Fireeye.

I strongly recommend you to refer the original <a href="https://github.com/fireeye/flare-ida"> flare-ida </a> project.

##The differences include:
1. Add a new plugin responsible for adding annotations to structure types and members.
2. Add a new script to parese windows sdk help-htmls to extract structures' annotations.
3. Add new regrex rules to parse the imported functions' name in IDA.

##Usage
Usage for script adding annotations to imported functions can be found at

1. https://github.com/fireeye/flare-ida (<b>MSDN Annotations Usage</b> section)
2. https://www.fireeye.com/blog/threat-research/2014/09/flare-ida-pro-script-series-msdn-annotations-ida-pro-for-malware-analysis.html

Usage for script adding annotations to structures is similar to the above

###NOTES about preparing sdk help files
After you install standalone Windows SDK into your local drive (By default, it is located at 'C:\Program Files\Microsoft SDKs\Windows\v7.0\Help\1033'), you can find the installed help files in folder 'C:\Program Files\Microsoft SDKs\Windows\v7.0\Help\1033'. However, these files (endwith '.Hxs') are compiled files and not human readable. You have to do something before running msdn_crawer.py.

1. *Prepare for decompiling* Install Vistual Studio 2008 and VS 2008 SDK version 1.0 (MUST BE) or lower VS and VS SDK version
2. 
