## 🚀 Projeto Atual & Destaque Técnico

### 🎮 Astro Bot (PC Port via AnyPS5)
Atualmente estou trabalhando na continuidade da compilação e otimização do **ASTRO BOT** (`PPSA21567`) no emulador **AnyPS5**.

- 🎯 **Status Atual:** Crash de alocação de GPU resolvido; o jogo carrega e roda com sucesso até a tela de título[cite: 1].
- 🛠️ **Foco de Otimização:** 
  - Redução de custo de CPU nos commits através do ajuste de pipeline de draws (`APS5_PIPELINED_DRAWS=32`, reduzindo de 594µs para 121µs por commit)[cite: 1].
  - Análise de profilers e gargalos de concorrência/esperas de labels (`WAIT_REG_MEM` nas filas de compute/queue 0)[cite: 1].
  - Otimização de importação de memória host (`APS5_HOST_IMPORT_MIB=6144`)[cite: 1].
- 🧰 **Tech Stack & Ferramentas:** C++, Vulkan, GCC 15, Ninja Build, PowerShell Benchmarking Harness, GPU Profiling[cite: 1, 2].
