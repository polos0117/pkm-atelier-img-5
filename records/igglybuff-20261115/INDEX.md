# 푸푸린 (0174 · Igglybuff) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 04d6234 · 2026-11-15T11:24:10.727Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(설계 주문 — 화풍 · 색 · 머리색 · 체형 · 장갑 폼 · 원작 특징 · 노출 · 구도 · 자세는 우리 것, 큰 실루엣은 목록에서 하나 + 원작에서 딴 제 아이디어 하나, 얼굴 · 눈색(우리 것이든 제 것이든) · 헤어스타일 · 화장 · 표정 · 장면(배경) · 타입 효과는 맡은 쪽이 지어 제 지시문을 쓴다, 둘째 장은 첫째와 확실히 다르게(자세는 같게)). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 174 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 올릴 파일 |
|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 941 | `85668c3f76f0` | `푸푸린_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 푸푸린_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1215 | `58c37c651c1d` | `푸푸린_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 푸푸린_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1155 | `1cb473070aa1` | `푸푸린_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 푸푸린_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1112 | `f60b74177da5` | `푸푸린_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 푸푸린_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1165 | `76dcc33f70ae` | `푸푸린_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 푸푸린_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1201 | `55aee1bd1448` | `푸푸린_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 푸푸린_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1067 | `612b6ce44ce2` | `푸푸린_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 푸푸린_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1149 | `7236cc077777` | `푸푸린_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 푸푸린_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1151 | `2757369cf651` | `푸푸린_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 푸푸린_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1263 | `0eb0babdf359` | `푸푸린_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 푸푸린_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1125 | `f24f38f65ec9` | `푸푸린_anime_25d_gloss_f_casual10.webp` |
| ◆ | casual90 | ① 푸푸린_light_anime_25d_gloss_f.webp | `casual90-prompt.txt` | 1022 | `406b085fd113` | `푸푸린_anime_25d_gloss_f_casual90.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 사우나 | a wooden sauna and cold plunge with a cooling lounge |
| 역할 | — |  |
| 의상 | 목욕 차림 · 목욕 유카타 | a light cotton bath yukata with a soft sash |
| 몸 자세 · 구도 | 걷기 · full_body · 3/4 정면 | walking |
| 손 · 소품 동작 | prop · down · 수건 · 목에 건 수건 끝을 잡는다 | holds one end of a towel hung around her neck |

옷 종류 traditional · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 deep V neckline, side cutouts · 장면 칸 첫머리 detail

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 호숫가 | a lakeside of flat rocks and still water |
| 역할 | — |  |
| 의상 | 란제리풍 · 자동 — 계열 안에서 장면에 맞게 | tasteful lingerie-inspired fashion, fully opaque and securely fitted, with full intimate coverage |
| 몸 자세 · 구도 | 헤엄치기 · chest_up · 정면 | swimming breaststroke, head and shoulders above the water |
| 손 · 소품 동작 | out · out |  |

옷 종류 crop_top · 옷 색 레드 · 와인 (deep red and wine) · 드러내기 plunging neckline, one-shoulder cut · 장면 칸 첫머리 action

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 무대·환상 | a stylised stage, editorial or fantasy setting not bound to a real year |
| 장소 | 사막 오아시스 | a desert oasis at golden hour — date palms, a still turquoise pool and silk tents on the dunes |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 바디수트형 | a daring adult costume version of {costume}, cut as a high-cut bodysuit with sheer thigh-high tights |
| 몸 자세 · 구도 | 걷기 · three_quarter · 옆모습 | walking |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 bodysuit + leggings · 옷 색 — · 드러내기 sweetheart neckline, mini length · 장면 칸 첫머리 place

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 호텔 방 | a hotel suite with a city view and an open suitcase |
| 역할 | — |  |
| 의상 | 웨딩 · 브라이덜 레이스 | a white lace bridal lingerie set with a short veil |
| 몸 자세 · 구도 | 기대 눕기 · waist_up · 뒤 3/4 | reclining on her back |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 lingerie_set · 옷 색 — · 장면 자유(자유 장면) · 드러내기 plunging neckline, high-cut leg · 장면 칸 첫머리 light

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 폭포 웅덩이 | a rocky waterfall pool under green trees |
| 역할 | — |  |
| 의상 | 무대·판타지 의상 · 요정 무도회 | a fae ball costume — a backless gown with a wing-shaped satin cape and a leaf mask |
| 몸 자세 · 구도 | 가장자리에 걸터앉기 · environmental · 뒤 3/4 | perched on a ledge or edge |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 coat + dress · 옷 색 라벤더 · 플럼 (lavender and plum) · 상황 움직임에 벌어진 트임 · 드러내기 deep V neckline, high thigh slit · 장면 칸 첫머리 detail

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 스티커 사진기 | an arcade photo-sticker booth under bright ring lights |
| 역할 | — |  |
| 의상 | 휴양지 차림 · 묶어 입은 알로하 셔츠 | a tropical-print shirt knotted at the waist over a bikini-style top with denim cut-offs |
| 몸 자세 · 구도 | 의자에 앉기 · three_quarter · 뒤 3/4 | seated on a chair |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 bikini + shirt · 옷 색 스카이 · 네이비 (sky blue and navy) · 드러내기 sweetheart neckline, strapless top · 장면 칸 첫머리 light

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 발코니 | a small balcony with potted plants, a railing and the city beyond |
| 역할 | — |  |
| 의상 | 수영복 · 자동 — 계열 안에서 장면에 맞게 | modern swimwear, fully lined and secure during movement |
| 몸 자세 · 구도 | 한쪽 무릎 꿇기 · chest_up · 3/4 정면 | kneeling on one knee, the other foot planted flat in front of her |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 skirt + traditional · 옷 색 민트 · 틸 (mint and teal) · 드러내기 deep V neckline, off-shoulder neckline · 장면 칸 첫머리 place

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 빨래방 | a coin laundromat late at night, rows of round machine doors |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 카지노 딜러 | a casino dealer costume with a fitted waistcoat, bow tie and cuffs |
| 몸 자세 · 구도 | 위로 손 뻗기 · full_body · 옆모습 | standing close to a high shelf or line, reaching up to it |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 vest · 옷 색 블랙 · 차콜 (black with charcoal accents) · 드러내기 plunging neckline, cutout waist · 장면 칸 첫머리 action

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 공원 산책길 | a park path lined with trees and benches |
| 역할 | — |  |
| 의상 | 홈웨어 · 오프숄더 니트 | an off-shoulder knit top slipping from one shoulder over shorts |
| 몸 자세 · 구도 | 의자에 앉기 · waist_up · 옆모습 | seated on a chair |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 knit_top + shorts · 옷 색 옐로 · 머스터드 (butter yellow and mustard) · 드러내기 sweetheart neckline, halter neck · 장면 칸 첫머리 place

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 의상 수선실 | a sewing and alteration room with a cutting table, a dress form and rolls of fabric |
| 역할 | — |  |
| 의상 | 전통 의상 · 크바야 | a daily kebaya — a sheer embroidered fitted blouse over a batik sarong |
| 몸 자세 · 구도 | 서기 · environmental · 옆모습 | standing |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 blouse · 옷 색 — · 옷 자유 · 드러내기 plunging neckline, open back · 장면 칸 첫머리 action · 직접 입력 outfit

## ◆ casual90 — 캐릭터만의 컷(심야 라디오 인턴 · 노출 bold)

일상 열 장에 더하는 한 장 — 채울 칸이 없다. 막히면 같은 지시문으로 두 번 더(모두 세 번), 그래도 막히면 계획기 `--own --own-level` 로 한 단계 내려 다시 짓는다(IMAGE_RULES 3절 「캐릭터만의 컷」).

| 칸 | 표의 글 |
|---|---|
| 장소 | a late-night radio studio — a mixing console, a soundproof glass window, round headphones on a hook and a small desk lamp |
| 장면 | she is an intern sitting upright on a chair beside the mixing console, resting and drowsily waiting for the next segment |
| 의상 | a radio host look fitted to her body — a short satin jacket over a fitted camisole and short skirt, bare shoulders and legs, a plain headphone band around her neck |
| 도구 | — |
| 자세 추천 | ankles_sit |
