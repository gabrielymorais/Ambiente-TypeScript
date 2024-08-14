# Configuracao do TypeScript

1. Inicializar um projeto Node.js
- `npm init`

2. Instalar o TypeScript
-  Instalacao Global (na maquina toda): `npm install -g typescript`
-  Instalacao Local (apenas no projeto)  `npm install typescript -D`

3. Utilizar o TypeScript instalado para transpilar o nosso codigo (Converter de TS para JS)
    - `npx tsc nomeArquivo.ts` (irá gerar um arquivo JS)
    - Sempre que mudar algo no codigo `nomeArquivo.ts` deve-se repetir a compilacao acima.
    - Para nao precisar ficar sempre compilando, fazemos assim: `npx tsc nomeArquivo.ts --watch`

# Como configurar tudo do typescript dentro do nosso projeto com muitos arquivos .ts

1.   Em projetos grandes, com muitos arquivos .ts nao é muito interessante todo esse trabalho em linha de comando, para isso, podemos ter um arquivo com todas as configuracoes possiveis para o TypeScript
- `npx tsc --init` Inicializa todas as configuracoes do typescript dentro do projeto, surgindo um arquivo tsconfig.json
- Para compilar programas .ts, vai ser preciso apenas `npx tsc`
