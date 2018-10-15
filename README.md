# Advanced Bash Homework

### Description
To fix a website that has some error in it, given access to the files on the server. Folder should only be accessible by the vagrant user. The files in the assets folder have the wrong file extension. Rename multiple files at once with the correct extensions.
Deleting multiple files with similar names with a single command. Making a hidden file appear. The owner needs full permissions but group only need to be able read to the files.

### Steps
1. ```sudo chown -R vagrant site``` - changes owner to vagrant user
2. ```chmod -R 700 site``` - gives full permissions to the owner only
3. ```cd site``` - go into the site directory
4. ```cd images``` - go into the images directory
5. ```file *file name*``` - see that they're jpgs
6. ```rename.ul -v "s/txt/jpg/g" *.txt images``` - renaming all txt types to jpgs
7. ```rm puppy*``` - deletes all 'puppy' files
8. ```cd ..``` - go back one directory
9. ```ls -a``` - list all files within directory
10. ```mv .index.html index.html``` - renaming it without the dot so it is no longer hidden
11. ```chmod g+r,o+rwx *``` - changing permissions: group can read; owner can read, write, and execute.

### Challenges
It was quite difficult to know where to carry out the first two steps (in the ubuntu user which is within the home directory).

### Learning Points
Learning new commands has helped me understand the whole process a bit better.