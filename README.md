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



## Print: Renato --> Luciano

![https://github.com/renatopuga/cowsay-azure/raw/master/print-valendo-pontos.png](https://github.com/renatopuga/cowsay-azure/raw/master/print-valendo-pontos.png)




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



## Azure Cloud Shell

1. Portal
2. Resource groups
3. Filtrar por: App Services
4. Copiar URL e colocar no Chrome
   1. Launch Bash (escolha ao gosto do cliente Bash ou PowerSheel)

```bash
 ________________________________________ 
< Agora, vamos no Azure Active Directory >
 ---------------------------------------- 
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```



## Azure Active Directory

1. Portal

2. Azure Active Directory

3. App registrations (se não tiver o seu na lista, vamos criar um novo)

4. New Registration an application

   1. Name: puga-fiap-asia-api

   2. Support account types

      1. Who can use this application or access this API?

         (x) Accounts in this organizational directory only (Fiap-Faculdade de Informática e Administração Paulista only - Single tenant)

5. Clicar em **Registrar**



## Api Permissions 

1. Dentro da Api criada clique em **Api Permissions**.

2. Add a permissions

3. Microsoft Graph

4. Delegated permissions

5. Select permissions: user

   (x) User.Read.All

   

## GUID Generator

* https://guidgenerator.com/online-guid-generator.aspx

  d0b89f8a-d88e-4028-a7e3-bf97bb7ff543

## App Roles

* Adicionar na linha 8:

```bash
"appRoles": [
     {
       "allowedMemberTypes": [
         "User",
         "Application"
       ],
       "displayName": "Administrator",
       "id": "<GUID>",
       "isEnabled": true,
       "description": "Blockchain Workbench administrator role allows creation of applications, user to role assignments, etc.",
       "value": "Administrator"
     }
   ],
```

* Alterar a linha 19 **Oauth2AllowImplicitFlow** de `false`para `true`:

Subscription ID: d1aa1416-3251-4a6c-94b0-2bc5b3b85267



**Step 1. Launch Cloud Shell and run the following command**:

```bash
cd; Invoke-WebRequest -Uri https://aka.ms/workbenchAADSetupScript -OutFile workbenchAADSetupScript.ps1; ./workbenchAADSetupScript.ps1 -SubscriptionID d1aa1416-3251-4a6c-94b0-2bc5b3b85267 -ResourceGroupName pugafiapasiarg -DeploymentId a66efz
```



### Azure Cloud Shell

```bash
Type "az" to use Azure CLI
Type "help" to learn about Cloud Shell


MOTD: Modules installed with 'Install-Module' are persisted across sessions

VERBOSE: Authenticating to Azure ...
VERBOSE: Building your Azure drive ...
Azure:/
PS Azure:\> ls
clouddrive  workbenchAADSetupScript.ps1
Azure:/
PS Azure:\> cd; Invoke-WebRequest -Uri https://aka.ms/workbenchAADSetupScript -OutFile workbenchAADSetupScript.ps1; ./workbenchAADSetupScript.ps1 -SubscriptionID d1aa1416-3251-4a6c-94b0-2bc5b3b85267 -ResourceGroupName pugafiapasiarg -DeploymentId a66efz
Please enter the Azure Active Directory tenant you would like to use (Go to https://aka.ms/workbenchFAQ for more info): fiap.com.brWARNING: To sign in, use a web browser to open the page https://microsoft.com/devicelogin and enter the code AHBXVLYX2 to authenticate.INFO: Creating the AAD application
INFO: Successfully created AAD application with appId: 6f832aee-bdc0-44df-ad00-1ad23e48fd9f
INFO: Creating the Service Principal for Azure Blockchain Workbench
INFO: Adding current service principal as an admin
INFO: Successfully created role assignment
INFO: Looking for your user 'RM333257@fiap.com.br' in 'fiap.com.br' tenant
INFO: 1 user(s) were found with email 'RM333257@fiap.com.br'
INFO: Assign the current logged in user to be the owner of the Application.
INFO: Added 'RM333257@fiap.com.br' as an admin on the application
INFO: Updating your Workbench Instance with the Active Directory Application Info. This may take some time...
INFO: Attempting to update the reply URl to https://pugafiapasia-a66efz.azurewebsites.net
INFO: Waiting for changes to propagate...

INFO: Azure Active Directory Domain Name: fiap.com.br
INFO: Application Name: Azure Blockchain Workbench pugafiapasia-a66efz
INFO: Application Client Id: 6f832aee-bdc0-44df-ad00-1ad23e48fd9f



SUCCESS: Your Workbench instance was successfully provisioned. Navigate to https://pugafiapasia-a66efz.azurewebsites.net to use your instance.
INFO: Please refer to https://aka.ms/workbenchFAQ to read more about user management in Workbench.
============================================================================================================================
PS /home/renato>
```



## Azure Cloud Sheell

* Abrir: https://pugafiapasia-a66efz.azurewebsites.net

![state diagram of workflow](https://github.com/Azure-Samples/blockchain/raw/master/blockchain-workbench/application-and-smart-contract-samples/hello-blockchain/media/5aba06dd9b98e017f7031946d0187fb7.png)



## Azure-Samples - Hello, Blockchain!

* https://github.com/Azure-Samples/blockchain

1. New
2. Upload: HelloBlockchain.json
3. Upload: HelloBlockchain.sol
4. Add a member (Adicionar dois membors com seu RM da fiap)
   1. Requester
   2. Responder
5. New
6. New Contract: 
   1. Request Message [ Enviando Mesangem]
7. Your contract was created successfully.



### HelloBlockchain.sol

```bash
pragma solidity >=0.4.25 <0.6.0;

contract HelloBlockchain
{
     //Set of States
    enum StateType { Request, Respond}

    //List of properties
    StateType public  State;
    address public  Requestor;
    address public  Responder;

    string public RequestMessage;
    string public ResponseMessage;

    // constructor function
    constructor(string memory message) public
    {
        Requestor = msg.sender;
        RequestMessage = message;
        State = StateType.Request;
    }

    // call this function to send a request
    function SendRequest(string memory requestMessage) public
    {
        if (Requestor != msg.sender)
        {
            revert();
        }

        RequestMessage = requestMessage;
        State = StateType.Request;
    }

    // call this function to send a response
    function SendResponse(string memory responseMessage) public
    {
        Responder = msg.sender;

        // call ContractUpdated() to record this action
        ResponseMessage = responseMessage;
        State = StateType.Respond;
    }
}
```

### HelloBlockchain.json

```json
{
  "ApplicationName": "HelloBlockchain",
  "DisplayName": "Hello, Blockchain!",
  "Description": "A simple application to send request and get response",
  "ApplicationRoles": [
    {
      "Name": "Requestor",
      "Description": "A person sending a request."
    },
    {
      "Name": "Responder",
      "Description": "A person responding to a request"
    }
  ],
  "Workflows": [
    {
      "Name": "HelloBlockchain",
      "DisplayName": "Request Response",
      "Description": "A simple workflow to send a request and receive a response.",
      "Initiators": [ "Requestor" ],
      "StartState": "Request",
      "Properties": [
        {
          "Name": "State",
          "DisplayName": "State",
          "Description": "Holds the state of the contract.",
          "Type": {
            "Name": "state"
          }
        },
        {
          "Name": "Requestor",
          "DisplayName": "Requestor",
          "Description": "A person sending a request.",
          "Type": {
            "Name": "Requestor"
          }
        },
        {
          "Name": "Responder",
          "DisplayName": "Responder",
          "Description": "A person sending a response.",
          "Type": {
            "Name": "Responder"
          }
        },
        {
          "Name": "RequestMessage",
          "DisplayName": "Request Message",
          "Description": "A request message.",
          "Type": {
            "Name": "string"
          }
        },
        {
          "Name": "ResponseMessage",
          "DisplayName": "Response Message",
          "Description": "A response message.",
          "Type": {
            "Name": "string"
          }
        }
      ],
      "Constructor": {
        "Parameters": [
          {
            "Name": "message",
            "Description": "...",
            "DisplayName": "Request Message",
            "Type": {
              "Name": "string"
            }
          }
        ]
      },
      "Functions": [
        {
          "Name": "SendRequest",
          "DisplayName": "Request",
          "Description": "...",
          "Parameters": [
            {
              "Name": "requestMessage",
              "Description": "...",
              "DisplayName": "Request Message",
              "Type": {
                "Name": "string"
              }
            }
          ]
        },
        {
          "Name": "SendResponse",
          "DisplayName": "Response",
          "Description": "...",
          "Parameters": [
            {
              "Name": "responseMessage",
              "Description": "...",
              "DisplayName": "Response Message",
              "Type": {
                "Name": "string"
              }
            }
          ]
        }
      ],
      "States": [
        {
          "Name": "Request",
          "DisplayName": "Request",
          "Description": "...",
          "PercentComplete": 50,
          "Value": 0,
          "Style": "Success",
          "Transitions": [
            {
              "AllowedRoles": ["Responder"],
              "AllowedInstanceRoles": [],
              "Description": "...",
              "Function": "SendResponse",
              "NextStates": [ "Respond" ],
              "DisplayName": "Send Response"
            }
          ]
        },
        {
          "Name": "Respond",
          "DisplayName": "Respond",
          "Description": "...",
          "PercentComplete": 90,
          "Value": 1,
          "Style": "Success",
          "Transitions": [
            {
              "AllowedRoles": [],
              "AllowedInstanceRoles": ["Requestor"],
              "Description": "...",
              "Function": "SendRequest",
              "NextStates": [ "Request" ],
              "DisplayName": "Send Request"
            }
          ]
        }
      ]
    }
  ]

```



## Contrato Feito

1. Clique no seu contrato
2. Take action
3. REQUEST MESSAGE
   1. RESPONSE MESSAGE: Tudo bem?
   2. Request Message: Tudo!

