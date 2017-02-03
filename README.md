# mod_substitute_append

##What is mod_substitute_append?

mod_substitute_append is an Apache httpd 2.2 module that provides ability to: * append strings at end of response bodies * search and substitute string inside response bodies * search and substitute string inside response bodies and, in case of unsuccessful search, append a string at end of response bodies

##Updates on version 1.1

Version 1.1 has been tested on several sites (about 160K and counting) since middle of April 2010.

##How it works?

If you have to manage many sites (i.e. hundreds of thousand of pages) and you need to modify every page adding simple javascript but you don't want modify all html sources (or you cannot modify because are dynamically created). * mod_substitute_append can be configured to inject html/javascript at end of response bodies * mod_substitute_append can search <body> and </body> tags and automagically include strings at the beginning and ending of a Web page * mod_substitute_append can search/replace html/javascript at end of response bodies. Injection will be executed only if searches were failed

This is particularly useful when html is produced by third part and you do not have even the privileges to modify it.
So it can be used to add javascript tracking code inside html pages, to wrap documents for a standard look and feel for a site (or to insert banners on any given document in a site). It can be also used together with mod_deflate
