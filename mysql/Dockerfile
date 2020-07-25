FROM mysql:5.7

# MySQLの操作ログのファイルを作成
RUN touch /var/log/mysql/mysqld.log

ADD ./conf.d/my.cnf /etc/mysql/my.cnf
RUN chmod 644 /etc/mysql/my.cnf