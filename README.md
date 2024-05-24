# CPNA-AWS-CheatSheet
CheatSheet del contenido de la certificación CPNA - AWS
# Terraform
## Instalación Terraform Linux
```bash
wget https://releases.hashicorp.com/terraform/1.1.9/terraform_1.1.9_linux_amd64.zip
```
```bash
unzip terraform_1.1.9_linux_amd64.zip
```
```bash
mv terraform /usr/local/bin/
```
## Despliegue Terraform Linux

> [!Note]
> Todos nuestros laboratorios requieren un usuario administrador para poder desplegar los diferentes componentes
```bash
terraform init
```
```bash
terraform apply
```

# Comandos CLI AWS
## Autenticación con AWS CLI

```bash
aws configure
```
Introducir valores para los campos requeridos.
```bash
AWS Access Key ID
AWS Secret Access Key
Default region name
Default output format
```
<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image.png)</kbd>

</details>

## Creación de perfiles con nombre
### Opción 1 - AWS CLI
```bash
aws configure --profile
```
### Opción 2 - Modificando archivos de configuración
Modificar el archivo:
<table><tr><td>config</td></tr></table>

<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-1.png)</kbd>

</details>

## Estructura comandos AWS CLI
```bash
aws <comando o servicio> <Sub-Comando> [Opciones y parámetros]
```
<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-2.png)</kbd>

</details>

## El whoami de AWS
### Opción 1
```bash
aws sts get-caller-identity
```
<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-3.png)</kbd>

</details>

### Opción 2 
> [!Note]
> Requiere privilegios iam:GetUser
```bash
aws iam get-user
```

<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-4.png)</kbd>

</details>

# Enumeración manual de IAM
## Enumerando usuarios
```bash
aws iam list-users
```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```

