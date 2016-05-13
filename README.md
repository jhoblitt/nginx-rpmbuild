Modified nginx RPM spec to add "nginx-sticky-module-ng" module
===

* Based on this SRPM: http://nginx.org/packages/centos/7/SRPMS/nginx-1.10.0-1.el7.ngx.src.rpm
* "nginx-sticky-module-ng": https://bitbucket.org/nginx-goodies/nginx-sticky-module-ng/get/c78b7dd79d0d.zip

Build
---

```
sudo yum install -y perl-devel perl-ExtUtils-Embed GeoIP-devel libxslt-devel gd-devel
rpmbuild -ba rpmbuild/SPECS/nginx.spec 
```
