<p align="center">
  <img width="450" src="./src/utils/adguard/logo.svg" alt="Adguard Logo">
</p>

<!-- <h1 align="center">Adguard</h1> -->

***

#### [Adguard](https://adguard.com/) é uma ferramenta única que bloqueia anúncios em aplicativos e navegadores, mesmo sem privilégios de um usuário root, protege sua privacidade e ajuda você a gerenciar seus aplicativos. Isso inclui anúncios em vídeo, anúncios em aplicativos, jogos e qualquer site que você possa imaginar

<h5 style="color: #42b983">Bloqueio de anúncios</h5>

* O AdGuard irá bloquear todos os banners irritantes, pop-ups e anúncios de vídeo.

<h5 style="color: #42b983">Proteção de privacidade</h5>

* O AdGuard oculta seus dados da maioria dos rastreadores e sistemas analíticos que vigiam a internet.

<h5 style="color: #42b983">Segurança da navegação</h5>

* Graças ao AdGuard, você será capaz de evitar todos os sites fraudulentos, phishing e malware.

<h5 style="color: #42b983">Controle parental</h5>

* Proteja seus filhos online, restringindo o acesso a conteúdo adulto e inapropriado.

<h4 style="color: #42b983">Por que vale a pena instalar o AdGuard no Chrome:</h4>

* Remove anúncios e bloqueia rastreamento;
* Protege dados pessoais: o AdGuard cuidará de todos os rastreadores que tentem espionar você na internet;
* Todos os sites maliciosos e perigosos serão bloqueados;
* O AdGuard também alertará sobre sites de reputação duvidosa;
* O Chrome é legitimamente considerado um dos navegadores mais rápidos que existem. Com o AdGuard ele funcionará ainda mais rápido!

<h4 style="color: #42b983">Docker Run</h4>

~~~bash
docker run --name Adguard\
    --restart unless-stopped\
    -v /my/own/workdir:/opt/adguardhome/work\
    -v /my/own/confdir:/opt/adguardhome/conf\
    -p 53:53/tcp -p 53:53/udp\
    -p 67:67/udp -p 68:68/udp\
    -p 80:80/tcp -p 443:443/tcp -p 443:443/udp -p 3000:3000/tcp\
    -p 853:853/tcp\
    -p 784:784/udp -p 853:853/udp -p 8853:8853/udp\
    -p 5443:5443/tcp -p 5443:5443/udp\
    -d adguard/adguardhome
~~~

<h4 style="color: #42b983">Docker-Compose</h4>

~~~yaml

version: "2"
services:

  adguardhome:
    image: adguard/adguardhome
    container_name: Adguard
    ports:
      - 53:53/tcp
      - 53:53/udp
      - 784:784/udp
      - 853:853/tcp
      - 3000:3000/tcp
      - 80:80/tcp
      - 443:443/tcp
    volumes:
      - adguard_work:/opt/adguardhome/work
      - adguard_conf:/opt/adguardhome/conf
    restart: unless-stopped

volumes:
  adguard_conf:
  adguard_work:
  
~~~

<h4 style="color: #42b983">Simple Review</h4>

<!-- <details>
<summary>Click Para ver os Screenshots</summary>
  
</details> -->

<p align="center">
    <img src="./src/utils/adguard/info.gif"/>
</p>
