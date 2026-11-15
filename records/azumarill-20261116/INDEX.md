# 마릴리 (0184 · Azumarill) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 8eaab62 · 2026-11-15T22:41:10.861Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(설계 주문 — 화풍 · 색 · 머리색 · 체형 · 장갑 폼 · 원작 특징 · 노출 · 구도 · 자세는 우리 것, 큰 실루엣은 목록에서 하나 + 원작에서 딴 제 아이디어 하나, 얼굴 · 눈색(우리 것이든 제 것이든) · 헤어스타일 · 화장 · 표정 · 장면(배경) · 타입 효과는 맡은 쪽이 지어 제 지시문을 쓴다, 둘째 장은 첫째와 확실히 다르게(자세는 같게)). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**일상컷 게임 코스프레 한 장**(2026-11-15 — 필수, 상황 노출 자리) — 계획에 「게임 코스프레」 로 적힌 컷의 Outfit 줄은 게임 · 캐릭터 이름이 든 코스프레 글이다(실제 작품 이름을 쓰는 유일한 갈래). 주인공 하나 게임 · 2회차(캐릭터 이름이 적힌 줄)는 그대로 그린다. **등장인물 많은 게임 1회차**(Outfit 줄 맨 앞이 「…」)는 **맡은 쪽이 캐릭터를 고른다** — 괄호 안 「이미 쓴」 목록에 없는 그 게임의 캐릭터 하나를 골라, 「…」 자리에 캐릭터 이름 + 그 의상의 알아볼 색 · 조각 + 괄호 안 재단 글을 쓰고 괄호 주문은 지운다(그 줄만 — 다른 줄은 그대로). 고를 캐릭터가 더 없으면(다 썼거나 알아볼 만한 캐릭터가 없으면) 새로 지어내지 말고 **같은 자리의 `<자리>-again-prompt.txt`**(계획기가 쓴 캐릭터 가운데 덜 입은 하나 · 아직 안 입은 재단을 정해 둔 2회차 지시문)를 그대로 그린다 — 기록 `generation.cosplay` 는 그 지시문의 캐릭터 · 재단. 그 파일이 없으면(쓴 캐릭터가 아직 없다) 1회차로 고른다. 그래도 막히면 그 컷을 다시 짠다: `node tools/casual-plan.cjs <카드> --session <같은 세션> --keep <카드>:<다른 컷 번호> --cosplay-full <게임 열쇠> --reserve --push`. 그린 뒤 기록에 `generation.cosplay: { "game": "<게임 열쇠>", "character": "<그린 캐릭터 영어 이름 — 1회차는 채운 이름>", "cut": "<재단 열쇠>" }`(세 공방이 이 칸으로 쓴 캐릭터를 센다)와 실제로 넘긴 글(`submitted`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 184 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 올릴 파일 |
|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 958 | `9ccfd8122788` | `마릴리_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 마릴리_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1089 | `90a2e20b01ff` | `마릴리_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 마릴리_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1224 | `8bc66275796d` | `마릴리_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 마릴리_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1137 | `0686921ce8d0` | `마릴리_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 마릴리_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1234 | `63eb88a76105` | `마릴리_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 마릴리_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1128 | `318f8137e037` | `마릴리_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 마릴리_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1212 | `447faad7b644` | `마릴리_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 마릴리_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1191 | `e5ff8d4300fd` | `마릴리_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 마릴리_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1096 | `a764f234c507` | `마릴리_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 마릴리_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1150 | `edd763407009` | `마릴리_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 마릴리_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1107 | `404e6fddd607` | `마릴리_anime_25d_gloss_f_casual10.webp` |
| ◆ | casual90 | ① 마릴리_light_anime_25d_gloss_f.webp | `casual90-prompt.txt` | 1008 | `9287d80896f0` | `마릴리_anime_25d_gloss_f_casual90.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 침실 | her bedroom, an unmade bed and soft window light |
| 역할 | — |  |
| 의상 | 게임 코스프레 · 원피스 수영복 | a daring adult cosplay of Link from The Legend of Zelda — Link's outfit — a green belted tunic, a long pointed green cap, brown leather belts and bracers, pale tights and brown boots, cut as a high-cut one-piece swimsuit |
| 몸 자세 · 구도 | 바닥에 앉기 · three_quarter · 3/4 정면 | sitting on the ground |
| 손 · 소품 동작 | chin_knee · floor_brace |  |

옷 종류 swimsuit · 옷 색 — · 게임 코스프레 젤다의 전설 · Link(링크) · 원피스 수영복 · 1회차 · 드러내기 sweetheart neckline, bare midriff · 장면 칸 첫머리 action

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 포켓몬 세계 돌계단 | a long outdoor stairway climbing through a town of a Pokémon-world town, lamps along the steps and rooftops below |
| 역할 | — |  |
| 의상 | 무대·판타지 의상 · 마법사 | a sorceress costume — an off-shoulder velvet robe gown with a jewelled belt and a crystal staff prop |
| 몸 자세 · 구도 | 서기 · face_close · 정면 | standing |
| 손 · 소품 동작 | v_sign · out |  |

옷 종류 dress + robe · 옷 색 레드 · 와인 (deep red and wine) · 드러내기 plunging neckline, backless · 장면 칸 첫머리 light

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 바 | a neon-lit bar counter with backlit bottles |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 코르셋형 | a daring adult costume version of {costume}, cut as a laced corset bustier with a short flared skirt |
| 몸 자세 · 구도 | 서기 · chest_up · 정면 | standing |
| 손 · 소품 동작 | wave · out |  |

옷 종류 lingerie_set + skirt · 옷 색 — · 드러내기 deep V neckline, strapless top · 장면 칸 첫머리 place

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 나무열매 과수원 | a sunny berry orchard of small trees heavy with ripe, colorful berries |
| 역할 | 나무열매 재배자 | a berry grower |
| 의상 | 휴양지 차림 · 와이드 팬츠와 밴도 | wide-leg palazzo trousers with a bandeau top and a wide-brimmed straw hat |
| 몸 자세 · 구도 | 서기 · waist_up · 3/4 정면 | standing |
| 손 · 소품 동작 | prop · pocket · 전지가위 · 전지가위로 잔가지를 친다 | prunes a small branch with a pair of pruning shears |

옷 종류 crop_top + trousers · 옷 색 — · 옷 자유 · 드러내기 sweetheart neckline, cropped hem · 장면 칸 첫머리 detail · 직접 입력 outfit

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 헌책 노점 | a second-hand book stall under an awning on a quiet street, crates of books on trestle tables and a folding stool |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 자동 — 계열 안에서 장면에 맞게 | a playful adult event costume inspired by an occupation or role — clearly a costume, not a real uniform, no real insignia |
| 몸 자세 · 구도 | 벽에 기대 서기 · chest_up · 3/4 정면 | standing, leaning back against a wall |
| 손 · 소품 동작 | arms_crossed · arms_crossed |  |

옷 종류 vest · 옷 색 스카이 · 네이비 (sky blue and navy) · 드러내기 plunging neckline, side cutouts · 장면 칸 첫머리 action

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 녹음실 | a foley recording booth with microphones and boxes of noisy props |
| 역할 | — |  |
| 의상 | 동탄룩 · 튜브탑 + 하이웨이스트 레깅스 | a tight tube top under an open cropped cardigan with glossy high-waisted leggings that outline the hips and legs |
| 몸 자세 · 구도 | 앉아 앞으로 기울이기 · environmental · 뒤 3/4 | seated, leaning slightly forward toward the table, forearms near its edge |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 cardigan + leggings · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 deep V neckline, cutout waist · 장면 칸 첫머리 place

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 여행 물품점 | a wooden travel-supply shop counter with route maps and feed pouches |
| 역할 | — |  |
| 의상 | 평상복 · 자동 — 계열 안에서 장면에 맞게 | everyday clothes that suit the place and activity |
| 몸 자세 · 구도 | 스툴·벤치에 옆으로 걸터앉기 · face_close · 정면 | seated sideways on a stool or bench, her torso turned toward the camera |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 shorts · 옷 색 핑크 · 로즈 (rose pink and blush) · 드러내기 sweetheart neckline, off-shoulder neckline · 장면 칸 첫머리 light

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 강가 선착장 | a wooden river dock above calm water |
| 역할 | — |  |
| 의상 | 란제리풍 · 사리 블라우스 응용 | a sari-blouse-inspired set with a short fitted top and a draped lower piece |
| 몸 자세 · 구도 | 걷기 · three_quarter · 3/4 정면 | walking |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 blouse + traditional · 옷 색 그레이 · 실버 (dove grey and silver) · 드러내기 deep V neckline, open back · 장면 칸 첫머리 detail

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 스티커 사진기 | an arcade photo-sticker booth under bright ring lights |
| 역할 | — |  |
| 의상 | 서브컬처 · 이모 | emo — a fitted striped long-sleeve top, a studded belt, skinny jeans and checkered sneakers |
| 몸 자세 · 구도 | 의자에 앉기 · environmental · 옆모습 | seated on a chair |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 trousers · 옷 색 — · 장면 자유(자유 장면) · 드러내기 plunging neckline, mini length · 장면 칸 첫머리 detail

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 목장 | a sunny ranch — a weathered wooden fence, hay bales and horses grazing in the distance |
| 역할 | — |  |
| 의상 | 수영복 · 링 장식 비키니 | a bikini joined at the centre and hips by polished metal rings |
| 몸 자세 · 구도 | 옆으로 눕기 · full_body · 뒤 3/4 | lying on her left side |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 bikini · 옷 색 블랙 · 차콜 (black with charcoal accents) · 드러내기 sweetheart neckline, high-cut leg · 장면 칸 첫머리 place

## ◆ casual90 — 캐릭터만의 컷(세차장 점장 · 노출 bold)

일상 열 장에 더하는 한 장 — 채울 칸이 없다. 막히면 같은 지시문으로 두 번 더(모두 세 번), 그래도 막히면 계획기 `--own --own-level` 로 한 단계 내려 다시 짓는다(IMAGE_RULES 3절 「캐릭터만의 컷」).

| 칸 | 표의 글 |
|---|---|
| 장소 | a hand car wash bay — a soapy car, a tall water hose reel, foam buckets, a drying rack of towels |
| 장면 | she is the car wash manager standing with one hand on her hip, looking over a gleaming car with a proud smile |
| 의상 | a car wash attendant look fitted to her body — a short wet-look vest over a fitted bikini-style crop top and short denim shorts, bare shoulders and legs, rubber sandals, a bubble-shaped pin on her vest |
| 도구 | — |
| 자세 추천 | hip_contra |
