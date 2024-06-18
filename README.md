## **Avaliação Técnica - Testes Manuais**


**1) Em suas palavras, defina o que é a pirâmide de testes.**

A pirâmide de testes é um modelo conceitual aplicado no desenvolvimento de software para ilustrar a proporção e o tipo de testes que devem ser realizados em nosso projeto, por exemplo.
 Essa pirâmide é composta por três níveis principais, que representam diferentes tipos de testes que devem ser aplicados para assegurar a qualidade do software. 

Lembro da aplicação dessa pirâmide em minha última atuação como Desenvolvedor Python, pois a própria pirâmide de teste traz como sugestão que a maioria dos testes devem ser compostos por: **testes de unidade**, seguindo para **testes de integração** e, finalizando com **testes de interface do usuário(UI)**. 


**2) Como você classifica a participação do QA dentro da squad? Considere todo o fluxo desde a criação das histórias até a entrega da demanda.**

O QA é um membro fundamental pois:

* Pode-se garantir a qualidade software;
* Revisa e analisa as especificações;
* Reporta e documenta bugs, problemas técnicos, boas pŕaticas e orientações;

Além de ser o principal responsável pelo o processo e garantia de qualidade do software buscando além da visão técnica,  usabilidade a nível de usuário.

Benefícios que observei em meu trabalho como **Desenvolvedor Python** foram potencializados com a participação do QA dentro da Squad, considerando todo o fluxo desde a criação até a entrega:

* **Mais eficiência e maior qualidade do Software**, ou seja, a participação do QA desde o início do ciclo de desenvolvimento contribui para a entrega de um software com menos bugs, mais estável e confiável.
* **Otimização de custos**, sendo que a  identificação e correção de bugs em fases iniciais do desenvolvimento evita retrabalho e custos adicionais.
* **Melhoria contínua e constante na experiência do usuário**, uma vez que o foco do QA está na qualidade do software garantindo uma experiência positiva para os usuários finais.
* **Agilidade no Desenvolvimento**, tendo em vista que a colaboração do QA com a equipe de desenvolvimento otimiza o processo de desenvolvimento e agiliza a entrega de valor aos usuários.

**3) Escreva cenários de testes para o cadastro de um novo cliente na plataforma Assertiva com base na imagem abaixo:**


**Objetivo**:

Validar o processo de cadastro de novos clientes na plataforma Assertiva, garantindo que funcione corretamente e esteja atendendo os requisitos do negócio.

**Parâmetros de aceitação**:
 
* O cliente deve conseguir se cadastrar com sucesso, fornecendo as informações obrigatórias e válidas.
* O sistema deve validar os dados informados, impedindo o cadastro com informações incorretas ou incompletas.
* O sistema deve enviar um e-mail de confirmação de cadastro para o endereço informado pelo cliente no ato do cadastro.
* O cliente deve conseguir ativar sua conta clicando no link enviado no e-mail de confirmação.
* O cliente deve conseguir acessar sua conta após a ativação, utilizando o login e senha informados no cadastro.

**Cenário 1: Cadastro com Sucesso (caminho feliz)**:

**Ações**:

* Acessar a página de cadastro de novo cliente.
* Preencher todos os campos obrigatórios com informações válidas.
* Clicar no botão "Cadastrar".

**Resultado Esperado**:

* O sistema deve exibir uma mensagem de sucesso informando que o cadastro foi realizado.
* O cliente deve receber um e-mail de confirmação de cadastro.
* O cliente deve conseguir ativar sua conta clicando no link enviado no e-mail de confirmação.
* O cliente deve conseguir acessar sua conta após a ativação, utilizando o login e senha informados no cadastro.

**Cenário 2: Cadastro com Dados Inválidos (caminho infeliz)**:

**Ações**:

* Acessar a página de cadastro de novo cliente.
* Preencher um ou mais campos obrigatórios com informações inválidas (ex: nome em branco, CPF inválido, e-mail inválido).
* Clicar no botão "Cadastrar".

**Resultado Esperado**:

* O sistema deve exibir mensagens de erro para cada campo com informações inválidas, indicando o problema e orientando o cliente a corrigir os dados.
* O cadastro não deve ser realizado.


**4) O QA identificou na versão de testes um bug na tela de Relatórios ao tentar Extrair o relatório de Boletos do seu sistema.**

**Com base na imagem e considerando que o QA estava com perfil de administrador no momento em que tentou extrair o relatório, como você reportaria o bug de forma escrita e detalhada. Utilize tópicos para facilitar o entendimento.**



**Relato de Bug na Tela de Relatórios: Falha ao Extrair Relatório de Boletos**


**Recapitulando**: 

O QA (que em breve será o Helder) identificou um bug na tela de Relatórios ao tentar extrair o relatório de Boletos. O bug ocorre quando um usuário com perfil de administrador tenta extrair o relatório, resultando em uma mensagem de erro.

**Passo a passo à verificar**:

* Acessar a tela de Relatórios.
* Selecionar a opção "Boletos" no menu "Relatórios".
* Preencher os campos de filtro com os dados desejados.
* Clicar no botão "Extrair Relatório".


**Resultado Esperado**:

O sistema deve gerar e apresentar o relatório de Boletos de acordo com os filtros selecionados pelo usuário.

**Resultado Obtido**:

O sistema exibe a seguinte mensagem de erro: **! Erro**

**Informações Adicionais**:

* O bug ocorreu quando o usuário estava logado com perfil de administrador.
* O bug foi reproduzido em diferentes navegadores e dispositivos **(essa afirmação se faz após de fato testar em diferentes navegadores e dispositivos)**.
* O bug não impede a extração de outros tipos de relatórios, como relatórios de dívidas ou relatórios de eventos **(afirmativa feita após realizar a extração de outros tipos de relatórios)**.

**Impacto**:

O bug impede que administradores extraiam o relatório de Boletos, dificultando o acompanhamento das finanças do sistema.

**Prioridade**:

Alta, pois o bug impede o acesso a informações importantes para a gestão financeira do sistema.

**Gravidade**:

Crítica, pois o bug afeta diretamente a funcionalidade de um usuário com perfil de administrador.

**Sugestões de Correções**:

* Verificar se há algum problema com os dados de filtro selecionados.
* Validar se o usuário (mesmo com perfil de administrador) possui as permissões necessárias para extrair o relatório de Boletos.
* Validar também se o erro ocorre nos ambientes de **Desenvolvimento** e **Produção**.
* Corrigir o erro na geração do relatório de Boletos.
* Implementar mecanismos de tratamento de erros que apresentem mensagens mais informativas ao usuário.

**Anexos e observações**:

* Print da tela que consta a mensagem de erro.
* Logs do sistema relacionados ao bug.

**Além de todo o report realizado acima, o Helder sendo esse QA faria**:

* Aguardar e acompanhar a correção do bug pela equipe de desenvolvimento, registrando ao time que permaneço à disposição pra fins de colaboração se necessário.
* Após a correção testar novamente a funcionalidade, para garantir que o bug, problema foi solucionado e assegurar a qualidade para o usuário final.




**Observação**: As imagens mencionadas nas questões 3 e 4 não foram carregadas, se necessário favor verificar o enunciado das questões e as imagens de ambas no arquivo em pdf enviado por e-mail. 





