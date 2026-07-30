# Automatic-Download-Cadernetas-Prediais---ADCP
Programa para fazer o download automático das Cadernetas Prediais no Portal das Finanças. É preciso Python, o ADCP  abre o browser no portal e as credenciais do Portal das Finanças são inseridas no browser e não no programa, faz uma checklist da listagem, e faz o download atribuindo o respetivo nome correto, e percorrendo todas as paginas.

Notas: 
Instalar o python.
Necessário ter o nif e password do portal das finanças para se fazer o login.
Fazer o download no portal das finanças da listagem dos itens prediais.

1 - Unzip a pasta cadernetas_prediais_autonomo_v6 para a pasta das transferências.

2 - Colocar dentro da pasta que foi unzip o ficheiro excel csv descarregado do portal das finanças, com a listagem dos itens prediais ( patrimonio_predial.csv )

3 - Dentro dessa pasta, na barra de caminho escrever powershell para abrir o powershell dentro da pasta e executar estes comandos:


python -m pip install selenium

 A seguir este comando:

python .\cadernetas_prediais_autonomo_v6.py --csv .\patrimonio_predial.csv --downloads "$env:USERPROFILE\Downloads" --saida .\Cadernetas --saltar-existentes


4 - Seguir as instruções, fazer login no portal das finanças no google chrome que vai abrir, escrever predial na barra pesquisa dentro do portal das finanças e  clicar em aceder.


 No final, pode-se consultar Cadernetas\log_cadernetas_autonomo_v6.csv para verificar se esta OK ou com algum erro.


RF
