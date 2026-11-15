# 페이검 (0167 · Spinarak) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 1fb15ef · 2026-11-15T06:49:27.258Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(설계 주문 — 화풍 · 색 · 머리색 · 체형 · 장갑 폼 · 원작 특징 · 노출 · 구도 · 자세는 우리 것, 큰 실루엣은 목록에서 하나 + 원작에서 딴 제 아이디어 하나, 얼굴 · 눈색(우리 것이든 제 것이든) · 헤어스타일 · 화장 · 표정 · 장면(배경) · 타입 효과는 맡은 쪽이 지어 제 지시문을 쓴다, 둘째 장은 첫째와 확실히 다르게(자세는 같게)). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 167 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 올릴 파일 |
|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 942 | `2349150cb7b3` | `페이검_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 페이검_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1104 | `f5eb62927dcb` | `페이검_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 페이검_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1206 | `ff46601bbabb` | `페이검_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 페이검_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1201 | `59686398031a` | `페이검_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 페이검_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1252 | `de760990f928` | `페이검_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 페이검_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1149 | `3af3dc86f42b` | `페이검_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 페이검_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1207 | `4fbab1b0c5a6` | `페이검_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 페이검_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1117 | `805a96a40482` | `페이검_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 페이검_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1167 | `ae97f267a2d4` | `페이검_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 페이검_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1092 | `0dc0f40dbac0` | `페이검_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 페이검_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1175 | `37a857caa627` | `페이검_anime_25d_gloss_f_casual10.webp` |
| ◆ | casual90 | ① 페이검_light_anime_25d_gloss_f.webp | `casual90-prompt.txt` | 1030 | `252225efea68` | `페이검_anime_25d_gloss_f_casual90.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 무대·환상 | a stylised stage, editorial or fantasy setting not bound to a real year |
| 장소 | 런웨이 | a fashion runway under white spotlights |
| 역할 | — |  |
| 의상 | 란제리풍 · 보디수트 | a lingerie bodysuit with a scooped neckline, wide straps and lace side panels |
| 몸 자세 · 구도 | 옆으로 눕기 · full_body · 정면 | lying on her left side |
| 손 · 소품 동작 | floor_front · head_rest |  |

옷 종류 bodysuit + lingerie_set · 옷 색 카멜 · 초콜릿 (camel and chocolate brown) · 드러내기 sweetheart neckline, high-cut leg · 장면 칸 첫머리 action

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 목장 | a sunny ranch — a weathered wooden fence, hay bales and horses grazing in the distance |
| 역할 | — |  |
| 의상 | 할로윈 코스튬 · 마녀 | a dark witch costume — a plunging black velvet bodysuit under a sheer black chiffon cape, a crooked wide-brimmed pointed hat and sheer thigh-high stockings |
| 몸 자세 · 구도 | 서기 · chest_up · 3/4 정면 | standing |
| 손 · 소품 동작 | prop · out · 등불 · 등불을 들어 비춘다 | lifts a small hand lantern to chest height |

옷 종류 bodysuit + coat · 옷 색 블랙 · 차콜 (black with charcoal accents) · 상황 흘러내린 어깨끈 · 드러내기 deep V neckline, halter neck · 장면 칸 첫머리 place

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 공연장 대기실 | a backstage dressing room with a bulb-lit mirror, a vanity table and costume racks |
| 역할 | — |  |
| 의상 | 수영복 · 컷아웃 원피스 | a fully lined one-piece swimsuit with large cut-outs at the sides of the waist |
| 몸 자세 · 구도 | 서기 · environmental · 옆모습 | standing |
| 손 · 소품 동작 | prop · prop · 카메라 · 사진을 찍는다 | raises a camera to her eye to take a photo |

옷 종류 swimsuit · 옷 색 라벤더 · 플럼 (lavender and plum) · 드러내기 plunging neckline, open back · 장면 칸 첫머리 light

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 울타리 친 풀밭 마당 | an enclosed grassy courtyard with a low wooden fence |
| 역할 | — |  |
| 의상 | 무대·판타지 의상 · 인어 쇼 | a mermaid show costume — a scale-sequined bodice and a flowing chiffon wrap skirt |
| 몸 자세 · 구도 | 서기 · waist_up · 3/4 정면 | standing |
| 손 · 소품 동작 | prop · natural · 나무열매 간식 · 동료에게 간식을 내민다 | offers a small berry treat to her companion |

옷 종류 skirt · 옷 색 그레이 · 실버 (dove grey and silver) · 드러내기 sweetheart neckline, off-shoulder neckline · 장면 칸 첫머리 detail

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 마을 열매 시장 | a village market stall piled with fresh berries |
| 역할 | — |  |
| 의상 | 운동복 · 스키웨어 — 몸에 붙는 스키 수트 | a sleek fitted one-piece ski suit with goggles pushed up on her head |
| 몸 자세 · 구도 | 걷기 · three_quarter · 뒤 3/4 | walking |
| 손 · 소품 동작 | prop · down · 쇼핑백 · 쇼핑백을 든다 | carries a paper shopping bag at her side |

옷 종류 swimsuit · 옷 색 — · 장면 자유(자유 장면) · 드러내기 deep V neckline, cutout waist · 장면 칸 첫머리 action

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 비행 포켓몬 승강장 | an open landing terrace for Flying-Pokémon travel, with harness racks and a wind sock |
| 역할 | — |  |
| 의상 | 동탄룩 · 자동 — 계열 안에서 장면에 맞게 | a body-hugging, curve-tracing going-out outfit in the Korean 'Dongtan look' style |
| 몸 자세 · 구도 | 서기 · chest_up · 옆모습 | standing |
| 손 · 소품 동작 | prop · out · 몬스터볼 · 몬스터볼을 얼굴 옆에 든다 | raises a Poké Ball beside her face |

옷 종류 knit_top + skirt · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 plunging neckline, cropped hem · 장면 칸 첫머리 light

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 보드게임 라운지 | a cozy board-game lounge with shelves of game boxes and low tables |
| 역할 | — |  |
| 의상 | 평상복 · 터틀넥 + 퀼팅 조끼 + 바지 | a fine knit turtleneck under a quilted vest with straight trousers |
| 몸 자세 · 구도 | 의자에 앉기 · environmental · 정면 | seated on a chair |
| 손 · 소품 동작 | prop · lap · 잔·컵 · 잔을 든다 | holds a cup at chest height |

옷 종류 trousers + vest · 옷 색 — · 옷 자유 · 드러내기 sweetheart neckline, one-shoulder cut · 장면 칸 첫머리 place

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 베이커리 작업실 | a small bakery workroom with a floury wooden worktable and warm ovens |
| 역할 | — |  |
| 의상 | 신화 드레이프 · 이집트 리넨 | an Egyptian-inspired look — a sheer pleated linen sheath over an opaque inner slip dress, a broad jewelled collar and gold arm bands |
| 몸 자세 · 구도 | 서기 · face_close · 정면 | standing |
| 손 · 소품 동작 | shush · out |  |

옷 종류 dress + slip · 옷 색 옐로 · 머스터드 (butter yellow and mustard) · 드러내기 deep V neckline, backless · 장면 칸 첫머리 detail

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 바 | a neon-lit bar counter with backlit bottles |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 바디수트형 | a daring adult costume version of {costume}, cut as a high-cut bodysuit with sheer thigh-high tights |
| 몸 자세 · 구도 | 의자에 앉기 · full_body · 옆모습 | seated on a chair |
| 손 · 소품 동작 | prop · lap · 밥그릇 · 한 끼 · 그릇을 든다 | holds a bowl of hot food at chest height |

옷 종류 bodysuit + leggings · 옷 색 — · 드러내기 plunging neckline, bare midriff · 장면 칸 첫머리 place

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 쇼핑몰 | a shopping mall atrium with a fountain and glass railings |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 정비용 점프수트 | a fitted mechanic's work jumpsuit with rolled sleeves and no real logos |
| 몸 자세 · 구도 | 서기 · waist_up · 정면 | standing |
| 손 · 소품 동작 | thumbs_up · hip |  |

옷 종류 jumpsuit · 옷 색 코랄 · 오렌지 (coral and soft orange) · 드러내기 sweetheart neckline, high thigh slit · 장면 칸 첫머리 light

## ◆ casual90 — 캐릭터만의 컷(인형극 견습 · 노출 bold)

일상 열 장에 더하는 한 장 — 채울 칸이 없다. 막히면 같은 지시문으로 두 번 더(모두 세 번), 그래도 막히면 계획기 `--own --own-level` 로 한 단계 내려 다시 짓는다(IMAGE_RULES 3절 「캐릭터만의 컷」).

| 칸 | 표의 글 |
|---|---|
| 장소 | a small puppet theater backstage — a painted miniature stage, hanging marionettes, a spool rack of thread, a stool and lamp |
| 장면 | she is a puppeteer apprentice standing at the stage with both hands on a control bar, tangling the strings a little |
| 의상 | a puppeteer look fitted to her body — a dark vest over a fitted off-shoulder top and short skirt, bare shoulders and legs, fingerless gloves, a single thread spool on a cord |
| 도구 | a wooden puppet control bar with strings (sig_both) |
| 자세 추천 | camera_shot |
