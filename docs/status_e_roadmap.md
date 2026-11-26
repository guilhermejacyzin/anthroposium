# Status do Projeto, Decisões Estratégicas & Roadmap — Anthroposium

**Última atualização:** 26/11/2026  
**Repositório GitHub:** `https://github.com/guilhermejacyzin/anthroposium.git`  
**Diretório Local:** `D:\anthroposium`  
**Fase Atual:** **Etapa A (Fundação Intelectual, Auditoria de Marca, Persona Acusmática, Bios YT/TT/FB, Grade dos 15 Episódios e Arquitetura Técnica) concluída!** → Próximo passo: **reservar os handles `@anthroposium` hoje** nas 3 plataformas, gerar o Kit Visual `[An]` em `assets/` e produzir o **Episódio Piloto #01**.

---

## 1. Registro de Decisões Estratégicas (O "Porquê" de Cada Escolha)

| Dimensão | Decisão Travada | Fundamento |
| :--- | :--- | :--- |
| **Marca Global** | **`Anthroposium`** (`@anthroposium`) | 100% virgem no YouTube, TikTok, Facebook e marcas registradas; une *Anthropos* (Humanas) + *-ium* (Química/Ciência) + *Symposium*; zero palavra sensível para filtros de moderação; não exige tradução |
| **Idioma & Escala** | **EN-first (EUA/UK/CA/AU)** + **MLA nativo para PT-BR e ES** no YouTube; **contas separadas por idioma no TikTok** (`@anthroposium`, `.br`, `.es`) | Maximiza RPM (`US$ 9–20+` vs. `R$ 15–30`) e patrocínios em dólar (`US$ 25–60 CPM`), permitindo atingir US\$ 30k+/mês com 400k–900k views longas/mês |
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
- [x] Templates oficiais de roteiro (`templates/template_longo_ctv_3_atos.md` e `templates/template_short_vertical.md`)

---

## 3. Roadmap Acionável (Próximos 90 Dias)

### Semana 1 — Blindagem de Marca & Kit Visual
1. [ ] **Reservar imediatamente os handles** nas 3 plataformas:
   - YouTube: `@anthroposium` (configurar idioma original `English (US)` + traduções PT-BR e ES de `docs/identidade_visual_e_bios.md`)
   - TikTok: `@anthroposium` (EN), `@anthroposium.br` (PT-BR), `@anthroposium.es` (ES)
   - Facebook: Página `Anthroposium` (e opcionalmente `Anthroposium Brasil`)
   - Domínio (opcional): checar `anthroposium.com`
2. [ ] Gerar e salvar em `assets/` o **Kit Visual Oficial**:
   - `avatar_anthroposium_1024x1024.png` (símbolo `[An]` + dupla hélice Ouro/Ciano sobre `#0D1117`)
   - `banner_youtube_2560x1440.jpg` (área segura `1546 × 423` validada)
   - `capa_facebook_1640x624.png` (canto inferior esquerdo limpo)
   - `watermark_anthroposium_150x150.png` (PNG transparente)

### Semanas 2 a 4 — Motor Modular & Episódio Piloto #01
3. [ ] Construir o núcleo do **`DarkStudio Engine`** (`D:\dark_studio_engine\`) reutilizando e modularizando seus módulos já validados (TTS, Whisper+difflib, DSP `48 kHz` com Mid-Side, render paralelo por cena e correção do z-index de partículas).
4. [ ] Escrever e revisar com fontes primárias (*Nature/Science/PubMed/arXiv*) o **Episódio #01** (`en/longos/001_*.md` + adaptações nativas `pt-br/longos/` e `es/longos/`) — recomendação de estreia de impacto máximo: **Ep. #01 (Simulação Molecular & Computação Quântica na Medicina)** OU **Ep. #02 (Aqua Tofana & Nascimento da Toxicologia)** para abrir com altíssimo CTR imediato!
5. [ ] Renderizar `ep01_master_16x9_clean.mp4` (3 faixas de áudio MLA + 3 `.srt` + 3 thumbnails A/B *Test & Compare*) + **3 cortes verticais `9:16` (`65–90s`)** em EN, PT-BR e ES.

### Dias 31 a 90 — Cadência de Estúdio & Aprovação YPP
6. [ ] Publicar **6 documentários longos (`18–30 min`)** + **18 a 24 cortes verticais** distribuídos em YouTube, TikTok (`15–30 min` antes) e Facebook Reels.
7. [ ] Ativar captura de e-mail para ***The Anthroposium Brief*** (newsletter semanal) já no Episódio #03.
8. [ ] Atingir **YPP Nível 2** (`1.000 inscritos` + `4.000h`), auditar retenção por faixa MLA (EN vs. PT-BR vs. ES) e preparar mídia kit para os primeiros patrocínios diretos (`US$ 25–55 CPM`) + contratação de narrador humano EN.
