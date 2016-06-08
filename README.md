# ida-msdn-annotator
Add MSDN annotations to IDA imported functions and structures

---------------------------------------------------------------------------------------------------------------------

This work is almost based on Moritz Raabe and William Ballenthin's work at Fireeye.

I strongly recommend you to refer the original <a href="https://github.com/fireeye/flare-ida"> flare-ida </a> project.

##The differences include:
1. Add a new plugin responsible for adding annotations to structure types and members.
2. Add a new script to parese windows sdk help-htmls to extract structures' annotations.
3. Add new regrex rules to parse the imported functions' name in IDA.

##Usage

