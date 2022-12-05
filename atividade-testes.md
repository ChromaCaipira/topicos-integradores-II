# Testes Unitários e Automatizados

## **"Por que devemos fazer testes automatizados nas aplicações que desenvolvemos?"**

> Suponha que você esteja desenvolvendo um sistema bancário, do qual tem seu devido cadastro para ser feito pelo usuário. Deve-se então perceber que, para evitar futuros erros por um campo preenchido com dados inválidos ou já cadastrados, precisa haver testes em função de checar todos os possíveis contornos contra a intenção desejada daquela seção.
> 
> Entretanto, isso também leva à reflexão que, após a adição de cada nova *feature* no sistema, seja preciso mais outras diversas checagens e testes para cada elemento dela e, até mesmo, revisar o que essas mudanças irão causar no resto do sistema, performando uma regressão total do fluxo do sistema antes de implementar essa atualização.
> 
> Visto o quão custoso seria de parar toda a produção desse software e confiar o tempo para resolução do desenvolvimento e a qualidade desses testes a um time de pessoas, que está muito mais favorável ao atraso e falhas, é proposto o uso de testes automatizados por um "robô" para realizar todas essas tarefas de maneira bem mais rápida, eficiente, econômica, confiável e até escalonável, afinal a máquina poderá atender praticamente quaisquer o número de alterações feitas.

## **Testes Unitários**

Esse se responsabiliza por testar certas partes, ou unidades, individuais do código, seja toda uma classe ou apenas um dos seus métodos para checar se está funcionando como esperado pelo desenvolvedor e pode ser "commitada" ou se ainda necessita de correção.

## **Testes Instrumentalizados**

Já os instrumentalizados, como o próprio nome sugere, se sustentam de um instrumento/ferramenta para executar esse teste, como o emulador de android em projetos Android, e testando as funções da aplicação dentro da mesma.

## **Pirâmide de Testes**

De baixo para cima, ou da base ao topo, temos:
- Teste de Unidade: Como explicado anteriormente, testa em unidades do código.
- Teste de Integração: Fica responsável por como tais unidades, testadas na base, interagem entre si.
- Teste de End-to-End (e2e, fim a fim): Curiosamente, por fim há o teste simulando a utilização de um usuário de toda a aplicação, tentando imitar o que fariam e buscando por erros durante a execução. Entretanto, embora seja bastante utilizada, acaba consumindo bem mais recursos no seu uso, afinal será necessário toda a aplicação inicializada, diferente dos outros métodos que fazem de parte por parte.