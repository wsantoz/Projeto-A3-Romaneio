<p align="center"><img src="mascote.png" alt="Malu Sinal, mascote do Grupo 5" width="260"></p>

# Malu Sinal, a vaca-semáforo

A Malu acende verde, amarelo ou vermelho antes da mistura, os mesmos três resultados da coleta (liberada, liberada com rebaixamento e bloqueada), para o motorista saber na hora se pode seguir.

> "Eu cuido do sinal, você cuida da entrega!"

---

# Romaneio e validação de carga

A3 de Projeto e Engenharia de Software · **Grupo 5**

Especificação de um sistema que avisa o motorista, antes da coleta, quando o leite de uma fazenda não pode ser misturado ao da carga. Este trabalho é o projeto do sistema (problema, requisitos, desenhos e painel). Não tem código.

## O problema

- O caminhão de leite tem **um compartimento só**, então tudo o que entra se mistura.
- **Búfala com vaca:** a carga inteira é descartada.
- **Orgânico com convencional:** o orgânico perde o prêmio e é pago como convencional.
- A rota vai impressa em papel. Se uma fazenda mudou de classe, o motorista não sabe e só descobre o erro na portaria do laticínio, com o caminhão cheio.

## O que o sistema faz

1. Monta a rota do dia, com os pontos em ordem.
2. Bloqueia a coleta que não pode ser misturada.
3. Registra o que foi bloqueado e por quê.

## Números da base de dados

Seis meses de dados fictícios (01/09/2025 a 28/02/2026): 40 fazendas e 1.092 coletas.

- 36 coletas bloqueadas (49.742 litros)
- 28 coletas liberadas com rebaixamento (39.488 litros)
- 64 coletas com problema, 5,9% do total

## O que tem neste repositório

| Arquivo | O que é |
|---|---|
| [relatorio.md](relatorio.md) | Relatório em PDCA: problema, Ishikawa, SWOT, requisitos, diagramas e painel |
| [diagramas/](diagramas/) | Ishikawa, casos de uso e classes (imagens) |
| relatorio.pbix | Painel feito no Power BI Desktop |
| relatorio.pdf | O mesmo painel exportado, para quem não tem o Power BI |
| [base/](base/) | Arquivos de dados: `fazendas.csv` e `romaneio.csv` |
| mascote.png | A Malu |

## Como ver o painel

- **Sem o Power BI:** abra o `relatorio.pdf`.
- **Com o Power BI Desktop:** abra o `relatorio.pbix`. As duas tabelas de `base/` já estão ligadas pela coluna `fazenda_id`.

## Integrantes

- Warley Rocha Santos
- Kauã Gabriel Lopes Catrinck
- João Victor de Melo Costa
- Marcus de Moraes Oliveira
