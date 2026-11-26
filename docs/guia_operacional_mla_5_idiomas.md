# Guia Operacional Definitivo — Multilíngue em 5 Idiomas (EN, DE, FR, ES, PT-BR)

Este manual documenta exatamente como operar **Anthroposium (`@anthroposium`)** em **5 idiomas simultâneos** sem perder retenção, sem dessincronizar cenas e sem desperdiçar esforço editorial.

---

## 1. Arquitetura por Plataforma (Resumo Executivo)

| Plataforma | Quantas contas? | Idiomas | Arquivo enviado |
| :--- | :---: | :--- | :--- |
| **YouTube** | **1 único canal** (`@anthroposium`) | Base `en-US` + MLA: `de`, `fr`, `es`, `pt-BR` | 1 único `master_16x9_clean.mp4` (universal, zero texto em inglês) + 4 faixas de áudio sincronizadas (`48 kHz`) + 5 `.srt` + 5 metadados/thumbnails |
| **TikTok** | **5 contas separadas** (`@anthroposium`, `.de`, `.fr`, `.es`, `.br`) | 1 idioma por conta | `vertical_9x16_burned_<lang>.mp4` (`70–90s`, legendas cinéticas queimadas no idioma nativo) |
| **Facebook** | Página principal `Anthroposium` (EN) + páginas regionais opcionais | 1 idioma por página | Mesmos MP4 verticais renderizados para o TikTok + cards visuais |

---

## 2. Configuração Inicial do Canal no YouTube Studio (Fazer 1 Única Vez)

1. **Criar o canal `@anthroposium`** e configurar o idioma padrão:
   - `YouTube Studio → Configurações → Padrões de envio → Configurações avançadas → Idioma do vídeo:` **`Inglês (Estados Unidos)`**.
2. **Ativar Recursos Avançados (pré-requisito obrigatório para subir faixas MLA manuais):**
   - `Configurações → Canal → Qualificação para recursos`:
     - *Recursos padrão* → ativo na criação.
     - *Recursos intermediários* → verificação por número de celular (SMS).
     - *Recursos avançados* → escolher **Verificação por vídeo** (30 segundos na câmera) ou **Documento de identidade válido**. Libera normalmente em **~24h**, sem precisar esperar 2 meses de histórico do canal.
3. **Controlar o Auto-Dubbing (Dublagem Automática do YouTube):**
   - Em `Configurações → Canal → Configurações avançadas` (ou nas opções de envio), **desative a publicação automática de dublagens automáticas** (ou exclua qualquer faixa automática gerada antes de enviar nossa faixa manual masterizada).
   - *Motivo:* A dublagem automática do YouTube substitui o nosso design sonoro `48 kHz` com Mid-Side Vocal Pocket por voz robótica chapada — e o YouTube bloqueia o upload manual de um idioma enquanto existir faixa automática ativa para ele.

---

## 3. Os 2 Pilares Técnicos da `DarkStudio Engine` para MLA 5 Idiomas

### Pilar A — Vídeo `16:9` 100% Universal (`universal_mla: true`)
Como 1 único `.mp4` é reproduzido para EUA, Alemanha, França, Espanha/LATAM e Brasil:
- **PROIBIDO** queimar legendas ou parágrafos em inglês na tela do `16:9`.
- **PERMITIDO** no HUD e Cartões Científicos (`data_card`):
  - **Números e grandezas universais:** `10⁴⁸`, `90.0%`, `US$ 2.6B`, `1957 → 1961`, `24`, `77 QUBITS`;
  - **Fórmulas químicas, genes e siglas internacionais:** `C₈H₁₀N₄O₂`, `FeMoco`, `CRBN`, `KRAS G12D`, `ATP`, `DNA`, `CRISPR`;
  - **Citações bibliográficas padrão científico:** `Feynman (1982)`, `Nature Reviews (2012)`, `Science Advances (2025)`, `Nature Biotech (2025)`;
  - **Marcações em algarismos romanos:** `ANTHROPOSIUM // I`, `II`, `III` e contador `01 / 24`.

### Pilar B — *Time-Locking* por Cena (`darkstudio.cli mla-sync`)
Idiomas latinos e germânicos (`DE`, `FR`, `ES`, `PT-BR`) tendem a ser **12%–22% mais longos** em palavras/sílabas do que o inglês. Se cada idioma rodar livre, as trocas de cena perdem sincronia em poucos minutos.

A `DarkStudio Engine` resolve isso automaticamente em 4 passos:
1. **Gera ou ingere a locução de cada cena** em todos os 5 idiomas (`en`, `de`, `fr`, `es`, `pt-br`).
2. **Calcula o Relógio Mestre por Cena (`master_scene_durations`):** define uma duração única travada por cena (baseada no *master* ou no tempo máximo entre os 5 idiomas com uma pequena margem musical de respiro de `0,35s`, ou aplica leve time-stretch preservando o pitch via FFmpeg `atempo` limitado entre `0.94×` e `1.08×` quando uma adaptação ficar ligeiramente maior que a janela).
3. **Monta 5 faixas de voz com a duração idêntica ao sample (`48.000 Hz`)**, todas virando cada cena exatamente no mesmo frame!
4. **Mixagem compartilhada:** sintetiza **1 único `music_stem_48khz.wav`** (alinhado aos `scene_starts` mestres) e aplica o **Mid-Side Smart Vocal Pocket** individualmente para cada uma das 5 vozes, gerando:
   - `master_16x9_clean.mp4` (vídeo universal + áudio `en` embutido)
   - `mla_audio_en.wav`, `mla_audio_de.wav`, `mla_audio_fr.wav`, `mla_audio_es.wav`, `mla_audio_pt-br.wav` (todos com a **exata mesma duração ao milissegundo!**)
   - `captions_en.srt`, `captions_de.srt`, `captions_fr.srt`, `captions_es.srt`, `captions_pt-br.srt`

---

## 4. Checklist de Publicação por Episódio no YouTube Studio

1. **Subir o Master (`Não listado`):**
   - Arquivo: `master_16x9_clean.mp4`
   - Idioma original: `Inglês (Estados Unidos)`
   - Título, descrição SEO, capítulos e `captions_en.srt` em inglês
   - Subir 3 variações de Thumbnail no *Test & Compare* (ou versões localizadas por idioma quando habilitado na aba *Idiomas*)
2. **Abrir `YouTube Studio → Idiomas` → selecionar o vídeo:**
   - Adicionar os 4 idiomas: **Alemão (`de`)**, **Francês (`fr`)**, **Espanhol (`es`)**, **Português (Brasil) (`pt-BR`)**.
3. **Para cada um dos 4 idiomas adicionados:**
   - `Título e descrição → Adicionar`: colar adaptação nativa;
   - `Áudio → Adicionar`: enviar `mla_audio_<lang>.wav` *(excluir antes qualquer rascunho de Auto-dubbing)*;
   - `Legendas → Adicionar`: enviar `captions_<lang>.srt`;
   - `Miniatura → Adicionar` *(quando disponível na conta)*: enviar thumbnail localizada daquele idioma.
4. **Auditoria obrigatória antes de publicar:**
   - Abrir o vídeo em *Não listado*, clicar em **Engrenagem → Faixa de áudio**, e alternar entre `EN`, `DE`, `FR`, `ES` e `PT-BR` em 3 marcas de tempo (início, meio e fim) confirmando que as viradas de cena e os cartões numéricos batem exatamente com a fala em todos os 5 idiomas.
5. **Agendamento Global Ideal:**
   - **14h00–15h30 (horário de Brasília)** = `12h00–13h30 EST (Nova York)` / `18h00–19h30 CET (Paris e Berlim)` — captura simultaneamente o horário nobre europeu (`DE`/`FR`/`ES`), o almoço/tarde norte-americano (`EN`) e a tarde brasileira (`PT-BR`).

---

## 5. Comando da `DarkStudio Engine` para Gerar o Pacote MLA Completo

```powershell
$env:PYTHONPATH = "D:\dark_studio_engine\src"
& "D:\producao_cynical\.venv\Scripts\python.exe" -m darkstudio.cli mla-sync D:\dark_studio_engine\examples\ep01_mla_5langs_demo.json --workers 3
```

Para disparar usando vozes reais Gemini TTS nos 5 idiomas, basta adicionar `--tts` ao final do comando.
