Como start o Electron
1° Utilize o comando npm init


2° Adicione o seguinte script no package.json
  "scripts": {
    "start": "electron ."
  }

3° npm install electron --save-dev

4° Configure o index.js da mesma forma que está no arquivo.

5° após tudo configurado, para starta o projeto basta utilizar o comando: npm start 

6° Para gerar o aplicativo desktop, é necessario instalar o electron package de forma global, utilizando o comando:
npm install electron-packager -g

7° Após a instalação do electron packager, navegue até a pasta do projeto electron e passe o seguinte comando:
electron-packager . "Nome Do Executavel" --platform=win32 --arch=x64

*No exemplo acima o projeto foi feito para ser executado na plataforma windows, para executar nas demais plataformas, basta consultar a documentação.

8° Tendo feito todos os passos de maneira correta, basta ir até a pasta do electron e abrir a pasta que foi gerada e executar o programa.

EXTRAS

Para alterar o icone de um aplicativo electron
    mainWindow = new BrowserWindow({
        icon: './src/assets/icons/app-logo.png'
    })
tambem é necessario fazer alterações no packager.json   "icon": "./src/assets/icons/app-logo.png"
