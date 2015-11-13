# gitExport
Export patch files from your GIT repository.


# Install
1. Download gitExport
2. Save to your `bin` directory. Ex(OSX). `/usr/bin/gitExport`
3. Change permission: `chmod +x gitExport`

# Parameters
1. path - location for saving patch file.
2. since - export starting date(date and time).
3. until - export ending date(date and time).
4. commit - commit id
5. include - list of file paths you wish to include
6. ignore - list of file paths you wish to ignore
7. log - flag for including log file to patch. By default log file is not included.

# How to use
Go to your GIT repository.

Export all updated files since the repo was created.

`gitExport path=/Users/guest/Documents/patch.tar.gz`



Export using `date` parameters.

`gitExport path=/Users/guest/Documents/patch.tar.gz since=2015-07-01`

or

`gitExport path=/Users/guest/Documents/patch.tar.gz since=2015-07-01 until=2015-07-20`



Export using `commit id`.

`gitExport path=/Users/guest/Documents/patch.tar.gz commit=b70f64209a0ee0844f74f0590070d590c19eb048`



Include files to your patch.

`gitExport path=/Users/guest/Documents/patch.tar.gz commit=b70f64209a0ee0844f74f0590070d590c19eb048 include=path/file1,path/file2,path/file3`



Ignore files to your patch.

`gitExport path=/Users/guest/Documents/patch.tar.gz commit=b70f64209a0ee0844f74f0590070d590c19eb048 ignore=path/file1,path/file2,path/file3`




Generate log file.

`gitExport path=/Users/guest/Documents/patch.tar.gz commit=b70f64209a0ee0844f74f0590070d590c19eb048 log`
