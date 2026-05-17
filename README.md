# 🌍 Jogo da Coleta Seletiva Inclusiva — Edição II

### Centro Universitário Internacional UNINTER
**Curso:** Tecnologia em Banco de Dados (CST)  
**Disciplina:** Atividade Extensionista II: Tecnologia Aplicada à Inclusão Digital – Projeto  
**Estudante:** Douglas Alexander Scaramuzzi  
**RU:** 5120066  
**Localização:** Suzano - SP  

---

## 📖 Apresentação do Projeto
Este projeto consiste no desenvolvimento e implementação de melhorias de software de um jogo educativo e altamente acessível voltado à conscientização sobre a reciclagem, descarte correto de resíduos sólidos e inclusão digital nas escolas e comunidade local de Suzano-SP. 

Trata-se da **fase final e prática (Projeto - Fase II)** do protótipo estruturado na fase anterior, evoluindo a arquitetura do jogo de um modelo linear de descarte para uma plataforma gamificada, inclusiva e adaptativa com gerenciamento local de dados.

---

## ♻️ Objetivos de Desenvolvimento Sustentável (ODS) Alinhados
* **ODS 4 – Educação de Qualidade:** Democratizar o acesso a ferramentas pedagógicas interativas, garantindo o Desenho Universal de aprendizagem para crianças com necessidades educacionais especiais ou limitações motoras.
* **ODS 12 – Consumo e Produção Responsáveis:** Conscientizar os alunos de forma lúdica sobre a correta separação, triagem e destinação de resíduos urbanos, com ênfase especial na destinação segura do lixo eletroeletrônico.

---

## 🚀 Melhorias Técnicas e de Inclusão Implementadas (Fase II)

Esta evolução do projeto focou no desenvolvimento de funcionalidades que combinam a **Modelagem e Persistência de Dados** (foco do curso do CST em Banco de Dados) com recursos avançados de **Acessibilidade Web (W3C)**:

1. **Persistência de Dados Relacional Simulada (`localStorage`)**:
   Implementação de um banco de dados local semiestruturado utilizando armazenamento em formato JSON. O sistema registra de forma local e persistente o histórico de sessões do jogo.
2. **Cronômetro de Alta Precisão e Algoritmo de Desempate Justo (Sorting)**:
   Medição de tempo com precisão de décimos de segundo (`performance.now`). O ranking (Leaderboard) organiza os recordistas simulando uma query relacional multicritério de ordenação:
   `ORDER BY score DESC, time_elapsed ASC LIMIT 5`
   Isso garante que em caso de empates na pontuação, o jogador que realizou a atividade no menor tempo fique no topo.
3. **Mecânica Cognitiva com Embaralhamento Aleatório ($Fisher-Yates$)**:
   Reforço da memória e do aprendizado dinâmico. O jogo seleciona 5 itens aleatórios de uma base de dados expandida de resíduos a cada rodada, garantindo que as partidas nunca sejam idênticas e estimulando a atenção da criança.
4. **Modo de Alto Contraste (Acessibilidade Visual)**:
   Adaptação de cores e remoção de elementos complexos para garantir usabilidade por alunos com baixa visão ou diferentes tipos de daltonismo.
5. **Narração de Voz Dinâmica e Inteligente (Web Speech API)**:
   Leitura de tela com velocidade otimizada ($1.50$) e frases simplificadas para facilitar a assimilação por deficientes visuais e crianças em processo de alfabetização.
6. **Controles Físicos e Motores de Entrada Alternativos**:
   * **Teclado:** Mapeamento de teclas rápidas de `1` a `6` correspondentes às lixeiras do nível ativo.
   * **Toque/Clique:** Mecânica de Clique-para-Selecionar, eliminando a dependência do arrastar-e-soltar (*drag-and-drop*) para facilitar o manuseio em celulares ou por indivíduos com limitações motoras finas.

---

## 🎮 Como Jogar
1. Acesse o jogo através do link de produção hospedado no **GitHub Pages**.
2. Digite seu primeiro nome na tela de boas-vindas para registrar sua sessão no banco de dados.
3. Arraste ou clique no objeto reciclável exibido no centro da tela.
4. Escolha e clique na lixeira correta para descartá-lo.
5. Conclua os 3 níveis de progressão pedagógica para registrar sua pontuação e tempo no Placar de Líderes local!

---

## 📂 Links do Projeto
* **Link de Produção (Jogar online):** [https://douglas-scaramuzzi.github.io/coleta-seletiva-atualizado/](https://douglas-scaramuzzi.github.io/coleta-seletiva-atualizado/)
* **Link do Repositório (Código-fonte):** [https://github.com/douglas-scaramuzzi/coleta-seletiva-atualizado](https://github.com/douglas-scaramuzzi/coleta-seletiva-atualizado)
