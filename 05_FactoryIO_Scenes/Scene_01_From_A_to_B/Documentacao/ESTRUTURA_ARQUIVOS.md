# Scene 01 - From A to B - Documentação Técnica

## 📁 Estrutura de Arquivos do Projeto

```
Scene_01_From_A_to_B/
├── README.md                           # Documentação principal
├── Projeto/
│   ├── From_A_t/                       # Projeto STEP 7 descompactado
│   │   └── From_A_t.s7p                # Arquivo principal do projeto
│   └── From_a_t.zip                    # Backup compactado do projeto
├── FactoryIO/
│   └── 1 - From A to B - S7-300.factoryio  # Scene do Factory IO
├── Imagens/
│   ├── HW Config.png                   # Configuração de hardware S7-300
│   ├── Ladder.png                      # Programa em Ladder Logic
│   ├── Simulation.png                  # Screenshot da simulação
│   ├── Structure.png                   # Estrutura do projeto
│   └── Symbol.png                      # Tabela de símbolos
├── Videos/
│   └── Simulation.mp4                  # Vídeo demonstrativo completo
├── Simulador/
│   └── plc1.plc                        # Arquivo simulador alternativo
└── Documentacao/
    └── ESTRUTURA_ARQUIVOS.md           # Este arquivo

```

## 🔧 Especificações Técnicas

### Hardware Configurado:
- **CPU:** S7-300 (Siemens)
- **Rack:** Configuração padrão
- **Módulos de I/O:**
  - DI (Digital Input): Módulo de entradas digitais
  - DO (Digital Output): Módulo de saídas digitais

### Software Utilizado:
- **Programação:** Simatic Manager STEP 7 v5.7
- **Simulação PLC:** S7-PLCSIM v5.4+
- **Simulação Processo:** Factory IO
- **Comunicação:** NetToPLCSim

### Linguagem de Programação:
- **Principal:** Ladder Logic (LAD)
- **Alternativa:** STL (Statement List) - se disponível

## 📊 Mapeamento de I/O

### Entradas (Inputs)
| Endereço | Símbolo | Tipo | Dispositivo Factory IO |
|----------|---------|------|------------------------|
| I0.0 | Start_Button | BOOL | Push Button (Momentary) |
| I0.1 | Sensor_At_B | BOOL | Diffuse Sensor / At Sensor |

### Saídas (Outputs)
| Endereço | Símbolo | Tipo | Dispositivo Factory IO |
|----------|---------|------|------------------------|
| Q0.0 | Conveyor_Motor | BOOL | Conveyor Motor |

## 🎯 Lógica de Controle

### Descrição Funcional:
O sistema implementa um controle simples de transporte de material:

1. **Estado Inicial:**
   - Sistema aguardando comando
   - Motor desligado
   - Caixa na posição inicial (ponto A)

2. **Ciclo de Operação:**
   - Operador pressiona Start_Button (I0.0 = 1)
   - Motor da esteira é acionado (Q0.0 = 1)
   - Caixa se desloca de A para B
   - Sensor detecta presença da caixa (I0.1 = 1)
   - Motor é desligado (Q0.0 = 0)
   - Sistema aguarda novo ciclo

### Equação Lógica:
```
Q0.0 (Conveyor_Motor) = I0.0 (Start_Button) AND NOT I0.1 (Sensor_At_B)
```

Ou em forma de retenção:
```
SET Q0.0 quando I0.0 = 1
RESET Q0.0 quando I0.1 = 1
```

## 📦 Conteúdo dos Arquivos

### Projeto STEP 7 (From_A_t.s7p):
- **OB1 (Organization Block 1):** Programa principal cíclico
- **Tabela de Símbolos:** Definição de tags/endereços
- **Configuração de Hardware:** S7-300 CPU e módulos I/O
- **Blocks:** Blocos de programa (FC, FB, DB se houver)

### Scene Factory IO:
- **Layout:** Esteira transportadora simples
- **Sensores:** 
  - 1x Sensor de presença (At Sensor)
  - 1x Botão Start
- **Atuadores:**
  - 1x Motor de esteira
- **Material:** Caixas (boxes)

### Arquivo Simulador (plc1.plc):
- Arquivo de simulador alternativo
- Possível formato: PLCSim Save State ou outro simulador

## 📈 Análise de Desempenho

### Tempo de Ciclo:
- **Tempo de transporte:** Depende da velocidade da esteira (~5-10 segundos)
- **Tempo de resposta do sensor:** Instantâneo (simulação)
- **Tempo de acionamento do motor:** Instantâneo (simulação)

### Ciclo de Scan do PLC:
- **Típico:** < 10ms (S7-300)
- **Determinístico:** Sim

## 🔍 Testes e Validação

### Cenários Testados:
1. ✅ Transporte único de caixa
2. ✅ Múltiplos ciclos consecutivos
3. ✅ Comportamento sem caixa presente
4. ✅ Resposta imediata ao sensor
5. ✅ Parada correta no destino

### Resultados:
- ✅ Todos os testes passaram com sucesso
- ✅ Sistema estável e confiável
- ✅ Lógica simples e eficiente

## 🎓 Valor Educacional

### Conceitos Ensinados:
1. **Básicos de Automação:**
   - Start/Stop logic
   - Sensor-based control
   - Motor control

2. **Programação STEP 7:**
   - Uso do OB1
   - Lógica Ladder básica
   - Endereçamento de I/O

3. **Integração:**
   - Conexão STEP 7 ↔ Factory IO
   - PLCSim setup
   - NetToPLCSim configuration

4. **Documentação:**
   - Screenshots técnicos
   - Vídeos demonstrativos
   - Estrutura organizada

## 📞 Suporte

Para dúvidas ou melhorias, consulte:
- README.md principal do projeto
- Repositório: github.com/jciterceros/Siemens_Simatic

---

**Documento criado em:** 20/11/2025  
**Versão:** 1.0  
**Autor:** jciterceros
