📘 Desafio: Monitoramento de Máquinas Virtuais no Azure
🎯 Objetivo
Demonstrar como configurar e gerenciar o monitoramento de recursos no Azure, com foco em VMs, garantindo visibilidade e resposta proativa a eventos críticos — como a exclusão de uma máquina virtual.

🛠️ Etapas Realizadas
1. Criação da Máquina Virtual
Acesse o Portal do Azure

Vá em "Máquinas Virtuais" > "Criar"

Configure a VM com:

Nome: vm-monitoramento

SO: Ubuntu 22.04 ou Windows Server 2022

Tamanho: B1s

Região: Brazil South

📸 Print sugerido: Tela de resumo da VM criada

2. Habilitar Diagnóstico e Monitoramento
Acesse a VM > "Monitoramento" > "Insights"

Clique em "Habilitar" para ativar o Azure Monitor

Selecione ou crie um Log Analytics Workspace

📸 Print sugerido: Tela de ativação do Azure Monitor 📸 Print sugerido: Tela de seleção do Log Analytics

3. Criar Alerta para Exclusão de VM
Vá em "Monitor" > "Alertas" > "Nova Regra"

Escopo: selecione a VM

Condição: "Quando uma operação for igual a Delete Virtual Machine"

Ação: enviar e-mail ou webhook

Nome da regra: alerta-exclusao-vm


