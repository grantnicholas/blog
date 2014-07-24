---
layout: post
title: Bypass sql file upload limits
---

Was trying to upload a sql file through drupal's built in FTP in order to migrate a database. There was an upload limit that I needed to bypass.
By zipping up the file I was able to get around the upload limit.  

cd ~/mysql/bin
mysqldump -u username databasename > thesqlfile.sql
gzip thesqlfile.sql

and voila. a zipped up sql file ready to be uploaded.



