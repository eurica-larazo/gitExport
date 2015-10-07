# gitExport
Export patch files from your GIT repository.


# Install
1. Download gitExport
2. Save to your `bin` directory. Ex(OSX). `/usr/bin/gitExport`
3. Change permission: `chmod +x gitExport`

# Parameters
1. location - `/Users/guest/Documents/patch.tar.gz`
2. since - `gitExport /Users/guest/Documents/patch.tar.gz 2015-07-01`
3. until - `gitExport /Users/guest/Documents/patch.tar.gz 2015-07-01 2015-07-30`

# How to use
Go to your GIT repository.

Export all updated files since the repo created.

`gitExport /Users/guest/Documents/patch.tar.gz`

  
Export all updated files since `date`. You can also specify time `2015-07-01-08:30`.

`gitExport /Users/guest/Documents/patch.tar.gz 2015-07-01`


Export all updated files since `date` until `date`.

`gitExport /Users/guest/Documents/patch.tar.gz 2015-07-01 2015-07-30`
