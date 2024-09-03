# Documento de Design de Software: Sistema de Reporte de Árvores Doentes - AMMA

## 1. Visão Geral do Projeto

Este documento descreve o design de software para um sistema que permitirá a AMMA (Associação de Monitoramento e Manutenção Ambiental) reportar e gerenciar informações sobre árvores doentes em áreas urbanas. O sistema será desenvolvido em C# utilizando a arquitetura MVC (Model-View-Controller).

---

## 2. Objetivos do Sistema

- Facilitar o reporte de árvores doentes por usuários e especialistas.
- Permitir a visualização, atualização e acompanhamento do status das árvores reportadas.
- Gerar relatórios para análise das condições ambientais e possíveis ações de intervenção.

---

## 3. Fluxos Principais do Sistema

### 3.1. Reportar Árvore Doente
1. Usuário acessa a página de reporte.
2. Preenche o formulário com as informações da árvore e a localização.
3. Envia o reporte.
4. O sistema armazena o reporte no banco de dados e exibe uma confirmação.

### 3.2. Visualizar Árvores Reportadas
1. Usuário acessa a página de visualização de árvores.
2. Filtra por localização, status ou data de reporte.
3. O sistema exibe a lista de árvores reportadas com suas respectivas informações.

### 3.3. Enviar fotos de árvores
1. Usuario acessa a árvore criada
2. Seleciona a opção para enviaar foto e seleciona a foto desejada.

### 3.4 Criar uma nova doença
1. Usuário acessa o cadastro de doenças
2. Define uma nova doença.

---

## 5. Questões Pertinentes ainda não definidas

### 5.1. Como será a estrutura do banco de dados?
- **Dúvida:** Quais tabelas são necessárias e como elas se relacionam?
- **Solução:** Tabelas principais incluem `Arvores`, `Reportes` e `Localizacoes`, com relações entre `Arvores`, `Reportes` e `Doenças`.

### 5.2. Como garantir a escalabilidade do sistema?
- **Dúvida:** O sistema poderá ser escalado facilmente com o aumento de usuários e reportes?
- **Solução:** Arquitetura baseada em camadas e uso de práticas de design como SOLID para facilitar a manutenção e expansão.

---

## 6. Conclusão

Este documento serve como uma base para o desenvolvimento do sistema de reporte de árvores doentes da AMMA. Com base nas questões levantadas e nas soluções propostas, o projeto pode ser desenvolvido de maneira organizada, garantindo a entrega de um sistema robusto e eficiente.
