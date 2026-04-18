# 🛡️ Estudos Blue Team - Segurança e Sistemas Livres

Repositório dedicado ao meu aprendizado em Defesa Cibernética e Administração de Sistemas.

## 🐧 Fundamentos de Software Livre (Aula 02)

### Definição e Filosofia
* **Software Livre:** Qualquer software cuja licença garante as **4 liberdades essenciais** (Executar, Estudar, Redistribuir e Modificar).
* **Projeto GNU:** Iniciado em 1983. O objetivo era criar um sistema operacional 100% livre.
* **GNU:** Significa "GNU is Not Unix" (Acrônimo recursivo).

### A União GNU + Linux
* **1983:** Início do Projeto GNU (Compiladores GCC, bibliotecas glibc).
* **1991:** Surgimento do Kernel Linux.
* **O Nome Correto:** **GNU/Linux**. O GNU é a ideia original e o conjunto complexo; o Linux é o núcleo (kernel) que foi acrescentado depois.

### 🌀 Distribuição Debian
* **Lançamento:** 16/08/1993.
* **História:** É a segunda distribuição mais antiga ainda ativa.
* **Proposta:** O "Sistema Operacional Universal", focado em ser 100% composto por software livre.
# 📓 Meus Estudos de Blue Team e Linux

## 🗓️ Registro de Dificuldades (Resolvido)
### Erro de Sincronização do Git
* **Problema:** O erro `[rejected] master -> master (fetch first)` apareceu ao tentar d>
* **Causa:** Conflito entre o que estava no site (GitHub) e o que estava no meu PC.
* **Solução:** Usei o comando `git pull origin master --rebase` para alinhar as duas ve>

---

## 🛡️ Notas de Aula - Próximos Passos
### 🐧 Comandos de Terminal que aprendi:
* `nano`: Editor de texto direto no terminal.
* `git add`: Prepara o arquivo para envio.
* `git commit -m`: Cria um ponto de salvamento com mensagem.
* `git push`: Envia as notas para a nuvem.

> **Dica de Ouro:** Sempre salvar no nano com `Ctrl + O`, `Enter` e sair com `Ctrl + X`.

---
### 📢 Status de Hoje:
> **"Passando para dar um alo! O progresso continua assim que possível, jaja estou de volta com as próximas aulas de Blue Team."** 🚀
---

---
## 🌍 Manifesto Global: Resiliência no Código

> "A persistência é o caminho do êxito."

| Idioma | Tradução | Idioma | Tradução |
| :--- | :--- | :--- | :--- |
| **Português** | Nunca desista | **Russo** | Никогда не сдавайся |
| **Tcheco** | Nikdy se nevzdávej | **Inglês** | Never give up |
| **Espanhol** | Nunca te rindas | **Francês** | N'abandonne jamais |
| **Alemão** | Gib niemals auf | **Italiano** | Non arrenderti mai |
| **Japonês** | 決して諦めないで | **Chinês** | 永不放弃 |
| **Coreano** | 절대 포기하지 마세요 | **Árabe** | لا تستسلم أبدا |
| **Hindi** | हार मत मानो | **Grego** | Ποτέ μην τα παρατάς |
| **Holandês** | Geef nooit op | **Polonês** | Nigdy się nie poddawaj |
| **Turco** | Asla vazgeçme | **Sueco** | Ge aldrig upp |
| **Vietnamita** | Đừng bao giờ bỏ cuộc | **Hebraico** | לעולם אל תתייאש |
| **Indonésio** | Jangan pernah menyerah | **Tailandês** | อย่า ยอม แพ้ |
| **Romeno** | Nu renunța niciodată | **Norueguês** | Gi aldri opp |
| **Húngaro** | Soha ne add fel | **Finlandês** | Älä koskaan luovuta |
| **Dinamarquês** | Giv aldrig op | **Ucraniano** | Ніколи не здавайся |
| **Latim** | Numquam cede | **Esperanto** | Neniam rezignu |

---
# 🖥️ Solução: Forçar 120Hz em Gráficos Integrados Intel (4ª Gen) no Debian

Este documento registra a solução técnica para habilitar a taxa de atualização de **120Hz** em 1080p usando o vídeo integrado (iGPU) de processadores Intel Haswell (i3-4160), corrigindo falhas de driver e limitações de largura de banda no Debian Trixie/Sid.

---

## ❌ O Problema (Erro de CRTC)
Ao tentar adicionar o modo manual via `xrandr`, o sistema retornava o erro:
`xrandr: Configure crtc 0 failed`

### Diagnóstico Lógico:
1. **Driver Inativo:** O sistema não carregava o driver `i915`, operando em modo genérico (sem o arquivo `/dev/dri/card0`).
2. **Estouro de Banda (Pixel Clock):** O sinal padrão de 120Hz gerado pelo `cvt` era de **369.50 MHz**, o que excedia o limite físico do controlador HDMI do processador de 4ª geração, causando a rejeição do sinal pelo Kernel.

---

## 🛠️ Passo a Passo da Solução

### 1. Habilitar Repositórios Non-Free
O Debian precisa de permissão para baixar os firmwares proprietários da Intel.
```bash
sudo sed -i 's/main/main contrib non-free non-free-firmware/g' /etc/apt/sources.list
sudo apt update

---
## 🔍 Ferramentas de OSINT: Maltego
### 🛠️ Status: Ambiente Configurado
Cadastro realizado com sucesso. O ambiente está pronto para os primeiros testes de coleta de dados.
---

---
## 🔍 Ferramentas de OSINT: Maltego
### 🛠️ Status: Ambiente Configurado
Hoje realizei a instalação e o cadastro oficial no **Maltego** (Community Edition). A ferramenta já está autenticada e pronta para os primeiros testes de mapeamento de infraestrutura e coleta de dados públicos.

**Próximos passos planejados:**
* [ ] Realizar o primeiro "Footprinting" de um domínio de teste.
* [ ] Explorar as *Transforms* básicas para mapear registros DNS.
* [ ] Integrar com outras APIs de busca.

> "A inteligência não é apenas coletar dados, mas conectar os pontos certos."
---

## Eu me cadastrei no linkedin
estou montando meu curriculo é indo atras de conhecimento e certificações.
