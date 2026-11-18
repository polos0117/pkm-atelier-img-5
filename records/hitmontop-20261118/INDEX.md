# 카포에라 (0237 · Hitmontop) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 07fc935 · 2026-11-18T11:15:45.680Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(설계 주문 — 화풍 · 색 · 머리색 · 체형 · 장갑 폼 · 원작 특징 · 노출 · 구도 · 자세는 우리 것, 큰 실루엣은 목록에서 하나 + 원작에서 딴 제 아이디어 하나, 얼굴 · 눈색(우리 것이든 제 것이든) · 헤어스타일 · 화장 · 표정 · 장면(배경) · 타입 효과는 맡은 쪽이 지어 제 지시문을 쓴다, 첫째(-1)는 A안 — 타입 추천 실루엣 하나 + 원작에서 가장 알아보기 쉬운 형태 특징 하나를 장갑의 단면 · 겹침 · 절개에, 둘째(-2)는 B안 — 타입 · 특징에서 경장의 기능 하나를 골라 장갑판 · 기능 모듈 배치로 새 외곽(목록 밖도, 경장 폼 안에서), 둘 다 우리 설계의 Face · Hair 와 다른 얼굴 인상 · 머리 외곽(2026-11-18 세계컷 GPT 설계안), 자세는 같게). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` · 어느 안인지(`generation.plan: "A"` 첫째 · `"B"` 둘째 — 2026-11-18) · 설계 요약(`generation.summary` — 지시문 첫 줄 `SUMMARY:` 그대로, 다음 주문의 비슷한 등록작 찾기 `tools/design-near.cjs` 가 읽는다) 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**일상컷 게임 코스프레 한 장**(2026-11-15 — 필수, 상황 노출 자리) — 계획에 「게임 코스프레」 로 적힌 컷의 Outfit 줄은 게임 · 캐릭터 이름이 든 코스프레 글이다(실제 작품 이름을 쓰는 유일한 갈래). **캐릭터 이름이 적힌 줄은 그대로 그린다** — 주인공 하나 게임, 등장인물 많은 게임도 계획기가 캐릭터를 정한다(2026-11-16 — 세 공방이 그린 것 · 예약한 것과 안 겹치게, 목록을 다 쓰면 2회차). 기록 `generation.cosplay` 는 그 줄의 캐릭터 · 재단. **옛 계획에만**(2026-11-16 전에 짠 계획 — Outfit 줄 맨 앞이 「…」 인 1회차 pick 칸): 되면 먼저 계획기로 그 칸만 다시 짠다 — `node tools/casual-plan.cjs <카드> --recosplay --plan <계획 파일> --dir <이 폴더> --reserve --push`(장소 · 다른 칸은 그대로, 그 자리 지시문을 다시 쓴다). 그대로 그릴 때만 **맡은 쪽이 캐릭터를 고른다** — 괄호 안 「이미 쓴」 목록에 없는 그 게임의 캐릭터 하나를 골라, 「…」 자리에 캐릭터 이름 + 그 의상의 알아볼 색 · 조각 + 괄호 안 재단 글을 쓰고 괄호 주문은 지운다(그 줄만 — 다른 줄은 그대로). 고를 캐릭터가 더 없으면(다 썼거나 알아볼 만한 캐릭터가 없으면) 새로 지어내지 말고 **같은 자리의 `<자리>-again-prompt.txt`**(계획기가 쓴 캐릭터 가운데 덜 입은 하나 · 아직 안 입은 재단을 정해 둔 2회차 지시문)를 그대로 그린다 — 기록 `generation.cosplay` 는 그 지시문의 캐릭터 · 재단. 그 파일이 없으면(쓴 캐릭터가 아직 없다) 1회차로 고른다. 그래도 막히면 그 컷을 다시 짠다: `node tools/casual-plan.cjs <카드> --session <같은 세션> --keep <카드>:<다른 컷 번호> --cosplay-full <게임 열쇠> --reserve --push`. 그린 뒤 기록에 `generation.cosplay: { "game": "<게임 열쇠>", "character": "<그린 캐릭터 영어 이름 — 1회차는 채운 이름>", "cut": "<재단 열쇠>" }`(세 공방이 이 칸으로 쓴 캐릭터를 센다)와 실제로 넘긴 글(`submitted`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
**「재생성 금지」 는 이미 받은 그림에만.** 돌아온 그림은 노출이 세 보여도 다시 만들지 않는다(검수에 적기만). 그림이 안 돌아온 막힌 컷은 상관없다 — IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 low 까지 → 계획기로 다른 장면 → 다른 장소 묶음)를 끝까지 밟고, 다 막혔을 때만 비운다. 비운 컷은 `qa.json` skipped 에 `tries`(step · request_id · scene · group), 올리기 전 `python3 tools/casual-ledger.py skips <기록 폴더>` 가 통과해야 끝난 묶음이다.
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 237 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 올릴 파일 |
|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 923 | `8d734d88da58` | `카포에라_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 카포에라_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1248 | `135c35d9914f` | `카포에라_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 카포에라_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1274 | `bfb80268b911` | `카포에라_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 카포에라_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1297 | `ee22edf9df7c` | `카포에라_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 카포에라_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1298 | `a0ec6e3d9929` | `카포에라_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 카포에라_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1156 | `505b9835d4eb` | `카포에라_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 카포에라_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1238 | `b544cd44a367` | `카포에라_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 카포에라_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1221 | `579d2335b0b8` | `카포에라_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 카포에라_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1163 | `5aab7a6fc030` | `카포에라_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 카포에라_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1253 | `ec8b2c87d6ab` | `카포에라_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 카포에라_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1141 | `51d0d77f44d0` | `카포에라_anime_25d_gloss_f_casual10.webp` |
| ◆ | casual90 | ① 카포에라_light_anime_25d_gloss_f.webp | `casual90-prompt.txt` | 1148 | `9df63dd8a2b0` | `카포에라_anime_25d_gloss_f_casual90.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 침실 | her bedroom, an unmade bed and soft window light |
| 역할 | — |  |
| 의상 | 게임 코스프레 · 크롭 투피스 | a daring adult cosplay of Soraka from League of Legends — the costume's recognisable colours and parts, cut as a cropped top and a micro skirt or hot pants that bare the midriff |
| 몸 자세 · 구도 | 걷기 · three_quarter · 뒤 3/4 | walking |
| 손 · 소품 동작 | prop · down · 기타 · 기타를 든다 | carries an acoustic guitar by its neck at her side |

옷 종류 crop_top + skirt + trousers · 옷 색 — · 게임 코스프레 리그 오브 레전드 · Soraka(계획기가 정함) · 크롭 투피스 · 1회차 · 드러내기 sweetheart neckline, open back · 장면 칸 첫머리 detail

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 그루밍 매트 있는 방 | a sunny room with a grooming mat, a towel and a small brush basket |
| 역할 | — |  |
| 의상 | 목욕 차림 · 스파 가운 | a plush spa robe tied at the waist |
| 몸 자세 · 구도 | 기대 눕기 · waist_up · 정면 | reclining on her back |
| 손 · 소품 동작 | behind_head · prop · 책 · 책을 안는다 | holds a book closed against her chest |

옷 종류 robe · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 deep V neckline, high thigh slit · 장면 칸 첫머리 place

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 포켓몬 세계 부엌 | a sunny home kitchen in a Pokémon-world town, bowls of berries on the counter |
| 역할 | — |  |
| 의상 | 무대·판타지 의상 · 자동 — 계열 안에서 장면에 맞게 | a stage or fantasy costume |
| 몸 자세 · 구도 | 서기 · chest_up · 정면 | standing |
| 손 · 소품 동작 | prop · prop · 반죽 그릇과 거품기 · 밀가루를 체에 쳐서 넣는다 | taps flour from a small sieve into a mixing bowl of batter and a whisk |

옷 종류 coat + dress · 옷 색 핑크 · 로즈 — 더스티 로즈 (dusty rose pink) · 상황 젖은 옷 — 비 · 물 튐 · 드러내기 plunging neckline, mini length · 장면 칸 첫머리 action

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 클럽 | a nightclub with a dance floor under moving coloured lights and a velvet-rope queue at its door |
| 역할 | — |  |
| 의상 | 평상복 · 자동 — 계열 안에서 장면에 맞게 | everyday clothes that suit the place and activity |
| 몸 자세 · 구도 | 가장자리에 걸터앉기 · face_close · 옆모습 | perched on a ledge or edge |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 dress + leggings + slip · 옷 색 그레이 · 실버 — 실버 (pale silver grey) · 드러내기 sweetheart neckline, off-shoulder neckline · 장면 칸 첫머리 light

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 롤러장 | a roller rink under coloured lights |
| 역할 | — |  |
| 의상 | 직업복 · 사육 작업복 | work overalls over a fitted tank top and rubber boots |
| 몸 자세 · 구도 | 쪼그려 앉기 · full_body · 정면 | crouching low on her heels |
| 손 · 소품 동작 | prop · lap · 물총 · 물총에 물을 채운다 | fills a bright plastic water gun under a tap |

옷 종류 overalls + tank · 옷 색 — · 옷 자유 · 드러내기 deep V neckline, halter neck · 장면 칸 첫머리 action

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 숲길 조사지 | a forest trail edge with a marked trail post, used for wild Pokémon field surveys |
| 역할 | — |  |
| 의상 | 수영복 · 크로셰 비키니 | a fully lined crochet-knit bikini in a sunny resort colour |
| 몸 자세 · 구도 | 무릎 꿇기 · three_quarter · 옆모습 | kneeling on the ground |
| 손 · 소품 동작 | prop · prop · 작은 손 공구 · 공구를 천 위에 가지런히 늘어놓는다 | lays out a small screwdriver in a neat row on a cloth |

옷 종류 bikini · 옷 색 라벤더 · 플럼 — 모브 (dusty mauve) · 드러내기 plunging neckline, high-cut leg · 장면 칸 첫머리 detail

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 포켓몬 세계 빨래터 | a washing place by a water channel of a Pokémon-world town, stone basins, drying lines overhead and wet flagstones |
| 역할 | — |  |
| 의상 | 홈웨어 · 오프숄더 잠옷 셔츠 | a loose off-shoulder sleep shirt |
| 몸 자세 · 구도 | 위로 손 뻗기 · environmental · 3/4 정면 | standing close to a high shelf or line, reaching up to it |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 shirt · 옷 색 — · 장면 자유(자유 장면) · 드러내기 sweetheart neckline, cropped hem · 장면 칸 첫머리 place

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 기차 침대칸 | a night-train sleeper compartment with a narrow berth, a fold-down table and a small window |
| 역할 | — |  |
| 의상 | 란제리풍 · 사리 블라우스 응용 | a sari-blouse-inspired set with a short fitted top and a draped lower piece |
| 몸 자세 · 구도 | 기대 눕기 · environmental · 3/4 정면 | reclining on her back |
| 손 · 소품 동작 | behind_head · prop · 수박 한 조각 · 수박 한 조각을 내민다 | holds a wedge of watermelon out toward the camera |

옷 종류 blouse + traditional · 옷 색 옐로 · 머스터드 — 해바라기 노랑 (sunflower yellow) · 드러내기 deep V neckline, one-shoulder cut · 장면 칸 첫머리 light

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 작은 가게 | a small shop — a bookstore, record store or plant shop — with crowded shelves |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 바디수트형 | a daring adult costume version of {costume}, cut as a high-cut bodysuit with sheer thigh-high tights |
| 몸 자세 · 구도 | 작업대에 몸 숙이기 · waist_up · 뒤 3/4 | standing at a work surface, upper body leaning slightly forward over it, hips back and weight on both feet |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 bodysuit + leggings · 옷 색 — · 드러내기 plunging neckline, bare midriff · 장면 칸 첫머리 detail

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 축제 거리 | a festival street of lanterns, food stalls and paper decorations |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 유니폼풍 | a stylised uniform-inspired costume with crisp lapels and decorative epaulettes, no real insignia |
| 몸 자세 · 구도 | 한 발 올려 서기 · full_body · 정면 | standing with one foot up on a step, the other leg straight |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 uniform · 옷 색 세이지 · 올리브 — 에메랄드 (deep emerald green) · 드러내기 sweetheart neckline, cutout waist · 장면 칸 첫머리 light

## ◆ casual90 — 캐릭터만의 컷(팽이 체조 강사 · 노출 bold)

일상 열 장에 더하는 한 장 — 채울 칸이 없다. 막히면 같은 지시문으로 두 번 더(모두 세 번), 그래도 막히면 계획기 `--own --own-level` 로 한 단계 내려 다시 짓는다(IMAGE_RULES 3절 「캐릭터만의 컷」).

| 칸 | 표의 글 |
|---|---|
| 장소 | a sports center studio — padded floor mats, hanging pads, a mirror wall and a rack of gloves |
| 장면 | she is a spinning-fitness instructor sitting on a chair with her legs crossed, looking over a padded glove in one hand |
| 의상 | a sports instructor look fitted to her body — a fitted sports top and short training shorts with bare midriff and legs, a spiral-print sash tied at her waist |
| 도구 | a padded glove (sig_hold) |
| 자세 추천 | chair_cross_prop |
