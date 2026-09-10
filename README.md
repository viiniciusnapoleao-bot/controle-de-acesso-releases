# Controle de Acesso — Releases

Repositório de **distribuição**. Contém apenas os instaladores publicados em
[Releases](../../releases) — nenhum código-fonte.

O aplicativo consulta este repositório para verificar atualizações
(ver `updater.py`). Cada release publica um instalador por variante:

| Arquivo | Produto |
| --- | --- |
| `ControleAcesso_Installer-<versão>.exe` | Academia (com catraca e biometria) |
| `ControleAcessoPersonal_Installer-<versão>.exe` | Personal |

O `.sha256` ao lado de cada executável é conferido pelo próprio app na
inicialização, e o updater valida o hash do arquivo baixado antes de executá-lo.
