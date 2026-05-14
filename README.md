# Monitoramento de Jornada · Gran Hortifruti + GRSM

> 🔒 **Uso interno · Confidencial.** Acesso restrito a gestores autorizados do Grupo A7. Não compartilhar fora do escopo de RH e gestão de loja.

Sistema interno de monitoramento semanal de jornada de trabalho para colaboradores das empresas Gran Hortifruti e GRSM (Grupo A7).

## Acesso ao relatório

[**Abrir relatório atual (S20/2026)**](https://grupoa7.github.io/gran-rh-monitoramento/)

## O que é

Relatório executivo gerado toda quarta-feira que cruza:
- **Batidas reais** do RHID Control iD
- **Escala mensal** dos colaboradores
- **Afastamentos** registrados

E aplica regras de negócio para detectar inconsistências, problemas técnicos de ponto e padrões comportamentais.

## Estrutura do relatório

### Aba 01 — Histórico & Tendência
KPIs cumulativos · gráfico de tendência · tabela semana a semana · heatmap multi-semana · top reincidentes · tornado piora/melhora.

### Aba 02 — Panorama da semana
KPIs e tabela com status atual de cada colaborador.

### Aba 03 — Detalhe diário
Tabela espelhando a escala. Cada célula tem previsto/bateu/alertas.

### Aba 04 — Tratativa RH
Casos sob responsabilidade da Consultora RH (falha biométrica suspeita, batidas a corrigir, convocação extraordinária). Acompanhamento de status pra medir desempenho.

## Regras aplicadas

1. **Atraso de entrada** > 10 min → alerta
2. **Saída antecipada** > 10 min → alerta
3. **Intervalo fora da faixa** 1h-1h05 → alerta
4. **Janela proibida** (descanso em horário de pico):
   - 16h-19:30 → todos os dias úteis em setores restritos
   - 11h-13h → só sábado, domingo e feriado nacional
5. **Pulou intervalo + jornada > 6h** → crítico (CLT)
6. **Falta seca** sem justificativa → crítico

Setores restritos: Encarregados, Operador de Loja, Operador de Caixas.

## Heurísticas do detector de suspeitos

- **REG-S1/S6** Falta excessiva → Tratativa RH (investigação biométrica)
- **REG-S2** Batida única isolada → confirmar com gestor + ajuste manual
- **REG-S3** Batidas ímpares (3 ou 5) → esquecimento típico
- **REG-S4** Trabalhou em folga → confirmar convocação

## Atualização

Toda **quarta-feira de manhã**. Próxima rodada: 20/05/2026.

---

Projeto interno do **Grupo A7** · Gran Hortifruti + GRSM · Salvador/BA
