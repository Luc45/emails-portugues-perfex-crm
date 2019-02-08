# emails-portugues-perfex-crm
Emails em português para o PERFEX CRM

### Observaçoes:
- "Tickets" são chamados de "Solicitações"
- "Discussões" são chamados de "Conversas"

### Falta traduzir emails relativos à:
- Contratos
- Assinaturas
- Propostas
- Colaboradores

### Instalação:

1. Faça um backup do seu banco de dados. SÉRIO!
2. Acesse o seu banco de dados com PHPMyAdmin ou similar, procure pelos emails em português do Brasil:

`SELECT * FROM `tblemailtemplates` WHERE `language` LIKE 'portuguese_br'`

3. Delete todos os resultados encontrados (se você usar PERFEX CRM maior que a versão 2.2.0, verifique se não foi adicionado nenhum email novo)
4. Insira os novos emails que estão no arquivo SQL deste repositório, executando ele como um comando SQL
5. Acesse seu Perfex -> Configurações -> Modelos de Email e clique em algum para ver se funcionou.
