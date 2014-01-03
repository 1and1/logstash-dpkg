logstash-dpkg
=============

logstash dpkg packaging for debian.

Create source packages step by step:

```
git clone https://github.com/logstash/logstash.git logstash-1.3.2
cd logstash-1.3.2
git checkout v1.3.2
tar czf ../logstash_1.3.2.orig.tar.gz ../logstash-1.3.2
git clone https://github.com/1and1/logstash-dpkg.git debian
cd ..
dpkg-source -b logstash-1.3.2
```

Now the binary package can be built with dpkg-buildpackage or pbuilder the usual way.
