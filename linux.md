# Descompactar arquivos .tar.gz
- tar xzf file.tar.gz
- tar xzvf file.tar.gz (para acompanhar o processo de extração)

# Instalar aquivos .sh
- chmod +x nomeDoArquivo.sh
- ./nomeDoArquivo.sh

# Excluir um arquivo
- rm /home/danilo/arquivo.txt

#Aumentar velocidade do Mouse
- xset m 2 1

# Alterrar o nome do diretório
- mv /home/danilo/vhosts/nome-do-projeto /home/danilo/vhosts/novo-nome

# Verificar os processos que estão abertos na porta 80/TCP
- sudo fuser -v 80/tcp
- sudo fuser -n tcp 8000

# Matar o processo aberto em determinada porta
- kill -9 "PID_NUMBER"

# Remover todos os diretórios e subdiretórios, com seu conteúdo
- rm -rf /home/data/2000

# Visualizar o conteúdo de um arquivo diretamente no terminal
- cat nomeDoArquivo.extensao
