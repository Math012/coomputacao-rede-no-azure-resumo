# Computação e Rede na Azure

### Serviços de computação 

- A computação do Azure é um serviço sob demanda e fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais.

### Máquinas virtuais do Azure

- As máquinas virtuais são recursos que emulam software de computadores físicos.

- Inclui processador virtual, memória, armazenamento e rede.

- Ofertas de laaS que oferece personalização (escolha de diferentes sistemas operacionais) e controle total.

- Aplica a responsabilidade compartilhada.

- Conjuntos de dimensionamento de VMs:
  - Os conjuntos oferecem uma oportunidade de balanceamento de carga para dimensionar os recursos automaticamente.
  -  Não chega a ser um modelo de loadbalance.

### Conjuntos de disponibilidade de Máquinas virtuais do Azure

- O rack onde estão as VMs são chamados de domínio de falha.

- Estratégia para que as VMs não fiquem acopladas em um único rack, assim evitando que todo o sistema fique fora caso o rack apresente falhas.

- Quando estamos criando os conjuntos de disponibilidade, a ideia é que seja separado em pelo menos 3 domínios de falha.

- Uma sequência de VMs é chamada de domínio de atualização.

- Conjuntos de disponibilidade podem resultar no alto custo, porque a VM é replicada em outro domínio de falha.

### Área de Trabalho Virtual 

- Área de Trabalho Virtual do Azure é uma virtualização de área de trabalho e aplicativo executada em nuvem.

- Crie um ambiente completo de virtualização da área de trabalho sem precisar executar outros servidores de gateway.

- Reduza o risco de que o recurso seja deixado para trás.

- Implantações reais de várias sessões.

- E possível criar um ambiente de trabalho totalmente personalizado e com regras de acesso.

- Alta segurança.

### Contêineres do Azure

- Os contêineres do Azure fornecem um ambiente leve e virtualizado que não exige o gerenciamento do sistema operacional e pode responder alterações sob demanda.

- Pode ser recriado.

- É um recurso leve.

-  O tipo de contêiner mais popular é o Docker e o Azure é compatível com o Docker.

-  As instâncias de contêiner do Azure são uma oferta no modelo de PaaS.

-  Não tem necessidade de executar uma VM.

-  Aplicativos de contêiner do Azure:
  -  PaaS, como instancias de contêineres, que podem balancear a carga e escalar.
  -  Permite maior flexibilidade.
    
- Serviço de Kubernetes do Azure:
  - um serviço de orquestração para contêineres com arquitetura distribuída e grandes volumes de contêineres.
  -  Focado na organização dos contêineres.

### Azure Functions

- Uma oferta de PaaS que dá suporte a operações de computação sem servidor.

- Ó código baseado em eventos é executado quando chamado, sem exigir uma infraestrutura de servidor durante períodos inativos.

- Personalização na hora de executar as functions podendo ter um temporizador, uma mensagem e quando ele pode ser executado.

- Baseada em eventos.

### Comparar opções de computação do Azure

- Máquinas virtuais
  - Servidor baseado em nuvem que da suporte a ambientes Windows ou Linux.
  - Útil para migrações de lift-and-shift(levar como está) para nuvem.
  - Pacotes do sistema operacional completo, incluindo o sistema operacional do host.
    
- Área de Trabalho Virtual.
  - Fornece uma experiência de área de trabalho Windows baseada em nuvem.
  - Aplicativos dedicados para conexão e uso ou acessíveis de qualquer navegador moderno.
  - O logon de varios clientes e um mesmo computador e, ao mesmo tempo.
 
- Contêineres
  - Gestão gerenciada pelo AKS (Serviço de Kubernetes do Azure).
  - Ambiente leve.
  - Adequado para a execução de microsserviços.
  - Projetado para escalabilidade.
  - Resiliência por meio da orquestração.
  - Aplicativos e serviços são empacotados em um contêiner que fica na parte superior do sistema operacional.

### Serviços de Aplicativo do Azure

- Consistem em uma plataforma totalmente gerenciada para criar, implantar e dimensionar aplicativos Web e APIs.

- Suporte a implantação contínua.

- Windows e Linux.

- Oferta de PaaS.

### Serviço de rede do Azure

- A rede Virtual do Azure(VNet) permite que os recursos do Azure se comuniquem, entre outros, com a internet e com as redes locais.

- Pontos de extremidade públicos, acessíveis de qualquer lugar na internet.

- Pontos de extremidade privados, acessíveis somente de dentro da sua rede.

- Duas VNet não se comunicam nativamente, precisam de um emparelhamento porque é necessário ter uma isolação para questão de segurança.

- Ips iguais em redes que se comunicam podem causar problemas.

- Gateway de VPN é usado para enviar tráfego criptografado entre uma rede virtual do Azure para uma rede pública na internet.

- ExpressRoute estende as redes locais para o Azure por meio de uma conexão privada facilitada por um provedor de conectividade.

### DNS do Azure

- Confiabilidade de desempenho aproveitando uma rede global de servidores de nome DNS usando a rede Anycast.

- A segurança do DNS do Azure baseia-se no gerenciador de recursos do Azure, habilitando o controle de acesso baseado na função e o monitoramento e registro de log.

- As redes virtuais personalizáveis permitem que você use nomes de domínio privados e totalmente personalizados em suas redes virtuais privadas.



