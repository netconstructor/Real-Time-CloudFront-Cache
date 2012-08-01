Real-Time-CloudFront-Cache
==========================

This script was created to create a "Live, Auto Updating Real-Time Cache for Amazon CloudFront".

In short, this script preforms the following functions:

1) automatically scans all your Amazon CloudFront directories
2) automatically builds a complete file index of all found files in all directories.
3) automatically recognizes which files were modified since it last checked
4) automatically clears the cache of all traces of these found files on the Amazon CloudFront servers.

Benefits: Depending on your website/application, by integrating this script you now have a very simple method of scaling your application horizontally utilizing the power of all of Amazons inexpensive caching servers while ensuring all of your website content is automatically kept current.

Usage: script.py data_dir [index_file] [dir_prefix]

data_dir - path to directory with uploaded data

index_file - path to files index

dir_prefix - needed if you data_dir path is different from url at CloudFront.For example: Your data_dir is '/data' but url at CloudFront is http://url.com/social/data/ so dir_prefix will be '/social/data/'

