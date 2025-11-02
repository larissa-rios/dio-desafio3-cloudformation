# Desafio 3: Implementação de Infraestrutura como Código (IaC) com CloudFormation

Repositório criado para a entrega do Desafio de Projeto 3. Este laboratório foi desafiador e focado no uso do **AWS CloudFormation** para provisionar recursos.

##  O Grande Aprendizado 

A parte mais difícil para mim foi a transição do método de "clicar" (o console) para o método de "código" (IaC). Mas o aprendizado é enorme:

* **O que é IaC:** É um jeito de dizer para a AWS o que eu quero (ex: "quero um Bucket S3") usando um arquivo de texto (o template YAML), e não clicando. O código é a sua infraestrutura.
* **A "Mágica" da Stack:** O CloudFormation lê esse código e cria tudo sozinho. O nome técnico para esse "projeto" que o CloudFormation gerencia é **Stack** (Pilha).

Eu entendi que a principal vantagem disso não é só a velocidade, mas o **controle**: se eu apagar a Stack, ele apaga *tudo* o que criou, o que garante a limpeza e evita custos por esquecimento.

## 🚀 Prática Realizada 

Como o arquivo ZIP do desafio não foi fácil de acessar, o foco foi praticar a criação da Stack com um template base:

1.  **Template:** Foi utilizado um template YAML simples (o código) que descreve um **Amazon S3 Bucket**.
2.  **Criação:** Fiz o upload do template e criei a Stack (`Desafio3-IaCSimples`) no serviço CloudFormation.
3.  **Resultado:** O Bucket S3 foi criado com sucesso.
4.  **Limpeza:** Para não gerar custos, a Stack foi deletada, e o CloudFormation automaticamente removeu o Bucket S3, provando o poder do IaC na limpeza.
