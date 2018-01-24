
[![N|Solid](http://www.nexthop.net.br/static/images/logo.png)](http://www.nexthop.net.br)

# NextHop DokuWiki 

Container Docker para DokuWiki.



### Criando e inicializando o container:


```sh
docker volume create dokuwiki-data
docker run \
  --restart always \
  -itd \
  -v dokuwiki-data:/var/dokuwiki-storage \
  -p 80:80 \
  --name=nexthop-dokouwiki \
  --hostname nexthop-dokuwiki \
  nexthopsolutions/docker-dokuwiki
```


Após a instalação, acesse:

```sh
http://<seuip>/install.php
```
 

E complete a instalação!

Go! 


Dúvidas ou informações: <elizandro@nexthop.net.br>
