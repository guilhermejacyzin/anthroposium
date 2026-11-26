# Status do Projeto, Decisões Estratégicas & Roadmap — Anthroposium

**Última atualização:** 26/11/2026  
**Repositório GitHub:** `https://github.com/guilhermejacyzin/anthroposium.git`  
**Diretório Local:** `D:\anthroposium`  
**Fase Atual:** **Etapas A (Fundação), B (Kit Visual `[An]`), C (Dossiê Científico + Roteiros Integrais EN/PT-BR/ES + 9 Cortes Verticais do Ep. #01) e D (`DarkStudio Engine v1.0` Modular Testada Ponta a Ponta) CONCLUÍDAS!** → Próximo passo operacional: **reservar os handles `@anthroposium` nas 3 plataformas**, revisar as escolhas de arte por cena e disparar o render final com voz Gemini TTS (`--tts`) ou narrador humano do Episódio Piloto #01.

---

## 1. Registro de Decisões Estratégicas (O "Porquê" de Cada Escolha)

| Dimensão | Decisão Travada | Fundamento |
| :--- | :--- | :--- |
| **Marca Global** | **`Anthroposium`** (`@anthroposium`) | 100% virgem no YouTube, TikTok, Facebook e marcas registradas; une *Anthropos* (Humanas) + *-ium* (Química/Ciência) + *Symposium*; zero palavra sensível para filtros de moderação; não exige tradução |
| **Idioma & Escala** | **1 Canal YouTube EN-first (EUA/UK/CA/AU)** + **MLA nativo em 5 idiomas (`EN`, `DE`, `FR`, `ES`, `PT-BR`)**; **contas separadas por idioma no TikTok** (`@anthroposium`, `.de`, `.fr`, `.es`, `.br`) | Maximiza RPM global (EUA/UK + DACH Alemanha/Suíça + França/Canadá) somando todas as views e horas de YPP em um único canal YouTube |
| **Posicionamento Editorial** | **Humanas no olhar + Ciência de fronteira no motor** — Fórmula dos 3 Atos (*História Humana → Autópsia Biológica/Química → Biotech, IA & Computação Quântica*) | Evita a armadilha do nicho estreito de "quântica pura" (~500k–2M pessoas) e captura o maior cluster intelectual do YouTube (**100M+ espectadores mensais**, equilíbrio ~50/50 de gênero, 22–54 anos) |
| **Formato Principal** | **2 a 4 Mini-Documentários/mês (`18–32 min`, `16:9` Smart TV, zero legendas queimadas)** + **3–4 cortes verticais `9:16` (`65–95s`) por episódio** | Captura a liderança da Smart TV (Nielsen 15,8% / Kantar IBOPE TV #1), multiplica *mid-rolls*, constrói catálogo evergreen de 5–10 anos e destrava TikTok Creator Rewards (`>60s`) |
| **Motor de Produção** | **`DarkStudio Engine` modular** (`D:\dark_studio_engine\`) — render paralelo por cena, áudio DSP `48 kHz` estéreo (Ato 1 Câmara → Ato 3 Strobe/Cosmos), saída dual `clean_master_16x9.mp4` + `burned_9x16.mp4` | Elimina a duplicação de scripts monolíticos de 1.000 linhas e reduz o custo marginal de produção para manter margem líquida acima de 75%–85% |
| **Estratégia de Voz** | **Fase 1:** `gemini-3.8-flash-tts` calibrado em registro documental BBC/Netflix; **Fase 2 (após US\$ 2k/mês):** narrador humano nativo em inglês na faixa EN | Elimina risco do *Auditory Uncanny Valley* em documentários longos e destrava patrocínios premium de US\$ 5k–15k por vídeo |

---

## 2. Concluído ✅

- [x] Auditoria global de marca e verificação de disponibilidade de `@anthroposium` (zero colisão no YouTube/TikTok/Facebook)
- [x] Criação da arquitetura completa em `D:\anthroposium` vinculada a `https://github.com/guilhermejacyzin/anthroposium.git`
- [x] `README.md` mestre + `.gitignore`
- [x] `docs/biblia_da_marca_e_persona.md` (persona acusmática, regras anti-slop e prompts vocais EN/PT-BR/ES)
- [x] `docs/identidade_visual_e_bios.md` (paleta *Museum Meets Quantum Lab*, logo `[An]`, tipografia e bios prontas YT/TT/FB)
- [x] `docs/metodo_tres_atos_e_grade_15_episodios.md` (fórmula dos 3 atos + 15 primeiros episódios no Nicho em T)
- [x] `docs/estrategia_monetizacao_e_crescimento.md` (equação US\$ 30k–80k+/mês, MLA, TikTok/FB e blindagem YPP)
- [x] `docs/arquitetura_darkstudio_engine.md` (projeto do motor Python modular dual 16:9 limpo + 9:16 burned)
- [x] **Kit Visual Oficial `[An]`** auditado e salvo em `assets/` (`avatar_anthroposium_1024x1024.png`, `banner_youtube_2560x1440.jpg`, `capa_facebook_1640x624.png`, `watermark_anthroposium_150x150.png`, `emblema_anthroposium_1024x1024.png` e `arte_base_thumbnail_1920x1080.png`)
- [x] Templates oficiais de roteiro (`templates/template_longo_ctv_3_atos.md` e `templates/template_short_vertical.md`)
- [x] **Dossiê Científico Verificado do Episódio #01** (`docs/dossie_cientifico_ep01.md`) com DOIs revisados por pares (Feynman 1982, Scannell 2012, Reiher 2017, Sun 2022, Lee 2023, AlphaFold 3 2024, Google Willow 2024, IBM SQD 2025, Insilico/Aspuru-Guzik KRAS 2025 + linha histórica Papiro de Ebers → Aspirina → Penicilina → Talidomida/Frances Kelsey)
- [x] **Guia Operacional Definitivo MLA 5 Idiomas** (`docs/guia_operacional_mla_5_idiomas.md`) cobrindo YouTube Studio, Recursos Avançados, controle de Auto-Dubbing, vídeo `16:9` universal e *time-locking* cena a cena
- [x] **5 Roteiros Longos Integrais (`~24–30 min` cada, sem resumos, nos 5 idiomas):**
  - `en/longos/001_quantum_medicine_simulation.md`
  - `de/longos/001_molekulare_simulation_quantenmedizin.md`
  - `fr/longos/001_simulation_moleculaire_medecine_quantique.md`
  - `es/longos/001_simulacion_molecular_medicina_cuantica.md`
  - `pt-br/longos/001_simulacao_molecular_medicina_quantica.md`
- [x] **15 Roteiros Completos de Cortes Verticais `9:16` (`70–85s`, otimizados para TikTok Creator Rewards + loop gramatical — 3 cortes × 5 idiomas):**
  - EN: `001a_caffeine_quantum_wall.md`, `001b_thalidomide_mirror_trap.md`, `001c_90_percent_drugs_fail_quantum.md`
  - DE: `001a_koffein_quantenmauer.md`, `001b_thalidomid_spiegelfalle.md`, `001c_90_prozent_medikamente_scheitern.md`
  - FR: `001a_cafeine_mur_quantique.md`, `001b_thalidomide_piege_miroir.md`, `001c_90_pourcent_medicaments_echouent.md`
  - ES: `001a_cafeina_muro_cuantico.md`, `001b_talidomida_trampa_espejo.md`, `001c_90_porciento_farmacos_fracasan.md`
  - PT-BR: `001a_cafeina_muro_quantico.md`, `001b_talidomida_armadilha_espelho.md`, `001c_90_porcento_remedios_falham.md`
- [x] **`DarkStudio Engine v1.1 (MLA 5 Idiomas)`** construída em `D:\dark_studio_engine\` (`config.py`, `tts.py`, `align.py`, `dsp_audio.py`, `compositor.py`, `mla.py`, `cli.py`) com modo **`universal_mla`** (vídeo `16:9` 100% livre de frases em inglês) + comando **`mla-sync`** gerando 5 faixas de áudio sincronizadas ao sample exato (`delta = 0`) + 5 `.srt` + 1 vídeo `16:9` universal testado ponta a ponta!

---

## 3. Roadmap Acionável (Próximos 90 Dias)

### Semana 1 — Blindagem de Marca & Vitrines
1. [ ] **Reservar imediatamente os handles** e subir as artes de `assets/` + bios de `docs/identidade_visual_e_bios.md`:
   - YouTube: `@anthroposium` (idioma original `English (US)` + traduções PT-BR e ES)
   - TikTok: `@anthroposium` (EN), `@anthroposium.br` (PT-BR), `@anthroposium.es` (ES)
   - Facebook: Página `Anthroposium` (e opcionalmente `Anthroposium Brasil`)
   - Domínio (opcional): checar `anthroposium.com`
2. [x] Gerar e validar visualmente o **Kit Visual Oficial `[An]`** em `assets/`

### Semanas 2 a 4 — Motor Modular & Episódio Piloto #01
3. [x] Construir e validar ponta a ponta o núcleo do **`DarkStudio Engine`** (`D:\dark_studio_engine\`) — TTS plugável + Whisper/SequenceMatcher + `.srt` automático + DSP `48 kHz` com Mid-Side Vocal Pocket + render paralelo por cena (`ProcessPoolExecutor` + FFmpeg concat) + z-index corrigido de partículas.
4. [x] Escrever e revisar com fontes primárias (*Nature/Science Advances/Nature Biotech/PNAS/Acta Pharm. Sin. B*) o **Episódio #01** completo em EN, PT-BR e ES + 9 cortes verticais `9:16` (`en/`, `pt-br/`, `es/`).
5. [ ] Gerar artes visuais por cena do Ep. #01 e disparar render final com voz (`--tts` ou `--voice-wav`) de `ep01_master_16x9_clean.mp4` (3 faixas MLA + 3 `.srt` + 3 thumbnails A/B *Test & Compare*) + **3 cortes verticais `9:16` (`70–85s`)** em EN, PT-BR e ES.

### Dias 31 a 90 — Cadência de Estúdio & Aprovação YPP
6. [ ] Publicar **6 documentários longos (`18–30 min`)** + **18 a 24 cortes verticais** distribuídos em YouTube, TikTok (`15–30 min` antes) e Facebook Reels.
7. [ ] Ativar captura de e-mail para ***The Anthroposium Brief*** (newsletter semanal) já no Episódio #03.
8. [ ] Atingir **YPP Nível 2** (`1.000 inscritos` + `4.000h`), auditar retenção por faixa MLA (EN vs. PT-BR vs. ES) e preparar mídia kit para os primeiros patrocínios diretos (`US$ 25–55 CPM`) + contratação de narrador humano EN.
