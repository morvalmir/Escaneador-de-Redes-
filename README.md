# Escaneador-de-Redes-

## Descrição

O **Escaneador-de-Redes-** é um script em Batch para Windows que realiza o escaneamento da rede local utilizando requisições ICMP (ping), permitindo detectar quais hosts estão ativos na mesma faixa de IP.

## Funcionalidades

- Varredura automática de IPs na rede local.
- Detecção rápida de hosts ativos via resposta ao ping.
- Exibição dos endereços IP encontrados diretamente no terminal.
- Possibilidade de identificação de fabricante, nome do Host e nome do usuário logado.
- Fácil execução em sistemas Windows, sem necessidade de instalar programas adicionais.

## Pré-requisitos

- Sistema operacional Windows (validação a partir do Windows 10/11).
- Permissões para executar comandos de linha de comando e enviar pings na rede.
- Script `ScanLocal.bat` disponível no repositório.

## Instalação

1. Baixe o arquivo `ScanLocal.bat` do repositório:
   - [Download direto](https://raw.githubusercontent.com/morvalmir/Escaneador-de-Redes-/refs/heads/main/ScanLocal.bat)

2. Salve o arquivo em uma pasta de sua preferência.

## Como usar

1. Abra o Prompt de Comando (cmd) do Windows.

2. Navegue até a pasta onde o script foi salvo:
   ```cmd
   cd caminho\para\a\pasta
   ```

3. Execute o script:
   ```cmd
   ScanLocal.bat
   ```
   ou
   ```
   ScanLocal.bat 10.1.1.0
   ```

4. O script irá escanear a faixa de IP (/24) configurada e mostrar quais hosts estão ativos.

## Exemplo de Saída

```
 REDE SCAN                                                                                                valmir.morais
 ‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾

   Endereço IPV4      MAC                  Fabricante              Nome do Host            Usuário
   ˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉ    ˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉ    ˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉ    ˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉ    ˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉˉ
      192.168.1.73    00-D7-6D-29-9E-83    Intel Corporate         Valmir-nt               Valmir
      192.168.1.64    b6-ec-d8-4c-7e-d3    ********************    ********************    *************************
      192.168.1.66    92-a2-0d-53-d9-f1    ********************    ********************    *************************
      192.168.1.69    46-e4-5e-30-2f-68    ********************    ********************    *************************
      192.168.1.74    ea-a2-95-59-01-74    ********************    ********************    *************************
     192.168.1.254    cc-ed-21-84-fb-40    Nokia Shanghai Bell     dsldevice               *************************


                                                    FINALIZADO!
 ‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾‾
 Tempo total de execução: 00:35,724
```

## Observações

- O escaneamento pode ser limitado por regras de firewall locais ou na rede.
- Utilize o script apenas em redes onde você tem autorização para realizar testes.
- O script foi desenvolvido para fins educacionais e administrativos.

## Licença

Este projeto está sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para mais informações.

## Autor

Morvalmir (Valmir Morais)
[GitHub](https://github.com/morvalmir)
