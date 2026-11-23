# DevSecOps Logo 3D Simulator

**[English](#english) · [Português](#português)**

---

## English

An interactive 3D simulator for the DevSecOps infinity logo (Dev · Sec · Ops, with the PLAN, CODE, BUILD, TEST, RELEASE, DEPLOY, OPERATE and MONITOR arrows). The logo is built as a double-sided medallion in high relief with [three.js](https://threejs.org/), and it can be exported as STL files for multi-color 3D printing.

### Features

- Parametric geometry: two rings joined by two straight bands at ±45°, tangent to the rings. The arrows have chevron tips, and the cream grooves have the same width everywhere.
- A double-sided medallion: the back is the front rotated 180°, so it reads correctly from behind. "Sec" is a single piece that goes through the medallion, so it appears mirrored on the back.
- Two base modes: **Solid plate** or **Cutout** (*vazado*), where the Dev and Ops centers are hollow.
- Three render modes: solid + wireframe, wireframe only, and polished solid.
- A relief height slider, and Front / 3D profile / Back camera presets.
- **STL export**: one file per color (cream, dark brown, medium brown), in millimeters, at the width you choose. All three files share the same coordinates, so they line up automatically in the slicer.

### What you need to install

**Nothing.** The simulator is a single HTML file. It needs:

- A modern browser with WebGL (Chrome, Edge, Firefox or Safari).
- An internet connection. three.js `0.169.0` and the Helvetiker Bold font load from the jsDelivr CDN.

Optional: Python 3 or Node.js, to serve the folder locally (recommended).

### How to run

Use a local server (recommended):

```bash
git clone https://github.com/mbastida43/devsecops_logo3D_simulator.git
cd devsecops_logo3D_simulator
python -m http.server 8000        # or: npx serve .
```

Then open <http://localhost:8000>.

You can also open `index.html` directly in the browser.

### How to use

| Control | What it does |
|---|---|
| Drag (left mouse button) | Rotates 360° |
| Scroll wheel | Zoom |
| Right mouse button | Pan |
| **Render mode** | Solid + wireframe / wireframe only / polished solid |
| **Base structure** | Solid plate / Cutout |
| **Relief height** | Relief thickness on each face |
| **Camera** | Front / 3D profile / Back |
| **3D printing → Export STL** | Downloads 3 STL files at the width in mm you set |

#### 3D printing tips

- Import the 3 STL files **together as parts of one object** (Bambu Studio, PrusaSlicer, Cura) and assign one filament to each.
- Print in **Solid plate** mode. In Cutout mode, the Dev and Ops letters sit loose inside the holes.
- At 150 mm wide, the piece is about 150 × 89 × 6 mm: a 2.5 mm plate with about 1.5 mm of relief on each side. Because it is double-sided, printing it flat needs supports underneath.
- Chrome may ask you to allow **multiple downloads**. Allow it, or only the first file will download.

### License

[MIT](LICENSE) © 2026 Marlon Bastida

---

## Português

Simulador 3D interativo do logo DevSecOps em forma de infinito (Dev · Sec · Ops, com as setas PLAN, CODE, BUILD, TEST, RELEASE, DEPLOY, OPERATE e MONITOR). O logo é montado como um medalhão dupla face em alto-relevo com [three.js](https://threejs.org/) e pode ser exportado em STL para impressão 3D multicolorida.

### Recursos

- Geometria paramétrica: dois anéis ligados por duas faixas retas a ±45°, tangentes aos anéis. As setas têm pontas em chevron e os sulcos creme têm a mesma largura em todo lugar.
- Medalhão dupla face: o verso é a frente girada 180°, então fica legível por trás. O "Sec" é uma peça única que atravessa o medalhão, por isso aparece espelhado no verso.
- Dois modos de base: **Placa Base** (sólida) ou **Vazado**, com os centros Dev e Ops furados.
- Três modos de renderização: sólido + malha, apenas malha e sólido polido.
- Controle da altura do relevo e câmeras prontas: Frente, Perfil 3D e Verso.
- **Exportação STL**: um arquivo por cor (creme, marrom escuro e marrom médio), em milímetros, na largura que você escolher. Os três arquivos usam as mesmas coordenadas e se alinham sozinhos no fatiador.

### O que precisa instalar

**Nada.** O simulador é um único arquivo HTML. Ele precisa de:

- Um navegador moderno com WebGL (Chrome, Edge, Firefox ou Safari).
- Conexão com a internet. O three.js `0.169.0` e a fonte Helvetiker Bold são carregados do CDN jsDelivr.

Opcional: Python 3 ou Node.js, para servir a pasta localmente (recomendado).

### Como rodar

Com um servidor local (recomendado):

```bash
git clone https://github.com/mbastida43/devsecops_logo3D_simulator.git
cd devsecops_logo3D_simulator
python -m http.server 8000        # ou: npx serve .
```

Depois abra <http://localhost:8000>.

Também dá para abrir o `index.html` direto no navegador.

### Como usar

| Controle | Função |
|---|---|
| Arrastar (botão esquerdo) | Gira 360° |
| Roda do mouse | Zoom |
| Botão direito | Move o logo |
| **Modo de Renderização** | Sólido + Malha / Apenas Malha / Sólido Polido |
| **Estrutura da Base** | Placa Base / Vazado |
| **Altura do Relevo** | Espessura do relevo em cada face |
| **Câmera** | Frente / Perfil 3D / Verso |
| **Impressão 3D → Exportar STL** | Baixa 3 arquivos STL na largura em mm informada |

#### Dicas de impressão 3D

- Importe os 3 STL **juntos, como partes de um mesmo objeto** (Bambu Studio, PrusaSlicer, Cura) e escolha um filamento para cada.
- Imprima no modo **Placa Base**. No modo Vazado, as letras Dev e Ops ficam soltas dentro dos furos.
- Com 150 mm de largura, a peça fica com cerca de 150 × 89 × 6 mm: placa de 2,5 mm e relevo de cerca de 1,5 mm de cada lado. Como é dupla face, imprimir deitada exige suporte embaixo.
- O Chrome pode pedir permissão para **vários downloads**. Aceite, senão só o primeiro arquivo baixa.

### Licença

[MIT](LICENSE) © 2026 Marlon Bastida
