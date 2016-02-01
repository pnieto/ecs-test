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
