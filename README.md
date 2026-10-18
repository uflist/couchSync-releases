<p align="center">
  <img src="https://raw.githubusercontent.com/uflist/couchSync-releases/main/couchsync-banner.svg" alt="couchSync — watch party sincronizada para o Stremio" width="100%">
</p>

<p align="center">
  <a href="https://github.com/uflist/couchSync-releases/releases/latest"><img alt="Última versão" src="https://img.shields.io/github/v/release/uflist/couchSync-releases?style=for-the-badge&label=vers%C3%A3o&color=e9a85f&labelColor=2a221c"></a>
  <a href="https://github.com/uflist/couchSync-releases/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/uflist/couchSync-releases/total?style=for-the-badge&label=downloads&color=d7774f&labelColor=2a221c"></a>
  <img alt="Windows" src="https://img.shields.io/badge/Windows-10%20%7C%2011-f2e6d8?style=for-the-badge&logo=windows&logoColor=f2e6d8&labelColor=2a221c">
</p>

<p align="center">
  <b>Vejam filmes e séries juntos, em sincronia, cada um na qualidade original.</b><br>
  O Discord fica só para falar — nada de screenshare pixelizada. 🍿
</p>

<p align="center">
  <a href="https://github.com/uflist/couchSync-releases/releases/latest">
    <img alt="Descarregar o couchSync" src="https://img.shields.io/badge/%E2%AC%87%20Descarregar%20o%20couchSync-.exe-e9a85f?style=for-the-badge&labelColor=d7774f">
  </a>
</p>

---

## 🛋️ O que é

O couchSync junta os amigos num sofá virtual. Uma pessoa é o **host** 👑: escolhe o filme e controla o play, a pausa e os saltos. Toda a gente vê **o mesmo momento ao mesmo tempo** — mas cada um reproduz o vídeo no seu próprio PC, através do seu Stremio, por isso a imagem é a original e não a da screenshare.

Se alguém estiver a carregar, a sala espera por essa pessoa. Se alguém se atrasar meio segundo, o couchSync acerta-o sem ninguém dar por isso.

---

## 👥 Vou só entrar na sala de alguém

**Não precisas de descarregar nada daqui.** Só precisas de:

- [x] **Stremio** desktop instalado e **aberto**
- [x] **Radmin VPN** ligado, na rede do grupo
- [x] O **link** que o host te mandou (`http://26.x.x.x:8000`)

Abre o link no Chrome, Edge ou Firefox, carrega no botão da porta de entrada, escolhe um nome (e uma foto, se quiseres) e entra na sala. Já está. ✨

---

## 👑 Quero ser o host

### Antes de começar
1. **Stremio** desktop instalado e **aberto** — é ele que vai buscar os filmes.
2. **Radmin VPN** ligado, na rede do grupo.

### Arrancar
1. Descarrega o **`couchSync-vX.Y.Z.exe`** em [*Releases*](https://github.com/uflist/couchSync-releases/releases/latest) e põe-no numa pasta só para ele (ex.: `Documentos\couchSync`).
2. Duplo clique no `.exe`.
3. Na primeira vez, a **firewall** do Windows pergunta se o deixas comunicar: carrega em **«Permitir»** (redes privadas). Sem isso os amigos não conseguem entrar.
4. Abre-se a **janelinha do couchSync** e o browser em `http://localhost:8000`.
5. Na janelinha está o link para os amigos (`http://26.x.x.x:8000`) — carrega em **«Copiar»** e manda-o no Discord.
6. Para desligar, fecha a janelinha.

> [!IMPORTANT]
> **«O Windows protegeu o seu PC»?** Carrega em **«Mais informações»** → **«Executar mesmo assim»**. Aparece porque o programa não tem uma assinatura digital paga, não porque tenha vírus. Se o antivírus o apagar, põe a pasta do couchSync nas exclusões dele.

> [!NOTE]
> O primeiro arranque demora uns segundos (o programa prepara-se); os seguintes são rápidos.

### ⚡ Real-Debrid (opcional)

Tens Real-Debrid? Na janelinha carrega em **«Real-Debrid»**, cola a tua chave ([real-debrid.com/apitoken](https://real-debrid.com/apitoken)) e **«Guardar»**. A janela diz logo se a chave serve — não é preciso reiniciar.
Sem chave, vês por torrent como os outros.

> [!TIP]
> 🔒 A chave fica guardada no `couchSync.env`, ao lado do `.exe`, **só no teu PC**. A app nunca a envia aos outros: os amigos veem o mesmo torrent pelo Stremio deles.

### 🔄 Atualizar

A versão aparece no fundo do ecrã de entrada. Quando houver uma nova, aparece lá um aviso com link: descarrega o `.exe` novo para a **mesma pasta** e apaga o antigo. O teu `couchSync.env` fica onde está (não tens de pôr a chave outra vez).

Quem só entra nas salas **nunca** precisa de atualizar — a página vem sempre do PC do host.

---

## ✨ O que dá para fazer

| | |
|:---:|---|
| 🎮 | **Sincronização a sério** — play, pausa e saltos do host para todos; pausa automática quando alguém está a carregar |
| 🍿 | **Catálogos e pesquisa** — populares, novidades, séries por episódio, lista de torrents com qualidade e seeders |
| 🗳️ | **Sugestões com votos** — quem não é host sugere, todos votam, o host aceita |
| 💬 | **Legendas à tua medida** — OpenSubtitles e embutidas; cada um escolhe língua, tamanho, estilo e atraso |
| 🔊 | **Faixa de áudio** à escolha |
| 📺 | **Séries sem pausas** — «A seguir» no fim do episódio e avanço automático |
| 🐢 | **Torrent morto ou lento?** O host troca por outro num clique |
| 🔁 | **Fizeste F5?** Voltas ao mesmo filme, no mesmo segundo |
| 🛋️ | **O sofá** — vês quem está na sala, com foto e progresso de carregamento |
| 👑 | **Passa a coroa** a outra pessoa com um clique no sofá |

### ⌨️ Atalhos

| Tecla | Ação |
|:---:|---|
| <kbd>F</kbd> | Ecrã inteiro |
| <kbd>C</kbd> | Legendas e áudio |
| <kbd>M</kbd> | Mudo |
| <kbd>↑</kbd> <kbd>↓</kbd> | Volume |
| <kbd>Espaço</kbd> | Play / pausa *(só host)* |
| <kbd>←</kbd> <kbd>→</kbd> | Recuar / avançar 10 s *(só host)* |

---

## 🩺 Problemas comuns

<details>
<summary><b>Os meus amigos não conseguem abrir o link</b></summary>

- Confirma que **todos** estão ligados ao Radmin VPN, na mesma rede.
- Na primeira vez, a firewall tinha de ser **permitida** em redes privadas. Se carregaste em «Cancelar», vai a *Segurança do Windows → Firewall → Permitir uma aplicação* e ativa o couchSync.
- Usa o link da janelinha (botão «Copiar»), não `localhost` — esse só funciona no teu PC.
</details>

<details>
<summary><b>Aparece um aviso a dizer que o Stremio não está aberto</b></summary>

Abre o Stremio desktop (não basta a versão web) e deixa-o aberto enquanto vês. Acontece tanto ao host como aos amigos: cada um precisa do seu.
</details>

<details>
<summary><b>O vídeo fica sempre a carregar</b></summary>

O torrent pode estar morto ou lento — o cartão de carregamento avisa. O host pode carregar em **trocar** para escolher outro torrent do mesmo título (ou um **mais leve**).
</details>

<details>
<summary><b>Como host, abri pelo link 26.x.x.x e aparece tudo estranho</b></summary>

No teu PC usa sempre `http://localhost:8000`. Pelo IP do Radmin, o browser é tratado como se fosses um amigo — a app deteta isso e sugere o endereço certo.
</details>

<details>
<summary><b>Depois de F5 o vídeo não arranca</b></summary>

Os browsers às vezes bloqueiam o som automático depois de recarregar a página. Carrega em **«Continuar a ver»**.
</details>

<details>
<summary><b>O antivírus apagou o .exe</b></summary>

É um falso positivo comum em programas sem assinatura paga. Restaura o ficheiro e põe a pasta do couchSync nas exclusões do antivírus.
</details>

---

## 📜 Histórico

<details open>
<summary><b>0.2.0</b></summary>

- Agora é **um único `.exe`**: para atualizar basta trocá-lo.
- **Janelinha do couchSync** em vez da consola: versão, estado, se o Stremio está aberto, link dos amigos com «Copiar» e «Abrir no browser».
- Chave do **Real-Debrid** posta na janelinha, verificada na hora, sem reiniciar.
- O `.exe` apaga sozinho os ficheiros das versões antigas.
- Logo no separador do browser.
- No lobby, o logo passeia pelo fundo como o velho «DVD» 📀, com efeito VHS e festa quando acerta num canto.
</details>

<details>
<summary><b>0.1.0 — primeira versão de testes</b></summary>

- Salas sincronizadas, pausa para todos em buffering, entrar a meio.
- Catálogos e pesquisa, torrents, Real-Debrid opcional no host.
- Conversão automática só para quem precisa.
- Legendas do OpenSubtitles e embutidas.
- Faixa de áudio, próximo episódio, troca de torrents, sofá, fotos, sugestões com votos.
</details>

---

<p align="center">
  <sub>Feito para as noites de cinema com os amigos 🛋️🍿</sub>
</p>
