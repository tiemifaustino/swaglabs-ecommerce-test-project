# Casos de teste

## Funcionalidade: Tela de login

<br>

| CT-01                | Realizando login com e-mail e senha válidos                                           |
| -------------------- | :------------------------------------------------------------------------------------ |
| Pré-condições        | Usuário tem acesso ao sistema                                                         |
| Passo a passo        | 1-Acessar tela de login (URL: https://www.saucedemo.com)                              |
|                      | 2-Inserir e-mail válido (`standard_user`)                                             |
|                      | 3-Inserir senha válida (`secret_sauce`)                                               |
|                      | 4-Clicar no botão 'Login'                                                             |
| Resultado esperado   | Usuário conecta com sucesso                                                           |
|                      | Usuário é redirecionado para a tela dos produtos                                      |
| Suite de teste       | Tela de login                                                                         |
| Ambiente de teste    | Web - Navegador Edge Versão 138.0.3351.55 (Compilação oficial) (64 bits) - Windows 11 |
| Resultado encontrado | O mesmo que o resultado esperado                                                      |
| Status               | ✅ Passou                                                                             |

<br>
<br>

| CT-02                | Realizando login com e-mail inválido e senha inválida                                         |
| -------------------- | :-------------------------------------------------------------------------------------------- |
| Pré-condições        | Usuário não tem acesso ao sistema                                                             |
| Passo a passo        | 1-Acessar tela de login (URL: https://www.saucedemo.com)                                      |
|                      | 2-Inserir e-mail inválido (`invalid_user`)                                                    |
|                      | 3-Inserir senha inválida (`invalid_password`)                                                 |
|                      | 4-Clicar no botão 'Login'                                                                     |
| Resultado esperado   | Mensagem de erro é exibida                                                                    |
|                      | Mensagem de erro: `Epic sadface: Username and password do not match any user in this service` |
| Suite de teste       | Tela de login                                                                                 |
| Ambiente de teste    | Web - Navegador Edge Versão 138.0.3351.55 (Compilação oficial) (64 bits) - Windows 11         |
| Resultado encontrado | O mesmo que o resultado esperado                                                              |
| Status               | ✅ Passou                                                                                     |

<br>
<br>

| CT-03                | Realizando login com e-mail inválido                                                          |
| -------------------- | :-------------------------------------------------------------------------------------------- |
| Pré-condições        | Usuário com e-mail inválido e senha existente                                                 |
| Passo a passo        | 1-Acessar tela de login (URL: https://www.saucedemo.com)                                      |
|                      | 2-Inserir e-mail inválido (`invalid_user`)                                                    |
|                      | 3-Inserir senha válida (`secret_sauce`)                                                       |
|                      | 4-Clicar no botão 'Login'                                                                     |
| Resultado esperado   | Mensagem de erro é exibida                                                                    |
|                      | Mensagem de erro: `Epic sadface: Username and password do not match any user in this service` |
| Suite de teste       | Tela de login                                                                                 |
| Ambiente de teste    | Web - Navegador Edge Versão 138.0.3351.55 (Compilação oficial) (64 bits) - Windows 11         |
| Resultado encontrado | O mesmo que o resultado esperado                                                              |
| Status               | ✅ Passou                                                                                     |

<br>
<br>

| CT-04                | Realizando login com senha inválida                                                           |
| -------------------- | :-------------------------------------------------------------------------------------------- |
| Pré-condições        | Usuário com e-mail válido e senha inválida                                                    |
| Passo a passo        | 1-Acessar tela de login (URL: https://www.saucedemo.com)                                      |
|                      | 2-Inserir e-mail válido (`standard_user`)                                                     |
|                      | 3-Inserir senha inválida (`invalid_password`)                                                 |
|                      | 4-Clicar no botão 'Login'                                                                     |
| Resultado esperado   | Mensagem de erro é exibida                                                                    |
|                      | Mensagem de erro: `Epic sadface: Username and password do not match any user in this service` |
| Suite de teste       | Tela de login                                                                                 |
| Ambiente de teste    | Web - Navegador Edge Versão 138.0.3351.55 (Compilação oficial) (64 bits) - Windows 11         |
| Resultado encontrado | O mesmo que o resultado esperado                                                              |
| Status               | ✅ Passou                                                                                     |

<br>
<br>

| CT-05                | Realizando login com campo de e-mail em branco e senha válida                         |
| -------------------- | :------------------------------------------------------------------------------------ |
| Pré-condições        | Usuário preenche somente o campo de senha com uma senha válida                        |
| Passo a passo        | 1-Acessar tela de login (URL: https://www.saucedemo.com)                              |
|                      | 2-Inserir senha válida (`secret_sauce`)                                               |
|                      | 3-Clicar no botão 'Login'                                                             |
| Resultado esperado   | Mensagem de erro é exibida                                                            |
|                      | Mensagem de erro: `Epic sadface: Username is required`                                |
| Suite de teste       | Tela de login                                                                         |
| Ambiente de teste    | Web - Navegador Edge Versão 138.0.3351.55 (Compilação oficial) (64 bits) - Windows 11 |
| Resultado encontrado | O mesmo que o resultado esperado                                                      |
| Status               | ✅ Passou                                                                             |

<br>
<br>

| CT-06                | Realizando login com e-mail válido e campo de senha em branco                         |
| -------------------- | :------------------------------------------------------------------------------------ |
| Pré-condições        | Usuário preenche somente o campo de e-mail com um e-mail válido                       |
| Passo a passo        | 1-Acessar tela de login (URL: https://www.saucedemo.com)                              |
|                      | 2-Inserir e-mail válido (`standard_user`)                                             |
|                      | 3-Clicar no botão 'Login'                                                             |
| Resultado esperado   | Mensagem de erro é exibida                                                            |
|                      | Mensagem de erro: `Epic sadface: Password is required`                                |
| Suite de teste       | Tela de login                                                                         |
| Ambiente de teste    | Web - Navegador Edge Versão 138.0.3351.55 (Compilação oficial) (64 bits) - Windows 11 |
| Resultado encontrado | O mesmo que o resultado esperado                                                      |
| Status               | ✅ Passou                                                                             |

<br>
<br>

| CT-07                | Realizando login com todos campos em branco                                           |
| -------------------- | :------------------------------------------------------------------------------------ |
| Pré-condições        | Usuário clica somente no botão 'Login'                                                |
| Passo a passo        | 1-Acessar tela de login (URL: https://www.saucedemo.com)                              |
|                      | 2-Clicar no botão 'Login'                                                             |
| Resultado esperado   | Mensagem de erro é exibida                                                            |
|                      | Mensagem de erro: `Epic sadface: Username is required`                                |
| Suite de teste       | Tela de login                                                                         |
| Ambiente de teste    | Web - Navegador Edge Versão 138.0.3351.55 (Compilação oficial) (64 bits) - Windows 11 |
| Resultado encontrado | O mesmo que o resultado esperado                                                      |
| Status               | ✅ Passou                                                                             |

<br>
<br>

| CT-08                | Realizando login com usuário bloqueado                                                |
| -------------------- | :------------------------------------------------------------------------------------ |
| Pré-condições        | Usuário está com o acesso bloqueado                                                   |
| Passo a passo        | 1-Acessar tela de login (URL: https://www.saucedemo.com)                              |
|                      | 2-Inserir e-mail (`locked_out_user`)                                                  |
|                      | 3-Inserir senha (`secret_sauce`)                                                      |
|                      | 4-Clicar no botão 'Login'                                                             |
| Resultado esperado   | Mensagem de erro é exibida                                                            |
|                      | Mensagem de erro: `Epic sadface: Sorry, this user has been locked out.`               |
| Suite de teste       | Tela de login                                                                         |
| Ambiente de teste    | Web - Navegador Edge Versão 138.0.3351.55 (Compilação oficial) (64 bits) - Windows 11 |
| Resultado encontrado | O mesmo que o resultado esperado                                                      |
| Status               | ✅ Passou                                                                             |
