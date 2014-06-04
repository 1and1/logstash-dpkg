logstash-dpkg
=============

logstash dpkg packaging for debian.

Create source packages step by step:

```
git clone https://github.com/logstash/logstash.git logstash-v1.4.1
cd logstash-v1.4.1
git checkout vv1.4.1
tar czf ../logstash_v1.4.1.beta1.orig.tar.gz ../logstash-v1.4.1
git clone https://github.com/1and1/logstash-dpkg.git debian
cd ..
dpkg-source -b logstash-v1.4.1
```

Now the binary package can be built with dpkg-buildpackage or pbuilder the usual way.
