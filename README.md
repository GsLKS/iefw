# IEFW - IECloud Framework

Um Framework de upload de arquivos locais para a IECloud

### Instalado **IEFW**

##### NPM

```
npm install --no-bin-links iefw
```

##### [MbCL Repo](https://repo.mbcl.ml):

```
./mbcl --dl latest/iefw
```

### Enviando Arquivos


**Exemplo de código:** [(disponível aqui)](/examples/default.js)

```js
const ie = require('iefw');
const fileUploader = new ie();

const filePath = './path/to/example.txt';

fileUploader.uploadFile(filePath)
  .then((fileUrl) => {
    console.log(`Arquivo enviado com sucesso. URL do arquivo: ${fileUrl}`);
  })
  .catch((err) => {
    console.error('Erro ao enviar o arquivo:', err);
  });
```

<hr>

[![npm](https://avatars.githubusercontent.com/u/6078720?s=25&v=4)](https://www.npmjs.com/package/iefw)
