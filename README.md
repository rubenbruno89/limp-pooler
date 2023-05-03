# limp-pooler

Este script em lote tem como objetivo limpar a fila de impressão do sistema Windows. 

A primeira linha do script interrompe o serviço Spooler, que é responsável pela administração de filas de impressão. A linha "pause" serve apenas para que o usuário possa ler a mensagem antes de continuar.

A segunda linha leva o usuário para a pasta de impressoras, que é o local onde os arquivos de impressão são armazenados. Novamente, há uma linha "pause" para permitir que o usuário leia a mensagem.

As próximas duas linhas removem os arquivos SHD e SPL, que são os arquivos de spool de impressão que podem causar problemas quando se acumulam na fila de impressão. A opção "/f" força a exclusão de arquivos de somente leitura, e "/s" remove os arquivos em todos os subdiretórios.

Por fim, a última linha inicia novamente o serviço Spooler. A fila de impressão agora estará limpa e pronta para receber novos trabalhos de impressão.
