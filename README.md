

Desafio QA — BeeDoo

## Análise inicial da aplicação

A aplicação tem como objetivo permitir o gerenciamento de uma listagem de cursos,
oferecendo as operações essenciais de inserção, visualização e exclusão de registros.
Cada curso conta com informações como título, descrição, modalidade (presencial ou online),
período com datas de início e fim, quantidade de vagas, instrutor e imagem de capa.

## Principais fluxos disponíveis

- **Cadastro de curso:** preenchimento do formulário e salvamento no localStorage
- **Listagem de cursos:** exibição dos cursos cadastrados em formato de cards
- **Exclusão de curso:** remoção de um curso da listagem a partir do card

## Pontos críticos para teste

Os pontos considerados mais críticos para a cobertura de testes foram:

- **Exclusão de curso:** operação fundamental do CRUD que, se falhar silenciosamente,
pode transmitir ao usuário uma falsa sensação de sucesso
- **Validações do formulário:** ausência de restrições nos campos pode permitir
dados inconsistentes, como números reais em vagas, datas ilógicas e links inválidos
- **Exibição correta dos dados no card:** garantir que todas as informações cadastradas
sejam corretamente renderizadas na listagem

## Decisões tomadas para criação dos testes

Os casos de teste foram escritos em Gherkin (DADO, QUANDO, ENTÃO) e organizados
em uma planilha cobrindo fluxo principal, cenários negativos, validações de campos
e comportamentos inesperados. A priorização seguiu a lógica de risco: primeiro
garantir que o fluxo principal funciona, depois que erros são tratados corretamente
e por fim que a interface está consistente.

## Raciocínio durante a análise

A análise partiu de uma exploração livre da aplicação antes da criação formal dos
casos de teste, o que permitiu identificar comportamentos inesperados com antecedência.
Os bugs encontrados foram documentados com passos de reprodução, resultado atual,
resultado esperado e severidade, e posteriormente relacionados aos casos de teste
correspondentes para garantir rastreabilidade.


## Links

- Planilha de casos de teste: [Google Sheets](https://docs.google.com/spreadsheets/d/1_z0FcI4RZuiCwBfcS4C4fOoTA_zMf_t0Tubj35aY3BU/edit?usp=sharing)
- Evidências de execução: [Google Drive](https://drive.google.com/drive/folders/1qRYza3M5am3cCMUmuH8GeV41NYF8KK0F?usp=sharing)
