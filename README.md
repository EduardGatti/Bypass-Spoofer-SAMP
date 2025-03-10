# Bypass.exe

## Descrição

`Bypass.exe` é um script em batch que permite realizar uma série de operações de limpeza e manutenção no sistema Windows. Através de um menu interativo, o usuário pode escolher várias opções para excluir arquivos específicos de logs, histórico, cache e outros arquivos temporários que podem acumular no sistema. Ele também fornece a opção de apagar completamente os rastros de atividades, incluindo histórico de navegação no Chrome, Firefox, e arquivos relacionados ao sistema operacional.

Este script é destinado a usuários avançados que desejam limpar dados e liberar espaço de maneira eficiente no sistema. No entanto, o uso inadequado deste script pode resultar em perda de dados importantes ou configurações do sistema, então deve ser utilizado com cuidado.

**Importante**: O script oferece um mecanismo de autenticação de login, e após um número limitado de tentativas falhas, o próprio script será apagado automaticamente, como uma medida de segurança.

## Funcionalidades

- **Login**: O script requer um login para acesso às funcionalidades. Caso o login seja errado por três vezes consecutivas, o script será apagado.
- **Limpeza de Arquivos**:
  - **LogBag**: Limpa logs de WMI (Windows Management Instrumentation).
  - **Logs do Sistema**: Apaga logs do sistema que ficam armazenados em `C:\Windows\System32\winevt\Logs`.
  - **ShallBag**: Limpa arquivos temporários do sistema em `C:\Windows\Temp`.
  - **Prefetch**: Limpa arquivos de prefetch que são utilizados para acelerar a inicialização de programas.
  - **Journal**: Limpa a lixeira do sistema (`C:\$Recycle.Bin`).
  - **Histórico do Chrome**: Limpa o histórico de navegação do Google Chrome.
  - **Histórico de Downloads do Chrome**: Limpa o histórico de downloads do Chrome.
  - **Arquivos de Atualização do Windows**: Remove arquivos de atualizações baixados em `C:\Windows\SoftwareDistribution\Download`.
  - **Cache do Sistema**: Limpa o cache de sistema em `C:\Windows\System32\catroot`.
  - **Histórico do Firefox**: Limpa o histórico e dados relacionados do Firefox.
  - **Lixeira**: Limpa a lixeira do sistema.
- **Reinício do Explorer**: Reinicia o processo `explorer.exe` para aplicar as mudanças feitas no sistema.
- **Apagar Script**: Oferece a opção de excluir o próprio script após a execução, garantindo que não deixe rastros.

## Como Usar

1. **Baixe o script** para seu computador.
2. **Execute o arquivo** em um prompt de comando no Windows.
3. **Autentique-se** fornecendo um nome de usuário e senha definidos no código.
4. Após a autenticação bem-sucedida, você verá um menu com várias opções. Digite o número da opção desejada para executar a ação.
5. **Confirme as operações** que deseja realizar, como limpar históricos, arquivos temporários ou reiniciar o sistema.

**Nota**: Sempre execute o script com privilégios de administrador para garantir que ele possa acessar as pastas e arquivos do sistema.

## Aviso

- O script contém uma série de ações que podem apagar permanentemente dados. Certifique-se de que você não está apagando informações importantes antes de proceder.
- Use com cautela em ambientes corporativos, pois a limpeza de certos arquivos pode afetar a performance ou configurar arquivos críticos do sistema.

## Tabela de Comandos

| Opção | Descrição |
|-------|-----------|
| 1     | Limpar LogBag (Logs WMI) |
| 2     | Limpar Logs do Sistema |
| 3     | Limpar ShallBag (Arquivos Temporários) |
| 4     | Limpar Prefetch |
| 5     | Limpar Journal (Lixeira) |
| 6     | Limpar Histórico do Google Chrome |
| 7     | Limpar Histórico de Downloads do Chrome |
| 8     | Limpar Tudo (executa todas as limpezas) |
| 9     | Excluir Arquivo Específico |
| 10    | Limpar Arquivos de Atualização do Windows |
| 11    | Limpar Lixeira |
| 12    | Limpar Cache do Sistema |
| 13    | Abrir Limpeza de Dados do Chrome |
| 14    | Limpar Histórico do Firefox |
| 15    | Reiniciar o explorer.exe |
| 0     | Sair e apagar o script |

# Spoofer (Manipulação de Rede)

## Descrição

O **Spoofer** é uma parte do script que oferece funcionalidades avançadas de manipulação de rede, permitindo que o usuário altere configurações como proxy, obtenha um novo IP, libere e renove o endereço IP, e outras operações úteis para controlar a rede do sistema Windows.

## Funcionalidades

- **Proxy IP**: Configura o sistema para usar um proxy local (127.0.0.1:8080).
- **Novo IP**: Renova o endereço IP da interface de rede atual, liberando e renovando a configuração de rede.
- **DHCP**: Configura a interface de rede para usar DHCP, permitindo que o IP seja obtido automaticamente.
- **Rede Info**: Exibe informações detalhadas sobre a rede, como IP, máscara de sub-rede, gateway, etc.
- **Flush DNS**: Limpa o cache DNS do sistema, forçando a atualização dos registros DNS.

## Instruções de Uso

1. **Menu de Operações**:
   - Após o login e a autenticação com o código OTP, o script exibe um menu de opções para manipulação de rede. As opções disponíveis são:
     - **1**: Configurar Proxy IP
     - **2**: Renovar IP
     - **3**: Ativar DHCP
     - **4**: Exibir Informações de Rede
     - **5**: Limpar Cache DNS
     - **0**: Sair do Script

2. **Configurações de Proxy IP**:
   - Ao selecionar a opção **1**, o script configura o sistema para usar o proxy local `127.0.0.1:8080`.

3. **Renovação de IP**:
   - Ao selecionar a opção **2**, o script libera e renova o IP da interface de rede atual.

4. **Ativar DHCP**:
   - Ao selecionar a opção **3**, o script configura a interface de rede para obter um IP automaticamente via DHCP.

5. **Exibir Informações de Rede**:
   - A opção **4** exibe informações detalhadas sobre o estado atual da rede, incluindo o endereço IP, gateway, máscara de sub-rede, etc.

6. **Limpar Cache DNS**:
   - A opção **5** limpa o cache DNS do sistema, o que pode ser útil para resolver problemas de conexão e forçar o sistema a buscar novos registros DNS.

## Exemplo de Uso

1. **Escolha de Comando**:
   - Após a autenticação, o script exibe um menu. O usuário pode escolher uma das opções para manipulação de rede.

2. **Renovação de IP**:
   - Se você deseja renovar o IP, basta selecionar a opção **2**. O script liberará e renovará o IP automaticamente.

3. **Configuração de Proxy**:
   - Se você deseja configurar um proxy, selecione a opção **1**. O script configurará o proxy local no sistema para `127.0.0.1:8080`.

## Observações Importantes

- **Permissões**: O script exige permissões de **Administrador** para modificar configurações de rede e enviar comandos de sistema.
- **Uso Responsável**: Certifique-se de usar o script de maneira ética e responsável, especialmente ao realizar alterações de rede como configuração de proxy ou renovação de IP.


## Como Contribuir

Este repositório foi criado para fins educacionais e para aqueles que desejam automatizar a limpeza do sistema Windows. Se você encontrar melhorias ou quiser adicionar mais funcionalidades, sinta-se à vontade para criar um **pull request** com suas sugestões.

## Licença

Este projeto é de código aberto. Use-o por sua conta e risco. O autor não se responsabiliza por danos ou problemas causados pelo uso deste script.
