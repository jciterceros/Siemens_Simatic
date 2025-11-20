# 🏭 Factory IO Scenes - Simatic STEP 7 v5.7

Esta pasta contém as implementações e soluções de diferentes scenes do Factory IO programadas com Simatic Manager STEP 7 v5.7.

## 📋 Índice de Scenes

| Scene | Nome | Status | Dificuldade | Descrição |
|-------|------|--------|-------------|-----------|
| 01 | [From A to B](./Scene_01_From_A_to_B/) | ✅ Concluído | ⭐ Básico | Transportar uma caixa até um sensor |
| 02 | [Aguardando] | ⏳ Planejado | - | - |
| 03 | [Aguardando] | ⏳ Planejado | - | - |

### Legenda de Status:
- ✅ **Concluído** - Scene implementada e documentada
- 🔄 **Em Desenvolvimento** - Trabalho em andamento
- ⏳ **Planejado** - Próxima na fila
- ❌ **Pausado** - Temporariamente em espera

### Legenda de Dificuldade:
- ⭐ **Básico** - Conceitos fundamentais
- ⭐⭐ **Intermediário** - Requer conhecimento prévio
- ⭐⭐⭐ **Avançado** - Lógica complexa

## 📁 Estrutura de Cada Scene

Cada scene segue o padrão de organização:

```
Scene_XX_[Nome]/
├── 📁 Projeto/              # Arquivos .s7p do Simatic Manager + backup .zip
├── 📁 FactoryIO/            # Arquivos .factoryio da scene
├── 📁 Imagens/              # Screenshots, diagramas, ladder
├── 📁 Videos/               # Vídeos demonstrativos curtos (.mp4)
├── 📁 Simulador/            # Arquivos do simulador alternativo (se houver)
├── 📁 Documentacao/         # Documentos adicionais (ESTRUTURA_ARQUIVOS.md)
└── README.md                # Documentação completa da scene
```

## 🚀 Como Usar

1. **Escolha uma scene** da lista acima
2. **Navegue até a pasta** da scene desejada
3. **Leia o README.md** para entender o problema e solução
4. **Abra o projeto** (.s7p) no Simatic Manager
5. **Carregue a scene** (.factoryio) no Factory IO
6. **Configure a conexão** PLCSim + NetToPLCSim
7. **Execute e teste** a solução

## 📚 Recursos Necessários

### Software:
- ✅ Simatic Manager STEP 7 v5.7
- ✅ S7-PLCSIM v5.4 ou superior
- ✅ Factory IO (versão atualizada)
- ✅ NetToPLCSim (para comunicação)

### Conhecimentos Prévios:
- 📖 Conceitos básicos de automação industrial
- 📖 Endereçamento de I/O em CLPs Siemens
- 📖 Programação em Ladder (LAD) ou STL
- 📖 Operação básica do Factory IO

## 🎯 Objetivos de Aprendizado

Ao trabalhar com estas scenes, você irá:

- ✅ Praticar programação de CLPs Siemens
- ✅ Entender lógica de controle industrial
- ✅ Aprender integração STEP 7 + Factory IO
- ✅ Desenvolver habilidades de troubleshooting
- ✅ Criar documentação técnica profissional

## 🤝 Contribuições

Sugestões de melhorias nas soluções são bem-vindas! Abra uma issue ou pull request.

---

**Nota:** Todas as scenes são desenvolvidas para fins educacionais e de aprendizado.
