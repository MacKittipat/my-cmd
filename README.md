# my-cmd

## Completely remove package

```
sudo apt-get purge ${package}
sudo apt-get --purge remove ${package}
```

Ref : http://askubuntu.com/a/151943

## Remove icon from launcher

Remove from the following location

```
/usr/share/applications
/usr/local/share/applications
~/.local/share/applications
```

Ref : http://askubuntu.com/a/71245

## Find permission number

```
stat -c "%a %n" *
stat -c %a ${file_path}
```

Ref : 
- http://askubuntu.com/a/152003
- http://askubuntu.com/a/29548

## Scroll MySQL table

```
 mysql -uroot -p --pager="less -S" ${db}
```

Ref : http://techmonks.net/horizontal-scrolling-for-mysql-queries-in-linux/

## Set executable java path

```
sudo update-alternatives --install "/usr/bin/java" "java" "${PATH}/jdk/bin/java" 1
sudo update-alternatives --install "/usr/bin/javac" "javac" "${PATH}/jdk/bin/javac" 1
sudo update-alternatives --install "/usr/bin/javaws" "javaws" "${PATH}/jdk/bin/javaws" 1
```

Ref : 
- http://askubuntu.com/questions/315646/update-java-alternatives-vs-update-alternatives-config-java
- http://askubuntu.com/questions/121654/how-to-set-default-java-version
