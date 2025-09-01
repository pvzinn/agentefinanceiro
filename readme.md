Este projeto realiza a implementação de um agente inteligente baseado no padrão ReAct (Reasoning and Acting), conforme o que é demonstrado no vídeo indicado (https://www.youtube.com/watch?v=hKVhRA9kfeM), usado como referencial.

O novo agente implementado no notebook "corporative_agent.ipynb" foi projetado para auxiliar no agendamento de reuniões em ambiente corporativo. O agente utiliza modelos de linguagem da Groq para processar solicitações de agendamento de forma autônoma.

As novas ferramentas que o agente possui são:

-  "check_availability": Verifica disponibilidade de horários no calendário
-  "schedule_meeting": Agenda reuniões em horários disponíveis
-  "send_email": Envia notificações automáticas para funcionários

As principais modificações feitas em relação ao agente construído no vídeo-referência foram:

1. System Prompt: Adaptado para contexto de agendamento
2. Mocks Corporativos: Simulação de funcionários + calendário pré-ocupado
3. Validação de Conflitos: Verifica disponibilidade antes de agendar
4. Fluxo Obrigatório: check → schedule → email
5. Tratamento de Erros: Utilização de prints estratégicos para identificar/tratar conflitos enfrentados