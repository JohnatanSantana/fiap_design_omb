Atividade para entregar Turmas ASO 
1. Montar um Story Telling sobre o problema que você resolve e definir o tema (Verificar nos 
slides da aula 1 sobre os temas sugeridos). 

2. O que esperamos aprender com esse projeto? 
Determinar os requisitos específicos;
Melhorar processos existentes;
Garantir conformidade com órgãos reguladores;


3. 3. Que perguntas precisamos que sejam respondidas? 
Problemas que existem no processo atual
Quantidade de usuários?
Saber se existem órgão regulador?
Quais são os nossos principais riscos?
Quais requisitos dos Órgãos reguladores?
Temos auditoria que o sistema deve passar?


4. Quais são os nossos principais riscos? 
Atraso;
Falta de entendimento;
Pessoas;
Segurança da informação;
Resistência a mudanças;

5. Crie um plano para aprender o que precisamos para responder a perguntas específicas. 
Sessões de alinhamento com as partes interessadas.
Aplicar metodologias para garantir a participação dos interessados para definição clara de requisitos.
Ambiente colaborativo;
Motivar os usuários participarem;


6. Crie um plano para reduzir riscos. 
Planejamento detalhado e gestão eficiente do projeto;
Implementação de medidas de segurança robustas;
Desenvolvimento de contingência;
Treinamentos para usuários;
Envolvimento dos usuários no processo de desenvolvimento;

7. Quem são as partes interessadas? 
Prefeito;
Gabinete de Gestão e Orçamento;
Empresas;
Equipe de Tecnologia;


8. O que eles esperam ganhar? 
Economia de custos;
Encontrar melhores contratos;
Tempo;
Eficiência operacional;



9. Quem são os usuários? 
Gabinete de Gestão e Orçamento;
Empresas Parceiras;
Departamento de tecnologia;

10. O que eles estão tentando realizar? 
Corte de Custos;
Encontrar melhores custos nos contratos;
Eficiência operacional

11. Qual o pior que pode acontecer? 
Segurança;
Não encontrar o melhor preço no contrato;
Falha no processo;
Fraudes no processo;


12. Desenhe uma arquitetura; 
MVA
![MVA](../images/arquitetura_omb-Arquitetura%20MVA.drawio.png)

Arquitetura Solução
![Solução](../images/arquitetura_omb-Arquitetura_solucao.drawio.png)

13. Faça uma descrição de cada um dos componentes que você desenhou; 
MVA
UI - Ponto de entrada para usuários.
Regras de negocio - Conter toda logica de cadastro, fluxo de RFP.
Banco de dados armazena dados;
ETL - Realiza a carga do banco transacional para o banco analitico;
Dashboard - Mostra indicadores importantes;
Solução

14. Descreva requisitos que você (s) considera importante e por quê? (Mínimo 5) 
IU responsiva - Melhora a experiência do usuário, facilitando a navegação.
Banco de dados com alta disponibilidade - Garanto que o sistema fique funcional em caso de falhas.
OLAP - para fins analiticos o banco de dados principal não seja acessado.
Dashboard intuitivo e informativo - fornecendo uma visão geral para tomada de decisões.
Segurança - Garantir que os acessos sejam feito de forma segura;

15. Sobre o que o diagrama ajuda você a raciocinar/pensar? 
Fluxo de dados e seu comportamento entre componentes;
Deixa claro o relacionamento entre Componentes;
Identificação de camadas;
Relacionamento funcional entre componentes;


16. Quais são os padrões essenciais no diagrama? 
Arquitetura de Camadas, camada de apresentação UI, camada lógica e camada de dados;
ETL, para carregar e transformar dados em um destino.

17. Existem padrões ocultos? 
Facade, interface com logica de negocio, proporcionando interface unica para componentes;

18. Qual é o Metamodelo? 
UML Metamodelo.

19. Pode ser discernido no diagrama único? 
Pode sim, apenas contendo a comunicação entre as camadas. Para aprofundar precisamos de outros diagramas.

20. O diagrama está completo? 
MVA, está faltando uma versão mais detalhada.
Solução está mais completa, mas ainda falta como vai ser acessado e as tecnologias.

21. Poderia ser simplificado e ainda assim ser eficaz? 
Se simplificarmos ainda mais, talvez perca alguma informação.

22. Houve alguma discussão importante que vocês tiveram como equipe? 
Qual tipo de Arquitetura utilizamos para resolver o problema, se partiríamos para uma solução mais escalável, onde utilizamos filas, etc ou uma solução mais simples.

23. Que decisões sua equipe teve dificuldade para tomar? 
Como seria a solução, optamos por uma solução mais simples, por conta de custos e também velocidade.

24. Que decisões foram tomadas sob incerteza? 
Volumetria e escalabilidade, se nossa solução precisaria ser muito escalável,

25. Houve algum ponto de decisão sem retorno que o forçou a desistir de uma determinada escolha? 

26. Desenhe 3 Arquiteturas com o projeto que você desenvolveu na aula em cada uma das 
camadas do C4; (Subir somente a Imagem jpg/jpeg) 

27. Nível Contexto 
**Contexto RFP**
![Contexto](../images/c4/context/c4_context.png)
27.1. Acessa Portal para Gerenciar RFPs
27.2. Visualiza Relatórios Financeiros
27.3. Acessa Portal para Avaliar Propostas
27.4. Visualiza Relatórios de Custos
27.5. Acessa Portal para Monitorar Processos
27.6. Visualiza Desempenho Operacional
27.7. Envia Propostas de RFP
27.8. Autentica Usuários Internos
27.9. Autentica Usuários Externos
27.10. Solicita Dados de Sistema
27.12. Solicita Dados de Sistema
27.11. Fornece Dados
27.13. Fornece Dados
27.14. Envia Dados Brutos"
27.15. Fornece Relatórios Processados


28. Nível Container 
**Colaborador**
![Container Colaborador](../images/c4/container/container_colaborador.png)
28.1.1. Acessa conteúdo via CDN
28.1.2. Distribui conteúdo
28.1.3. Autentica Usuários Internos
28.1.4. Gerencia Sessões
28.1.5. Solicita acesso Web
28.1.6. Fornece Dados de Propostas
28.1.7. Armazena Dados
28.1.8. Envia Dados Brutos
28.1.9. Transfere Dados Processados
28.1.10. Fornece Dados para Relatórios
28.1.11. Fornece Dados em Tempo Real
28.1.12. Fornece relatórios Sistemicos
**Empresas Interessadas**
![Container Empresas](../images/c4/container/container_empresas.png)
28.2.1. Acessa conteúdo via CDN
28.2.2. Distribui conteúdo
28.2.3. Autentica Usuários Externos
28.2.4. Fornece Dados de Propostas
28.2.5. Acessa Web
28.2.6. Gerencia Sessões

29. Nível Componente 
![Componente Colaborador](../images/c4/component/canal_colaborador.png)
29.1.1. Acessa conteúdo via CDN
29.1.2. Distribui conteúdo
29.1.3. Solicita acesso Web
29.1.4. Autentica Usuários Internos
29.1.5. Autentica Usuários Internos
29.1.6. Gerencia RFPs
29.1.7. Envia solicitações de RFP
29.1.8. Processa Dados de RFPs
29.1.9. Gerencia Propostas
29.1.10. Armazena Documentos
29.1.11. Registra Eventos de Auditoria
29.1.12. Armazena e Recupera Documentos
29.1.13. Autentica Usuários
29.1.14. [jdbc]\nLe e escreve]
29.1.15. Registra Mudanças
29.1.16. [jdbc]\nLe e escreve]
29.1.17. Envia Notificações
29.1.18. [jdbc]\nLe]
29.1.19. [jdbc]\nLe e escreve]
![Componente Colaborador](../images/c4/component/dashboard_colaborador.png)
29.2.1. Fornece dados brutos para processamento
29.2.2. Passa dados extraídos para transformação
29.2.3. Passa dados transformados para carregamento
29.2.4. Carrega dados transformados
29.2.5. Consulta dados para relatórios")  
29.2.6. Fornece dados para visualizações e relatórios
29.2.7. Acessa relatórios e visualizações
![Componente Empreas](../images/c4/component/canal_empresas.png)
29.3.1. Acessa conteúdo via CDN"
29.3.2. Distribui conteúdo"
29.3.3. Solicita acesso Web"
29.3.4. Autentica Usuários Externos"
29.3.5. Autentica Usuários Externos"
29.3.6. Submete Propostas de RFP"
29.3.7. Envia solicitações de RFP"
29.3.8. Submete Propostas de RFP"
29.3.9. Solicita Visualização de RFPs"
29.3.10. Solicita Visualização de RFPs"
29.3.11. Obtém RFPs e Notas"
29.3.12. Valida Propostas"
29.3.13. Avalia Propostas"
29.3.14. [jdbc]\nLê e escreve"
29.3.15. Gerencia Sessões"
29.3.16. Valida Usuários para Propostas"
30. Code (Opcional) 
31. Validar no checklist (opcional) - https://c4model.com/review/ 
32. Gravar um vídeo explicando o projeto com um todo e desenhos, Obs: todos os integrantes 
devem apresentar uma parte do projeto. 
Subir em um repositório no github e compartilha com o professor 
Dúvidas contatar os E-mail: 
profleonardo.pinho@fiap.com.br/leonardo.c.pinho@gmail.com 
