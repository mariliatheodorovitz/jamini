# jamini - Agente de Jam Sessions

## Descrição do Projeto

Este projeto é um agente de inteligência artificial desenvolvido para conectar músicos, facilitar a formação de grupos musicais e auxiliar no agendamento de estúdios para ensaios e jams. O agente utiliza processamento de linguagem natural (PLN) para entender as informações fornecidas pelos músicos, geolocalização para encontrar músicos e estúdios próximos, e um sistema de pontuação para sugerir os matches mais relevantes.

## Funcionalidades Atuais

* **Geração de Músicos Fictícios:** Criação de uma base de dados simulada de músicos com informações como nome, instrumento, estilo musical, localização e disponibilidade (em texto livre).
* **Processamento de Linguagem Natural (PLN):** Utilização da biblioteca spaCy para extrair informações relevantes (nível de experiência e disponibilidade) do texto livre fornecido pelos músicos.
* **Geolocalização (Fictícia):** Inclusão de coordenadas geográficas simuladas para os músicos e estúdios.
* **Cálculo de Distância:** Utilização da fórmula de Haversine para calcular a distância entre músicos e estúdios.
* **Sistema de Pontuação de Match:** Cálculo de uma pontuação de compatibilidade entre músicos com base em diversos critérios (instrumento, gênero, localização, nível, disponibilidade e distância).
* **Formação de Grupos:** Lógica para sugerir a formação de grupos de músicos com base na compatibilidade.
* **Filtragem de Estúdios:** Identificação de estúdios relevantes próximos aos grupos de músicos.
* **Proposta de Horários:** Sugestão de horários para ensaio/jam que coincidem com a disponibilidade dos músicos e dos estúdios.
* **Simulação de Pedido de Reserva:** Geração de uma mensagem simulada para solicitar uma reserva de estúdio, incluindo detalhes do grupo e necessidades.
* **Fluxo de Confirmação:** Simulação de um processo de confirmação da reserva pelo usuário.
* **Interface Web (via Gradio):** Interface web simples para interagir com algumas funcionalidades do agente.

## Próximos Passos e Melhorias Planejadas

* **Aprimoramento do PLN:** Melhorar a extração de informações de nível de experiência e disponibilidade do texto livre, talvez utilizando modelos de PLN mais avançados.
* **Integração com APIs Reais:**
    * Utilizar a API do Google Maps para obter dados de geolocalização precisos a partir de endereços ou CEPs.
    * Explorar e integrar APIs de plataformas de reserva de estúdios para obter informações atualizadas sobre disponibilidade e preços.
    * Integrar com uma API do WhatsApp Business para automatizar o envio de mensagens de reserva.
* **Melhoria da Representação da Disponibilidade:** Adotar um formato estruturado para a coleta e armazenamento da disponibilidade dos músicos (e.g., calendários ou intervalos de tempo).
* **Lógica de Agendamento Aprimorada:** Refinar a lógica para encontrar horários que funcionem para grupos, considerando preferências e otimizações.
* **Interface de Usuário Mais Completa:** Desenvolver uma interface web mais robusta e amigável (possivelmente com Streamlit ou outra framework) para todas as funcionalidades do agente.
* **Persistência de Dados:** Implementar um sistema para armazenar informações sobre músicos, grupos e histórico de agendamentos.
* **Sistema de Avaliações:** Incorporar um sistema para que músicos avaliem seus matches e estúdios.

## Como Usar (Testando no Google Colab)

1.  **Execute as células de código em ordem** no notebook do Google Colab.
2.  **Observe a saída** de cada etapa para verificar o funcionamento.
3.  Para interagir com a interface web (se implementada com Gradio ou Streamlit), siga o link público fornecido após a execução da célula correspondente.

## Bibliotecas Utilizadas

* **faker:** Para gerar dados fictícios de músicos.
* **spaCy:** Para processamento de linguagem natural.
* **math:** Para cálculos matemáticos (fórmula de Haversine).
* **json:** Para trabalhar com arquivos JSON (armazenamento de dados).
* **random:** Para geração de dados aleatórios.
* **datetime:** Para manipulação de datas e horários.
* **gradio (opcional):** Para criar uma interface web simples.
* **streamlit (opcional):** Para criar uma interface web mais elaborada.



## Autor

[Marília Andreo Theodorovitz/mariliatheodorovitz]
