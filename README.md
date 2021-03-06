# tdd-app

## Configuração do projeto 


### Pré-Requisitos

- [Node](https://nodejs.org/en/download/)
```
curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
```
```
sudo apt-get install -y nodejs
```

- npm sem sudo

```
mkdir ~/.npm-global
```
ADD no bashrc ou zshrc: 

export NPM_CONFIG_PREFIX=~/.npm-global
export PATH=~/.npm-global/bin:$PATH 


- Aumentar Watchers

```
echo fs.inotify.max_user_watches=524288 | sudo tee -a /etc/sysctl.conf && sudo sysctl -p

```
- Yarn
  
```
npm install -g yarn
```

### Dependências

```
yarn
```


### Executar os testes
```
yarn test:unit


yarn test:unit:watch
```

### Links
Tutorial [Fazendo uma aplicação em Vue.js com TDD](https://medium.com/magnetis-backstage/fazendo-uma-aplica%C3%A7%C3%A3o-em-vue-js-com-tdd-um-guia-extensivo-para-quem-quer-aprender-parte-1-d9952be6a29).
