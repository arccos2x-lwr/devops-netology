# devops-netology

В репозитории настроены следующие игнорируемые файлы:

### Для Terraform:
- Локальные каталоги `.terraform/`
- Файлы состояний (`*.tfstate`, `*.tfstate.*`)
- Файлы журналов (`crash.log`, `crash.*.log`)
- Файлы переменных (`*.tfvars`, `*.tfvars.json`)
- Файлы переопределений (`override.tf`, `override.tf.json`, `*_override.tf`, `*_override.tf.json`)
- Файлы конфигурации CLI (`.terraformrc`, `terraform.rc`)