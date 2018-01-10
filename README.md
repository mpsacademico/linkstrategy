# Link Strategy

Características do sistema:

- manipulador de links
- controle estatístico de links (registro de acesso e análise de logs)
- entrada e saída de links

## Registro
1) O link é recebido pelo sistema, seja por descobrimento automático ou por entrada explícita
2) É gerado um parâmetro único e humanamente indecifrável ("curto" no caso de um encurtador)
3) O link e o seu código são armazenadas na base de dados
4) É dado o retorno da criação do link

## Acesso
1) Todos os links são para um sub-domínio interno do sistema
2) Cada link possui um parâmetro único e humanamente indecifrável
3) A requisição do link faz com que ele seja decifrado comparando com os registros da base de dados
4) Um conjunto de informações sobre a requisição e o link são armazenadas
5) É feito um redirecionamento para o link externo
