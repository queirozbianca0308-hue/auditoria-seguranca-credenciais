# Auditoria de Segurança de Credenciais em Laboratório

## 1. Apresentação

Este projeto reúne um estudo introdutório sobre segurança de credenciais, autenticação e serviços de rede. O conteúdo acompanha os temas apresentados no desafio da DIO sobre Kali Linux, Medusa e Metasploitable 2.

**Importante:** este repositório documenta conceitos e um roteiro de estudo. Ele não afirma que testes práticos foram executados. Qualquer atividade prática deve ocorrer somente em laboratório próprio, isolado e com autorização.

## 2. Objetivos

- Entender riscos associados a senhas fracas ou reutilizadas.
- Diferenciar Password Spraying, Credential Stuffing e força bruta.
- Conhecer ferramentas de auditoria presentes no Kali Linux.
- Compreender, em nível conceitual, a enumeração de serviços SMB.
- Identificar medidas para reduzir riscos de acesso não autorizado.

## 3. Conceitos estudados

### Password Spraying

É uma técnica de tentativa de autenticação que testa uma senha comum em várias contas. Ela pode ser detectada por monitoramento de autenticação e políticas de bloqueio ou limitação de tentativas.

### Credential Stuffing

Consiste no uso de pares de usuário e senha expostos em incidentes anteriores para tentar acessar outros serviços. A reutilização de senhas aumenta esse risco.

### Ataques de força bruta

São tentativas sistemáticas de descobrir credenciais por meio de várias combinações. Controles como limitação de tentativas, MFA e senhas fortes ajudam a reduzir esse risco.

### Wordlists

São listas de palavras ou valores usadas em atividades de auditoria. Seu uso deve ser restrito a ambientes de teste autorizados.

### SMB e enumeração

SMB é um protocolo utilizado para compartilhamento de arquivos e recursos em redes. A enumeração consiste em identificar informações que um serviço disponibiliza. Compartilhamentos e permissões devem ser configurados com privilégio mínimo.

## 4. Ferramentas mencionadas no desafio

| Ferramenta | Finalidade geral |
|---|---|
| Kali Linux | Distribuição Linux voltada a testes e estudos de segurança. |
| Hydra | Ferramenta de auditoria de autenticação em serviços de rede. |
| Ncrack | Ferramenta de avaliação de autenticação em serviços de rede. |
| John the Ripper | Ferramenta de auditoria de resistência de senhas. |
| WPScan | Ferramenta de avaliação de segurança de sites WordPress. |
| Medusa | Ferramenta de auditoria de autenticação. |
| Metasploitable 2 | Máquina virtual intencionalmente vulnerável para treinamento em laboratório. |
| SMBClient | Cliente para interagir com compartilhamentos SMB. |

## 5. Ambiente de estudo

O desafio apresenta o uso de Kali Linux e Metasploitable 2 em um ambiente de laboratório. A máquina vulnerável deve permanecer isolada de redes públicas e ser utilizada apenas pelo responsável pelo laboratório ou com autorização expressa.

Este documento não registra resultados de execução, evidências ou credenciais. Esses itens só devem ser adicionados após a realização legítima das atividades e a coleta de evidências reais, sem expor senhas ou dados pessoais.

## 6. Riscos identificados

- Senhas curtas, previsíveis ou reutilizadas.
- Ausência de autenticação multifator.
- Tentativas de login sem limitação ou monitoramento.
- Serviços de rede expostos sem necessidade.
- Compartilhamentos com permissões excessivas.
- Sistemas desatualizados ou mal configurados.

## 7. Recomendações de segurança

1. Utilizar senhas longas, únicas e armazenadas em um gerenciador confiável.
2. Ativar autenticação multifator sempre que possível.
3. Aplicar limitação de tentativas e alertas para logins suspeitos.
4. Desabilitar serviços que não sejam necessários.
5. Restringir SMB às redes e aos usuários autorizados.
6. Aplicar atualizações de segurança.
7. Revisar permissões e adotar o princípio do menor privilégio.
8. Nunca reutilizar senhas entre serviços.

## 8. Conclusão

O estudo dos ataques contra credenciais mostra que a segurança depende de controles técnicos e de hábitos responsáveis. Senhas únicas, MFA, monitoramento, atualização dos sistemas e configuração adequada dos serviços reduzem a possibilidade de acessos indevidos.

A prática de auditoria deve ser ética, autorizada e limitada a ambientes controlados.

## 9. Registro de execução

Preencher esta seção somente depois de realizar as atividades no laboratório:

- **Ambiente utilizado:** [preencher]
- **Atividades realmente realizadas:** [preencher]
- **Resultados observados:** [preencher sem incluir senhas ou dados sensíveis]
- **Medidas de proteção propostas:** [preencher]

Se uma atividade não foi realizada, registrar isso claramente em vez de inventar resultados.

## 10. Referências para estudo

- Documentação oficial do Kali Linux: https://www.kali.org/docs/
- Projeto Metasploitable 2 (Rapid7): https://docs.rapid7.com/metasploit/metasploitable-2/
- OWASP Authentication Cheat Sheet: https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html
