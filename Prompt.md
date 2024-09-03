# Guia para Criar uma Conta de Armazenamento no Azure

Este guia passo a passo irá ajudá-lo a criar uma conta de armazenamento no Azure usando o portal Azure.

## Pré-requisitos

Antes de começar, certifique-se de que você possui:

1. Uma conta ativa no Azure. Se você não tiver uma, pode criar uma [aqui](https://azure.microsoft.com/free/).
2. Acesso ao [Portal do Azure](https://portal.azure.com/).

## Passo 1: Acesse o Portal do Azure

1. Vá para o [Portal do Azure](https://portal.azure.com/) e faça login com suas credenciais.

## Passo 2: Iniciar a Criação de uma Conta de Armazenamento

1. No painel de navegação à esquerda, clique em **Criar um recurso**.
2. Na barra de pesquisa, digite **Conta de Armazenamento** e selecione **Conta de Armazenamento** nos resultados da pesquisa.
3. Clique no botão **Criar** para iniciar o assistente de criação de conta de armazenamento.

## Passo 3: Configurar a Conta de Armazenamento

### Configurações Básicas

1. **Assinatura**: Selecione a assinatura do Azure que você deseja usar.
2. **Grupo de Recursos**: Escolha um grupo de recursos existente ou clique em **Criar novo** para criar um novo grupo.
3. **Nome da Conta de Armazenamento**: Insira um nome único para sua conta de armazenamento. O nome deve ter entre 3 e 24 caracteres e só pode conter letras minúsculas e números.
4. **Região**: Escolha a região onde você deseja criar a conta de armazenamento (ex: "Leste dos EUA").
5. **Desempenho**: Selecione o nível de desempenho:
   - **Padrão**: Para armazenamento de dados acessados com menos frequência ou com maior latência.
   - **Premium**: Para dados que requerem baixa latência e altas taxas de transferência.
6. **Tipo de Conta de Armazenamento**: Selecione o tipo de conta de armazenamento, como **Armazenamento v2 (uso geral)**, **BlobStorage**, **Armazenamento v1 (uso geral)**, etc.
7. **Replicação**: Escolha uma opção de replicação para seus dados:
   - **Locally-redundant storage (LRS)**: Replicação dentro de um único datacenter.
   - **Zone-redundant storage (ZRS)**: Replicação entre datacenters na mesma região.
   - **Geo-redundant storage (GRS)**: Replicação entre datacenters em regiões diferentes.
   - **Read-access geo-redundant storage (RA-GRS)**: Similar ao GRS, mas com acesso de leitura aos dados replicados.

### Configurações Avançadas

1. Clique na guia **Avançado** para configurar as seguintes opções (opcional):
   - **Secure transfer required**: Ative ou desative a transferência segura para exigir que todas as conexões usem HTTPS.
   - **Large file shares**: Habilite ou desabilite o suporte para compartilhamentos de arquivos grandes (relevante para o Azure Files).
   - **Hierarchical namespace**: Habilite para usar o Azure Data Lake Storage Gen2, que é ideal para análises de big data.

### Configurações de Rede

1. Clique na guia **Rede** para definir as configurações de conectividade de rede (opcional):
   - **Método de Conexão**: Selecione **Público (ponto de extremidade de rede pública)** ou **Privado (ponto de extremidade de rede privada)**.
   - **Firewall e Redes Virtuais**: Configure as regras de firewall para restringir o acesso à conta de armazenamento.

### Configurações de Tags

1. Clique na guia **Tags** para adicionar tags (opcional):
   - As tags são pares de chave-valor que ajudam a organizar e gerenciar seus recursos no Azure.

## Passo 4: Revisar e Criar

1. Clique em **Revisar + criar** para revisar suas configurações.
2. Verifique se todas as informações estão corretas.
3. Clique em **Criar** para iniciar a criação da conta de armazenamento.

## Passo 5: Acessar a Conta de Armazenamento

1. Após a implantação, vá para **Contas de Armazenamento** no painel de navegação à esquerda.
2. Selecione sua nova conta de armazenamento na lista para acessar o painel de visão geral e começar a gerenciar seus dados.

## Conclusão

Parabéns! Você criou com sucesso uma conta de armazenamento no Azure. Você pode usar essa conta para armazenar blobs, arquivos, tabelas e filas. Para mais informações sobre como gerenciar e utilizar sua conta de armazenamento, consulte a [documentação oficial do Azure Storage](https://docs.microsoft.com/azure/storage/).