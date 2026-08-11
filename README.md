# devops-netology

В репозитории настроены следующие игнорируемые файлы:

### Для Terraform:

| Правило из .gitignore | Что оно означает |
|------------------------|------------------|
| `.terraform/` | Игнорируется директории `.terraform` (и всё, что внутри) |
| `*.tfstate` | Игнорируются все файлы с расширением `.tfstate` |
| `*.tfstate.*` | Игнорируются все файлы, у которых есть расширение `.tfstate.` и после него что-то ещё (например, `.tfstate.backup`) |
| `crash.log` | Игнорируются файлы `crash.log` |
| `crash.*.log` | Игнорируются все файлы, которые начинаются с `crash.` и заканчиваются на `.log` (например, `crash.20260811.log`) |
| `*.tfvars` | Игнорируются все файлы с расширением `.tfvars` |
| `*.tfvars.json` | Игнорируются все файлы с расширением `.tfvars.json` |
| `override.tf` | Игнорируются файлы `override.tf` |
| `override.tf.json` | Игнорируются файлы `override.tf.json` |
| `*_override.tf` | Игнорируются все файлы, имя которых заканчивается на `_override.tf` |
| `*_override.tf.json` | Игнорируются все файлы, имя которых заканчивается на `_override.tf.json` |
| `.terraform.tfstate.lock.info` | Игнорируются файлы `.terraform.tfstate.lock.info` |
| `.terraformrc` | Игнорируется файлы `.terraformrc` |
| `terraform.rc` | Игнорируются файлы `terraform.rc` |