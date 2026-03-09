<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=000000&height=200&section=header&text=Computer%20Architecture&fontSize=50&fontAlignY=35&desc=Memory,%20Assembly%20and%20Debuggers&descAlignY=55&descSize=20&fontColor=ffffff" alt="Header Banner" width="100%" />

# 💻 FIAP 2026 - Computer Architecture, Memory, Assembly & Debuggers

  **Turma 1TDCPV - 1º e 2º Semestres**

  <p>
    <img src="https://img.shields.io/badge/Course-Computer_Architecture-blue?style=for-the-badge&logo=intel" alt="Course" />
    <img src="https://img.shields.io/badge/Institution-FIAP-ed145b?style=for-the-badge&logo=minutemailer" alt="FIAP" />
    <img src="https://img.shields.io/badge/Status-In_Progress-success?style=for-the-badge&logo=google-scholar" alt="Status" />
  </p>
  <p>
    <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux" />
    <img src="https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows" />
    <img src="https://img.shields.io/badge/Assembly_x86-6E4C13?style=for-the-badge&logo=assemblyscript&logoColor=white" alt="Assembly" />
    <img src="https://img.shields.io/badge/GDB-100000?style=for-the-badge&logo=gnu&logoColor=white" alt="GDB" />
    <img src="https://img.shields.io/badge/Metasploit-126DE6?style=for-the-badge&logo=metasploit&logoColor=white" alt="Metasploit" />
  </p>
</div>

---

## 📌 Visão Geral

Repositório dedicado à disciplina de **Computer Architecture**, ministrada na **FIAP** no ano de **2026** (Turma **1TDCPV**). O objetivo central desta matéria é proporcionar um entendimento profundo sobre o funcionamento da memória, registradores corporativos, binários, engenharia reversa e o desenvolvimento de exploits focados no conceito de **Buffer Overflow (BOF)**.

> **⚠️ Foco Principal do Ano:** `BUFFER OVERFLOW`

---

## 📢 Avisos Importantes da Disciplina

De acordo com as anotações do professor na aula inaugural, preste atenção nestes pontos chave:

- 🙋 **CHAMADA:** A presença é avaliada e fundamental.
- ✅ **Check Points (CPs):**
  - Valor: **10 pontos** cada.
  - A composição total será de **20 pontos** (teremos a regra em que **1 avaliação será descartada/ignorada**).
  - *Dica do Professor:* **FAÇAM OS CPs!** As avaliações serão avisadas com **7 dias de antecedência**.
- 🏆 **Global Solution (GS):**
  - Valor atribuído: **40 pontos**.
  - O prazo de aviso e organização também ocorrerá com **7 dias de antecedência**.
- 🤖 **Ferramentas Extras:** O uso do **GitHub Copilot** é abordado e integrado aos seus alertas, recomendando o uso responsável na trilha.

---

## 📅 Conteúdo Programático (Syllabus)

O curso está dividido estrategicamente em uma base **Teórica** (primeiro semestre), focada nos rudimentos arquiteturais do sistema, e numa etapa intensamente **Prática** (segundo semestre) focada no desenvolvimento e exploração do Buffer Overflow.

### 📚 1º Semestre: Foco Teórico e Base Arquitetural

| Semana | Tema Principal | Detalhamento |
| :---: | :--- | :--- |
| **01** | 🎯 Aula Inaugural | Apresentação do Professor, objetivos e plano de ensino. |
| **02** | 🧮 Arquitetura de Computadores | Base matemática (*Bits, Bytes, Hexadecimal*). |
| **03** | 🧠 Gerência de Memória | Tipos de Memória e os Modos de Operação da CPU. |
| **04** | 🗃️ Registradores | Características dos Registradores de **32 e 64 bits**. |
| **06-07** | 🖥️ Estrutura de Binários | Análise estruturada tanto para **Windows** quanto **Linux**. |
| **08** | 💻 Linguagem Assembly | Vislumbre e Introdução à Arquitetura e Linguagem **Assembly x86**. |
| **10** | 🐛 GNU Debugger | Conhecendo e utilizando o **GDB**. |
| **11** | 🔍 Rastreio e Inspeção | Utilização avançada de comandos como `ltrace` e `strace`. |
| **12** | 🥞 Organização da Pilha | Estrutura arquitetural e fluxo de execução da *Stack*. |
| **13** | 🐚 Shellcode (Linux) | Conceitos vitais na criação de payloads e Shellcodes. |
| **14** | 🛠️ Automação de Shellcode | Geração eficiente e otimizada por meio do **Metasploit**. |

*Observação: As Semanas 05, 09 e 15 são dedicadas à validação dos **Check Points**. Fim de semestre dedicado às Provas semestrais, vista de avaliações e substitutivas.*

### 💥 2º Semestre: Foco Prático (Buffer Overflow - BOF)

| Semana | Tema Principal | Exploração & Contenções |
| :---: | :--- | :--- |
| **01-02** | 🚨 Corrupção de Memória | Mecanismos gerais causadores do Buffer Overflow Clássico. |
| **03-04** | 🕹️ Controle de Fluxo | EIP, entendendo e manipulando o fluxo de execução do programa (**BOF Vanilla**). |
| **06-08** | 🪟 Exploração Local Windows | Introdução ao Windows Debugger e prática de BOF para acesso e exploração local. |
| **10-12** | 🌐 Exploração Remota Windows| BOF injetado via malhas de rede (Exploração Remota Extra incluída). |
| **13** | 🛡️ Proteções e Controles | Ferramentas de Defesa Definitivas: **NX/DEP, ASLR, Canaries/Stack Cookies**. |

---

## 🏗️ Diagrama de Tecnologias (Roadmap)

Abaixo está o mapeamento fluído e lógico conectando o nível de silício primário até a construção final do software e suas manipulações (Metasploit):

```mermaid
graph TD
    A[Hardware & Memória] -->|Abstração| B(Nível de CPU & Instrucional)
    B --> C{Registradores}
    C -->|Arquiteturas 32/64 bit| D[Pilha / Stack Memory]

    D --> E(Sistema Operacional)
    E -->|Exploração Windows| F[Binários Win & WinDbg]
    E -->|Exploração Linux| G[Binários ELF & GDB]

    F --> H[BOF - Ataques Locais e Remotos]
    G --> I[strace / ltrace Inspect]
    
    H --> J((Shellcoding Payload))
    I --> J

    J -->|Criação Avançada| K[Automação e Deploy]
    K --> L(Metasploit Framework)
    
    classDef main fill:#1e1e1e,stroke:#fff,stroke-width:2px,color:#fff;
    class A,B,C,D,E,F,G,H,I,J,K,L main;
```

---

## 🛠️ Tecnologias Chave Envolvidas

Para o sucesso efetivo nesta jornada, o repositório abordará os seguintes componentes estruturais:

<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" height="40" alt="C" title="C" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" height="40" alt="C++" title="C++" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="40" alt="Python" title="Python Scripts" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" height="40" alt="Linux" title="Linux" />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/windows8/windows8-original.svg" height="40" alt="Windows" title="Windows" />
</div>

- **Assembly x86/x64**: Para entendimento detalhado sobre arquitetura de registradores e salto de instruções.
- **C/C++**: A linguagem basal do sistema, responsável por alocar os bytes na Stack possibilitando o ambiente de simulação e aprendizado para corrupção de memória.
- **Python**: Poderosa arma utilizada em *exploit scripts* rápidos para a injeção contínua de malwares de teste em portas de serviços ou de forma local.
- **GDB & Metasploit**: Ferramentas core dos analistas e góticos das profundezas do *Debugging*, guiadoras na injeção exata dos Endereços de Instruções.

---

> ✨ **Nota:** *Este `README.md` foi inteiramente personalizado mediante os requerimentos da disciplina e aos artefatos originais disponibilizados (`1TDCPV_anotado.pdf` e `ementa.png`). Feito para um acompanhamento dinâmico de classe.*
