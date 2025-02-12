# Resumo AZ-900

Resumo das lições aprendidas durante o desenvolvimento do lab na DIO

# Computação em Nuvem: Domínio do objetivo

A computação em nuvem é o fornecimento de serviços de computação pela Internet, facilitando inovações mais rápidas, recursos flexíveis e economias de escala.

## Quando faz sentido?

- Criar recursos de maneira rápida
- Necessita pessoas capacitadas em nuvem
- Custo / Pagar apenas pelo que usa
- Não necessita de infraestrutura própria (luz, equipamentos, etc)

## Nuvem privada

- Ambiente 100% on Premises
- Ambiente em nuvem em datacenter próprio
- São responsáveis por operar os próprios serviços
- Não fornece acesso externo a organização

## Nuvem pública

- Ambiente espalhado por máquinas ao redor do mundo
- Pertencente a um provedor de gistubg
- Fornece recursos a várias organizações e usuários
- Acessada via conexão segura

## Nuvem híbrida

- Busca usar o melhor dos dois mundos
- Possui parte da arquitetura on premises e outra parte em nuvem pública

## Modelo Multi Cloud

- Possui serviços em mais de 1 provedor de nuvem, públicas e privadas, que se comunicam entre si

# Comparação de Modelos de Nuvem

## Nuvem pública

- Nenhuma despesa de capital para escalar verticalmente (CAPEX)
- Aplicativos podem ser provisionados e desprovisionados rapidamente
- Paga apenas o que utiliza

## Nuvem Privada

- Controle total de recursos e segurança por parte da empresa
- Responsáveis pela atualização tanto dos hardwares quanto do software
- Aumento de capacidade exige investimento em infraestrutura maior, mais trabalho e demanda tempo e profissionais para as tarefas

## Nuvem híbrida

- Organização determina onde executar os aplicativos
- Controlam a segurança, conformidade e os requisitos legais
- Fornece maior flexibilidade

# CapEx e OpEx

## Despesas de Capital (CapEx)

- Gasto inicial em infraestrutura física (cabos, máquinas, switches, eletricidade, ar condicionado)
- Despesas têm um valor que se reduz com o tempo

## Despesas operacionais (OpEx)

- Gastar com produtos e serviços conforme necessários, pagamento conforme o uso
- Cobrança imediata

## Modelo baseado em consumo

- Paga somente pelos recursos que foram usados
- Melhor previsão de custos
- Cobrança é feita com base no uso real
- Fornecidos preços para recursos/serviços individualmente
- Painel para acompanhar custos
- Travas para custos

Benefícios da Nuvem Azure

# Benefícios da nuvem: domínio de objetivo

## Alta disponibilidade, independente de interrupções ou eventos

- Acordo de nível de serviço - SLA - % de disponibilidade alto
- Possibilidade de créditos em caso de não cumprimento do SLA contratado

## Escalabilidade

- Capacidade de ajustar recursos a demanda
- Possível adicionar recursos para lidar com aumento de demanda
- Paga apenas pelo necessário e não além
- Em nuvem, paga-se apenas pelo que usa
- Se demanda cai, é possível reduzir os recursos
- Escala vertical possibilita adicionar mais CPU e RAM à máquina virtual

## Elasticidade

- Possível expandir os recursos num aumento acentuado (automaticamente ou manualmente)
- Possível configurar expansão de máquinas e contêineres automaticamente. Ex: Chegando a 75%, aumenta 1 máquina. Diminuindo a demanda, reduz 1 máquina, até um limite de N máquinas.
- Ao adotarmos a nuvem pública podemos adaptar nossos sistemas para que os mesmos atendam as requisições externas com agilidade e rapidez

## Confiabilidade

- Infraestrutura confiável e resiliente
- Permite que os recursos estejam implantados em várias regiões do mundo
- Ocorrendo problemas em uma região, é possível utilizar a infra de outro local

## Previsibilidade

- Confiança para avançar, seja no desempenho ou custo, de forma previsível

## Segurança

- Nuvem oferece ferramentas de segurança avançadas, porém necessita implementação do cliente
- Infraestrutura como serviço oferece recursos físicos, mas permite gerenciamento dos sistemas instalados, incluindo atualizações. Porém cabe ao cliente fazer as atualizações
- Para aplicação de atualizações automáticas, plataforma como serviço / software é uma estratégia melhor. O cliente escolhe a plataforma e recebe as últimas versões

## Governança

- Auditoria em nuvem ajuda a sinalizar recursos fora de conformidade com os padrões
- Dependendo do modelo, atualizações podem ser aplicadas automaticamente, ajudando na governança e segurança
- Governança quando gerada cedo, mantém a presença da nuvem atualizada, segura e confiável

## Gerenciabilidade

- Opções de capacidade de gerenciamento (linha de comando, script, portal)
- Gerenciar nuvem
  - Escalar automaticamente implantação de recursos
  - Implantar recursos com base em modelo pré-configurado

Tipos de Serviço de Nuvem

# Tipos de serviço de nuvem: domínio do objetivo

## IaaS - Infraestrutura como serviço

- Servidores de armazenamento, máquinas virtuais
- Firewalls/segurança
- Planta física
- Exige mais configuração, porém é mais flexível
- Permite maior domínio da infraestrutura, maior personalização, maior liberdade

## PaaS - Plataforma como serviço

- Focado no desenvolvimento de aplicativos
- Ferramentas de dev
- Análise de negócios
- Gerenciamento de banco de dados
- Sistemas operacionais
- Ambiente para criação, teste e implantação de aplicativos de software
- Não foca no gerenciamento da infra

## SaaS - Software como serviço

- Aplicativos / Apps hospedados
- Ex: Office 365, Teams
- Usuário se conecta pela internet
- Não cuidamos das configurações de arquitetura, apenas de uso do software

Componentes de arquitetura do Azure

# Principais componentes arquitetônicos do Azure

## Regiões

- Regiões disponíveis
- Regiões anunciadas
- Zonas de disponibilidades
- mais de 60 regiões em mais de 140 países
- Compostas por um ou mais datacenters próximos
- Fornecem flexibilidade e escala para reduzir latência
- Preservam a residência dos dados

## Zonas de Disponibilidade

- Fornece proteção contra tempo de inatividade devido a falha do datacenter
- Separa fisicamente os datacenters dentro da mesma região
- Cada datacenter tem alimentação, resfriamento e rede independentes
- Conectados por meio de redes privadas

## Pares de regiões

- Mínimo 300 milhas de separação
- Réplica automática de alguns serviços
- Recuperação de região priorizada em caso de interrupção
- Atualizações distribuídas sequencialmente

## Regiões soberanas do Azure

- Serviços governamentais americanos
  - Atende necessidades de segurança de agências federais americanas, governos estaduais e locais
- Azure Governamental
  - instância separada do Azure
  - Fisicamente isolada de implantações que não sejam do governo americano
  - Acessível somente a pessoal autorizado
- Azure China
  - Microsoft foi o primeiro a prover cloud para a China, seguindo as regulamentações chinesas
  - Fisicamente separada de outras instâncias da Azure, operada pela 21Vianet
  - Todo dado fica dentro da China

# Recursos do Azure

São componentes como armazenamento, máquinas virtuais e redes que estão disponíveis para criar soluções de nuvem.

- Máquinas virtuais
- Contas de armazenamento
- Redes virtuais
- Serviços de aplicativos
- Bancos de dados SQL
- Funções

## Grupo de recursos

- Agrupamento de recursos
- Contêiner que você usa para gerenciar e agregar recursos em única unidade
- Não é possível renomear um grupo de recursos
- Recursos podem existir em apenas um grupo (não pode estar em dois, por exemplo)
- Recursos podem existir em diferentes regiões
- Recursos podem ser movidos para diferentes grupos
- Aplicativos podem utilizar vários grupos

# Assinaturas do Azure

## Contas do Azure

- Assinatura do desenvolvimento
- Assinatura do teste
- Assinatura da produção
- Conta > assinatura: 1 > N
- Faturas individuais para cada assinatura
  - Facilita na gerência de gastos de, por exemplo, cada projeto

Grupos de Gerenciamento

- Podem incluir várias assinaturas
- Herdam as condições aplicadas ao grupo
