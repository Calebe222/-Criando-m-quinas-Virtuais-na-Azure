# 🖥️ Conceitos de SLA e Criação de Máquinas Virtuais no Azure

Resumo dos principais pontos aprendidos no bootcamp sobre **criação de máquinas virtuais (VMs) no Microsoft Azure**, com foco em **SLA (Service Level Agreement)** e **opções de disponibilidade**.

## 📊 SLA (Service Level Agreement)

- **Definição:** SLA representa o nível de disponibilidade garantido pelo serviço, expresso em porcentagem.  
- **Exemplos:** 99%, 99,9%, 99,99% (quanto mais “noves”, menor o tempo de inatividade ⏳).  
- **Impacto:**  
  - ✅ **Mais noves = maior disponibilidade** e menor tempo fora do ar.  
  - ⚠️ **Menos noves = maior tempo de indisponibilidade**, mas geralmente com custo mais baixo.  
- **Planejamento:** Como arquiteto de soluções, é fundamental analisar o SLA necessário para cada projeto, evitando gastos desnecessários 💰 e garantindo a confiabilidade esperada.

## 🏗️ Opções de Disponibilidade de VMs

- É possível distribuir VMs em **até 3 zonas de disponibilidade** 🌎.  
- Cada zona é uma região física separada, o que aumenta a resiliência em caso de falhas 💪.  
- Essa configuração melhora o SLA geral da aplicação.

## 💾 Contas de Armazenamento e Redundância

O tipo de redundância afeta diretamente o SLA do armazenamento:

- 🟢 **LRS (Locally Redundant Storage):** Redundância dentro de um único datacenter.  
- 🟠 **ZRS (Zone Redundant Storage):** Dados replicados entre zonas da mesma região.  
- 🔵 **GRS (Geo-Redundant Storage):** Replicação para uma região secundária distante.  
- 🟣 **GZRS (Geo-Zone-Redundant Storage):** Combina redundância geográfica e em zonas.

## 🏁 Conclusão

Ao projetar infraestruturas na nuvem, é essencial:
- Avaliar o SLA exigido pelo negócio 📈.  
- Balancear custo e disponibilidade ⚖️.  
- Escolher a redundância de armazenamento adequada 🔑.
