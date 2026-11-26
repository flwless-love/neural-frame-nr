<p align="center">
  <img src="media/neural-frame.png" alt="Neural Frame" width="380">
</p>

<h1 align="center">Neural Frame 2.2</h1>

<p align="center"><strong>Neural Rendering, Frame Gen e PS5 Streaming no Windows</strong></p>
<p align="center">
  <a href="#downloads">Downloads</a> ·
  <a href="#novidades-da-22">Novidades da 2.2</a> ·
  <a href="#como-usar">Como usar</a> ·
  <a href="#ps5-streaming">PS5 Streaming</a> ·
  <a href="#comunidade-e-apoio">Comunidade e apoio</a> ·
  <a href="#english">English</a>
</p>

## Downloads

Escolha a série da sua GPU NVIDIA RTX. As duas opções abaixo são da versão **2.2 para Windows**.

| Série | Arquitetura | Portátil | Instalador |
| --- | --- | --- | --- |
| **RTX 2000** | Turing | [Baixar ZIP][p20] | [Baixar EXE][i20] |
| **RTX 3000** | Ampere | [Baixar ZIP][p30] | [Baixar EXE][i30] |
| **RTX 4000** | Ada Lovelace | [Baixar ZIP][p40] | [Baixar EXE][i40] |
| **RTX 5000** | Blackwell | [Baixar ZIP][p50] | [Baixar EXE][i50] |

- **Portátil** · Extraia a pasta inteira do ZIP e abra `NeuralFrame.exe`.
- **Instalador** · Execute o EXE da sua série. Ele inclui os componentes NVIDIA Video Effects correspondentes para o NVIDIA Upscaling.

[Release 2.2 e notas completas](https://github.com/flwless-love/neural-frame-nr/releases/tag/v2.2) · [Versões anteriores](https://github.com/flwless-love/neural-frame-nr/releases)

## Novidades da 2.2

| Recurso | O que mudou |
| --- | --- |
| **Frame Gen** | Ajustes na cadência do VFG para reduzir pulos em giros de câmera e suavizar variações de FPS. Remoção automática de quadros duplicados aplicável durante a captura por placa em modos compatíveis. |
| **FPS real** | O painel mostra os FPS reais da fonte abaixo da latência. O indicador de Frame Gen mostra a taxa de saída. |
| **Neural Rendering** | Ajustes no fluxo óptico para reduzir piscadas, camadas controladas por slider e resoluções agrupadas na aba Qualidade. |
| **Painel e gravação** | Cores do painel acessíveis no topo, estatísticas do PC em cartão compacto e guia de captura para OBS com acesso ao plugin Spout2. |
| **PS5 Streaming** | Caminho adicional para obter o ID da PSN e relatórios que distinguem pausas na chegada do vídeo, na decodificação e na fila de exibição. |

A recuperação automática para o erro **CUDA 700** no **VFG Médio** é específica da série **RTX 4000**. A confirmação em jogo nos computadores afetados e a investigação de engasgos intermitentes via PSN continuam em andamento.

## Como usar

1. Escolha a entrada na tela inicial. Use **Placa de captura** para um console via HDMI, **Aplicativo ou jogo** para uma janela, **Área de trabalho** para um monitor ou **PS5 Streaming** para jogar pela rede.
2. Selecione a resolução, o formato de vídeo e a taxa de captura disponíveis na fonte. Clique em **Iniciar processamento**.
3. Abra o painel com **Home** e ajuste Qualidade, Frame Gen, Upscaling, Nitidez / Cor, HDR, Tela, Áudio ou Interface.
4. Use **Tela inicial** no painel para encerrar a sessão e trocar a entrada.

| Atalho padrão | Ação |
| --- | --- |
| **Home** | Abrir o painel durante a sessão |
| **F3** | Alternar Frame Gen |
| **F6** | Alternar Neural Rendering |
| **F11** | Alternar tela cheia |
| **F7** | Alternar o upscaling no PS5 Streaming compatível |
| **Alt + Esc** | Voltar à tela inicial |

### Frame Gen e quadros duplicados

Se sua placa de captura envia 60 FPS e o jogo roda a 30 FPS ou menos, experimente **Frame Gen → Captura → Remover quadros duplicados → Remoção automática**. O filtro acompanha as mudanças na imagem, e o VFG interpola entre os quadros distintos. Por exemplo, 27 FPS na fonte podem resultar em uma saída perto de 54 FPS com VFG 2×, conforme a carga e o ritmo da captura.

Use **Hyper Motion** na RTX 2000. O NVIDIA VFG é experimental na RTX 3000 e é o método recomendado nas séries RTX 4000 e RTX 5000.

### Neural Rendering e HDR

Cada camada pode usar uma resolução própria ou seguir a **Resolução padrão do NR**. O painel reúne intensidade, estilo, aparência, fonte de movimento e ajustes de resultado. Em **Interface**, você pode trocar as cores e ocultar o cartão de desempenho.

O **RTX Video HDR** converte SDR em HDR em um monitor compatível. Para um sinal já em HDR, use a configuração de HDR de entrada correspondente à fonte.

## PS5 Streaming

| Modo | Como conectar |
| --- | --- |
| **Rede local** | Ative o **Uso remoto** no PS5, encontre o console no aplicativo e informe o ID da PSN. O painel oferece duas opções para obter o ID. Use o código do PS5 para parear e conectar. |
| **Remoto via PSN** | Abra **Remoto via PSN**, autorize sua conta PlayStation, selecione o console e clique em **Conectar**. |
| **Controle pela rede com vídeo HDMI** | Conecte o PS5 pela rede para enviar comandos e use a placa HDMI como fonte de vídeo. |

Você pode ajustar codec, decodificação, bitrate e resolução do stream. Os modos de 30 ou 60 FPS são opções da transmissão. Para dúvidas de configuração no console, consulte o guia oficial. [Configurações de Uso remoto do PlayStation](https://www.playstation.com/pt-br/support/games/remote-play-settings/)

## OBS e suporte

Em **Saída para OBS → Como capturar**, veja como usar a captura de jogo ou o Spout2. A opção **Ocultar painel durante captura** permite tirar painéis e avisos da transmissão.

Se houver congelamento, queda de FPS ou engasgo, gere o ZIP pelo botão **Suporte / Logs** na mesma sessão. O relatório guarda o histórico de ajustes e ajuda a localizar onde começou a pausa. Envie o relatório pelo canal de suporte usado para acompanhar o caso.

## Comunidade e apoio

<p align="center">
  <a href="https://discord.com/invite/4UC2FZfZaw"><img alt="Discord da comunidade" src="https://img.shields.io/badge/Discord-Participar-5865F2?style=for-the-badge&amp;logo=discord&amp;logoColor=white"></a>
  <a href="https://www.youtube.com/@Zanitzada"><img alt="Canal Zanitzada no YouTube" src="https://img.shields.io/badge/YouTube-Zanitzada-BD2026?style=for-the-badge&amp;logo=youtube&amp;logoColor=white"></a>
  <a href="https://livepix.gg/zanit"><img alt="Apoiar pelo LivePix" src="https://img.shields.io/badge/LivePix-Apoiar-007D86?style=for-the-badge"></a>
</p>

<details>
  <summary>Apoiar pelo QR Code</summary>
  <p><a href="https://livepix.gg/zanit"><img src="media/livepix-zanit.png" alt="QR Code do LivePix do Zanit" width="160"></a></p>
</details>

Este repositório público reúne a documentação e os downloads do aplicativo. Os arquivos automáticos **Source code** do GitHub contêm os documentos e as imagens do repositório. Para executar o Neural Frame, use o ZIP ou EXE da tabela acima.

---

## English

**Neural Frame 2.2** brings real-time Neural Rendering, frame generation, upscaling and PS5 Remote Play to Windows. It can process video from an HDMI capture card, a game or app window, a desktop display, or a PS5 stream.

[Downloads for Windows](#downloads-for-windows) · [What's new](#whats-new-in-22) · [Getting started](#getting-started) · [PS5 Remote Play](#ps5-remote-play) · [Community and support](#community-and-support)

### Downloads for Windows

| NVIDIA GPU | Architecture | Portable | Installer |
| --- | --- | --- | --- |
| **RTX 2000 series** | Turing | [Download ZIP][p20] | [Download EXE][i20] |
| **RTX 3000 series** | Ampere | [Download ZIP][p30] | [Download EXE][i30] |
| **RTX 4000 series** | Ada Lovelace | [Download ZIP][p40] | [Download EXE][i40] |
| **RTX 5000 series** | Blackwell | [Download ZIP][p50] | [Download EXE][i50] |

- **Portable** · Extract the entire ZIP and run `NeuralFrame.exe`.
- **Installer** · Run the EXE for your GPU series. It includes the corresponding NVIDIA Video Effects components for NVIDIA Upscaling.

[Full 2.2 release notes](https://github.com/flwless-love/neural-frame-nr/releases/tag/v2.2) · [Previous releases](https://github.com/flwless-love/neural-frame-nr/releases)

### What's new in 2.2

| Feature | What changed |
| --- | --- |
| **Frame Gen** | Updated VFG pacing to reduce jumps during camera pans and smooth out variations in source frame rate. Automatic duplicate-frame removal can be enabled during supported capture-card sessions. |
| **Source and output FPS** | The performance panel shows actual source FPS below latency. The Frame Gen indicator shows output FPS. |
| **Neural Rendering** | Optical flow changes reduce flicker. Sliders control the layers, and the related resolution settings are grouped in the Quality tab. |
| **Interface and recording** | Panel colors are accessible from the top bar. The compact performance panel shows PC stats. The in-app OBS guide includes a link to the Spout2 plugin. |
| **PS5 Streaming** | An additional way to get your PSN account ID, plus support logs that distinguish gaps in video delivery, decoding and the display queue. |

The **RTX 4000 series** can attempt to recover from **CUDA error 700** by restarting VFG at Low quality after a Medium-quality failure. We are still validating this on affected computers and investigating intermittent PSN streaming stutters.

### Getting started

1. Choose your input. Select **Capture card** for an HDMI console, **Application or game** for a PC window, **Desktop** for a display, or **PS5 Streaming** to play over the network.
2. Pick the resolution, video format and capture frame rate your source offers, then start processing.
3. Press **Home** to open the settings panel. Use **F3** to toggle Frame Gen, **F6** to toggle Neural Rendering, and **F11** to switch fullscreen. **F7** toggles upscaling for supported PS5 Streaming sessions.
4. Return to the home screen from the panel or press **Alt + Esc** to change inputs.

If your capture card receives 60 FPS while the game runs at 30 FPS or less, try **Frame Gen → Capture → Remove duplicate frames → Automatic removal**. VFG interpolates between distinct source frames. For example, a 27 FPS source can produce close to 54 FPS in VFG 2×, depending on system load and frame pacing.

Use **Hyper Motion** on RTX 2000. NVIDIA VFG is experimental on RTX 3000 and recommended for RTX 4000 and RTX 5000. In Neural Rendering, each layer can use its own resolution or follow the default NR resolution. **RTX Video HDR** converts SDR video for HDR displays.

### PS5 Remote Play

| Connection | How to connect |
| --- | --- |
| **Local network** | Enable Remote Play on the PS5, find the console, and enter your PSN account ID. The app offers two ways to get the ID. Pair with the code shown on the console. |
| **Remote via PSN** | Open the remote mode, authorize your PlayStation account, choose the console, and connect. |
| **Remote controls with HDMI video** | Send controller input over the network while using the capture card as the video source. |

Set the stream resolution, frame rate, codec, decoder and bitrate in **PS5 Streaming**. [Official PlayStation Remote Play settings](https://www.playstation.com/en-us/support/games/remote-play-settings/)

### OBS and troubleshooting

Open **OBS output → How to capture** for instructions on Game Capture and Spout2. You can hide panels and notifications from recordings in the session settings.

If you see a freeze, FPS drop or stutter, generate a ZIP with **Support / Logs** during the same session. The report captures what changed and helps locate where the interruption began. Share the report through the support channel handling your case.

### Community and support

[Join the Discord](https://discord.com/invite/4UC2FZfZaw) · [Zanitzada on YouTube](https://www.youtube.com/@Zanitzada) · [Support the project on LivePix](https://livepix.gg/zanit)

This repository contains the public documentation and downloads. Use the portable ZIP or installer EXE to run the Windows app. GitHub's automatically generated **Source code** archives contain the repository's documents and images.

[p20]: https://github.com/flwless-love/neural-frame-nr/releases/download/v2.2/NeuralFrame-2.2-Portable-RTX2000.zip
[i20]: https://github.com/flwless-love/neural-frame-nr/releases/download/v2.2/NeuralFrame-Setup-2.2-RTX2000.exe
[p30]: https://github.com/flwless-love/neural-frame-nr/releases/download/v2.2/NeuralFrame-2.2-Portable-RTX3000.zip
[i30]: https://github.com/flwless-love/neural-frame-nr/releases/download/v2.2/NeuralFrame-Setup-2.2-RTX3000.exe
[p40]: https://github.com/flwless-love/neural-frame-nr/releases/download/v2.2/NeuralFrame-2.2-Portable-RTX4000.zip
[i40]: https://github.com/flwless-love/neural-frame-nr/releases/download/v2.2/NeuralFrame-Setup-2.2-RTX4000.exe
[p50]: https://github.com/flwless-love/neural-frame-nr/releases/download/v2.2/NeuralFrame-2.2-Portable-RTX5000.zip
[i50]: https://github.com/flwless-love/neural-frame-nr/releases/download/v2.2/NeuralFrame-Setup-2.2-RTX5000.exe
