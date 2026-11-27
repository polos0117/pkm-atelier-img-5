# 피그점프 (0325 · Spoink) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 51b2bda · 2026-11-27T14:41:20.698Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(칸 채우기 — 2026-11-18. 주문 아래 우리 경장 지시문을 그대로 싣고 칸만 비웠다: [HAIRSTYLE: …] 은 우리와 다른 헤어스타일, [ARMOR SILHOUETTE: …] 은 주문의 목록(그 타입 추천에서 우리 것 빼고)에서 하나를 글 그대로, Design idea 줄은 원작 형태 특징 하나를 장갑 구조에, [TYPE EFFECTS: …] 은 주문의 우리 효과 표에서 손 · 몸 · 주변 문장 하나씩 글 그대로(우리 것과 같아도 된다), [BODY TYPE: …] 은 우리 체형 목록(CARD_FIGURE · VOCAB_EN.body)에서 하나를 글 그대로(우리 것 그대로도 된다 — 2026-11-18 「피부랑 체형까지는 바꿈 허용해줘」), Face 줄은 얼굴 칸 일곱([FACE SHAPE] · [JAW] · [EYE SHAPE] · [EYE COLOUR] · [BROWS] · [NOSE] · [LIPS] — 칸마다 얼굴 설계표 선택지에서 우리 것 말고 하나를 글 그대로, 두 장도 칸마다 서로 다르게 — 2026-11-19 「Face 쪽은 다 다르게로 하자」), Impression(피부색 · 화장 · 표정) 줄은 고쳐도 되고 Setting detail 은 채우거나 지운다 — 나머지 줄은 글자 그대로, 첫 줄 SUMMARY:, 두 장은 헤어스타일 · 실루엣이 서로 다르게. 그리기 전에 `node tools/world-fill-check.cjs <이 폴더> <채운 글> --other <다른 장>` 이 통과해야 하고, 그릴 때는 SUMMARY 줄을 뺀 채운 글 그대로). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` · 몇째 설계인지(`generation.plan: "A"` 첫째 · `"B"` 둘째 — 2026-11-18) · 설계 요약(`generation.summary` — 지시문 첫 줄 `SUMMARY:` 그대로, 다음 주문의 비슷한 등록작 찾기 `tools/design-near.cjs` 가 읽는다) 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**일상컷 게임 코스프레 한 장**(2026-11-15 — 필수, 상황 노출 자리) — 계획에 「게임 코스프레」 로 적힌 컷의 Outfit 줄은 게임 · 캐릭터 이름이 든 코스프레 글이다(실제 작품 이름을 쓰는 유일한 갈래). **캐릭터 이름이 적힌 줄은 그대로 그린다** — 주인공 하나 게임, 등장인물 많은 게임도 계획기가 캐릭터를 정한다(2026-11-16 — 세 공방이 그린 것 · 예약한 것과 안 겹치게, 목록을 다 쓰면 2회차). 기록 `generation.cosplay` 는 그 줄의 캐릭터 · 재단. **옛 계획에만**(2026-11-16 전에 짠 계획 — Outfit 줄 맨 앞이 「…」 인 1회차 pick 칸): 되면 먼저 계획기로 그 칸만 다시 짠다 — `node tools/casual-plan.cjs <카드> --recosplay --plan <계획 파일> --dir <이 폴더> --reserve --push`(장소 · 다른 칸은 그대로, 그 자리 지시문을 다시 쓴다). 그대로 그릴 때만 **맡은 쪽이 캐릭터를 고른다** — 괄호 안 「이미 쓴」 목록에 없는 그 게임의 캐릭터 하나를 골라, 「…」 자리에 캐릭터 이름 + 그 의상의 알아볼 색 · 조각 + 괄호 안 재단 글을 쓰고 괄호 주문은 지운다(그 줄만 — 다른 줄은 그대로). 고를 캐릭터가 더 없으면(다 썼거나 알아볼 만한 캐릭터가 없으면) 새로 지어내지 말고 **같은 자리의 `<자리>-again-prompt.txt`**(계획기가 쓴 캐릭터 가운데 덜 입은 하나 · 아직 안 입은 재단을 정해 둔 2회차 지시문)를 그대로 그린다 — 기록 `generation.cosplay` 는 그 지시문의 캐릭터 · 재단. 그 파일이 없으면(쓴 캐릭터가 아직 없다) 1회차로 고른다. 그래도 막히면 그 컷을 다시 짠다: `node tools/casual-plan.cjs <카드> --session <같은 세션> --keep <카드>:<다른 컷 번호> --cosplay-full <게임 열쇠> --reserve --push`. 그린 뒤 기록에 `generation.cosplay: { "game": "<게임 열쇠>", "character": "<그린 캐릭터 영어 이름 — 1회차는 채운 이름>", "cut": "<재단 열쇠>" }`(세 공방이 이 칸으로 쓴 캐릭터를 센다)와 실제로 넘긴 글(`submitted`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
**「재생성 금지」 는 이미 받은 그림에만.** 돌아온 그림은 노출이 세 보여도 다시 만들지 않는다(검수에 적기만). 그림이 안 돌아온 막힌 컷은 상관없다 — IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 low 까지 → 계획기로 다른 장면 → 다른 장소 묶음)를 끝까지 밟고, 다 막혔을 때만 비운다. 비운 컷은 `qa.json` skipped 에 `tries`(step · request_id · scene · group), 올리기 전 `python3 tools/casual-ledger.py skips <기록 폴더>` 가 통과해야 끝난 묶음이다.
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 325 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 크기 | 올릴 파일 |
|---|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 847 | `aba835f7ad97` | 2:3 1024×1536 | `피그점프_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 피그점프_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1215 | `008b0f600d73` | 3:2 1536×1024 | `피그점프_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 피그점프_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1227 | `b84dc1da1b0b` | 2:3 1024×1536 | `피그점프_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 피그점프_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1253 | `d1fe3efad976` | 2:3 1024×1536 | `피그점프_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 피그점프_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1298 | `9cb4f68ca4ef` | 2:3 1024×1536 | `피그점프_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 피그점프_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1258 | `a41f61b31323` | 2:3 1024×1536 | `피그점프_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 피그점프_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1228 | `b9112a4b5c9f` | 1:1 1024×1024 | `피그점프_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 피그점프_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1371 | `06b585666fe7` | 2:3 1024×1536 | `피그점프_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 피그점프_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1230 | `769ea35486a2` | 2:3 1024×1536 | `피그점프_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 피그점프_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1206 | `55a90235b58c` | 3:2 1536×1024 | `피그점프_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 피그점프_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1279 | `d6f9c3b44886` | 1:1 1024×1024 | `피그점프_anime_25d_gloss_f_casual10.webp` |
| ◆ | casual90 | ① 피그점프_light_anime_25d_gloss_f.webp | `casual90-prompt.txt` | 1140 | `9d3a1d8fb085` | 1:1 1024×1024 | `피그점프_anime_25d_gloss_f_casual90.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 공연장 대기실 | a backstage dressing room with a bulb-lit mirror, a vanity table and costume racks |
| 역할 | — |  |
| 의상 | 란제리풍 · 코르셋 + 테일러드 재킷 | a satin corset worn as outerwear under a sharply tailored open blazer with matching wide-leg trousers |
| 몸 자세 · 구도 | 의자에 앉기 · environmental · 정면 | seated on a chair |
| 손 · 소품 동작 | prop · lap · 손거울 · 손거울을 탁 닫는다 | snaps a compact mirror shut with one hand |

옷 종류 jacket + lingerie_set + trousers · 옷 색 스카이 · 네이비 — 스카이 블루 (soft sky blue) · 드러내기 plunging neckline, side cutouts · 장면 칸 첫머리 detail

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 호숫가 | a lakeside of flat rocks and still water |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 라이프가드 이벤트 | a lifeguard event costume — a red one-piece-style costume with a whistle on a cord |
| 몸 자세 · 구도 | 가장자리에 걸터앉기 · full_body · 옆모습 | perched on a ledge or edge |
| 손 · 소품 동작 | edge_brace_both · edge_brace_both |  |

옷 종류 swimsuit · 옷 색 레드 · 와인 (deep red and wine — 구체 색은 조립부가 정한다) · 드러내기 sweetheart neckline, cutout waist · 장면 칸 첫머리 place

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 대학 축제 부스 | a university festival lane of booths under bunting and paper lanterns, a stall counter with hand-drawn signs without readable text and a small stage beyond |
| 역할 | — |  |
| 의상 | 게임 코스프레 · 란제리 | a daring adult cosplay of Xinyan from Genshin Impact — the costume's recognisable colours and parts, cut as a lace bralette and high-waisted briefs with garter straps |
| 몸 자세 · 구도 | 난간·창턱에 기대 서기 · waist_up · 정면 | standing at a waist-high railing or sill |
| 손 · 소품 동작 | rail · hair_tuck |  |

옷 종류 crop_top · 옷 색 — · 게임 코스프레 원신 · Xinyan(계획기가 정함) · 란제리 · 1회차 · 드러내기 deep V neckline, open back · 장면 칸 첫머리 action

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 열기구 바구니 | the wicker basket of a hot-air balloon drifting at sunrise, the rim at her waist, the bright envelope above and valleys far below |
| 역할 | — |  |
| 의상 | 동탄룩 · 클럽 — 메탈릭 슬립 미니 | a club outfit — a liquid-metallic cowl-neck slip mini dress with thin straps and strappy heels |
| 몸 자세 · 구도 | 서기 · chest_up · 옆모습 | standing |
| 손 · 소품 동작 | prop · out · 카메라 · 카메라 끈을 목에 건다 | loops the strap of a camera over her head |

옷 종류 dress + slip · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 plunging neckline, backless · 장면 칸 첫머리 light

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 미술관 전시실 | a bright art museum gallery of white walls hung with large abstract paintings, a polished pale floor and a long viewing bench |
| 역할 | — |  |
| 의상 | 휴양지 차림 · 묶어 입은 알로하 셔츠 | a tropical-print shirt knotted at the waist over a bikini-style top with denim cut-offs |
| 몸 자세 · 구도 | 서기 · face_close · 정면 | standing |
| 손 · 소품 동작 | v_sign · out |  |

옷 종류 bikini + shirt · 옷 색 스카이 · 네이비 (sky blue and navy — 구체 색은 조립부가 정한다) · 드러내기 sweetheart neckline, bare midriff · 장면 칸 첫머리 place

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 그루밍 매트 있는 방 | a sunny room with a grooming mat, a towel and a small brush basket |
| 역할 | — |  |
| 의상 | 홈웨어 · 캐미솔 + 랩 바텀 | a thin-strap camisole with wrap shorts tied at the hip |
| 몸 자세 · 구도 | 무릎 꿇기 · three_quarter · 3/4 정면 | kneeling on the ground |
| 손 · 소품 동작 | pet_companion · natural |  |

옷 종류 shorts + tank · 옷 색 카멜 · 초콜릿 — 카멜 (warm camel) · 상황 젖은 옷 — 비 · 물 튐 · 드러내기 deep V neckline, off-shoulder neckline · 장면 칸 첫머리 detail

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 녹음실 | a foley recording booth with microphones and boxes of noisy props |
| 역할 | — |  |
| 의상 | 신화 드레이프 · 아라비안 나이트 | an Arabian-nights look — a jewelled cropped top, a sheer veil scarf over the shoulders, low-slung flowing chiffon trousers and gold coin anklets |
| 몸 자세 · 구도 | 허리 젖혀 서기 · full_body · 뒤 3/4 | standing with her back gently arched and her weight shifted onto one hip, shoulders eased back |
| 손 · 소품 동작 | hip · down |  |

옷 종류 crop_top + trousers · 옷 색 — · 옷 자유 · 드러내기 plunging neckline, mini length · 장면 칸 첫머리 action

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 스티커 사진기 | an arcade photo-sticker booth under bright ring lights |
| 역할 | — |  |
| 의상 | 서브컬처 · 록 | rock — a leather mini skirt, a cropped vest and a choker |
| 몸 자세 · 구도 | 서기 · waist_up · 3/4 정면 | standing |
| 손 · 소품 동작 | collar · hip |  |

옷 종류 skirt + vest · 옷 색 — · 장면 자유(자유 장면) · 드러내기 sweetheart neckline, one-shoulder cut · 장면 칸 첫머리 light

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 드레스룸 | a walk-in closet with open shelves, hanging rails, a full-length mirror and a low stool |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 바디수트형 | a daring adult costume version of {costume}, cut as a high-cut bodysuit with sheer thigh-high tights |
| 몸 자세 · 구도 | 바닥에 앉기 · environmental · 옆모습 | sitting on the ground |
| 손 · 소품 동작 | lap · floor_brace |  |

옷 종류 bodysuit + leggings · 옷 색 — · 드러내기 deep V neckline, strapless top · 장면 칸 첫머리 light

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 배틀 연습장 | an outdoor battle practice field marked with cones and chalk lines |
| 역할 | — |  |
| 의상 | 수영복 · 수영복 위 유카타 | swimwear with a light yukata worn open over it |
| 몸 자세 · 구도 | 스툴·벤치에 옆으로 걸터앉기 · three_quarter · 3/4 정면 | seated sideways on a stool or bench |
| 손 · 소품 동작 | prop · prop · 플루트 · 플루트를 분다 | plays a silver flute, held level out to one side of her lips |

옷 종류 traditional · 옷 색 민트 · 틸 — 아쿠아 (clear aqua) · 드러내기 deep V neckline, high thigh slit · 장면 칸 첫머리 detail

## ◆ casual90 — 캐릭터만의 컷(트램펄린 견습 강사 · 노출 bold)

일상 열 장에 더하는 한 장 — 채울 칸이 없다. 막히면 같은 지시문으로 두 번 더(모두 세 번), 그래도 막히면 계획기 `--own --own-level` 로 한 단계 내려 다시 짓는다(IMAGE_RULES 3절 「캐릭터만의 컷」).

| 칸 | 표의 글 |
|---|---|
| 장소 | a trampoline park — padded trampolines, a foam pit, a wall of colored grips |
| 장면 | she is a trainee instructor giving a bouncy thumbs-up |
| 의상 | a trampoline instructor look fitted to her body — a fitted sleeveless sports top and short shorts, bare midriff and legs, grip socks, a spring-shaped hair tie |
| 도구 | — |
| 자세 추천 | thumbs_waist |
