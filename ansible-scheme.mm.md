## ansible-schema
- app1
app2
app39
app-qa
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

