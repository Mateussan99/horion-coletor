# Coletor Horion

Instalador do **Coletor Horion**, o programa que roda no computador do cliente, lê as batidas dos relógios de ponto e envia para o HORION.

Este repositório só hospeda os arquivos para baixar. O código do HORION é privado.

## Baixar

[**Baixar o instalador mais recente**](https://github.com/Mateussan99/horion-coletor/releases/latest/download/ColetorHorion-Setup.exe)

Todas as versões estão em [Releases](https://github.com/Mateussan99/horion-coletor/releases).

## Instalar

1. Execute `ColetorHorion-Setup.exe` em um computador Windows ligado à mesma rede dos relógios.
2. Siga o assistente. O coletor é instalado como serviço do Windows e inicia sozinho.
3. No HORION, abra **Configurações › Relógios** para cadastrar os relógios e ativar o coletor.

## Conferir o arquivo

Cada release publica o SHA-256 do instalador nas notas. Para conferir no PowerShell:

```powershell
Get-FileHash .\ColetorHorion-Setup.exe -Algorithm SHA256
```

## Atualizações

O coletor se atualiza sozinho: ele consulta um manifesto assinado e só aceita pacote com assinatura válida. Não é preciso baixar o instalador de novo.
