# Capitulo 01: Básico


## Configuração básica

1. [Criar um usuário IAM para uso pessoal](#011---criar-um-usuário-iam-para-uso-pessoal)
2. [Ativar MFA (Multi-Factor Authentication)](#012---ativar-mfa-multi-factor-authentication)
3. [Desabilitar chaves para o usuário root](#013---desabilitar-chaves-para-usuário-root)

4. [Ativar alertas e/ou orçamento](#014---ativar-alertas-eou-orçamento) (afinal, não queremos gastar nada por enquanto. rs)
5. [Configurar a AWS CLI](#015---configurar-a-aws-cli)

## 01.1 - Criar um usuário IAM para uso pessoal

/Least privilege principle/. Princípio do menor privilégio: tenha apenas o mínimo de privilégios necessários para desempenhar suas funções.

Acessível em [Identity and Access Management Console](https://console.aws.amazon.com/iam/)


## 01.2 - Ativar MFA (Multi-Factor Authentication)

Mais uma camada de proteção para a conta. Aconselhável.

## 01.3 - Desabilitar chaves para o usuário root

Raciocínio análogo ao item [01.1](#011---criar-um-usuário-iam-para-uso-pessoal).

Acessível em [Identity and Access Management Console](https://console.aws.amazon.com/iam/).

Documentação: [O usuário raiz da conta da AWS](https://docs.aws.amazon.com/pt_br/IAM/latest/UserGuide/id_root-user.html)

## 01.4 - Ativar alertas e/ou orçamento

Bem, a ideia é termos o máximo de conhecimento com o mínimo de gastos, para isso, é possível estabelecer quantias máximas de gasto e alertas na página de [cobrança](https://console.aws.amazon.com/billing) no Console.

## 01.5 - Configurar a AWS CLI

Para utilizarmos a AWS CLI é necessário configurar as credenciais de acesso que serão utilizadas. Para isso, basta executar `$ aws configure` e inserir as credenciais de acesso.

```
$ aws configure
AWS Access Key ID [None]: ...
AWS Secret Access Key [None]: ...
Default region name [None]: ...
Default output format [None]: json
```

Essa configuração fica disponível em `~/.aws/config` e `~/.aws/credentials` no Linux, macOS e Unix.

Documentação: [Configurar o AWS CLI](https://docs.aws.amazon.com/pt_br/cli/latest/userguide/cli-chap-configure.html)
