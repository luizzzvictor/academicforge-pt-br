# 🎓 Academic Forge

<div align="center">

**Uma coleção curada de skills para escrita acadêmica e pesquisa**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Skills](https://img.shields.io/badge/Skills-6-blue.svg)](./skills)

[English](./README_en.md) | Português (Brasil)

</div>

## 📖 O que é um Forge?

O nome "Forge" é inspirado no **sistema de carregadores de mods do Minecraft** (como Forge ou Fabric), que permite executar vários mods juntos sem fricção. Assim como o Minecraft Forge oferece um modpack que integra diferentes mods para experiências específicas de jogo, o **Academic Forge** integra múltiplas skills do Claude Code para um fluxo de escrita acadêmica mais focado.

### Por que "Forge"?

- 🔧 **Integração em vez de instalação** - Como em modpacks do Minecraft, você recebe uma coleção curada que funciona bem em conjunto
- 🎯 **Construído com propósito** - Cada forge é voltado a um domínio específico (escrita acadêmica, desenvolvimento web, ciência de dados etc.)
- 🔄 **Atualizações automáticas** - As skills ficam atuais via submódulos git + fontes sincronizadas no modo skills-only
- 🤝 **Orientado pela comunidade** - Construído sobre o excelente trabalho de vários criadores de skills

## 🎯 Objetivo

O Academic Forge resolve um problema comum: **skills demais podem reduzir a precisão do agente de IA**. Ao curar apenas as skills relevantes para escrita acadêmica e pesquisa, o Claude Code consegue:

- ✅ Fazer invocações de skill mais precisas
- ✅ Evitar confusão entre skills semelhantes
- ✅ Manter foco no seu fluxo de pesquisa
- ✅ Permanecer atualizado com melhorias dos autores originais

## 📦 Skills incluídas

Este forge integra as seguintes skills cuidadosamente selecionadas:

### [claude-scientific-skills](https://github.com/k-dense-ai/claude-scientific-skills) (140 Skills)
- **Autor**: [@k-dense-ai](https://github.com/k-dense-ai) - By K-Dense Inc.
- **Licença**: MIT
- **Cobertura**: 140 skills científicas prontas para uso em mais de 15 domínios
- **Inclui**:
  - 🧬 **Bioinformática e Genômica** - BioPython, Scanpy, single-cell RNA-seq, anotação de variantes
  - 🧪 **Quimioinformática e Descoberta de Fármacos** - RDKit, DeepChem, docking molecular, triagem virtual
  - 🏥 **Pesquisa Clínica** - ClinicalTrials.gov, ClinVar, bases da FDA, farmacogenômica
  - 📊 **Análise de Dados** - Análise estatística, matplotlib, seaborn, figuras para publicação
  - 📚 **Comunicação Científica** - Formatação LaTeX, gestão de citações, peer review
  - 🔬 **Automação de Laboratório** - PyLabRobot, Benchling, integração com Opentrons
  - 🤖 **Machine Learning** - PyTorch Lightning, scikit-learn, fluxos de deep learning
  - 📚 **Bancos de Dados** - 28+ bases científicas (PubMed, OpenAlex, ChEMBL, UniProt etc.)
- **Melhor para**: Fluxos científicos em múltiplas etapas, da revisão bibliográfica à publicação
- **Sanitização de anúncios**: Em cada execução de instalação/download/atualização, o script remove automaticamente trechos promocionais embutidos dos arquivos SKILL.md

### [AI-research-SKILLs](https://github.com/zechenzhangAGI/AI-research-SKILLs) (82 Skills)
- **Autor**: [@zechenzhangAGI](https://github.com/zechenzhangAGI) - By Orchestra Research
- **Licença**: MIT
- **Cobertura**: 82 skills de engenharia de pesquisa em IA de nível avançado em 20 categorias
- **Inclui**:
  - 🏗️ **Arquitetura de Modelos** - LitGPT, Mamba, RWKV, NanoGPT, TorchTitan (5 skills)
  - 🎯 **Fine-Tuning** - Axolotl, LLaMA-Factory, PEFT, Unsloth (4 skills)
  - 🎓 **Pós-Treinamento** - TRL, GRPO, OpenRLHF, SimPO, verl (8 skills de RLHF/DPO)
  - ⚡ **Treinamento Distribuído** - DeepSpeed, FSDP, Megatron-Core, Accelerate (6 skills)
  - 🚀 **Otimização** - Flash Attention, bitsandbytes, GPTQ, AWQ (6 skills)
  - 🔥 **Inferência** - vLLM, TensorRT-LLM, SGLang, llama.cpp (4 skills)
  - 📊 **Avaliação** - lm-eval-harness, BigCode, NeMo Evaluator (3 skills)
  - 🤖 **Agents e RAG** - LangChain, LlamaIndex, Chroma, FAISS (9 skills)
  - 🎨 **Multimodal** - CLIP, Whisper, LLaVA, Stable Diffusion (7 skills)
  - 📝 **Escrita de Artigos de ML** - Templates LaTeX para NeurIPS, ICML, ICLR, ACL (1 skill)
- **Qualidade da documentação**: ~420 linhas por skill + 300KB+ de materiais de referência
- **Melhor para**: Fluxos de pesquisa em IA da hipótese à publicação

### [humanizer](https://github.com/blader/humanizer)
- **Autor**: [@blader](https://github.com/blader)
- **Licença**: Consulte o repositório original
- **Objetivo**: Refinar tom acadêmico, melhorar legibilidade e evitar padrões detectáveis de texto gerado por IA
- **Melhor para**: Polimento de rascunhos, manutenção de voz acadêmica e preparação para revisão por pares

### [superpowers](https://github.com/obra/superpowers) (somente `skills/`)
- **Autor**: [@obra](https://github.com/obra)
- **Licença**: MIT
- **Objetivo**: Biblioteca de skills de fluxo estruturado (ex.: brainstorming, writing-plans, systematic-debugging, test-driven-development)
- **Melhor para**: Clarificação de requisitos, planejamento, depuração sistemática e execução com TDD em projetos acadêmicos
- **Modo de integração**: Este forge sincroniza intencionalmente apenas o diretório `skills/` do upstream (sem plugins ou pastas não relacionadas a skills)

### [planning-with-files](https://github.com/OthmanAdi/planning-with-files) (skills-only, pasta única)
- **Autor**: [@OthmanAdi](https://github.com/OthmanAdi)
- **Licença**: MIT
- **Objetivo**: Planejamento baseado em arquivos no estilo Manus com `task_plan.md`, `findings.md` e `progress.md` para persistir contexto em trabalhos complexos
- **Melhor para**: Tarefas longas e em múltiplas etapas (implementação ou pesquisa) que exigem planejamento durável e recuperação de sessão
- **Modo de integração**: Este forge sincroniza intencionalmente apenas `.opencode/skills/planning-with-files` do upstream (não como submódulo)

### scientific-visualization (skill local integrada)
- **Autor**: Colaboradores do Academic Forge (manutenção local)
- **Licença**: MIT (herda a licença deste repositório)
- **Objetivo**: Melhorar figuras científicas para qualidade de publicação com mais consistência visual e acessibilidade
- **Melhor para**: Fluxos de plotagem para periódicos (layouts com múltiplos painéis, barras de erro/marcadores de significância, paletas amigáveis para daltonismo e otimização de exportação)
- **Modo de integração**: Skill local em `skills/scientific-visualization`, sem dependência de sincronização upstream

> **Nota**: Todas as skills mantêm suas licenças e autorias originais. Este forge oferece apenas integração conveniente. Consulte [ATTRIBUTIONS.md](./ATTRIBUTIONS.md) para créditos detalhados.

## 🚀 Início rápido

### Instalação

Instale o Academic Forge diretamente no seu projeto Claude Code/OpenCode:

**macOS/Linux:**
```bash
cd your-project
curl -sSL https://raw.githubusercontent.com/HughYau/AcademicForge/refs/heads/master/scripts/install.sh | bash
```

**Windows (PowerShell):**
```powershell
cd your-project
irm https://raw.githubusercontent.com/HughYau/AcademicForge/refs/heads/master/scripts/install.ps1 | iex
```

Ou manualmente:

```bash
# Clone o repositório (com submódulos; fontes skills-only são sincronizadas por scripts)
git clone --recursive https://github.com/HughYau/AcademicForge .opencode/skills/academic-forge

# Se já clonou sem --recursive
git submodule update --init --recursive
```

### Download/Sincronização de Skills

Se você quiser sincronizar skills em um clone existente (submódulos + fontes skills-only):

**Windows (PowerShell):**
```powershell
.\scripts\download-skills.ps1
```

**Linux/macOS:**
```bash
bash scripts/download-skills.sh
```

Esses scripts sincronizam automaticamente a pasta local `skills/`, incluindo submódulos, snapshot de `skills/` do `superpowers` e snapshot de `.opencode/skills/planning-with-files`. A `scientific-visualization` é local e não depende de sincronização upstream.

### Atualização de Skills

Mantenha todas as skills atualizadas com as melhorias mais recentes:

```bash
cd .opencode/skills/academic-forge
./scripts/update.sh  # ou use update.ps1 no Windows
```

> Opcional: para bloquear skills específicas do upstream, edite `scripts/skill-blacklist.txt`. Os scripts de instalação/download/atualização removem automaticamente os caminhos listados.

#### 🔄 Atualizações automáticas

Este repositório está configurado com workflows automáticos que atualizam todas as fontes de skills upstream (submódulos + sincronização skills-only de superpowers/planning-with-files) **toda segunda-feira às 09:00 UTC**. A `scientific-visualization` é mantida localmente neste repositório.

- ✅ As skills permanecem sempre atualizadas
- ✅ Recebe automaticamente melhorias e correções dos autores originais
- ✅ Não é necessário executar scripts de atualização manualmente
- 📅 Agenda de atualização: toda segunda-feira às 09:00 UTC

## 🎓 Casos de uso

O Academic Forge é ideal para:

- 📝 **Escrita de artigos científicos** - Do esboço ao manuscrito pronto para submissão
- 🔬 **Desenho experimental** - Planejamento e documentação de metodologia de pesquisa
- 📊 **Análise de dados** - Análise estatística e interpretação de resultados
- 🖼️ **Figuras científicas** - Criação e refinamento de gráficos com qualidade de publicação
- 📚 **Revisão de literatura** - Organização e síntese de fontes acadêmicas
- ✍️ **Redação de tese/dissertação** - Gestão de documentos acadêmicos longos
- 👥 **Pesquisa colaborativa** - Manutenção de estilo consistente entre membros da equipe

## 📄 Documentação

- [Guia de início rápido](./QUICKSTART.md) - Comece em 5 minutos
- [Exemplos de uso](./EXAMPLES.md) - Fluxos reais de trabalho
- [Atribuições das skills](./ATTRIBUTIONS.md) - Informações detalhadas de autoria e licença
- [Guia de contribuição](./CONTRIBUTING.md) - Como contribuir ou criar o seu próprio forge

## 🤝 Contribuição

Encontrou uma skill perfeita para escrita acadêmica? Veja [CONTRIBUTING.md](./CONTRIBUTING.md) para:

- Sugerir novas skills
- Reportar problemas
- Melhorar documentação
- Criar seu próprio forge de domínio específico

## 📄 Licença

A **estrutura do forge** (scripts, configuração e documentação) é licenciada sob a [MIT License](./LICENSE).

As **skills individuais** mantêm suas licenças originais — consulte [ATTRIBUTIONS.md](./ATTRIBUTIONS.md) e os repositórios de cada skill para mais detalhes.
