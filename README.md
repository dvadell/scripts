# scripts
Misc. scripts and utilities I use daily

### ro
ro runs something (defaults to /bin/bash) with a given directory as read-only.

Suppose you have some precious documents in the "Documents" folder.
Suppose you want to run a program, let's call it "indexer", that indexes
your documents. 

The indexer program only needs to read your documents, not write them.
Suppose you are paranoid and suspect that maybe indexer is going to
change something. 

Running:
> $ ro Documents indexer

will run "indexer", but "indexer" won't be able to write anything in the "Documents"
folder.

