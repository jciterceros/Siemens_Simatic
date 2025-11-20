# 🏭 Siemens STEP 7 & Factory IO - Estudos de Automação Industrial

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![STEP 7](https://img.shields.io/badge/STEP%207-v5.7-blue)](https://www.siemens.com)
[![Factory IO](https://img.shields.io/badge/Factory%20IO-Simulation-green)](https://factoryio.com/)

## 📋 Sobre o Projeto

Repositório dedicado aos meus estudos de programação de CLPs Siemens com **STEP 7 v5.7 (Simatic Manager)** integrado com simulações no **Factory IO**. Aqui você encontrará projetos práticos, exemplos de scenes resolvidas e documentação visual completa com imagens e vídeos.

### 📊 Estatísticas do Projeto

- 🎯 **Scenes Concluídas:** 1
- 📝 **Documentações Criadas:** 3 (READMEs + Docs técnicas)
- 📸 **Imagens Documentadas:** 5+
- 🎬 **Vídeos Demonstrativos:** 1
- 💾 **Projetos STEP 7:** 1 completo

## 🎯 Objetivos

- 📚 Documentar o aprendizado em automação industrial
- 💻 Desenvolver projetos práticos de CLP
- 🎮 Resolver e documentar scenes do Factory IO
- 🔗 Integrar STEP 7 com Factory IO
- 📸 Criar material visual educativo (imagens e vídeos)
- 🚀 Compartilhar conhecimento com a comunidade

## 📁 Estrutura do Repositório

### 🎯 Foco Atual: Factory IO Scenes

```
📁 Siemens_Simatic/
└── 📁 05_FactoryIO_Scenes/         # 🔥 EM DESENVOLVIMENTO
    ├── 📁 Scene_01_From_A_to_B/    # ✅ CONCLUÍDO
    │   ├── 📁 Projeto/             # Arquivos .s7p do STEP 7
    │   ├── 📁 FactoryIO/           # Arquivos .factoryio
    │   ├── 📁 Imagens/             # Screenshots e diagramas
    │   ├── 📁 Videos/              # Vídeos demonstrativos
    │   ├── 📁 Simulador/           # Arquivos do simulador
    │   ├── 📁 Documentacao/        # Descrição e explicações
    │   └── README.md               # Documentação da scene
    ├── 📁 Scene_01_Exemplo/        # Template de referência
    └── ...
```

### 📋 Estrutura Planejada (Futuro)

<details>
<summary>Clique para ver a estrutura completa planejada</summary>

```
📁 Siemens_Simatic/
├── 📁 01_Fundamentos/              # Conceitos básicos de automação
├── 📁 02_Step7_Basico/             # Programação básica STEP 7
├── 📁 03_Step7_Intermediario/      # Conceitos intermediários
├── 📁 04_Step7_Avancado/           # Programação avançada
├── 📁 05_FactoryIO_Scenes/         # ✅ Scenes do Factory IO resolvidas
├── 📁 06_Integracao_Step7_FactoryIO/ # Projetos integrados
├── 📁 07_Bibliotecas_FCs_FBs/      # Functions e Function Blocks
├── 📁 08_HMI_SCADA/                # Interfaces homem-máquina
├── 📁 09_Comunicacao_Redes/        # Redes industriais
└── 📁 10_Recursos/                 # Manuais, templates e recursos
```

</details>

## 🛠️ Tecnologias e Ferramentas

- **Simatic Manager STEP 7 v5.7** - Ambiente de programação para CLPs S7-300/400
- **Factory IO** - Simulador de automação industrial
- **PLCSim v5.4+** - Simulador de CLP Siemens
- **WinCC Flexible** - Sistema SCADA/HMI
- **NetToPLCSim** - Comunicação entre Factory IO e PLCSim

## 🚀 Como Usar Este Repositório

### Para Scenes do Factory IO (Foco Atual):

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/jciterceros/Siemens_Simatic.git
   ```

2. **Navegue até a scene desejada:**
   ```bash
   cd Siemens_Simatic/05_FactoryIO_Scenes/Scene_XX_[Nome]
   ```

3. **Abra o projeto no Simatic Manager:**
   - Localize o arquivo `.s7p` na pasta `Projeto/`
   - Abra com Simatic Manager STEP 7 v5.7

4. **Configure o PLCSim:**
   - Inicie o S7-PLCSIM v5.4+
   - Carregue o programa no simulador

5. **Conecte com Factory IO:**
   - Abra o arquivo `.factoryio` na pasta `FactoryIO/`
   - Configure a conexão com S7-PLCSIM via NetToPLCSim
   - Inicie a simulação

6. **Consulte a documentação:**
   - Leia o `README.md` da scene para entender a lógica
   - Veja as imagens para entender o layout e ladder
   - Assista ao vídeo demonstrativo

## 📚 Conteúdo em Desenvolvimento

### 🔥 Fase Atual: Factory IO Scenes

**Objetivo:** Resolver e documentar scenes do Factory IO com programação STEP 7 v5.7

#### ✅ Estrutura Criada
- [x] Repositório e README principal
- [x] Estrutura de pastas para scenes
- [x] Template de exemplo (Scene_01_Exemplo)

#### 🔄 Em Desenvolvimento
- [x] Scene 01 - From A to B ✅ **CONCLUÍDO**
- [ ] Scene 02 - [Aguardando implementação]
- [ ] Scene 03 - [Aguardando implementação]

#### 📋 Metodologia de Documentação de Cada Scene
Cada scene resolvida inclui:
- ✅ Código STEP 7 (.s7p + backup .zip)
- ✅ Arquivo Factory IO (.factoryio)
- ✅ Documentação explicativa (README.md completo)
- ✅ Imagens do processo e lógica (Ladder, HW Config, Símbolos, etc.)
- ✅ Vídeo curto demonstrando o funcionamento (.mp4)
- ✅ Lista de tags e endereçamento I/O
- ✅ Descrição do problema e solução implementada
- ✅ Arquivo simulador alternativo (quando aplicável)
- ✅ Documentação técnica adicional (ESTRUTURA_ARQUIVOS.md)

### 📅 Fases Futuras

<details>
<summary>Roadmap de implementação futura</summary>

#### Fase 2: Fundamentos e Teoria
- [ ] Conceitos básicos de automação industrial
- [ ] Introdução ao STEP 7 v5.7
- [ ] Estrutura de projetos no Simatic Manager

#### Fase 3: Programação STEP 7
- [ ] Programação básica (Ladder, STL, FBD)
- [ ] Conceitos intermediários (FCs, FBs, DBs)
- [ ] Programação avançada (SCL, SFC, comunicação)

#### Fase 4: Integração e Recursos
- [ ] Projetos integrados completos
- [ ] Biblioteca de FCs e FBs reutilizáveis
- [ ] HMI/SCADA com WinCC Flexible
- [ ] Redes industriais (Profibus, Profinet)

</details>

## 🎓 Recursos de Aprendizado

- [Siemens Support Center](https://support.industry.siemens.com)
- [Factory IO Documentation](https://docs.factoryio.com/)
- [STEP 7 V5.x Documentation](https://support.industry.siemens.com/cs/document/18652056)

## 📸 Galeria de Projetos

### 🎬 Factory IO Scenes Resolvidas

#### Scene 01 - From A to B ✅
![Scene Simulation](./05_FactoryIO_Scenes/Scene_01_From_A_to_B/Imagens/Simulation.png)

**Descrição:** Transporte básico de caixa do ponto A ao ponto B  
**Status:** Concluído  
**Dificuldade:** ⭐ Básico  

📹 [Ver Vídeo Demonstrativo](./05_FactoryIO_Scenes/Scene_01_From_A_to_B/Videos/Simulation.mp4)  
� [Ver Documentação Completa](./05_FactoryIO_Scenes/Scene_01_From_A_to_B/)

**Recursos incluídos:**
- ✅ Projeto STEP 7 completo (.s7p)
- ✅ Scene Factory IO (S7-300)
- ✅ 5 imagens documentadas (Ladder, HW Config, Símbolos, etc.)
- ✅ Vídeo demonstrativo
- ✅ Documentação técnica completa

---

_Mais scenes em desenvolvimento..._

## 🤝 Contribuições

Sugestões e feedback são sempre bem-vindos! Sinta-se à vontade para:

- 🐛 Reportar bugs ou problemas
- 💡 Sugerir novas funcionalidades
- 📖 Melhorar a documentação
- ⭐ Dar uma estrela se este repositório foi útil

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👤 Autor

**jciterceros**

- GitHub: [jciterceros](https://github.com/jciterceros)
- LinkedIn: [Fernando Flores Terceros](https://www.linkedin.com/in/fernando-flores-terceros-83486625/)

## 📞 Contato

Dúvidas ou sugestões? Entre em contato através das issues do GitHub!

---

⭐ **Se este repositório foi útil para você, considere dar uma estrela!** ⭐

---

## 📈 Progresso do Projeto

```
Fase 1: Factory IO Scenes ████████░░░░░░░░░░ 10% (1/10 scenes planejadas)
├── ✅ Scene 01 - From A to B (Concluída)
├── ⏳ Scene 02 - Planejada
├── ⏳ Scene 03 - Planejada
└── ... mais 7 scenes

Documentação  ████████████████████ 100% (Sistema implementado)
Infraestrutura ███████████████████ 95% (Estrutura + Templates)
```

## 🗓️ Histórico de Atualizações

- **20/11/2025** - ✅ Scene 01 "From A to B" concluída e documentada
- **20/11/2025** - 📁 Estrutura de pastas e templates criados
- **20/11/2025** - 🚀 Repositório inicial criado

---

*Última atualização: 20/11/2025*
