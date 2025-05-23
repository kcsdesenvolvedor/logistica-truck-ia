# 🚚 Logística Truck AI 🛣️

Bem-vindo ao **Logística Truck AI**! Este projeto utiliza o poder da Inteligência Artificial com Agentes para ajudar caminhoneiros a otimizar suas rotas de entrega, economizando tempo e combustível. Chega de dores de cabeça no planejamento – deixe nossos agentes inteligentes guiarem você!

## 🌟 Visão Geral do Projeto

Este sistema foi desenvolvido para simplificar a vida dos caminhoneiros, fornecendo uma maneira fácil e rápida de planejar rotas com múltiplos destinos. Utilizando o Google Gemini e o framework de Agentes (ADK), criamos uma solução interativa que:

1.  Coleta informações sobre a **localização atual** do caminhoneiro.
2.  Recebe a lista de **cidades de destino** para as entregas.
3.  Processa essas informações para gerar uma **rota estratégica**.
4.  Fornece um **link direto para o Google Maps** com a rota otimizada e todos os pontos de parada.

## ✨ Funcionalidades Principais

* **Interface Conversacional Simples:** Interaja com o sistema de forma natural para fornecer os dados da sua rota. 🗣️
* **Coleta de Dados Inteligente:** O primeiro agente garante que todas as informações necessárias (origem e destinos) sejam coletadas corretamente. 📝
* **Geração de Rotas Estratégicas:** O segundo agente pesquisa e constrói a melhor URL para o Google Maps, considerando todos os seus pontos de entrega. 🗺️
* **Link Direto para Google Maps:** Receba um link clicável que abre o Google Maps diretamente com sua rota calculada, pronta para a navegação. 📱➡️🚗
* **Otimização de Entregas:** Facilita o planejamento para múltiplas paradas, tornando as entregas mais ágeis. 📦💨
* **Baseado em Agentes de IA:** Utiliza agentes especializados para cada etapa do processo, garantindo eficiência e precisão. 🧠

## 🤖 Conheça Nossos Agentes Inteligentes

Este projeto é orquestrado por dois agentes principais, cada um com sua especialidade:

### 1. 🕵️‍♂️ `AgenteColetorDeDados`
   * **Descrição:** Este agente é o seu primeiro ponto de contato! Ele é amigável e eficiente, responsável por conversar com você, caminhoneiro, para obter as informações cruciais para o planejamento.
   * **Tarefas:**
      * 💬 Perguntar e registrar sua **cidade de origem atual**.
      * 🏘️ Perguntar e registrar a(s) **cidade(s) de destino** para suas entregas.
      * ✔️ Confirmar os dados coletados para garantir a precisão.
   * **Ferramentas Utilizadas:** Nenhuma ferramenta externa, apenas suas habilidades de conversação e compreensão!

### 2. 🗺️ `AgenteGeradorDeRotas`
   * **Descrição:** Com os dados em mãos, este agente entra em ação! Ele é um especialista em logística e no uso do Google Maps. Sua missão é transformar as informações de cidades em um plano de rota acionável.
   * **Tarefas:**
      * 🧠 Analisar a cidade de origem e os destinos fornecidos.
      * 🔍 Utilizar a ferramenta `Google Search` para pesquisar e determinar o formato ideal de URL do Google Maps que inclua a origem e todos os destinos como pontos de parada (waypoints) na ordem correta.
      * 🔗 Construir o link mágico do Google Maps, codificando os nomes das cidades adequadamente para o formato de URL.
      * 📤 Retornar uma mensagem amigável contendo o link direto para a rota no Google Maps.
   * **Ferramentas Utilizadas:** `Google Search`

## 🛠️ Tecnologias Utilizadas

* **Google Gemini:** O cérebro por trás dos nossos agentes, fornecendo a inteligência para entender e processar as solicitações.
* **Google ADK (Agent Development Kit):** Framework utilizado para construir, gerenciar e executar os agentes de IA.
* **Python:** A linguagem de programação que une tudo. 🐍
* **Google Colab / Jupyter Notebook:** Ambiente de desenvolvimento e execução do projeto. 📓
* **Google Search (como ferramenta):** Utilizado pelo `AgenteGeradorDeRotas` para encontrar a melhor forma de montar os links do Google Maps.

## 🚀 Como Usar

1.  **Abra o Notebook:** Carregue o arquivo `.ipynb` no Google Colab.
2.  **Configure sua API Key:** Certifique-se de que sua `GOOGLE_API_KEY` (para o Gemini) está configurada nos "Secrets" do Google Colab.
3.  **Execute as Células:** Rode as células do notebook em sequência.
4.  **Interaja com o Assistente:**
    * Informe sua cidade atual quando o `AgenteColetorDeDados` perguntar.
    * Informe as cidades de destino (separadas por vírgula, se mais de uma).
5.  **Receba sua Rota:** O `AgenteGeradorDeRotas` fornecerá um link. Clique nele e boa viagem! 🎉

## 🤝 Contribuições

Contribuições são sempre bem-vindas! Se você tem ideias para melhorar este assistente, sinta-se à vontade para:

* Abrir uma *Issue* para discutir novas funcionalidades ou reportar bugs.
* Enviar um *Pull Request* com suas melhorias.

Juntos, podemos tornar esta ferramenta ainda mais poderosa para a comunidade de caminhoneiros!

## 📄 Licença

Este projeto é distribuído sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes (se aplicável).

---

Esperamos que este assistente torne suas viagens mais tranquilas e eficientes! 🛣️✨
