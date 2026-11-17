# 무장조 (0227 · Skarmory) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 ea5a4cf · 2026-11-17T13:40:41.114Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(설계 주문 — 화풍 · 색 · 머리색 · 체형 · 장갑 폼 · 원작 특징 · 노출 · 구도 · 자세는 우리 것, 큰 실루엣은 목록에서 하나 + 원작에서 딴 제 아이디어 하나, 얼굴 · 눈색(우리 것이든 제 것이든) · 헤어스타일 · 화장 · 표정 · 장면(배경) · 타입 효과는 맡은 쪽이 지어 제 지시문을 쓴다, 둘째 장은 첫째와 확실히 다르게(자세는 같게)). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**일상컷 게임 코스프레 한 장**(2026-11-15 — 필수, 상황 노출 자리) — 계획에 「게임 코스프레」 로 적힌 컷의 Outfit 줄은 게임 · 캐릭터 이름이 든 코스프레 글이다(실제 작품 이름을 쓰는 유일한 갈래). **캐릭터 이름이 적힌 줄은 그대로 그린다** — 주인공 하나 게임, 등장인물 많은 게임도 계획기가 캐릭터를 정한다(2026-11-16 — 세 공방이 그린 것 · 예약한 것과 안 겹치게, 목록을 다 쓰면 2회차). 기록 `generation.cosplay` 는 그 줄의 캐릭터 · 재단. **옛 계획에만**(2026-11-16 전에 짠 계획 — Outfit 줄 맨 앞이 「…」 인 1회차 pick 칸): 되면 먼저 계획기로 그 칸만 다시 짠다 — `node tools/casual-plan.cjs <카드> --recosplay --plan <계획 파일> --dir <이 폴더> --reserve --push`(장소 · 다른 칸은 그대로, 그 자리 지시문을 다시 쓴다). 그대로 그릴 때만 **맡은 쪽이 캐릭터를 고른다** — 괄호 안 「이미 쓴」 목록에 없는 그 게임의 캐릭터 하나를 골라, 「…」 자리에 캐릭터 이름 + 그 의상의 알아볼 색 · 조각 + 괄호 안 재단 글을 쓰고 괄호 주문은 지운다(그 줄만 — 다른 줄은 그대로). 고를 캐릭터가 더 없으면(다 썼거나 알아볼 만한 캐릭터가 없으면) 새로 지어내지 말고 **같은 자리의 `<자리>-again-prompt.txt`**(계획기가 쓴 캐릭터 가운데 덜 입은 하나 · 아직 안 입은 재단을 정해 둔 2회차 지시문)를 그대로 그린다 — 기록 `generation.cosplay` 는 그 지시문의 캐릭터 · 재단. 그 파일이 없으면(쓴 캐릭터가 아직 없다) 1회차로 고른다. 그래도 막히면 그 컷을 다시 짠다: `node tools/casual-plan.cjs <카드> --session <같은 세션> --keep <카드>:<다른 컷 번호> --cosplay-full <게임 열쇠> --reserve --push`. 그린 뒤 기록에 `generation.cosplay: { "game": "<게임 열쇠>", "character": "<그린 캐릭터 영어 이름 — 1회차는 채운 이름>", "cut": "<재단 열쇠>" }`(세 공방이 이 칸으로 쓴 캐릭터를 센다)와 실제로 넘긴 글(`submitted`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 227 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 올릴 파일 |
|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 916 | `e4b10b0dce86` | `무장조_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 무장조_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1108 | `e90dbac0c9c2` | `무장조_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 무장조_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1109 | `3671afb01ee8` | `무장조_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 무장조_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1155 | `cef2328ffd5a` | `무장조_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 무장조_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1111 | `b29dad3c7154` | `무장조_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 무장조_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1149 | `2f9d77ba1bab` | `무장조_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 무장조_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1153 | `94eb8954fc8e` | `무장조_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 무장조_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1129 | `6cba5393348c` | `무장조_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 무장조_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1183 | `d2cef76064e9` | `무장조_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 무장조_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1131 | `3cba74c3c259` | `무장조_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 무장조_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1044 | `f9ea418b02e8` | `무장조_anime_25d_gloss_f_casual10.webp` |
| ◆ | casual90 | ① 무장조_light_anime_25d_gloss_f.webp | `casual90-prompt.txt` | 1116 | `df32c8325463` | `무장조_anime_25d_gloss_f_casual90.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 의상 수선실 | a sewing and alteration room with a cutting table, a dress form and rolls of fabric |
| 역할 | — |  |
| 의상 | 운동복 · 스키 재킷 + 스키 팬츠 | a fitted ski jacket and padded ski pants |
| 몸 자세 · 구도 | 의자에 앉기 · environmental · 정면 | seated on a chair |
| 손 · 소품 동작 | prop · lap · 닦는 천 · 천을 든다 | holds a folded cleaning cloth at chest height |

옷 종류 jacket + trousers · 옷 색 민트 · 틸 — 민트 (cool mint) · 상황 소매를 걷고 단추 하나를 풂 · 드러내기 deep V neckline, open back · 장면 칸 첫머리 place

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 요트 갑판 | the cushioned foredeck of a moored yacht |
| 역할 | — |  |
| 의상 | 란제리풍 · 비대칭 세트 | an asymmetric lingerie set with one shoulder strap and a diagonal neckline |
| 몸 자세 · 구도 | 옆으로 눕기 · full_body · 정면 | lying on her left side |
| 손 · 소품 동작 | floor_front · head_rest |  |

옷 종류 lingerie_set · 옷 색 레드 · 와인 — 와인 (deep wine red) · 드러내기 sweetheart neckline, high-cut leg · 장면 칸 첫머리 light

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 역·전철 | a city station platform or the inside of a commuter train |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 바텐더 | a bartender costume — a fitted satin waistcoat over a shirt with rolled sleeves and the top buttons open, a bow tie and a high-waisted pencil mini skirt |
| 몸 자세 · 구도 | 걷기 · three_quarter · 뒤 3/4 | walking |
| 손 · 소품 동작 | prop · down · 쇼핑백 · 쇼핑백을 든다 | carries a paper shopping bag at her side |

옷 종류 shirt + skirt + vest · 옷 색 옐로 · 머스터드 — 버터 옐로 (soft butter yellow) · 드러내기 plunging neckline, off-shoulder neckline · 장면 칸 첫머리 action

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 무대·환상 | a stylised stage, editorial or fantasy setting not bound to a real year |
| 장소 | 화보 스튜디오 | an editorial photo studio with a seamless backdrop and dramatic lights |
| 역할 | — |  |
| 의상 | 게임 코스프레 · 레오타드 | a daring adult cosplay of Blue Mary from The King of Fighters 2002 — the costume's recognisable colours and parts, cut as a gymnastic leotard with sheer tights |
| 몸 자세 · 구도 | 서기 · waist_up · 정면 | standing |
| 손 · 소품 동작 | clasp_both · clasp_both |  |

옷 종류 bodysuit + leggings · 옷 색 — · 게임 코스프레 더 킹 오브 파이터즈 2002 · Blue Mary(계획기가 정함) · 레오타드 · 1회차 · 드러내기 deep V neckline, strapless top · 장면 칸 첫머리 detail

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 극장·오페라 | the grand lobby and staircase of an opera house |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 미니 드레스형 | a daring adult costume version of {costume}, cut as a fitted strapless mini dress |
| 몸 자세 · 구도 | 서기 · chest_up · 옆모습 | standing |
| 손 · 소품 동작 | prop · out · 접부채 · 부채로 얼굴을 가린다 | lifts a folding fan open to just below her eyes |

옷 종류 dress · 옷 색 — · 드러내기 sweetheart neckline, backless · 장면 칸 첫머리 detail

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 밤 택시 | the back seat of a taxi at night, city lights streaking past |
| 역할 | — |  |
| 의상 | 저녁 드레스 · 슬립 위 실크 로브 | a silk robe over an evening slip |
| 몸 자세 · 구도 | 서기 · face_close · 옆모습 | standing |
| 손 · 소품 동작 | hair_tuck · out |  |

옷 종류 robe + slip · 옷 색 아이보리 · 크림 — 에크루 (natural ecru cream) · 드러내기 plunging neckline, high thigh slit · 장면 칸 첫머리 place

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 사우나 | a wooden sauna and cold plunge with a cooling lounge |
| 역할 | — |  |
| 의상 | 홈웨어 · 오프숄더 니트 | an off-shoulder knit top slipping from one shoulder over shorts |
| 몸 자세 · 구도 | 걷기 · full_body · 3/4 정면 | walking |
| 손 · 소품 동작 | prop · down · 수건 · 목에 건 수건 끝을 잡는다 | holds one end of a towel hung around her neck |

옷 종류 knit_top + shorts · 옷 색 — · 장면 자유(자유 장면) · 드러내기 deep V neckline, bare midriff · 장면 칸 첫머리 action

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 보드게임 라운지 | a cozy board-game lounge with shelves of game boxes and low tables |
| 역할 | — |  |
| 의상 | 할로윈 코스튬 · 늑대 | a she-wolf costume — a grey faux-fur crop top and mini skirt, a wolf-ear headband, a fluffy tail and fingerless gloves |
| 몸 자세 · 구도 | 서기 · chest_up · 옆모습 | standing |
| 손 · 소품 동작 | prop · out · 동전 · 동전을 들어 보인다 | holds a single coin up between two fingers |

옷 종류 crop_top + skirt · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 sweetheart neckline, cropped hem · 장면 칸 첫머리 light

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 케이블카 | a cable car cabin over a misty valley |
| 역할 | — |  |
| 의상 | 직업복 · 사육 작업복 | work overalls over a fitted tank top and rubber boots |
| 몸 자세 · 구도 | 서기 · environmental · 옆모습 | standing |
| 손 · 소품 동작 | prop · prop · 종이 지도 · 지도를 두 손으로 펼친다 | unfolds a folded paper map in both hands in front of her |

옷 종류 overalls + tank · 옷 색 — · 옷 자유 · 드러내기 plunging neckline, side cutouts · 장면 칸 첫머리 place

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 욕실 | a bright bathroom with a mirror, tiles and folded towels |
| 역할 | — |  |
| 의상 | 수영복 · 수영복 위 유카타 | swimwear with a light yukata worn open over it |
| 몸 자세 · 구도 | 서기 · three_quarter · 3/4 정면 | standing |
| 손 · 소품 동작 | hip · hair_tuck |  |

옷 종류 traditional · 옷 색 스카이 · 네이비 — 스카이 블루 (soft sky blue) · 드러내기 deep V neckline, one-shoulder cut · 장면 칸 첫머리 action

## ◆ casual90 — 캐릭터만의 컷(펜싱 선수 · 노출 bold)

일상 열 장에 더하는 한 장 — 채울 칸이 없다. 막히면 같은 지시문으로 두 번 더(모두 세 번), 그래도 막히면 계획기 `--own --own-level` 로 한 단계 내려 다시 짓는다(IMAGE_RULES 3절 「캐릭터만의 컷」).

| 칸 | 표의 글 |
|---|---|
| 장소 | a fencing hall — a long strip of floor with lines, a rack of foils, a wall of protective masks, polished wooden floor |
| 장면 | she is a fencer with one hand on her hip, looking down along the blade of a fencing foil in the other hand |
| 의상 | a fencer look fitted to her body — a fitted white fencing jacket cut short at the hips over a short pleated fencing skirt, bare legs, white shoes, a silver feather-shaped crest on the jacket |
| 도구 | a fencing foil (sig_hold) |
| 자세 추천 | stand_inspect |
