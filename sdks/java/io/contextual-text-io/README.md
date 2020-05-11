#STATUS: Exploration phase.

##Contextual TextIO
Exploration of more advanced TextIO which is aware of contextual information from the file.
Some goals of the exploration (TBC).

# FileMetadata
Access file information per row in DoFn's

# Line position
Access ordinal position within original file per row.

# RFC4180
Fields containing line breaks (CRLF), double quotes, and commas should be enclosed in double-quotes.  For example:

       "aaa","b CRLF
       bb","ccc" CRLF
       zzz,yyy,xxx

If double-quotes are used to enclose fields, then a double-quote appearing inside a field must be escaped by preceding it with another double quote.  For example:

       "aaa","b""bb","ccc"
# Better watermark for continuous file read
Ability to have better watermark for continuous file read, where even time is stored in the rows of the file. 

# Dealing with first header line in files
Option to remove the first line of the file. 
Option to have the header be present with each row of data.
Option to have the Row object be created with header information.
