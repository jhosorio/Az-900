# Az-900
Criar uma Conta Gratuita no Portal Azure
Localizando os Serviços por Categoria

Configurações de Tela Cores e Layout
-Canto superior clique em Settings --> Appearance + Startup Views no menu lateral esquerdo
-Language + region para alterar a Linguagem e Região que mais você se adequa
Acesse All Services e descubra quais o serviços estão disponiveis por categoria (Analytics, Compute, Containers, Databases, etc.

Networking
- Bastions
- DNS
- DSN Zones
- Etc

Tipos de Serviçoes na Nuvem da Azure
IaaS (Infraestrutura como Serviço) é um modelo de serviço de computação em nuvem que oferece recursos de rede, armazenamento e computação. 
Com o IaaS, as empresas podem acessar esses recursos sob demanda, pagando apenas pelo que usam. Isso elimina a necessidade de comprar, configurar e gerenciar servidores físicos. 

Vantagens do IaaS 
-Reduz a manutenção de datacenters locais
-Economiza em custos de hardware
-Permite escalar e reduzir recursos de TI conforme a demanda
-Aumenta a confiabilidade da infraestrutura
-Permite provisionar novas aplicações rapidamente
-Permite obter informações empresariais em tempo real

Como funciona o IaaS
O IaaS é um dos principais modelos de serviços em nuvem, juntamente com a PaaS (plataforma como serviço) e o SaaS (software como serviço). 
Um provedor de serviços de computação em nuvem, como o Azure ou o AWS, gerencia a infraestrutura. O cliente compra, instala, configura e gerencia o seu próprio software, incluindo sistemas operativos, middleware e aplicações. 

PaaS pode referir-se a Plataforma como Serviço 
Plataforma como Serviço
PaaS é um modelo de computação em nuvem que oferece uma plataforma para desenvolver, implantar, executar e gerenciar aplicações 
O PaaS é um ambiente de desenvolvimento e implantação completo na nuvem 
O PaaS inclui infraestrutura, servidores, armazenamento, rede, middleware, ferramentas de desenvolvimento, e muito mais 
O PaaS ajuda as empresas a evitar o custo de instalar hardware ou software 
O PaaS permite que os desenvolvedores se concentrem no código do aplicativo 

SaaS (Software as a Service) 
É um modelo de negócio que disponibiliza software por meio da internet, como um serviço. 

Vantagens do SaaS:
-Não é preciso instalar, manter e atualizar hardwares ou softwares
-É possível reduzir custos
-É possível implementar, dimensionar e atualizar soluções de negócios mais rapidamente
-É possível prever o custo total de propriedade com maior precisão
-É possível alugar o uso de aplicativo para a organização

Exemplos de SaaS:
-Email
-Calendário
-Ferramentas do Office (como Microsoft Office 365)
-Google Workspace
-Slack
-Stripe
-ClickUp
-Dropbox
-Zoom

Como funciona o SaaS
O provedor de nuvem desenvolve e mantém software de aplicação em nuvem, fornece atualizações automáticas e disponibiliza software para seus clientes através da Internet. 
Como escolher um SaaS
É importante optar por um sistema com metodologia de implantação eficiente. 

Modelo de Responsabilidade Compartilhada (Nuvem) - Vale para todos tipos de Nuvem (Azure, AWS, Google, etc)
IaaS
. O Serviço de nuvem mais flexível.
. Você configura e gerencia o hardware para seu aplicativo.

A Resposabilidade é sempre retida pelo Cliente
- Informações e dados
- Disposotivos (Móveis e PCs)
- Contas e Identidades
- Infraestrutura de identidade e diretório
- Aplicativos, Controles de rede, Sistema Operacional

PaaS
. Focado em desenvolvimento de aplicativos
. O gerenciamento de plataforma é realizado pelo provedor da nuvem

A Resposabilidade é sempre retida pelo Cliente
-Informações e dados
-Disposotivos (Móveis e PCs)
- Contas e Identidades

- Infraestrutura de identidade e diretório, Aplicativos, Controles de rede, Sistema Operacional (Responsabilidade Compartilhada)


SaaS
. Modelo de preço de pagamento conforme o uso.
. Os usuários pagam pelo software que utilizam em um modelo de assinatura.

A Resposabilidade é sempre retida pelo Cliente
-Informações e dados
-Disposotivos (Móveis e PCs)
- Contas e Identidades

- Infraestrutura de identidade e diretório (Responsabilidade Compartilhada)


On Promisses (Não está na Nuvem) - Resposável por toda a Infra Compra, Manutenção, Instalação, Atualização, Etc

Criação de Grupo de Recursos

Ferramentas de Configuração:
- Portal Azure: Interface gráfica.
- Azure CLI: Automação via linha de com

Configurar recursos e dimensionar máquinas virtuais (VMs) no Azure envolve ajustar especificações como CPU, memória, armazenamento e rede para atender às necessidades do seu projeto. 
1. **Escolha do Tipo de VM**: O Azure oferece diferentes séries de VMs, como:
   - Série A: Para cargas de trabalho básicas.
   - Série D/E: Balanceadas para aplicações empresariais.
   - Série F: Alta performance em CPU.
   - Série N: Com GPU para processamento gráfico e aprendizado de máquina.

2. **Dimensionamento de Recursos**:
   - **Vertical**: Alteração de recursos (CPU/RAM) na mesma instância.
   - **Horizontal**: Adição ou remoção de instâncias para balanceamento de carga.

3. **Configurações Avançadas**:
   - Zonas de disponibilidade para alta disponibilidade.
   - Grupos de dimensionamento para gerenciar múltiplas VMs.
   - Extensões para adicionar softwares ou scripts.

4. **Automação e Monitoramento**:
   - Configuração de autoescalabilidade com base em métricas como uso de CPU.
   - Uso do Azure Monitor para monitorar desempenho e ajustar recursos.

5. **Ferramentas de Configuração**:
   - Portal Azure: Interface gráfica.
   - Azure CLI: Automação via linha de comando.
   - ARM Templates: Infraestrutura como código.

A **Área de Trabalho Virtual do Azure** é um serviço de virtualização que permite acessar desktops e aplicativos remotamente, com segurança e flexibilidade. Ele oferece:

- **Experiência completa do Windows**: Compatível com Windows 11, Windows 10 e Windows Server.
- **Multissessões**: Permite que vários usuários compartilhem uma única máquina virtual, reduzindo custos.
- **Gerenciamento centralizado**: Controle unificado para configurar e gerenciar desktops e aplicativos.
- **Escalabilidade**: Ajuste automático de capacidade com base na demanda.
- **Integração com Microsoft 365**: Otimizado para uso em ambientes virtuais.
A criação de um **Pool de Hosts** no Azure é um processo essencial para configurar a **Área de Trabalho Virtual do Azure**. Aqui está um resumo dos passos principais:

1. **Planejamento**:
   - Defina o tipo de atribuição: *Pessoal* (um usuário por VM) ou *Multissessão* (vários usuários por VM).
   - Escolha o tamanho e a série das máquinas virtuais (VMs) com base nas necessidades de desempenho.

2. **Criação do Pool de Hosts**:
   - Acesse o **Portal do Azure**.
   - Navegue até **Área de Trabalho Virtual** e clique em **Pools de Hosts**.
   - Clique em **Criar** e forneça as informações:
     - Nome do pool.
     - Tipo de atribuição.
     - Localização (região do Azure).

3. **Adição de Hosts de Sessão**:
   - Configure as VMs que serão usadas como hosts de sessão.
   - Adicione as VMs ao pool de hosts, especificando o número de hosts necessários.
   - Configure o licenciamento e as propriedades do protocolo RDP.

4. **Configuração de Workspace e Aplicativos**:
   - Associe o pool de hosts a um workspace.
   - Adicione grupos de aplicativos para permitir que os usuários acessem desktops ou aplicativos específicos.

5. **Automatização e Gerenciamento**:
   - Use ferramentas como **Azure PowerShell** ou **CLI** para automatizar a criação e configuração.
   - Configure políticas de escalabilidade para ajustar a capacidade com base na demanda.

A criação de **Funções do Azure** (Azure Functions) permite executar código em um ambiente sem servidor, ideal para tarefas orientadas a eventos. Aqui está um resumo do processo:

1. **Planejamento**:
   - Escolha o gatilho (ex.: HTTP, Timer, Blob Storage) que iniciará a execução da função.
   - Defina a linguagem de programação (C#, JavaScript, Python, etc.).

2. **Criação do Aplicativo de Funções**:
   - No **Portal do Azure**, selecione **Criar um recurso** > **Computação** > **Aplicativo de Funções**.
   - Configure:
     - **Plano de Hospedagem**: Escolha entre Consumo (paga apenas pelo uso) ou Premium.
     - **Região**: Escolha a mais próxima para reduzir latência.
     - **Conta de Armazenamento**: Necessária para logs e dados temporários.

3. **Criação da Função**:
   - No aplicativo de funções, clique em **+ Nova Função**.
   - Escolha o tipo de gatilho (ex.: HTTP Trigger para APIs).
   - Escreva o código diretamente no portal ou use ferramentas como Visual Studio/VS Code para desenvolvimento local.

4. **Configuração e Implantação**:
   - Configure variáveis de ambiente para conexões e chaves de API.
   - Implante o código no Azure usando o portal, CLI ou pipelines de CI/CD.

5. **Monitoramento e Escalabilidade**:
   - Use o **Azure Monitor** para rastrear logs e métricas.
   - Configure escalabilidade automática para lidar com picos de demanda.

Você pode explorar mais detalhes sobre a criação de funções no [Microsoft Learn](https://learn.microsoft.com/pt-br/azure/azure-functions/functions-create-function-app-portal) ou [aqui](https://learn.microsoft.com/pt-br/azure/azure-functions/functions-get-started). Precisa de ajuda com algum aspecto específico? 🚀

A **redundância de armazenamento no Azure** é uma estratégia para proteger dados contra falhas e garantir alta disponibilidade e durabilidade. O Azure oferece diferentes níveis de replicação para atender a diversas necessidades de custo e resiliência:

1. **Armazenamento com Redundância Local (LRS)**:
   - Replica os dados três vezes dentro de um único data center na região primária.
   - É a opção mais econômica, mas não protege contra falhas de data center.
   - Não indicado pra Produção

2. **Armazenamento com Redundância de Zona (ZRS)**:
   - Replica os dados de forma síncrona em três zonas de disponibilidade dentro da mesma região.
   - Oferece maior proteção contra falhas de data center.
   - Assincrono

3. **Armazenamento com Redundância Geográfica (GRS)**:
   - Replica os dados em uma região secundária geograficamente distante.
   - Protege contra desastres regionais, mas o acesso aos dados replicados é limitado.

4. **Armazenamento com Redundância Geográfica com Acesso de Leitura (RA-GRS)**:
   - Similar ao GRS, mas permite acesso de leitura aos dados replicados na região secundária.


![image](https://github.com/user-attachments/assets/f63bc8a6-8611-421e-a58b-1a0ca1fa5c53)

Essas opções permitem que você escolha o nível de redundância ideal com base nos requisitos de disponibilidade, custo e recuperação de desastres. Você pode explorar mais detalhes sobre isso [aqui](https://learn.microsoft.com/pt-br/azure/storage/common/storage-redundancy). Se precisar de ajuda para configurar ou entender melhor, é só avisar! 🚀

O **Azure Blob Storage** é uma solução de armazenamento de objetos altamente escalável e segura, projetada para armazenar grandes volumes de dados não estruturados, como texto, imagens, vídeos e backups. Aqui estão os principais pontos sobre ele:

1. **Tipos de Blobs**:
   - **Blobs de Bloco**: Ideais para armazenar arquivos grandes, como vídeos e imagens.
   - **Blobs de Página**: Usados para armazenamento de dados que exigem acesso aleatório, como discos de máquinas virtuais.
   - **Blobs de Acrescentar**: Projetados para operações de acréscimo, como logs.

2. **Casos de Uso**:
   - Armazenamento de arquivos para acesso distribuído.
   - Streaming de áudio e vídeo.
   - Backup e recuperação de desastres.
   - Armazenamento de dados para análise em data lakes.

3. **Acesso e Integração**:
   - Os dados podem ser acessados via HTTP/HTTPS de qualquer lugar.
   - Suporte a APIs REST, Azure CLI, PowerShell e bibliotecas de cliente para várias linguagens, como Python, .NET e Java.

4. **Armazenamento em Camadas**:
   - **Hot**: Para dados acessados frequentemente.
   - **Cool**: Para dados acessados ocasionalmente.
   - **Archive**: Para dados raramente acessados, com custo reduzido.

5. **Segurança e Confiabilidade**:
   - Criptografia em repouso e em trânsito.
   - Controle de acesso baseado em funções (RBAC).
   - Alta durabilidade e disponibilidade com opções de redundância (LRS, ZRS, GRS, RA-GRS).

O Azure Blob Storage é amplamente utilizado para criar aplicativos nativos de nuvem, data lakes e soluções de backup. Você pode explorar mais detalhes [aqui](https://azure.microsoft.com/pt-br/products/storage/blobs/) ou [aqui](https://learn.microsoft.com/pt-br/azure/storage/blobs/storage-blobs-introduction). Se precisar de ajuda com algo específico, é só avisar! 🚀

Os **Arquivos do Azure** são uma solução de armazenamento em nuvem que oferece compartilhamentos de arquivos totalmente gerenciados, acessíveis por meio de protocolos padrão como SMB (Server Message Block) e NFS (Network File System). Aqui estão os principais aspectos:

1. **Funcionalidade**:
   - Permite criar compartilhamentos de arquivos que podem ser montados simultaneamente em sistemas locais ou na nuvem.
   - Compatível com Windows, Linux e macOS.

2. **Casos de Uso**:
   - Substituir servidores de arquivos locais ou dispositivos NAS.
   - Compartilhar dados entre contêineres e aplicativos distribuídos.
   - Armazenar configurações de aplicativos em um local centralizado.

3. **Recursos Avançados**:
   - Sincronização de Arquivos do Azure: Cache local para acesso rápido.
   - Integração com Active Directory para controle de acesso baseado em identidade.
   - Suporte a camadas de armazenamento (quente, fria e arquivamento).

4. **Segurança**:
   - Criptografia em trânsito e em repouso.
   - Conformidade com padrões de segurança e privacidade.

Os Arquivos do Azure são ideais para empresas que buscam simplificar o gerenciamento de dados e integrar soluções híbridas. Você pode explorar mais detalhes [aqui](https://azure.microsoft.com/pt-br/products/storage/files/) ou [aqui](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-introduction). Precisa de ajuda com algo específico? 🚀

Os **pontos de extremidade públicos** do serviço de armazenamento da Azure permitem que os recursos de armazenamento sejam acessados por meio de endereços IP públicos, garantindo conectividade global. Aqui estão os principais aspectos:

1. **Acesso Global**:
   - Os pontos de extremidade públicos são acessíveis de qualquer lugar do mundo via HTTP ou HTTPS.
   - Ideal para cenários onde o acesso remoto é necessário.

2. **Segurança**:
   - Embora sejam públicos, podem ser protegidos com configurações de firewall e regras de rede.
   - É possível restringir o acesso a endereços IP específicos ou redes virtuais.

3. **Tipos de Serviços**:
   - Aplicável a diferentes serviços de armazenamento, como Blobs, Arquivos, Filas e Tabelas.

4. **Alternativa: Pontos de Extremidade Privados**:
   - Para maior segurança, o Azure também oferece pontos de extremidade privados, que utilizam endereços IP dentro de uma rede virtual.

Você pode explorar mais detalhes sobre os pontos de extremidade públicos e como configurá-los [aqui](https://learn.microsoft.com/pt-br/azure/storage/files/storage-files-networking-endpoints) ou [aqui](https://learn.microsoft.com/pt-br/azure/virtual-network/virtual-network-service-endpoints-overview). Caso precise de ajuda com configurações específicas, é só avisar! 🚀

![image](https://github.com/user-attachments/assets/e34a3141-6d06-4155-bc7d-f5eb6e1a8370)





