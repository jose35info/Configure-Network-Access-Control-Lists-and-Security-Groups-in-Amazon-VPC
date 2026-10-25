# Aprendizados e checklist de testes

## Checklist antes de testar

- [ ] Confirmar a sub-rede associada a cada Network ACL.
- [ ] Conferir as regras de entrada e saída, prioridades e regra final `*`.
- [ ] Conferir as regras de entrada e saída dos Security Groups.
- [ ] Conferir tabelas de rotas e Internet Gateway.
- [ ] Confirmar portas e protocolos necessários para o teste.
- [ ] Não usar regras abertas além do necessário.

## Registro de testes

Para cada teste, preencher:

| Data/hora | Origem | Destino | Protocolo/porta | Resultado | Hipótese/observação |
|---|---|---|---|---|---|
| | | | | | |

## Conceito-chave

- Security Group = stateful: permite automaticamente o tráfego de resposta de uma conexão permitida.
- Network ACL = stateless: avalia entrada e saída separadamente; as regras devem permitir os fluxos necessários em ambos os sentidos.

Uma falha de conectividade não deve ser atribuída automaticamente à ACL. Verifique também Security Groups, rotas, endereçamento, DNS e o serviço de destino.
