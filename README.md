## O que é Javascript 😎 ?
É uma linguagem de alto nível, single thread e interpretada. Criado por Brendan Eich, com a ideia de facilitar o desenvolvimento WEB.
- ### Memory heap    
    Memória prè alocada.
- ### Call stack    
    É uma única ``thread de execucao``, onde são executadas as funções.
- ### WEB APIs    
    Sao recursos disponibilizados pelo browser.
- ### Event loop    
    Gerencia as chamadas assíncronas usando duas filas. ``Microtask`` e ``Macrotask``.
- ### Pilhas    
    Uma coleção de elementos e ideia de um conjunto de caixas empilhadas. No javascript é usado o padrão **``LIFO``** (Last in First Out). O último que entra é o primeiro a sair.
- ### Microtask    
    Após a execução de chamadas síncronas na ``Call stack`` a microtask primeira fila a ser consumida, é alocado nelas apenas algumas funções assíncronas, sendo as principais. ``Promisse`` e ``async``.
- ### Macrotask     
    É consumida quando a fila ``Microtask`` estiver vazia, as funções são fornecidas pelo **browser** usando ``WEB APIs``.

    
<br/>

Ilustração:

<br/>

![https://dev.to/lydiahallie/javascript-visualized-promises-async-await-5gke](https://res.cloudinary.com/practicaldev/image/fetch/s--05Fi8vBq--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_66%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/42eatw03fcha0e1qcrf0.gif)
<sub>ref: Lydia Hallie</sub>


<br/>


## O que é V8 Engine ?
É uma engine open source criada pela Google em ``C++``, que interpreta, converte e compilado para código de máquina em tempo de execução.

- ### Parser
    Compila o código para ``AST (Abstract Syntax Tree)``. Uma representação abstrata do código.
- ### Garbage Collector
    Gerencia a alocação de memória removendo itens não usados.
- ### Ignition
    È um interpretador que converte ``AST`` para ``bytecode``
- ### Turbo FAN 
    Compilador otimiza o código em tempo de execução e compilado para código de máquina.

<br/>

Ilustração:

<br/>

![https://www.geeksforgeeks.org/what-is-the-relationship-between-node-js-and-v8/](https://media.geeksforgeeks.org/wp-content/uploads/20211002235143/workinggfg.png)

<sub>ref: geeksforgeeks</sub>