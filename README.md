# Implementação do Standard MIMS para BioData.pt

Este repositório contém o código necessário para a implementação do standard MIMS (Minimum Information about a Microarray Experiment) para o BioData.pt.

## Instruções de Upload

Para realizar o upload deste código para o servidor, siga os passos descritos no website https://guides.dataverse.org/en/latest/admin/metadatacustomization.html#id29:

1. Faça o upload do arquivo de texto contendo o código para o servidor. O arquivo de código deve estar no formato TSV (Tab-Separated Values).

2. Use o seguinte comando `curl` para carregar o novo bloco de metadados:

   ```sh
   curl http://localhost:8080/api/admin/datasetfield/load -H "Content-type: text/tab-separated-values" -X POST --upload-file /tmp/new-metadata-block.tsv
