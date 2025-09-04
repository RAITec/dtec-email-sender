TUTORIAL DE COMO USAR PROS FUTUROS RAITECOS
- clone o repositorio
- abra o diretorio no terminal
- digite "pip install -r requirements.txt" (sem as aspas)
- peça a um coordenador para que acesse o drive pelo e-mail da coordenação e lhe envie o arquivo em Meu Drive -> Google API Tokens -> Gmail -> credentials.json
- salve esse arquivo na pasta do projeto
- abra o notebook
- faça uma planilha no google sheets com duas colunas, uma chamada "nome" e uma chamada "e-mail", apenas, e preencha com os dados das escolas a serem convidadas
- copie o link da planilha, fazendo a modificação no final como exemplificado abaixo:
    https://docs.google.com/spreadsheets/d/1QKThZF7CxoHhdp4HNj1gjJOb0YfsUj2BEeY0-2PlJi0/edit?gid=0#gid=0
    para
    https://docs.google.com/spreadsheets/d/1QKThZF7CxoHhdp4HNj1gjJOb0YfsUj2BEeY0-2PlJi0/export?format=csv&gid=0
    adicionando export?format=csv& ali no finalzinho antes de gid=0
- vá para a décima célula e copie o link na variável _filepath como string
- na célula abaixo, escreva a mensagem na variável email_body
- rode todas as células para realizar autenticação da conta google
- vá para a última célula, descomente o código e rode ela pra enviar os e-mails
