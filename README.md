# Angular Ref

O principal objetivo deste repositório é centralizar alguns conceitos muito utilizados do angular (como a criação de componentes, servicos, bind de informações, etc) em um local de fácil acesso e para rápida consulta para o desenvolvimento de um novo projeto. Conforme novas experiências, irei adicionar novos conteúdos.

Este projeto foi criado seguindo o passo a passo do [Tutorial do Angular](https://angular.io/tutorial/). 

Ainda falta implementar a parte final, referente aos Observables e uso do HttpClient e finalizar a implementação da etapa de rotas.

Abaixo, alguns comandos de referência para simplificar a implementação de um novo projeto em angular:

**Para instalar o Angular:** npm install -g @angular/cli
**Para criar um novo app:** ng new <nome do app>
**Para compilar o projeto e já abrir em uma nova janela:** ng serve -o (ou --open)
**Para criar um novo componente:** ng g c <caminho + nome do componente> *ou* ng generate component <caminho + nome do componente>
**Para criar um novo serviço:** ng g s <caminho + nome do serviço> *ou* ng generate service <caminho + nome do serviço>
**Para gerar o módulo de rotas:** ng generate module app-routing --flat --module=app 
- *--flat* faz com que o módulo seja criado fora de uma pasta específica, diretamente na pasta app. 
- *--module* informa para o cli registrar o módulo diretamente no array de imports do AppModule

### Importante
1. Todo novo componente criado precisa ser declarado no app.component.ts, dentro do declarations. (E, obviamente, importado para dentro do .ts, com o *import {} from ''*). Se utilizar o cli para gerar o componente, isto é feito automaticamente.