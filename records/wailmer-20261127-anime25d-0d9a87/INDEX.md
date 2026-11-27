# 고래왕자 (0320 · Wailmer) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 acb8456 · 2026-11-27T02:33:58.176Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(칸 채우기 — 2026-11-18. 주문 아래 우리 경장 지시문을 그대로 싣고 칸만 비웠다: [HAIRSTYLE: …] 은 우리와 다른 헤어스타일, [ARMOR SILHOUETTE: …] 은 주문의 목록(그 타입 추천에서 우리 것 빼고)에서 하나를 글 그대로, Design idea 줄은 원작 형태 특징 하나를 장갑 구조에, [TYPE EFFECTS: …] 은 주문의 우리 효과 표에서 손 · 몸 · 주변 문장 하나씩 글 그대로(우리 것과 같아도 된다), [BODY TYPE: …] 은 우리 체형 목록(CARD_FIGURE · VOCAB_EN.body)에서 하나를 글 그대로(우리 것 그대로도 된다 — 2026-11-18 「피부랑 체형까지는 바꿈 허용해줘」), Face 줄은 얼굴 칸 일곱([FACE SHAPE] · [JAW] · [EYE SHAPE] · [EYE COLOUR] · [BROWS] · [NOSE] · [LIPS] — 칸마다 얼굴 설계표 선택지에서 우리 것 말고 하나를 글 그대로, 두 장도 칸마다 서로 다르게 — 2026-11-19 「Face 쪽은 다 다르게로 하자」), Impression(피부색 · 화장 · 표정) 줄은 고쳐도 되고 Setting detail 은 채우거나 지운다 — 나머지 줄은 글자 그대로, 첫 줄 SUMMARY:, 두 장은 헤어스타일 · 실루엣이 서로 다르게. 그리기 전에 `node tools/world-fill-check.cjs <이 폴더> <채운 글> --other <다른 장>` 이 통과해야 하고, 그릴 때는 SUMMARY 줄을 뺀 채운 글 그대로). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` · 몇째 설계인지(`generation.plan: "A"` 첫째 · `"B"` 둘째 — 2026-11-18) · 설계 요약(`generation.summary` — 지시문 첫 줄 `SUMMARY:` 그대로, 다음 주문의 비슷한 등록작 찾기 `tools/design-near.cjs` 가 읽는다) 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**일상컷 게임 코스프레 한 장**(2026-11-15 — 필수, 상황 노출 자리) — 계획에 「게임 코스프레」 로 적힌 컷의 Outfit 줄은 게임 · 캐릭터 이름이 든 코스프레 글이다(실제 작품 이름을 쓰는 유일한 갈래). **캐릭터 이름이 적힌 줄은 그대로 그린다** — 주인공 하나 게임, 등장인물 많은 게임도 계획기가 캐릭터를 정한다(2026-11-16 — 세 공방이 그린 것 · 예약한 것과 안 겹치게, 목록을 다 쓰면 2회차). 기록 `generation.cosplay` 는 그 줄의 캐릭터 · 재단. **옛 계획에만**(2026-11-16 전에 짠 계획 — Outfit 줄 맨 앞이 「…」 인 1회차 pick 칸): 되면 먼저 계획기로 그 칸만 다시 짠다 — `node tools/casual-plan.cjs <카드> --recosplay --plan <계획 파일> --dir <이 폴더> --reserve --push`(장소 · 다른 칸은 그대로, 그 자리 지시문을 다시 쓴다). 그대로 그릴 때만 **맡은 쪽이 캐릭터를 고른다** — 괄호 안 「이미 쓴」 목록에 없는 그 게임의 캐릭터 하나를 골라, 「…」 자리에 캐릭터 이름 + 그 의상의 알아볼 색 · 조각 + 괄호 안 재단 글을 쓰고 괄호 주문은 지운다(그 줄만 — 다른 줄은 그대로). 고를 캐릭터가 더 없으면(다 썼거나 알아볼 만한 캐릭터가 없으면) 새로 지어내지 말고 **같은 자리의 `<자리>-again-prompt.txt`**(계획기가 쓴 캐릭터 가운데 덜 입은 하나 · 아직 안 입은 재단을 정해 둔 2회차 지시문)를 그대로 그린다 — 기록 `generation.cosplay` 는 그 지시문의 캐릭터 · 재단. 그 파일이 없으면(쓴 캐릭터가 아직 없다) 1회차로 고른다. 그래도 막히면 그 컷을 다시 짠다: `node tools/casual-plan.cjs <카드> --session <같은 세션> --keep <카드>:<다른 컷 번호> --cosplay-full <게임 열쇠> --reserve --push`. 그린 뒤 기록에 `generation.cosplay: { "game": "<게임 열쇠>", "character": "<그린 캐릭터 영어 이름 — 1회차는 채운 이름>", "cut": "<재단 열쇠>" }`(세 공방이 이 칸으로 쓴 캐릭터를 센다)와 실제로 넘긴 글(`submitted`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
**「재생성 금지」 는 이미 받은 그림에만.** 돌아온 그림은 노출이 세 보여도 다시 만들지 않는다(검수에 적기만). 그림이 안 돌아온 막힌 컷은 상관없다 — IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 low 까지 → 계획기로 다른 장면 → 다른 장소 묶음)를 끝까지 밟고, 다 막혔을 때만 비운다. 비운 컷은 `qa.json` skipped 에 `tries`(step · request_id · scene · group), 올리기 전 `python3 tools/casual-ledger.py skips <기록 폴더>` 가 통과해야 끝난 묶음이다.
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 320 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 크기 | 올릴 파일 |
|---|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 856 | `e784b0eb0431` | 2:3 1024×1536 | `고래왕자_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 고래왕자_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1335 | `7f133ff647d5` | 2:3 1024×1536 | `고래왕자_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 고래왕자_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1247 | `efa0e110256b` | 2:3 1024×1536 | `고래왕자_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 고래왕자_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1465 | `edcdd0e3ab46` | 2:3 1024×1536 | `고래왕자_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 고래왕자_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1256 | `5857d134a143` | 1:1 1024×1024 | `고래왕자_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 고래왕자_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1157 | `053c28bdf0ed` | 2:3 1024×1536 | `고래왕자_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 고래왕자_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1254 | `4802521c7125` | 2:3 1024×1536 | `고래왕자_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 고래왕자_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1301 | `d7fc1eca6e01` | 2:3 1024×1536 | `고래왕자_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 고래왕자_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1174 | `5d46eeea10ad` | 3:2 1536×1024 | `고래왕자_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 고래왕자_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1315 | `c9f95ad896d6` | 2:3 1024×1536 | `고래왕자_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 고래왕자_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1227 | `e38e1613ddb4` | 2:3 1024×1536 | `고래왕자_anime_25d_gloss_f_casual10.webp` |
| ◆ | casual90 | ① 고래왕자_light_anime_25d_gloss_f.webp | `casual90-prompt.txt` | 1147 | `6a5f5506eb25` | 1:1 1024×1024 | `고래왕자_anime_25d_gloss_f_casual90.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 범퍼카 | a bumper-car arena under a ring of coloured bulb lights, little padded cars with tall poles on a shiny floor |
| 역할 | — |  |
| 의상 | 웨딩 · 2부 미니드레스 | a short beaded after-party wedding dress |
| 몸 자세 · 구도 | 의자에 앉기 · face_close · 3/4 정면 | seated on a chair |
| 손 · 소품 동작 | prop · out · 표 · 승차권 · 표를 얼굴 옆에 들어 보인다 | holds up a paper ticket beside her face |

옷 종류 dress · 옷 색 레드 · 와인 — 버건디 (dark burgundy) · 드러내기 sweetheart neckline, strapless top · 장면 칸 첫머리 detail

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 캠퍼스 잔디밭 | a sunny campus lawn under old trees, ivy-covered brick buildings around it and a few students resting on the grass far off |
| 역할 | — |  |
| 의상 | 레트로 · 50년대 핀업 란제리 | a 1950s pin-up lingerie set with a structured bra and high-waisted bottoms |
| 몸 자세 · 구도 | 가장자리에 걸터앉기 · three_quarter · 뒤 3/4 | perched on a ledge or edge |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 lingerie_set · 옷 색 — · 장면 자유(자유 장면) · 드러내기 deep V neckline, high-cut leg · 장면 칸 첫머리 action

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 양궁장 | an archery range of targets on a green field |
| 역할 | — |  |
| 의상 | 직업복 · 글래머 연구복 | a cropped fitted lab coat over a silk camisole and a high-waisted pencil skirt |
| 몸 자세 · 구도 | 난간·창턱에 기대 서기 · waist_up · 뒤 3/4 | standing at a waist-high railing or sill |
| 손 · 소품 동작 | rail · natural |  |

옷 종류 coat + skirt + tank · 옷 색 — · 옷 자유 · 드러내기 plunging neckline, cutout waist · 장면 칸 첫머리 place

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 무대·환상 | a stylised stage, editorial or fantasy setting not bound to a real year |
| 장소 | 공중 정원 | a floating sky garden of hanging vines and flowering terraces above the clouds |
| 역할 | — |  |
| 의상 | 저녁 드레스 · 슬립 위 실크 로브 | a silk robe over an evening slip |
| 몸 자세 · 구도 | 위로 손 뻗기 · three_quarter · 옆모습 | standing close to a high shelf or line, reaching up to it |
| 손 · 소품 동작 | reach_high · natural |  |

옷 종류 robe + slip · 옷 색 라벤더 · 플럼 — 바이올렛 (rich violet) · 상황 흘러내린 어깨끈 · 드러내기 sweetheart neckline, high thigh slit · 장면 칸 첫머리 light

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 요트 조타석 | the helm of a white sailing yacht heeling gently on a blue sea, the wheel in front of her and taut sails above |
| 역할 | — |  |
| 의상 | 수영복 · 조개 컵 비키니 | a bikini with moulded shell-shaped cups and sculpted high-cut bikini bottoms |
| 몸 자세 · 구도 | 서기 · full_body · 3/4 정면 | standing |
| 손 · 소품 동작 | wheel_both · wheel_both |  |

옷 종류 bikini · 옷 색 핑크 · 로즈 — 파우더 핑크 (pale powder pink) · 드러내기 deep V neckline, bare midriff · 장면 칸 첫머리 detail

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 수리 가게 작업대 | a small repair kiosk with a cluttered workbench, a low stool, tools hanging on the wall and an open shutter onto the street |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 바디수트형 | a daring adult costume version of {costume}, cut as a high-cut bodysuit with sheer thigh-high tights |
| 몸 자세 · 구도 | 서기 · chest_up · 정면 | standing |
| 손 · 소품 동작 | reach · out |  |

옷 종류 bodysuit + leggings · 옷 색 — · 드러내기 plunging neckline, mini length · 장면 칸 첫머리 light

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 길가 노점 | a small roadside stall with a counter, a juice pitcher and steaming pots |
| 역할 | — |  |
| 의상 | 운동복 · 스키웨어 — 몸에 붙는 스키 수트 | a sleek fitted one-piece ski suit with goggles pushed up on her head |
| 몸 자세 · 구도 | 스툴·벤치에 옆으로 걸터앉기 · waist_up · 뒤 3/4 | seated sideways on a stool or bench |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 swimsuit · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 sweetheart neckline, halter neck · 장면 칸 첫머리 action

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 강변 자전거 길 | a sunny riverside cycle path, a bicycle beneath her, reeds and a low stone wall along the water |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 유니폼풍 | a stylised uniform-inspired costume with crisp lapels and decorative epaulettes, no real insignia |
| 몸 자세 · 구도 | 쪼그려 앉기 · environmental · 3/4 정면 | crouching down low |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 uniform · 옷 색 옐로 · 머스터드 — 머스터드 (deep mustard yellow) · 드러내기 deep V neckline, off-shoulder neckline · 장면 칸 첫머리 place

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 재즈바 | a dim jazz bar with a grand piano |
| 역할 | — |  |
| 의상 | 란제리풍 · 자동 — 계열 안에서 장면에 맞게 | tasteful lingerie-inspired fashion, fully opaque and securely fitted, with full intimate coverage |
| 몸 자세 · 구도 | 카메라 쪽으로 상체 숙이기 · chest_up · 옆모습 | standing and leaning her upper body forward toward the camera from the hips, her back gently arched and her shoulders lowered toward the viewer, as if leaning in close |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 skirt + traditional · 옷 색 민트 · 틸 — 딥 틸 (deep teal) · 드러내기 deep V neckline, one-shoulder cut · 장면 칸 첫머리 action

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 테마 카페 | a themed concept café of pastel booths, a frilled counter with cake stands and a small photo corner of paper flowers |
| 역할 | — |  |
| 의상 | 게임 코스프레 · 바디수트 | a daring adult cosplay of Keith from Langrisser II — the costume's recognisable colours and parts, cut as a high-cut bodysuit with sheer thigh-high stockings |
| 몸 자세 · 구도 | 벽에 기대 서기 · environmental · 뒤 3/4 | standing, leaning back against a wall |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 bodysuit · 옷 색 — · 게임 코스프레 랑그릿사 II · Keith(계획기가 정함) · 바디수트 · 1회차 · 드러내기 plunging neckline, cropped hem · 장면 칸 첫머리 detail

## ◆ casual90 — 캐릭터만의 컷(세차 견습 · 노출 bold)

일상 열 장에 더하는 한 장 — 채울 칸이 없다. 막히면 같은 지시문으로 두 번 더(모두 세 번), 그래도 막히면 계획기 `--own --own-level` 로 한 단계 내려 다시 짓는다(IMAGE_RULES 3절 「캐릭터만의 컷」).

| 칸 | 표의 글 |
|---|---|
| 장소 | a car wash bay — a foam brush rack, a rinse bay, a drain grate |
| 장면 | she is a trainee attendant holding a hose in both hands, splashed with water |
| 의상 | a car wash attendant look fitted to her body — a short waterproof apron over a halter top and short shorts, bare shoulders and legs, rubber boots, a blue towel over her shoulder |
| 도구 | a high-pressure water hose (sig_both) |
| 자세 추천 | camera_shot |
