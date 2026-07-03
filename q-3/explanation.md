# Explanation for Question 3

The experiment created one regular file, one hard link, and one symbolic link to compare how each behaves. The output from `ls -li` and `stat` showed that the hard link shares the same inode as the original file, while the symbolic link has its own inode and points to the target path. After removing the original file, the hard link still worked because it still referred to the same data, but the symbolic link broke because its target path no longer existed.
