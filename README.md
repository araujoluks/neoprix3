# neoprix3 — Grand Prix 3 on modern Windows

*Português abaixo · English below*

---

## Português

Mod para o Grand Prix 3 (versão 1.13) no Windows 10/11: aceleração 3D via
dgVoodoo, widescreen de verdade (Hor+), espelho virtual no topo, FPS mais alto,
Alt+Tab sem travar e um menu de ajustes dentro do jogo (F11).

### Instalação

1. **dgVoodoo2** (necessário para a aceleração 3D): baixe a versão **2.87.6**
   em <https://github.com/dege-diosg/dgVoodoo2/releases>. Do zip, copie para a
   pasta do jogo **só** estes dois arquivos da pasta `MS\x86`:
   `DDraw.dll` e `D3DImm.dll`.
2. Copie para a pasta do jogo os arquivos deste pacote: `dinput.dll`,
   `gp3mod.ini` e `dgVoodoo.conf`.
3. Abra o `gp3mod.ini` num editor de texto e, em `[display]`, coloque a
   resolução do seu monitor em `width` e `height` (ex.: 2560 e 1440). A
   mesma resolução também precisa constar em `ExtraEnumeratedResolutions`
   no `dgVoodoo.conf`.
4. No jogo, em Options → Graphics, escolha a aceleração por hardware
   (Direct3D) e a sua resolução (ela aparece no lugar de 1280x1024).

Para desinstalar, apague `dinput.dll`, `gp3mod.ini`, `dgVoodoo.conf`,
`DDraw.dll` e `D3DImm.dll` da pasta do jogo.

### Uso

- **F11** durante a corrida (também com o jogo pausado) abre o menu:
  setas ↑↓ escolhem, ←→ (ou Enter) mudam, Esc fecha. As mudanças são
  gravadas no `gp3mod.ini`.
  - Virtual mirror: espelho no topo da tela, desligado ou 50–200%.
  - Mirror position: altura do espelho na tela (0% = colado no topo).
  - Field of view: campo de visão, 50–200%.
  - Widescreen (Hor+): em telas largas, mostra mais nas laterais em vez
    de esticar a imagem.
  - VSync: liga/desliga a espera pelo monitor (desligado = FPS estável).
  - Frame rate: FPS da corrida; vale a partir da próxima sessão (marcado
    com `*`). A física do jogo roda um passo por frame, então o FPS
    escolhido também é o passo da física.
- Todas as opções estão comentadas no `gp3mod.ini`.

### Problemas

O mod grava um `gp3mod.log` na pasta do jogo a cada execução. Abra uma issue
em <https://github.com/araujoluks/neoprix3/issues> com a descrição do problema
e esse arquivo anexado. Se uma linha começar com `SKIP`,
o seu executável é diferente do esperado e aquela parte do mod não foi
aplicada (o jogo continua funcionando normalmente).

---

## English

Mod for Grand Prix 3 (version 1.13) on Windows 10/11: 3D acceleration through
dgVoodoo, proper widescreen (Hor+), a virtual mirror at the top, higher frame
rate, Alt+Tab that does not break the game, and an in-game settings menu (F11).

### Install

1. **dgVoodoo2** (needed for 3D acceleration): download version **2.87.6**
   from <https://github.com/dege-diosg/dgVoodoo2/releases>. From the zip, copy
   **only** these two files from the `MS\x86` folder into the game folder:
   `DDraw.dll` and `D3DImm.dll`.
2. Copy this package's files into the game folder: `dinput.dll`,
   `gp3mod.ini` and `dgVoodoo.conf`.
3. Open `gp3mod.ini` in a text editor and, under `[display]`, set `width`
   and `height` to your monitor's resolution (e.g. 2560 and 1440). The same
   resolution must also be listed in `ExtraEnumeratedResolutions` in
   `dgVoodoo.conf`.
4. In the game, Options → Graphics, pick hardware acceleration (Direct3D)
   and your resolution (it shows up in place of 1280x1024).

To uninstall, delete `dinput.dll`, `gp3mod.ini`, `dgVoodoo.conf`,
`DDraw.dll` and `D3DImm.dll` from the game folder.

### Use

- **F11** in a race (also while paused) opens the menu: ↑↓ select, ←→ (or
  Enter) change, Esc closes. Changes are saved to `gp3mod.ini`.
  - Virtual mirror: mirror at the top of the screen, off or 50–200%.
  - Mirror position: how far down the screen the mirror sits (0% = top).
  - Field of view: 50–200%.
  - Widescreen (Hor+): on wide screens, shows more at the sides instead of
    stretching the picture.
  - VSync: wait for the monitor or not (off = steady frame rate).
  - Frame rate: race frame rate; applies from the next session (marked
    `*`). The game runs one physics step per frame, so this is also the
    physics step.
- Every option is commented in `gp3mod.ini`.

### Problems

The mod writes `gp3mod.log` to the game folder on every run. Open an issue at
<https://github.com/araujoluks/neoprix3/issues> with a description of the
problem and that file attached. A line starting with `SKIP` means
your executable differs from the expected one and that part of the mod was
not applied (the game keeps working as usual).
