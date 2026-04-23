# Modalidade Passe e Bate

## Status
Proposed

## Problema
A inclusão da baratada como vitória imediata cria incentivos para jogo artificial:

- Jogadores podem passar intencionalmente para tentar encaixar a 0-0 no final  
- A vitória pode ocorrer sem consistência estratégica ao longo da rodada  

Isso reduz o mérito tático e aumenta comportamentos exploratórios.

## Proposta
Definir a modalidade “Passe e Bate” com as seguintes regras:

- Jogo em duplas  
- Sem compra de peças (jogador passa se não puder jogar)  

- Se uma dupla vencer a primeira rodada jogando a peça 0-0 (barata):
  - A partida termina imediatamente (baratada)  

- Cláusula de validação:
  - A baratada só é válida se a dupla vencedora não tiver passado nenhuma vez na rodada  

- Caso não ocorra baratada:
  - Vence a dupla que alcançar 4 vitórias em rodadas  

## Impacto

**Duração média da partida:**  
Variável, com redução de finais abruptos injustificados  

**Complexidade estratégica:**  
Moderada → Alta na 1ª rodada (maior exigência de consistência)  

**Potencial de discussão:**  
Moderado (critério claro, mas sujeito a atenção da mesa)  

**Risco de virar mesa:**  
Moderado (especialmente em disputas sobre “passou ou não passou”)  

## Compatibilidade

- Mantém a estrutura base do dominó em duplas  
- Modifica a condição de vitória especial (baratada)  
- Introduz uma restrição comportamental inexistente no modelo clássico  

---

## ⚖️ Observação crítica (vale decidir antes de “aprovar”)

Essa cláusula resolve o problema mais óbvio, mas cria outro mais sutil:

### 👉 Rastreabilidade
- A mesa precisa lembrar se alguém da dupla passou  
- Em jogos informais, isso pode gerar dúvida ou discussão  

### 🔧 Possível refinamento futuro

Se isso virar problema real:

> “A dupla perde automaticamente o direito à baratada ao primeiro passe”

Ou seja, não precisa lembrar no final — o status já fica “morto” no momento que acontece.