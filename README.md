# 🤖 Automação de Relatórios Técnicos com Python

Este projeto automatiza o ciclo completo de análise de dados e geração de documentos técnicos, transformando bases de dados brutas em relatórios PDF personalizados com inteligência de armazenamento. Os dados utilizados são fictícios.

---

## ⚙️ Funcionamento do Pipeline

O sistema executa um fluxo de trabalho (end-to-end) focado em performance e escalabilidade:

1.  **Leitura e Identificação:** O script processa uma base tabular (CSV) e separa automaticamente cada cliente e seus respectivos indicadores.
2.  **Geração de Gráficos em Memória:** Para otimizar a velocidade, os gráficos de desempenho são gerados e manipulados em **Buffer (RAM)**, evitando gravações desnecessárias em disco durante o processamento.
3.  **PDF Individualizado:** Cada empresa recebe um relatório exclusivo contendo seus dados analisados e visuais personalizados.

> [!TIP]
> **Observação de Dados:** O pipeline foi desenhado para garantir integridade total dos indicadores desde a leitura do CSV até a renderização final no PDF.

---

## ☁️ Inteligência de Armazenamento e Saída

O script possui lógica de detecção de ambiente para garantir que os arquivos nunca sejam perdidos:

* **Prioridade 1 (Nuvem):** Salva os relatórios diretamente em pastas específicas no **Google Drive**.
* **Prioridade 2 (Local/Fallback):** Caso o caminho da nuvem não seja detectado, o sistema:
    * Cria uma pasta local organizada.
    * Agrupa todos os PDFs gerados.
    * Compacta tudo em um arquivo **ZIP** para download imediato.

---

## 🚀 Tecnologias Utilizadas

* **Linguagem:** Python
* **Manipulação de Dados:** Pandas
* **Visualização:** Matplotlib / Seaborn
* **Geração de PDF:** FPDF / ReportLab
* **Integração:** Google Colab / PyDrive

---

## 📂 Como utilizar

1. Faça o upload da sua base de dados no formato `.csv`.
2. Configure o caminho do seu Google Drive (opcional).
3. Execute todas as células do notebook.
4. O sistema entregará os relatórios processados na nuvem ou disponibilizará o link para download do `.zip`.

---
🖼️ Fotos do Projeto

1. Tabela de dados simples em csv: cliente x Período x Eficiência produtiva (%)

<img width="389" height="269" alt="2" src="https://github.com/user-attachments/assets/69faf0ec-fdda-48d1-9a94-7faa2ce12855" />

---

2. Relatório automatizado com gráfico construído para empresa ficiticia 'Delta Química Ltda'

<img width="864" height="616" alt="1" src="https://github.com/user-attachments/assets/3a3193ff-6ea8-4708-88dd-c2ae3bb164b5" />

---
**Operação 100% automatizada, sem necessidade de intervenção manual.**

---
**Autor:** Sander Gustavo Piva 
