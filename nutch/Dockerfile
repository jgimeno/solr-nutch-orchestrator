FROM jgimeno/nutch

ADD conf/nutch-site.xml conf/nutch-site.xml
ADD conf/regex-urlfilter.txt conf/regex-urlfilter.txt

RUN mkdir urls
ADD urls/seed.txt urls/seed.txt
