# Capitulo 02: Primeiros passos

## Criando um ambiente de desenvolvimento na nuvem

1. [O início do projeto](#021---inicio-do-projeto)
2. [Configurando o `provider`](#022---configurando-provider)
3. [Criar uma chave de acesso para os recursos](#023---criar-uma-chave-de-acesso-para-os-recursos)


## 02.1 - O início do projeto

Para iniciarmos o projeto, devemos entender primeiro como as informações serão organizadas.
No terraform, utilizamos a seguinte estrutura:

- Arquivos `*.tf`: onde ficam armazenados os códigos da infraestrutura.
> Nota: todos os arquivos `*.tf` no diretórios são carregados.
- Arquivo `terraform.tfstate`: onde ficam armazenados os dados do último estado da infra.
> Nota: o arquivo é sempre atualizado antes de qualquer ação do terraform. A atualização pode ser forçada através de `$ terraform refresh`.

Além disso, os arquivos `*.tf` são organizados com `blocks`.

## 02.2 - Configurando o `provider`



## 02.2 - Criar uma chave de acesso para os recursos

Para garantirmos o acesso aos recursos criados devemos criar uma chave de acesso que depois de criada pode ser referenciada na hora de invocarmos os novos recursos, geralmente com a expressão `key_name`.
