ETL4LOD
=======

ETL4LOD - Steps do Pentaho Data Integration (Kettle) relacionados a Linked Data.

* Data Property Mapping: 

O step Data Property Mapping oferece a capacidade de mapear, a partir da linhas do fluxo de entrada, os componentes de uma tripla RDF (sujeito, predicado e objeto) nas linhas do fluxo de sa�da, sendo o objeto um valor literal.

* Object Property Mapping: 

O step Object Property Mapping � similar ao step Data Property Mapping, com a diferen�a de que o valor do objeto enviado no fluxo de sa�da � uma URI de um recurso.

* Sparql Endpoint: 

O step Sparql Endpoint oferece a capacidade de extrair dados de um SPARQL Endpoint, a partir da especifica��o da URL relacionada ao SPARQL Endpoint e da defini��o de uma consulta SPARQL.

* Sparql Update Output: 

O step Sparql Update Output oferece a capacidade de carregar triplas RDF em um banco de triplas (exemplo: Virtuoso).

* NTriple Generator: 

O step NTriple Generator oferece a facilidade de gera��o de seten�as RDF no formato NTriple. � um step �til, por exemplo, para receber as linhas de dados enviadas por um step Data Property Mapping ou Object Property Mapping e gerar, no fluxo de sa�da, as linhas de dados com as triplas RDF a serem inseridas em um banco de triplas, por meio do step Sparql Update Output.

* Annotator: 

O step Annotator anota uma tripla com termos de vocabul�rios e ontologias, de acordo com um mapeamento "de-para" definido em um arquivo XML.

* SparqlRunQuery: 

O step SparqlRunQuery recebe um campo com uma query SPARQL e executa esta query em um SPARQL Endpoint.

Observa��o: Os steps "Data Property Mapping", "Object Property Mapping", "Sparql Endpoint" e "Sparql Update Output" disponibilizados s�o extens�es dos steps produzidos originalmente pelo projeto LinkedDataBR (https://www.rnp.br/pd/gts2010-2011/gt_linkeddatabr.html). As vers�es iniciais destes 4 steps possibilitavam o armazenamento dos metadados de composi��o dos steps somente em um reposit�rio Kettle do tipo sistema de arquivos. As vers�es disponibilizadas aqui possibilitam o armazenamento dos metadados de composi��o dos steps tamb�m em um reposit�rio Kettle do tipo banco de dados. Al�m disso, os c�digos fonte foram adequados � estrutura do maven (http://maven.apache.org). 
