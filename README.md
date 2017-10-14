# XML-RPC-PHP7
XML-RPC modified for PHP7

# Modifications
Using repDeprec.pl (available from http://nthinking.net/index.html#reDeprec )
modifications to an old installation of PEAR:XML-RPC was performed to make it
compatible with PHP7.

The regular expression matching isn't perfect, and additional tweaks were
required to fix the errors which cropped up. 

The included files are working for my legacy product, but I cannot promise they will
work for anyone else.

However, it has made it possible for a <PHP5.3 application to function in a PHP7
environment, in so far as this XML-RPC library is concerned.

# The Problem
Legacy php code had functions replaced as follows:

split -> replaced by -> preg_split (and additional slashes/regex)

ereg -> replaced by -> preg_match (and additional slashes/regex)

ereg_replace -> replaced by -> preg_replace (and additional slashes/regex)
