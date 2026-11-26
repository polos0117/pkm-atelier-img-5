# 샤크니아 (0319 · Sharpedo) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 bec707b · 2026-11-26T23:26:13.310Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(칸 채우기 — 2026-11-18. 주문 아래 우리 경장 지시문을 그대로 싣고 칸만 비웠다: [HAIRSTYLE: …] 은 우리와 다른 헤어스타일, [ARMOR SILHOUETTE: …] 은 주문의 목록(그 타입 추천에서 우리 것 빼고)에서 하나를 글 그대로, Design idea 줄은 원작 형태 특징 하나를 장갑 구조에, [TYPE EFFECTS: …] 은 주문의 우리 효과 표에서 손 · 몸 · 주변 문장 하나씩 글 그대로(우리 것과 같아도 된다), [BODY TYPE: …] 은 우리 체형 목록(CARD_FIGURE · VOCAB_EN.body)에서 하나를 글 그대로(우리 것 그대로도 된다 — 2026-11-18 「피부랑 체형까지는 바꿈 허용해줘」), Face 줄은 얼굴 칸 일곱([FACE SHAPE] · [JAW] · [EYE SHAPE] · [EYE COLOUR] · [BROWS] · [NOSE] · [LIPS] — 칸마다 얼굴 설계표 선택지에서 우리 것 말고 하나를 글 그대로, 두 장도 칸마다 서로 다르게 — 2026-11-19 「Face 쪽은 다 다르게로 하자」), Impression(피부색 · 화장 · 표정) 줄은 고쳐도 되고 Setting detail 은 채우거나 지운다 — 나머지 줄은 글자 그대로, 첫 줄 SUMMARY:, 두 장은 헤어스타일 · 실루엣이 서로 다르게. 그리기 전에 `node tools/world-fill-check.cjs <이 폴더> <채운 글> --other <다른 장>` 이 통과해야 하고, 그릴 때는 SUMMARY 줄을 뺀 채운 글 그대로). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` · 몇째 설계인지(`generation.plan: "A"` 첫째 · `"B"` 둘째 — 2026-11-18) · 설계 요약(`generation.summary` — 지시문 첫 줄 `SUMMARY:` 그대로, 다음 주문의 비슷한 등록작 찾기 `tools/design-near.cjs` 가 읽는다) 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**일상컷 게임 코스프레 한 장**(2026-11-15 — 필수, 상황 노출 자리) — 계획에 「게임 코스프레」 로 적힌 컷의 Outfit 줄은 게임 · 캐릭터 이름이 든 코스프레 글이다(실제 작품 이름을 쓰는 유일한 갈래). **캐릭터 이름이 적힌 줄은 그대로 그린다** — 주인공 하나 게임, 등장인물 많은 게임도 계획기가 캐릭터를 정한다(2026-11-16 — 세 공방이 그린 것 · 예약한 것과 안 겹치게, 목록을 다 쓰면 2회차). 기록 `generation.cosplay` 는 그 줄의 캐릭터 · 재단. **옛 계획에만**(2026-11-16 전에 짠 계획 — Outfit 줄 맨 앞이 「…」 인 1회차 pick 칸): 되면 먼저 계획기로 그 칸만 다시 짠다 — `node tools/casual-plan.cjs <카드> --recosplay --plan <계획 파일> --dir <이 폴더> --reserve --push`(장소 · 다른 칸은 그대로, 그 자리 지시문을 다시 쓴다). 그대로 그릴 때만 **맡은 쪽이 캐릭터를 고른다** — 괄호 안 「이미 쓴」 목록에 없는 그 게임의 캐릭터 하나를 골라, 「…」 자리에 캐릭터 이름 + 그 의상의 알아볼 색 · 조각 + 괄호 안 재단 글을 쓰고 괄호 주문은 지운다(그 줄만 — 다른 줄은 그대로). 고를 캐릭터가 더 없으면(다 썼거나 알아볼 만한 캐릭터가 없으면) 새로 지어내지 말고 **같은 자리의 `<자리>-again-prompt.txt`**(계획기가 쓴 캐릭터 가운데 덜 입은 하나 · 아직 안 입은 재단을 정해 둔 2회차 지시문)를 그대로 그린다 — 기록 `generation.cosplay` 는 그 지시문의 캐릭터 · 재단. 그 파일이 없으면(쓴 캐릭터가 아직 없다) 1회차로 고른다. 그래도 막히면 그 컷을 다시 짠다: `node tools/casual-plan.cjs <카드> --session <같은 세션> --keep <카드>:<다른 컷 번호> --cosplay-full <게임 열쇠> --reserve --push`. 그린 뒤 기록에 `generation.cosplay: { "game": "<게임 열쇠>", "character": "<그린 캐릭터 영어 이름 — 1회차는 채운 이름>", "cut": "<재단 열쇠>" }`(세 공방이 이 칸으로 쓴 캐릭터를 센다)와 실제로 넘긴 글(`submitted`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
**「재생성 금지」 는 이미 받은 그림에만.** 돌아온 그림은 노출이 세 보여도 다시 만들지 않는다(검수에 적기만). 그림이 안 돌아온 막힌 컷은 상관없다 — IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 low 까지 → 계획기로 다른 장면 → 다른 장소 묶음)를 끝까지 밟고, 다 막혔을 때만 비운다. 비운 컷은 `qa.json` skipped 에 `tries`(step · request_id · scene · group), 올리기 전 `python3 tools/casual-ledger.py skips <기록 폴더>` 가 통과해야 끝난 묶음이다.
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 319 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 크기 | 올릴 파일 |
|---|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 885 | `93743a36be8a` | 2:3 1024×1536 | `샤크니아_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 샤크니아_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1316 | `0582d2010027` | 1:1 1024×1024 | `샤크니아_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 샤크니아_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1233 | `81a383c6a90d` | 2:3 1024×1536 | `샤크니아_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 샤크니아_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1263 | `f50af03350aa` | 2:3 1024×1536 | `샤크니아_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 샤크니아_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1300 | `20c26d329f4a` | 2:3 1024×1536 | `샤크니아_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 샤크니아_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1239 | `2eebda128c66` | 3:2 1536×1024 | `샤크니아_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 샤크니아_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1247 | `de1b7ec3d941` | 1:1 1024×1024 | `샤크니아_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 샤크니아_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1287 | `6e0ac813e19a` | 2:3 1024×1536 | `샤크니아_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 샤크니아_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1262 | `9cae5ce2c227` | 2:3 1024×1536 | `샤크니아_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 샤크니아_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1316 | `ecc9b8b3ee8f` | 1:1 1024×1024 | `샤크니아_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 샤크니아_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1236 | `05ef0a0fb6b8` | 2:3 1024×1536 | `샤크니아_anime_25d_gloss_f_casual10.webp` |
| ◆ | casual90 | ① 샤크니아_light_anime_25d_gloss_f.webp | `casual90-prompt.txt` | 1137 | `9594c0556088` | 1:1 1024×1024 | `샤크니아_anime_25d_gloss_f_casual90.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 포켓몬 목장 | a sunlit Pokémon ranch shelter with fresh straw and feed bins |
| 역할 | — |  |
| 의상 | 수영복 · 수영복 위 유카타 | swimwear with a light yukata worn open over it |
| 몸 자세 · 구도 | 난간·창턱에 기대 서기 · waist_up · 옆모습 | standing at a waist-high railing or sill |
| 손 · 소품 동작 | prop · rail · 몬스터볼 · 몬스터볼을 든다 | holds a Poké Ball at chest height |

옷 종류 traditional · 옷 색 세이지 · 올리브 — 포레스트 (dark forest green) · 드러내기 deep V neckline, one-shoulder cut · 장면 칸 첫머리 detail

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 축구장 관중석 | the stands of a football stadium — a steep bank of seats, waving scarves and flags in made-up colours, the floodlit pitch far below |
| 역할 | — |  |
| 의상 | 전통 의상 · 부부 | a flowing West African boubou — a wide floor-length embroidered robe with a matching head wrap |
| 몸 자세 · 구도 | 걷기 · three_quarter · 뒤 3/4 | walking |
| 손 · 소품 동작 | prop · down · 카메라 · 카메라를 든다 | carries a camera by its grip at her side |

옷 종류 robe · 옷 색 — · 장면 자유(자유 장면) · 드러내기 sweetheart neckline, strapless top · 장면 칸 첫머리 light

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 빨래방 | a coin laundromat late at night, rows of round machine doors |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 메이드 코스튬 | a black-and-white maid costume with a structured bodice, puffed sleeves and a full apron |
| 몸 자세 · 구도 | 서기 · chest_up · 옆모습 | standing |
| 손 · 소품 동작 | prop · out · 비눗방울 막대 · 비눗방울을 분다 | blows a stream of bubbles through a bubble wand with a little bottle of soap |

옷 종류 apron · 옷 색 아이보리 · 크림 (ivory and warm cream — 구체 색은 조립부가 정한다) · 드러내기 plunging neckline, bare midriff · 장면 칸 첫머리 place

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 열기구 바구니 | the wicker basket of a hot-air balloon drifting at sunrise, the rim at her waist, the bright envelope above and valleys far below |
| 역할 | — |  |
| 의상 | 운동복 · 스키 재킷 + 스키 팬츠 | a fitted ski jacket and padded ski pants |
| 몸 자세 · 구도 | 서기 · face_close · 정면 | standing |
| 손 · 소품 동작 | v_sign · out |  |

옷 종류 jacket + trousers · 옷 색 라벤더 · 플럼 — 모브 (dusty mauve) · 드러내기 sweetheart neckline, off-shoulder neckline · 장면 칸 첫머리 action

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 산장 | a mountain lodge with a front counter and a fireplace |
| 역할 | — |  |
| 의상 | 란제리풍 · 크바야 응용 레이스 | a kebaya-inspired sheer lace top with floral embroidery over a fitted camisole |
| 몸 자세 · 구도 | 기대 눕기 · environmental · 3/4 정면 | reclining on her back |
| 손 · 소품 동작 | behind_head · prop · 수박 한 조각 · 수박 한 조각을 내민다 | holds a wedge of watermelon out toward the camera |

옷 종류 tank · 옷 색 민트 · 틸 — 터콰이즈 (bright turquoise) · 드러내기 plunging neckline, cropped hem · 장면 칸 첫머리 place

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 결혼식장 | a bridal room, garden aisle or reception hall |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 코르셋형 | a daring adult costume version of {costume}, cut as a laced corset bustier with a short flared skirt |
| 몸 자세 · 구도 | 가장자리에 걸터앉기 · three_quarter · 정면 | perched on a ledge or edge |
| 손 · 소품 동작 | prop · prop · 꽃 몇 송이 · 꽃으로 화관을 엮는다 | weaves a few loose flower stems into a small crown in her lap |

옷 종류 lingerie_set + skirt · 옷 색 — · 드러내기 deep V neckline, open back · 장면 칸 첫머리 light

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 요트 갑판 | the cushioned foredeck of a moored yacht |
| 역할 | — |  |
| 의상 | 휴양지 차림 · 랩 점프슈트(짧은) | a wrap-front holiday romper with a deep V neckline and a tie belt |
| 몸 자세 · 구도 | 한 발 올려 서기 · full_body · 3/4 정면 | standing with one foot up on a step, the other leg straight |
| 손 · 소품 동작 | hip · natural |  |

옷 종류 jumpsuit · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 sweetheart neckline, backless · 장면 칸 첫머리 detail

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 방탈출 카페 | an escape room dressed as an old study — locked chests, a wall of clue cards without readable text, a dim desk lamp and a heavy wooden door |
| 역할 | — |  |
| 의상 | 평상복 · 멜빵바지 | fitted denim overalls over a cropped top |
| 몸 자세 · 구도 | 한쪽 무릎 꿇기 · full_body · 3/4 정면 | kneeling on one knee, the other foot planted flat in front of her |
| 손 · 소품 동작 | prop · floor_brace · 녹슨 열쇠 · 열쇠를 자물쇠에 넣어 돌린다 | turns an old brass key on a ring in a small lock |

옷 종류 crop_top + overalls · 옷 색 — · 옷 자유 · 드러내기 plunging neckline, halter neck · 장면 칸 첫머리 action · 직접 입력 outfit

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 조용한 정원 | a quiet garden with a feeding bowl set on the grass |
| 역할 | — |  |
| 의상 | 홈웨어 · 오프숄더 니트 | an off-shoulder knit top slipping from one shoulder over shorts |
| 몸 자세 · 구도 | 카메라 쪽으로 상체 숙이기 · waist_up · 정면 | standing and leaning her upper body forward toward the camera from the hips, her back gently arched and her shoulders lowered toward the viewer, as if leaning in close |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 knit_top + shorts · 옷 색 그레이 · 실버 — 도브 그레이 (soft dove grey) · 상황 밑단을 묶어 올림 · 드러내기 deep V neckline, cutout waist · 장면 칸 첫머리 detail

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 노래방 | a private karaoke room with spinning coloured lights |
| 역할 | — |  |
| 의상 | 게임 코스프레 · 바디수트 | a daring adult cosplay of Cloe da Pontina from TalesWeaver — the costume's recognisable colours and parts, cut as a high-cut bodysuit with sheer thigh-high stockings |
| 몸 자세 · 구도 | 의자에 앉기 · chest_up · 3/4 정면 | seated on a chair |
| 손 · 소품 동작 | v_eye · out |  |

옷 종류 bodysuit · 옷 색 — · 게임 코스프레 테일즈위버 · Cloe da Pontina(계획기가 정함) · 바디수트 · 1회차 · 드러내기 sweetheart neckline, side cutouts · 장면 칸 첫머리 light

## ◆ casual90 — 캐릭터만의 컷(인명구조대장 · 노출 bold)

일상 열 장에 더하는 한 장 — 채울 칸이 없다. 막히면 같은 지시문으로 두 번 더(모두 세 번), 그래도 막히면 계획기 `--own --own-level` 로 한 단계 내려 다시 짓는다(IMAGE_RULES 3절 「캐릭터만의 컷」).

| 칸 | 표의 글 |
|---|---|
| 장소 | a beach lifeguard post — a high chair, red flags, a rescue board |
| 장면 | she is the head lifeguard standing with a hand on her hip, scanning the surf from the foot of the high chair |
| 의상 | a lifeguard look fitted to her body — a fitted red swimsuit with a short wrap skirt and a whistle, bare shoulders and legs, a sharp-finned silver badge |
| 도구 | — |
| 자세 추천 | hip_contra |
