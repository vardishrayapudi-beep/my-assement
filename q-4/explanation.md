# Explanation for Question 4

The investigation used `lsof` and `/proc/$$/fd` to inspect the file descriptors opened by the shell. This showed that the shell had opened the test log file on descriptor 3 and that standard streams were attached to the terminal. The redirection commands demonstrated how stdout, stderr, and combined output can be captured into files, which is a core part of Linux I/O management.
