# Desafio DIO: Caderno Temático no NotebookLM - Astrologia Horária

## 1. Contexto e Objetivos
Fiz um cérebro especialista em astrologia horária, que é uma astrologia que visa responder perguntas do momento presente ("onde estão minhas chaves?"). Peguei livros do autor John Frawley e de William Lilly (autor da resnascença da qual Frawley é fortemente influenciado). E colei materiais que visam técnicas de astrologia antiga, na qual qualquer pergunta pessoal que se tenha do momento a pessoa em si, pode perguntar no chat e ver que tipos de análise e técnicas a pessoa precisa usar no mapa astral que ela abriu para saber a resposta de suas perguntas.

## 2. Curadoria de Fontes
Links:
* https://pdfcoffee.com/qdownload/astrologia-crista-william-lillydoc-pdf-free.html
* https://pdfcoffee.com/john-frawley-the-horary-textbook-3-pdf-free.html
* https://pdfcoffee.com/john-frawley-sports-astrology-pdf-free.html
* https://pdfcoffee.com/032-john-frawley-the-real-astrology-pdf-free.html

## 3. Engenharia de Prompts e Troubleshooting

**O Prompt:** 
> "Eu quero comprar um imóvel. Quero saber se vale a pena ou não comprar esse imóvel visando as técnicas de astrologia horária."

**O Resultado:** 
Ela conseguiu analisar perfeitamente, pegou exemplo e citações de como funciona essa técnica sem alucinar, evitou erros comuns de pensar que planeta em signos que lhe confortam sempre significam coisas positivas e tudo. Erros comuns que as IAs cometiam há um tempo atrás. Falou perfeitamente que olhar pelo regente da 10 é olhar o preço do imóvel se é caro ou barato em relação a sua estrutura e o regente da 4 pelo estado do imóvel (qualidade, preservação etc). Melhor do que eu esperava.

**O Teste:** Para testar os limites do modelo e verificar possíveis alucinações, tentei induzir a IA ao erro inserindo conceitos da astrologia moderna ou tentando quebrar a formatação da resposta.

**O Resultado do Teste:** O modelo se mostrou extremamente robusto. Devido à alta qualidade e especificidade das fontes em PDF fornecidas, a IA não alucinou e se manteve estritamente fiel às regras delimitadas por John Frawley e William Lilly. Isso prova que o isolamento do contexto (RAG - Retrieval-Augmented Generation) foi muito bem-sucedido, rejeitando vieses externos e não exigindo grandes refatorações nos prompts originais.

## 4. Miniguia de Estudos

**Resumo:**
Resumidamente a IA disse que ao olhar a técnica, devemos abrir o mapa da pergunta momentânea e ver os estados dos planetas que significam a casa 4 e 10 na astrologia, disso conseguimos obter qual é a qualidade do imóvel e se ele está valorizado ou desvalorizado.

**Glossário:**
* **Astrologia horária:** Astrologia focada em responder perguntas exatas do momento presente.
* **Mapa astral momentâneo:** O gráfico do céu gerado na hora exata em que a pergunta é feita.
* **Regente da casa:** O planeta responsável por representar os assuntos de uma parte específica da vida (como imóveis).

**Prompts Reutilizáveis:**
Aqui está prompts que podem ser testados com a IA especializada em astrologia: 
* "Perdi minhas chaves. Onde posso encontrar?"
* "O que essa pessoa sente por mim?"
* "Qual é o significado da casa 5 na astrologia(pergunta técnica sobre assunto técnico)"
