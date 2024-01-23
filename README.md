## Overview

A lista de etapas abaixo foi criada para simplificar o processo de controle de versão de arquivos .pbix fazendo o uso do pbi-tools.

### Etapas

#### Setup inicial
1. Baixar o pbi-tools;
1. Incluir o diretório onde a ferramenta foi extraída nas variáveis de ambiente;
1. Executar ```pbi-tools extract <nome_do_arquivo.pbix>``` no diretório onde o .pbix está localizado;
1. Instanciar um repositório git;
1. Publicar a primeira versão em um repositório remoto;

#### Em alterações
1. Abrir o Power BI Desktop;
1. Executar ```pbi-tools info``` e anotar o pid da instância do Power BI Desktop que deve ser monitorada;
1. Executar ```pbi-tools extract <nome_do_arquivo.pbix> <pid> -watch``` no diretório onde o .pbix está localizado;
1. Aplicar as alterações desejadas;
1. Salvar as alterações e fechar a aplicação;
1. Adicionar os arquivos alterados, criar o commit e fazer o push para o repositório remoto;
