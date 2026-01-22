Automação de Relatórios Técnicos com Python

O objetivo deste projeto é processar uma base de dados tabular (CSV) e identificar automaticamente cada cliente e seus indicadores. O sistema gera um gráfico de desempenho personalizado para cada empresa, que é armazenado temporariamente em memória (buffer) para otimização de performance. Este gráfico é inserido em um relatório PDF individualizado.

O pipeline possui inteligência de armazenamento: os arquivos são salvos diretamente no Google Drive ou, caso o caminho não seja detectado, são agrupados em uma pasta local e compactados em formato ZIP para download imediato. Toda a operação é executada de ponta a ponta sem necessidade de intervenção manual.
