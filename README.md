# Access-Denied Datasets

We release the datasets we used to study real-world access-denied issues. Some of the findings are summarized in the paper,

T. Xu, H. M. Naing, L. Lu, and Y. Zhou, How Do System Administrators Resolve Access-Denied Issues in the Real World? Proceedings of the 35th Annual CHI Conference on Human Factors in Computing Systems (CHI'17), May 6-11, 2017, Denver, CO, USA. [[Download](http://cseweb.ucsd.edu/~tixu/papers/chi17.pdf)]

Please cite the paper if you use the datasets :-)

# What is included in the datasets?

The dataset contains 486 cases reported upon three software projects: Apache HTTP server (http://httpd.apache.org/), MySQL (https://www.mysql.com/), Hadoop (https://hadoop.apache.org/), and CentOS (https://www.centos.org/).

| Software      |  #cases    |  period    |
| ------------- |:----------:|:----------:|
| Apache        |  126       | 2001--2016 |
| MySQL         |  117       | 1999--2016 |
| Hadoop        |  101       | 2009--2016 |
| CentOS        |  142       | 2005--2016 |

We do not consider version in this datasets, which means a case could be from any version of the software.

# How did we collect the datasets?

Please refer to the paper for details. Basically, all the cases are collected from mailing list archives and Q&A forums the studied software, including

1. ServerFault (http://serverfault.com/)

2. StackOverflow (http://stackoverflow.com/)

3. Database Administrators (http://dba.stackexchange.com/)

4. CentOS Forums (https://www.centos.org/forums/)

5. Apache HTTP Server Users Mailing Lists (<users@httpd.apache.org>)

6. MYSQL General List (<mysql@lists.mysql.com>)

7. Hadoop User Mailing Lists (<user@hadoop.apache.org>)

8. CentOS Mailing Lists (https://lists.centos.org/pipermail/centos/)

We crawled/downloaded the entire mailing list archives and online posts with specific tags from the first mail/post to the most recent ones at the collection period. The collection is conducted during January to March in 2016. We automatically parsed the entire mailing list archives and all the posts on the above sources via a number of filter pipelines. At the end of the pipeline, we manually collect the files from the sources.

# How can you use the datasets?
Each data file is in the CSV format (the first row is a title row); you can parse it using CSV parsers. If you are not clear about any field, you can post an issue on this repo and I will answer there.

