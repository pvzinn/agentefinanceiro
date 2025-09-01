# Agente Financeiro
Agente ReAct para o FastCamp

Este projeto realiza a implementação de um agente inteligente baseado no padrão ReAct (Reasoning and Acting), conforme o que é demonstrado no vídeo indicado (https://www.youtube.com/watch?v=hKVhRA9kfeM), usado como referencial.

O novo agente implementado no notebook "corporative_agent.ipynb" foi projetado para auxiliar no agendamento de reuniões em ambiente corporativo. O agente utiliza modelos de linguagem da Groq para processar solicitações de agendamento de forma autônoma.

As novas ferramentas que o agente possui são:

1. "check_availability": Verifica disponibilidade de horários no calendário
2. "schedule_meeting": Agenda reuniões em horários disponíveis
3. "send_email": Envia notificações automáticas para funcionários
As principais modificações feitas em relação ao agente construído no vídeo-referência foram:

System Prompt: Adaptado para contexto de agendamento
Mocks Corporativos: Simulação de funcionários + calendário pré-ocupado
Validação de Conflitos: Verifica disponibilidade antes de agendar
Fluxo Obrigatório: check → schedule → email
Tratamento de Erros: Utilização de prints estratégicos para identificar/tratar conflitos enfrentados
