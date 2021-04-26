## ansible-schema
- app1
app2
app3
app4
app6
app7
app8
app9
app18
app19
app20
app21
app22
app23
app25
app26
app27
app28
app30
app31
app32
app33
app34
app35
app36
app37
app38
app39
app-qa
app-dev
  - configure
    - ssh client
    - ssh server
    - systemctl
    - rc.local
    - users
    - rsyslog config for haproxy
    - logrotate
    - rsyslog
    - nginx
  - install n run
    - sshd
    - sudo
    - node exporter
    - when: ansible_distribution == 'Ubuntu' install
      - haproxy=1.8*
      - socat
      - mysql-client
    - haproxy-exporter (0.8.0)
    - nginx
      - "libluajit-5.1-dev"
      - "libgeoip-dev"
      - "lua5.2"
      - "libmaxminddb0"
      - "libmaxminddb-dev"
      - nginx_1.12.1
      - nginx-vts-exporter
      - nginx-log-exporter
    - php5.6
      - "php5.6-cli"
      - "php5.6-curl"
      - "php5.6-fpm"
      - "php5.6-json"
      - "php5.6-mysql"
      - "php5.6-opcache"
      - "php5.6-pgsql"
      - "php5.6-xml"
      - "php5.6-redis"
      - "php5.6-memcache"
      - "php5.6-mbstring"
      - "libboost-thread1.58.0"
      - "libboost-thread1.58.0"
      - "librdkafka1"
  - install
    - git
    - rsync
    - python-pip
    - s3cmd    

  - when: ansible_pkg_mgr == "apt" install
    - apt-transport-https
    - tmux
    - htop
    - atop
    - iptables-persistent
    - curl
    - nscd
    - ipmitool    
  
- app-lb1
app-lb2
app-lb.dev
  - configure
    - ssh client
    - ssh server
    - systemctl
    - rc.local
    - users
  - install n run
    - sshd
    - sudo
    - node exporter
    - nginx
      - "libluajit-5.1-dev"
      - "libgeoip-dev"
      - "lua5.2"
      - "libmaxminddb0"
      - "libmaxminddb-dev"
      - nginx_1.12.1
      - nginx-vts-exporter
      - nginx-log-exporter 
  - when: ansible_pkg_mgr == "apt" install
    - apt-transport-https
    - tmux
    - htop
    - atop
    - iptables-persistent
    - curl
    - nscd
    - ipmitool  

- mysql-master1
mysql-master2
mysql-slave01
mysql-slave02
mysql-slave03
mysql-slave04
mysql-slave05
mysql-slave06
  - configure
    - ssh client
    - ssh server
    - systemctl
    - rc.local
    - users
  - install n run
    - sshd
    - sudo
    - node exporter 
  - when: ansible_pkg_mgr == "apt" install
    - apt-transport-https
    - tmux
    - htop
    - atop
    - iptables-persistent
    - curl
    - nscd
    - ipmitool  

