## 📱 PviniksFlix

Este projeto é a implementação de uma interface gráfica de usuário (GUI) para um aplicativo de *streaming* de vídeo, semelhante à interface de reprodução de um episódio do Netflix, como parte de uma atividade acadêmica.

### 🎯 Objetivo

O projeto foi desenvolvido para atender aos requisitos da **Atividade de Aprendizagem a Distância 2** (AAD 2) da disciplina de **Programação para Dispositivos Móveis** do **Instituto Federal Catarinense (IFC) - *Campus* Camboriú**.

O objetivo principal desta atividade foi realizar a implementação da interface gráfica de um aplicativo de minha escolha (neste caso, baseado no exemplo de reprodução da Netflix apresentado na vídeoaula do professor), utilizando o sistema de *layouts* do Android.

### ✨ Funcionalidades da Interface Implementada

A interface `activity_main.xml` simula a tela de reprodução de um episódio, contendo os seguintes elementos principais:

* **Barra de Ferramentas (`MaterialToolbar`):**
    * Título: "PviniksFlix".
    * Fundo na cor primária (`?attr/colorPrimary`).
* **Informações do Conteúdo:**
    * Título da Série/Filme: "The Office" (com um ícone de *download* no topo).
    * Episódio: "T2E01 – The Dundies".
* **Controles de Ação (Ícones):**
    * Adicionar à Lista (`icon_add_lista`).
    * Controle de Volume (`icon_volume`).
    * Favoritar (`icon_favorito`).
* **Visualização do Conteúdo (`ImageView`):**
    * Imagem representativa do episódio (`thedundies`).
* **Barra de Progresso (`SeekBar`):**
    * Exibe o progresso da reprodução (exemplo: `progress="5"`).
    * Marcação de tempo: "00:39" (atual) e "20:30" (total).
* **Controles de Mídia:**
    * Recomeçar/Voltar (`icon_recomecar`).
    * Avançar/Retroceder (o ícone `icon_download` está rotacionado para este propósito, e há outro ícone com rotação de 90 graus).
    * Pa-usar (`icon_pause`).

### 🛠️ Detalhes Técnicos

* **Linguagem:** Java (para `MainActivity.java`) e XML (para os *layouts*).
* **Layout Principal:** `ConstraintLayout` (em `activity_main.xml`) para organizar a interface.
* **Estilização:** O tema (`themes.xml`) utiliza `Theme.Material3.DayNight.NoActionBar` como base e personaliza as cores:
    * `colorPrimary`: `#673AB7`
    * `colorPrimaryDark`: `#3C1583`
    * Cor de fundo da tela (`android:background` no `ConstraintLayout`): `#120E23` (roxo/preto escuro).
    * Cor do texto (`android:textColor`): `@color/white`.
* **Componentes Utilizados:** `MaterialToolbar`, `TextView`, `ImageView`, `SeekBar`, `ConstraintLayout`, `Guideline`, `Barrier`.