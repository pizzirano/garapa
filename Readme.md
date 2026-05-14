## Subindo listmonk para testes

## ainda inicial sem entrypoint.sh 

## executar comando para interface e acessar na 9000

docker run --rm \
  --network host \
  -e LISTMONK_db__host=localhost \
  -e LISTMONK_db__port=5432 \
  -e LISTMONK_db__user=admin \
  -e LISTMONK_db__password=admin123 \
  -e LISTMONK_db__database=newsletter \
  -e LISTMONK_db__ssl_mode=disable \
  listmonk/listmonk:v5.0.2 \
  ./listmonk --install --yes

## senha padrão user admin e senha listmonk 
