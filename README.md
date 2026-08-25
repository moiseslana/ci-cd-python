# ci-cd-python
# Pipeline CI/CD com Python e GitHub Actions

## 1. O que representa a etapa de CI neste projeto?

A etapa de Continuous Integration (CI) baixa o código, configura o ambiente Python, instala as dependências e executa os testes automatizados.

## 2. O que impede a execução do Continuous Delivery quando existe um defeito?

O job Continuous Delivery possui uma dependência do job Continuous Integration por meio de `needs: ci`. Se os testes do CI falharem, o Continuous Delivery não é executado.

## 3. Qual seria a próxima etapa necessária para transformar este pipeline em Continuous Deployment?

Seria necessário adicionar uma etapa de implantação automática, fazendo com que o código aprovado fosse publicado automaticamente em um ambiente de destino.
