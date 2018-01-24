
[![N|Solid](http://www.nexthop.net.br/static/images/logo.png)](http://www.nexthop.net.br)

# NextHop DokuWiki 

Container Docker para DokuWiki.



### Criando e inicializando o container:


```sh
mkdir data -p
docker run \
  --restart always \
  -itd \
  -v $('pwd')/data:/var/dokuwiki-storage \
  -p 80:80 \
  --name=nexthop-dokouwiki \
  --hostname nexthop-dokuwiki \
  nexthopsolutions/docker-dokuwiki
```


Para verificar o status:

```sh
$ docker ps
```
 

Go! 


Dúvidas ou informações: <elizandro@nexthop.net.br>
