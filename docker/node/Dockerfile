# FIXME: tutum/debian will be deprecated soon: https://github.com/tutumcloud/tutum-debian/blob/master/README.md
FROM tutum/debian:jessie

# Set aliyun repo for speed
RUN rm /etc/apt/sources.list
COPY sources.list /etc/apt/sources.list

RUN rm /etc/apt/apt.conf.d/docker-clean && apt-get update && apt-get install -y sudo net-tools wget sysvinit-core sysvinit sysvinit-utils curl vim man faketime unzip iptables iputils-ping logrotate && apt-get remove -y --purge --auto-remove systemd
