# File-Comparison

After making a backup, I always have my file manager count the files and directories of all my partitions to compare the figures with the respective counts of the just finished backup. And sometimes, there seems to be the one or other "$RECYCLE.BIN" or "System Volume Information" that seem to be responsible for a slight difference in the counts. Although the help page of robocopy states that "System Volume Information" is not being copied when mirroring a partition, "$RECYCLE.BIN" is still not skipped.
So, just to be sure everything has really gotten backed up, but more for fun than out of neccessity, I wrote this program that uses a recursive algorithm and compares files and directories by their names (without system files) and shows found differences in the output.
