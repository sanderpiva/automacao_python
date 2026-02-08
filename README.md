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
**Operação 100% automatizada, sem necessidade de intervenção manual.**
