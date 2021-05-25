# 命令

- mvn -version

- 安装步骤
  - 下载maven安装包
    - http://maven.apache.org/download.cgi
  - 修改环境变量
    - vim ~/.bash_profile
    ***
    export M2_HOME=/usr/local/maven/apache-maven-3.8.1
    export PATH=$PATH:$M2_HOME/bin
    ***
    - source ~/.bash_profile

- 修改setting.xml配置
  - 修改镜像地址
    <mirror>
        <id>rjoy-releases</id>
        <name>nexus maven</name>
        <url>
            https://repository.rjoy.com:8443/repository/maven-public
        </url>
        <mirrorOf>central</mirrorOf>
    </mirror>

  - 修改账号信息
    <server>
      <id>nexus</id>
      <username>dengjuming</username>
      <password>bGg5y8M76</password>
    </server>