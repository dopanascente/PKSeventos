# PKS Gestão — Estruturas & Eventos

Aplicação administrativa local em HTML, CSS e JavaScript, sem servidor e sem dependências externas.

## Como abrir
1. Extraia a pasta `PKS_Painel_Gestao`.
2. Abra `index.html` com duplo clique no Chrome ou Edge.
3. Os dados são guardados no `localStorage` do navegador e não sincronizam entre computadores.

## Funcionalidades implementadas
- Painel com indicadores, caixa, eventos futuros, pendências e gráfico de entradas/saídas.
- Tela Hoje com eventos de hoje/amanhã, atalhos de telefone, WhatsApp e mapas.
- Agenda mensal com criação de eventos por data.
- Cadastro, edição e exclusão de clientes, itens de catálogo, eventos, lançamentos financeiros, fornecedores e equipe.
- Itens de evento com cálculo de preço, custo previsto e alerta de conflito de estoque.
- Orçamentos copiáveis, impressão/PDF pelo navegador e abertura manual do WhatsApp.
- Modelo básico de contrato com campos `[definir]` para revisar.
- Geração de cobranças de sinal e restante.
- Financeiro com marcação de pago/reabertura, vencidos, categorias e exportação CSV.
- Busca global com Ctrl+K, tema escuro/claro, backup/restauração JSON e dados de demonstração.
- Layout adaptável a desktop e celular.

## Backup
Abra **Configurações → Baixar backup JSON** regularmente. Para restaurar, selecione um arquivo JSON exportado por este sistema. A restauração substitui os dados atuais.

## Limitações conhecidas desta versão
- Não há sincronização entre dispositivos, login, backend ou envio automático de mensagens.
- Comprovantes de imagem/PDF em IndexedDB, paginação completa, testes automatizados Playwright, gráficos avançados e suporte detalhado a contratos ainda precisam de uma etapa adicional.
- O teste automatizado de `file://` varia conforme navegador; faça uma revisão manual antes de usar em produção.
- O contrato é apenas um modelo administrativo e deve ser revisado antes de utilização.
- O navegador pode apagar os dados locais; mantenha cópias de backup externas.

## Estrutura
- `index.html`: página e navegação.
- `css/styles.css`: temas, layout, tabelas, formulários e responsividade.
- `js/app.js`: armazenamento local, regras de negócio e telas.
- `tests/`: reservado para testes futuros.
