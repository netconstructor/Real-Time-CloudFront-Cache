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


data_dir - the path to the directory containing the uploaded data


index_file - the path location for the file index which is maintained


dir_prefix - required if your data_dir path is different at CloudFront

   FOR EXAMPLE:
   - In your system you have the following data_dir setting
            data_dir = '/data'

   - Your CloudFront URL is something like
            http://domain-name.com/category/news/

   - so in this case you would set dir_prefix to
            '/category/news/'


