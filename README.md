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
> Requiere privilegios <strong>iam:GetUser</strong>
```bash
aws iam get-user
```

<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-4.png)</kbd>

</details>

# Enumeración manual de IAM
## Enumerando usuarios
### Enumerando todos los usuarios exitentes en la cuenta AWS 
```bash
aws iam list-users
```
<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-5.png)</kbd>

</details>

### Enumerando todos los grupos a los que pertenece un usuario especifico 

```bash
aws iam list-groups-for-user --user-name Usuario
```
<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-6.png)</kbd>

</details>

### Enumerando información de las llaves públicas SSH de un usuario especifico
```bash
aws iam list-ssh-public-keys --user-name Usuario
```
<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-7.png)</kbd>

</details>

```bash
aws iam get-ssh-public-key --user-name Usuario -- encoding PEM --ssh-public-key-id ID
```
<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-8.png)</kbd>

</details>

### Enumerando certificados de firma asociados a un usuario especifico
```bash
aws iam list-signing-certificates --user-name Usuario
```
<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-9.png)</kbd>

</details>

### Enumerando dispositivos MFA virtuales de la cuenta de AWS

```bash
aws iam list-virtual-mfa-devices
```
<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-10.png)</kbd>

</details>

### Enumerando politicas gestionadas aplicadas a un usuario especifico
```bash
aws iam list-attached-user-policies --user-name Usuario
```
<details>
  <summary>Ejemplo:</summary>

  <kbd>![alt text](image-11.png)</kbd>

</details>

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
<details>
  <summary>Ejemplo:</summary>

  <kbd></kbd>

</details>

<details>
  <summary>Ejemplo:</summary>

  <kbd></kbd>

</details>

<details>
  <summary>Ejemplo:</summary>

  <kbd></kbd>

</details>

<details>
  <summary>Ejemplo:</summary>

  <kbd></kbd>

</details>

<details>
  <summary>Ejemplo:</summary>

  <kbd></kbd>

</details>
