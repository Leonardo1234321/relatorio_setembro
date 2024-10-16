# Mês de Agosto (Incluindo Setembro) Leonardo Furtado Kauffmann  

## Introdução

Este primeiro mês serviu para situar no Programa. Portanto, os principais objetivos foram conhecer novas tecnologias acompanharão este processo por todo tempo no Programa. Mas, houveram sim contribuições no auxílio de atividades didáticas, como os testes das tecnologias usadas como recursos didáticos para turma de INFO1V, que será o foco do tópico de contribuições.

## Processo de ensino e contribuições

### Semana 19/08 - 23/08

Durante os primeiros dias (20/08 até 23/08), estudou-se os fundamentos da linguagem de marcação MarkDown, que são cruciais para criação do documentações e, especificamente neste programa, a criação dos relatórios. Posteriormente, o MarkDown pode ser utilizado no processo de aprendizagem da turma de INFO1V, que criará documentações dos códigos, ajudando aqueles que possuem dificuldade ou dúvida em algoritmos.  
  
Em Seguida, introduziu-se o MkDocs, um gerador de sites estáticos para documentações de projetos, em que os documentos são feitos em Markdown e configurados em arquivos YAML. Este relatório é um exemplo do uso desta tecnologia. Como parte dos estudos de Markdown, foi atribuído a tarefa de desenvolver um site (veja o [anexo 1](#anexos)) de documentação markdown utilizando o MkDocs que pode ser utilizado futuramente como anotações para o desenvolvimento de outros projetos. Durante esse período também foi introduzido o modelo do relatório onde usou-se os seguintes comandos para instalação das dependências do modelo:  

1. `python3 -m venv .venv`
2. `source ./.venv/bin/activate`
3. `pip3 install -r requirements.txt`

### Semana 26/08 - 30/08

A partir do dia 29/08, foram feitos testes no software Asciinema, um gravador de tela interativo e acessível, que permite a publicação de gravações na nuvem, com ele foi feito a correção de um teste da turma de INFO1V na disciplina de Fundamentos de Algoritmo e Lógica. A seguir, um exemplo de comando de gravação do terminal:

    $ asciinema rec -i 2.5 -t "Primeira Gravação"
  
Onde ‘-i ‘ define o tempo máximo ‘idle’, ou seja, quanto tempo se passa parado no terminal, já o -t indica o título da gravação ao ser publicada.  
  
Na mesma semana, foi testado outra ferramenta poderosa, o mermaid. Este é feito em JavaScript, e é baseado em Markdown, seu propósito é a criação de diagramas dos mais variados tipos. Isto ajuda no processo de ensino, pois ajuda a explicar, de forma didática, os fluxos de um script. Além disso, consegue representar visualmente diferentes processos, como a repetição, as condicionais e etc.  
  
Nesta semana também foi feito um ensaio de acompanhamento especial com Lucas sob orientação do professor João.
  
### Semana 02/09 - 06/09  
  
Nesta semana introduziu-se a Oulu, um dos servidores do campus com acesso à área remota (RDP) baseado no sistema operacional Debian. O foco  era familiarizar-se com o acesso via SSH, RDP e HTTP (<http://oulu/>). Exemplo do acesso SSH:

    ssh -XY “nome do usuário”@oulu

Em seguida, alguns testes foram feitos para verificar o script, em python, desenvolvido pelo professor Jurandy Soares, que automatizava a criação de usuários para uma aula na turma de INFO1V com acesso remoto à oulu.  
  
O Resultado da configuração dos usuários da conta oulu na turma de info1v foi positivo. A aula, do dia 05/10, fluiu normalmente e os alunos interagiram com os códigos um dos outros no sistema remoto concluindo o objetivo da aula de revisão de expressões em python.

  
### Semana 09/09 - 13/09

A partir deste momento, foram feitos testes no script de correção das provas [Anexo 2](#anexos).  

Em seguida, foram feito algumas simulações da criação de usuário definitivo na oulu com um script python 'cria-meu-usuario' desenvolvido por Jurandy. A simulação foi feita com o CSSH (Cluster Administration tool), permitindo o uso de diversas instâncias do xterm como se fossem uma "turma" completa.

    cssh usuario-{01..40}@oulu

O usuario-{01..40} representa que serão criadas 40 instâncias, indo de 1 até 40. O usuario-01, 02, 03, ... Já existem pois foram criados de forma temporaria na aula do dia 05/10, para que fossem criadas contas definitivas posteriormente. 
  
## Anexos

1. Site de Documentação Markdown (host pelo github Pages): <https://leonardo1234321.github.io/demomd/>  

2. Repositório do script corretor (Desenvolvido por Jurandy): <https://github.com/jurandysoares/dycorrigir>
