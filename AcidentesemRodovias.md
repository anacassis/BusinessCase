

# Business Case - Acidentes em Rodovias (Empowerdata)
Este repositório documenta o processo de coleta de dados, limpeza, tratamento, além da criação de tabelas no banco de dados e apresentação dos resultados em visualizações interativas.

## Objetivos 
#### Quantificar o total de eventos ocorridos, com visões por horários, dias da semana e estado;
#### Levantar a quantidade de óbitos e feridos;
#### Criar um mapa com a geolocalização dos eventos;
#### Avaliar quais são as “Top 7” causas de acidentes;
#### Quantificar as ocorrencias onde um único acidente registra mais de 3 óbitos.


## Requerimento 
* windows 10.
* pgAdmim 4 PostgreSQL : para criação do SGBD.
* Power BI : para visualizações de Relatórios.

## Arquitetura
![Modelo](https://user-images.githubusercontent.com/97900395/150194733-f267a1f8-66c7-4a2e-ad0d-b165a78184f6.png)

PgAdimim 4
#### Primeiramente, criei meu banco no pgAdmim com o nome de rodovia1, e fiz a criação da unica tabela e adicionei as seguintes colunas:

id, data, hora, uf, br, km, municipio, causa_acidente, tipo_acidente, classificacao_acidente, fase_dia, 
sentido_via, condicao_metereologica, tipo_pista, tracado_via, pessoas,	mortos,	feridos_leves,	feridos_graves,
ilesos,	ignorados,	feridos,	veiculos,	latitude,	longitude.

![Colunas](https://user-images.githubusercontent.com/97900395/150195280-9443d74f-ece3-425a-9637-213d9b66afbc.png)


Power Bi
#### Fiz a analise e a transformação dos dados, carreguei o database postegre no Power BI.

![conexão com banco de daodos](https://user-images.githubusercontent.com/97900395/150197625-cb52b726-5a32-41f0-85be-58c3e3f60ae1.png)


Dashboard interativo pronto com os objetivos estabelecidos
![Dashboard Github](https://user-images.githubusercontent.com/97900395/150392947-219f5af7-d6f4-4702-88d1-8655081e060b.png)


### Objetivos 

#### Quantificar o total de eventos ocorridos, com visões por horários, dias da semana e estado; 

![Pergunta 1](https://user-images.githubusercontent.com/97900395/150387670-653c4b69-3bee-417f-b95b-4b30a7f1db71.png)

#### Levantar a quantidade de óbitos e feridos;
![Pergunta 2](https://user-images.githubusercontent.com/97900395/150388349-c174c4aa-d01f-4754-8e01-60dfd96518a7.png)

#### Criar um mapa com a geolocalização dos eventos;
![Pergunta 3](https://user-images.githubusercontent.com/97900395/150388716-dce7cf11-118c-4853-a4a5-c20416dbe6e2.png)

#### Avaliar quais são as “Top 7” causas de acidentes;
![7 acidentes](https://user-images.githubusercontent.com/97900395/150393542-c5fef289-f1c6-4fea-9bfe-af368537a747.png)

#### Quantificar as ocorrencias onde um único acidente registra mais de 3 óbitos.
![ocorrencia](https://user-images.githubusercontent.com/97900395/150393107-764ee004-0af0-46ef-b399-14fb20ccf010.png)

#### Conclusão
Analisando  as causas de acidentes a causa que ocorre numeros maiores de acidentes é "Falta de atenção a Condução" e vesse um numero maior no estado de MG. 
Observandoo historico geral, os acidentes acontecem com mais frêquencia aos domingos com uma maior alta nos meses de dezembro e janeiro. Entre os anos analisados, 2018 foi o que obteve mais acidentes, em 2019 e 2020 ocorreram menos acidentes porém houve um maior número de pessoas feridase/ou mortas.  
Geralmente a maior parte costumam ocorrer em pistas dupla, simples e com menor taxa em multiplas. 




