# Bug Report

## Funcionalidade: Tela de Produtos

<br>

| BR-01                  | Não é possível ordenar produtos em ordem alfabética decrescente                                                            |
| ---------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| Pré-condições          | Usuário está autenticado (logado) no sistema com o usuário `problem_user` e senha `secret_sauce`                           |
| Passos para reprodução | 1-Acessar tela de produtos (URL: https://www.saucedemo.com/inventory.html)                                                 |
|                        | 2-Clicar no campo de seleção no canto superior à direita                                                                   |
|                        | 3-Clicar na opção `Name (Z to A)`                                                                                          |
| Resultado esperado     | Produtos ficam ordenados em ordem alfabética decrescente                                                                   |
| Resultado encontrado   | Ao selecionar a opção `Name (Z to A)` é selecionada a opção `Name (A to Z)`e produtos ficam em ordem alfabética ascendente |
| Ambiente de teste      | Web - Navegador Edge Versão 138.0.3351.55 (Compilação oficial) (64 bits) - Windows 11                                      |
| Prioridade             | Alta                                                                                                                       |
| Tipo                   | Funcional                                                                                                                  |
| Evidência              | <img src="../evidencias/CT-09.gif" width="800">                                                                            |
