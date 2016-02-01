### ecs-test
Proyecto de pruebas Amazon ECS

### Instalación ecs-cli
* Listamos las zonas disponibles en Amazon
```bash
ec2-describe-regions
```
* Configuramos zona deseada, clave de acceso al API y creamos un nuevo cluster:
```bash
ecs-cli configure --region eu-west-1 --access-key $AWS_ACCESS_KEY --secret-key $AWS_SECRET_KEY --cluster demo-contenedores
```
* Configuramos clave de acceso
```bash
ec2-import-keypair pnieto --public-key-file $path_public_key
````
* Arrancamos instacia contenedores
```bash
ecs-cli up --keypair pnieto --capability-iam --size 2 --instance-type t2.micro
```
