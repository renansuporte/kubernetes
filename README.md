# kubernetes
Atividade de kubernetes
-- Arquivo de configuração dev-configmap.yml

Segue abaixo as váriaveis de ambiente. 
  MYSQL_ROOT_PASSWORD: q1w2e3r4 
  MYSQL_DATABASE: empresa
  MYSQL_PASSWORD: q1w2e3r4

-- Arquivo pod-mysql.yml 
Contém a configuração do pod e também o tipo do service para expor o cluster para o mundo externo. 

-- Arquivo pod-servico-nginx.yml 
Contém a configuração do pod e também o tipo do service para expor o cluster para o mundo externo. 

Exemplo de como testar a comunicação externa 
Teste MySQL: 
mysql -uroot -pq1w2e3r4 --host=<SEU IP> --port=30005

Teste serviço NGINX 
 curl 192.168.99.100:30006
