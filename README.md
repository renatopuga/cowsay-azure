# cowsay-azure

```bash
 _____________________________ 
< Azure Blockchain Workbench! >
 ----------------------------- 
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```




## Documentação 

* https://pad.riseup.net/p/fiapblock-2019-10

* https://docs.microsoft.com/en-us/azure/blockchain/workbench/deploy

* https://101blockchains.com/azure-blockchain/

  

## Introdução

Fonte: https://101blockchains.com/azure-blockchain/

### O que é o Azure Blockchain?

A Microsoft é líder em tecnologia com raízes na tecnologia de nuvem. Sua plataforma de nuvem do Azure provou seu domínio. Mas, a Microsoft sabia que eles têm um papel mais importante a desempenhar no mercado. É aí que entram os aplicativos Azure Blockchain e Azure Blockchain. Também podemos chamar de "Blockchain no Azure".

### Blockchain como serviço não é blockchain!

Se você é novo no blockchain, pode ficar confuso com os termos. Ou talvez você ache que o BaaS do Azure e a tecnologia blockchain são iguais? Mas isso não é verdade.

Blockchain é a tecnologia que possui recursos como transparência, integridade, descentralização e assim por diante. No entanto, existem diferentes tipos de blockchain, incluindo híbrido, privado, etc. Mas, um verdadeiro blockchain é dedicado principalmente ao fato de executar uma rede verdadeiramente descentralizada, e não a variações dela. A verdadeira ideia de blockchain surgiu com o bitcoin. É um acúmulo de rede completamente descentralizado de nós que cuida do consenso geral.

O Blockchain como serviço (BaaS) do Azure, por outro lado, usa a tecnologia blockchain e presta serviço aos seus clientes. No entanto, sua abordagem não é descentralizada. O BaaS é totalmente o oposto do descentralizado, pois oferece uma plataforma centralizada para vender, construir e comercializar blockchain. O BaaS como um ecossistema fornece valor, mas, para fazer isso, tem que ir contra a idéia básica da blockchain descentralizada.

### Redes Blockchain suportadas pelo Azure Blockchain

No momento da redação deste artigo, o Serviço Blockchain do Azure oferece suporte ao Ethereum [Quorum](https://101blockchains.com/quorum-blockchain-tutorial/) Ledger, [Corda](https://101blockchains.com/corda-blockchain/) e [Hyperledger](https://101blockchains.com/hyperledger-blockchain/) Fabric. Como empresa, você não precisa gerenciar o razão. Além disso, não há custo associado ao próprio razão. No entanto, você precisa pagar pelo desenvolvimento do aplicativo e seu custo quando ele é executado na blockchain. Você obterá máquinas virtuais e a infraestrutura associada alocando os recursos e tempo necessários.

## O que é o Azure Blockchain Workbench?

A visualização do Azure Blockchain Workbench é uma coleção de serviços e recursos do Azure projetados para ajudá-lo a criar e implantar aplicativos blockchain para compartilhar dados e processos de negócios com outras organizações

## Arquitetura Azure Blockchain Workbench

![https://docs.microsoft.com/en-us/azure/blockchain/workbench/media/architecture/architecture.png](https://docs.microsoft.com/en-us/azure/blockchain/workbench/media/architecture/architecture.png)



## Microsoft AZURE

1. Conta gratuita: Free Azure Trial: http://azure.microsoft.com/en-us/free/
2. Clique em **Marketplace > Azure Marketplace** e na busca procure por: **Azure Blockchain Workbench**
3. Em Azure Blockchain Workbench clique no botão **Create**.

```bash
 __________________________________ 
/ Funcionou apenas com a Location: \
\ Southeast Asia!                  /
 ---------------------------------- 
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```



### Basic Settings 

| Configuração                         | Descrição                                                    |
| :----------------------------------- | :----------------------------------------------------------- |
| Prefixo do recurso                   | Identificador único curto para sua implantação. Este valor é usado como base para nomear recursos. |
| Nome de usuário da VM                | O nome do usuário é usado como administrador para todas as máquinas virtuais (VM). |
| Tipo de Autenticação                 | Selecione se deseja usar uma senha ou chave para conectar-se às VMs. |
| Senha                                | A senha é usada para conectar-se às VMs.                     |
| SSH                                  | Use uma chave pública RSA no formato de linha única começando com **ssh-rsa** ou use o formato PEM de várias linhas. Você pode gerar chaves SSH usando `ssh-keygen`no Linux e OS X ou usando PuTTYGen no Windows. Mais informações sobre as chaves SSH, consulte [Como usar chaves SSH com o Windows Azure](https://docs.microsoft.com/en-us/azure/virtual-machines/linux/ssh-from-windows) . |
| Senha do banco de dados e Blockchain | Especifique a senha a ser usada para acessar o banco de dados criado como parte da implantação. A senha deve atender a três dos quatro requisitos a seguir: o comprimento precisa ter entre 12 e 72 caracteres, 1 caractere em minúscula, 1 caractere em maiúscula, 1 número e 1 caractere especial que não é sinal de número (#), porcentagem (% ), vírgula (,), estrela (*), aspas (`), aspas duplas ("), aspas simples ('), traço (-) e semicoluna (;) |
| Região de implantação                | Especifique onde implantar os recursos do Blockchain Workbench. Para uma melhor disponibilidade, isso deve corresponder à configuração do **local** . |
| Inscrição                            | Especifique a assinatura do Azure que você deseja usar para sua implantação. |
| Grupos de recursos                   | Crie um novo grupo de recursos selecionando **Criar novo** e especifique um nome exclusivo para o grupo de recursos. |
| Localização                          | Especifique a região que você deseja implantar a estrutura.  |



### Basic valores

* Subscription: Azure para Estudantes
* Resource group: pugafiapasiarg
* Location: Southeast Asia
* Resource prefix: pugafiap1
* VM user name: pugavm1 



### Advanced Settings

| Configuração                                    | Descrição                                                    |
| :---------------------------------------------- | :----------------------------------------------------------- |
| Camada de preços do Serviço Blockchain do Azure | Escolha a camada **básica** ou **padrão do** Serviço Blockchain do Azure usada para o Blockchain Workbench |
| Configurações do Azure Active Directory         | Escolha **Adicionar mais tarde** . Nota: Se você optar por [pré-configurar o Azure AD](https://docs.microsoft.com/en-us/azure/blockchain/workbench/deploy#azure-ad-configuration) ou estiver reimplantando, escolha *Adicionar agora* . |
| Seleção de VM                                   | Selecione o desempenho de armazenamento preferido e o tamanho da VM para sua rede blockchain. Escolha um tamanho de VM menor, como o *Standard DS1 v2,* se você estiver em uma assinatura com baixos limites de serviço, como o nível gratuito do Azure. |



### Advanced Valores

1. Create new
2. Azure Blockchain Service Pricing Tier: Basic
3. Azure Active Directory Settings: Add Later
4. VM selection: 1x Standard DS1 v2 (1 vcpu, 3.5 GiB memory)



```bash
 ____________________________________ 
/ WTF? 90min??? Tempo pra ler a      \
\ documentação não vai faltar LOL /
 ------------------------------------ 
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

NOTA: **A implantação pode levar até 90 minutos.**  Maiores informações, acesse: https://docs.microsoft.com/en-us/azure/blockchain/workbench/deploy
