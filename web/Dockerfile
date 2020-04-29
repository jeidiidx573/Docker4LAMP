FROM centos:centos7

RUN yum update -y

# apache
RUN yum install -y httpd
RUN yum install -y vim
RUN yum install -y perl
RUN yum install -y perl-CGI

# apache設定ファイルをコピー
COPY ./httpd.conf /etc/httpd/conf/httpd.conf

# httpd起動
CMD /usr/sbin/httpd -DFOREGROUND
