# 안농 (0201 · Unown) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 3917318 · 2026-11-16T09:42:55.719Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(설계 주문 — 화풍 · 색 · 머리색 · 체형 · 장갑 폼 · 원작 특징 · 노출 · 구도 · 자세는 우리 것, 큰 실루엣은 목록에서 하나 + 원작에서 딴 제 아이디어 하나, 얼굴 · 눈색(우리 것이든 제 것이든) · 헤어스타일 · 화장 · 표정 · 장면(배경) · 타입 효과는 맡은 쪽이 지어 제 지시문을 쓴다, 둘째 장은 첫째와 확실히 다르게(자세는 같게)). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**일상컷 게임 코스프레 한 장**(2026-11-15 — 필수, 상황 노출 자리) — 계획에 「게임 코스프레」 로 적힌 컷의 Outfit 줄은 게임 · 캐릭터 이름이 든 코스프레 글이다(실제 작품 이름을 쓰는 유일한 갈래). **캐릭터 이름이 적힌 줄은 그대로 그린다** — 주인공 하나 게임, 등장인물 많은 게임도 계획기가 캐릭터를 정한다(2026-11-16 — 세 공방이 그린 것 · 예약한 것과 안 겹치게, 목록을 다 쓰면 2회차). 기록 `generation.cosplay` 는 그 줄의 캐릭터 · 재단. **옛 계획에만**(2026-11-16 전에 짠 계획 — Outfit 줄 맨 앞이 「…」 인 1회차 pick 칸): 되면 먼저 계획기로 그 칸만 다시 짠다 — `node tools/casual-plan.cjs <카드> --recosplay --plan <계획 파일> --dir <이 폴더> --reserve --push`(장소 · 다른 칸은 그대로, 그 자리 지시문을 다시 쓴다). 그대로 그릴 때만 **맡은 쪽이 캐릭터를 고른다** — 괄호 안 「이미 쓴」 목록에 없는 그 게임의 캐릭터 하나를 골라, 「…」 자리에 캐릭터 이름 + 그 의상의 알아볼 색 · 조각 + 괄호 안 재단 글을 쓰고 괄호 주문은 지운다(그 줄만 — 다른 줄은 그대로). 고를 캐릭터가 더 없으면(다 썼거나 알아볼 만한 캐릭터가 없으면) 새로 지어내지 말고 **같은 자리의 `<자리>-again-prompt.txt`**(계획기가 쓴 캐릭터 가운데 덜 입은 하나 · 아직 안 입은 재단을 정해 둔 2회차 지시문)를 그대로 그린다 — 기록 `generation.cosplay` 는 그 지시문의 캐릭터 · 재단. 그 파일이 없으면(쓴 캐릭터가 아직 없다) 1회차로 고른다. 그래도 막히면 그 컷을 다시 짠다: `node tools/casual-plan.cjs <카드> --session <같은 세션> --keep <카드>:<다른 컷 번호> --cosplay-full <게임 열쇠> --reserve --push`. 그린 뒤 기록에 `generation.cosplay: { "game": "<게임 열쇠>", "character": "<그린 캐릭터 영어 이름 — 1회차는 채운 이름>", "cut": "<재단 열쇠>" }`(세 공방이 이 칸으로 쓴 캐릭터를 센다)와 실제로 넘긴 글(`submitted`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 201 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 올릴 파일 |
|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 869 | `281facbfcd05` | `안농_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 안농_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1156 | `c719a7ace6dc` | `안농_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 안농_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1150 | `b0e1f8101434` | `안농_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 안농_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1160 | `c4f0b9a488d1` | `안농_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 안농_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1205 | `24d59f0559c9` | `안농_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 안농_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1152 | `d17811833d5b` | `안농_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 안농_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1236 | `421d690cebec` | `안농_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 안농_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1196 | `df91ae10d27e` | `안농_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 안농_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1098 | `f4115ed535ac` | `안농_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 안농_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1382 | `3a820df51e04` | `안농_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 안농_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1126 | `a866a808512d` | `안농_anime_25d_gloss_f_casual10.webp` |
| ◆ | casual90 | ① 안농_light_anime_25d_gloss_f.webp | `casual90-prompt.txt` | 1114 | `1f30abb1e322` | `안농_anime_25d_gloss_f_casual90.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 운전석 | the driver's seat of a small car parked on a quiet street, the steering wheel in front of her, the windscreen and side window bright |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 바디수트형 | a daring adult costume version of {costume}, cut as a high-cut bodysuit with sheer thigh-high tights |
| 몸 자세 · 구도 | 서기 · chest_up · 정면 | standing |
| 손 · 소품 동작 | prop · prop · 잔·컵 · 두 손으로 잔을 감싼다 | holds a cup in both hands, wrapped around its warm sides |

옷 종류 bodysuit + leggings · 옷 색 — · 드러내기 deep V neckline, cutout waist · 장면 칸 첫머리 action

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 루프탑 인피니티 풀 | a rooftop infinity pool with the city skyline behind it |
| 역할 | — |  |
| 의상 | 홈웨어 · 플리스 상의 + 조거 팬츠 | a soft fleece pullover with relaxed jogger pants |
| 몸 자세 · 구도 | 스툴·벤치에 옆으로 걸터앉기 · three_quarter · 3/4 정면 | seated sideways on a stool or bench, her torso turned toward the camera |
| 손 · 소품 동작 | prop · prop · 비치볼 · 비치볼을 두 손으로 든다 | holds a striped beach ball in both hands in front of her |

옷 종류 sweater + trousers · 옷 색 — · 장면 자유(자유 장면) · 드러내기 plunging neckline, off-shoulder neckline · 장면 칸 첫머리 light

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 무대·환상 | a stylised stage, editorial or fantasy setting not bound to a real year |
| 장소 | 성 계단 | the grand staircase of an old castle |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 메이드 코스튬 | a black-and-white maid costume with a structured bodice, puffed sleeves and a full apron |
| 몸 자세 · 구도 | 서기 · chest_up · 3/4 정면 | standing |
| 손 · 소품 동작 | prop · out · 등불 · 등불을 들어 비춘다 | lifts a small hand lantern to chest height |

옷 종류 apron · 옷 색 아이보리 · 크림 (ivory and warm cream) · 드러내기 sweetheart neckline, open back · 장면 칸 첫머리 place

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 정비 창고 | a maintenance shed with a long workbench, tool racks overhead and its door open onto the yard |
| 역할 | — |  |
| 의상 | 할로윈 코스튬 · 시스루 유령 | a sheer ghost costume — layers of translucent white chiffon draped over a short white satin slip |
| 몸 자세 · 구도 | 한쪽 무릎 꿇기 · full_body · 3/4 정면 | kneeling on one knee, the other foot planted flat in front of her |
| 손 · 소품 동작 | prop · floor_brace · 닦는 천 · 앞의 면을 천으로 닦는다 | wipes the surface in front of her with a folded cleaning cloth |

옷 종류 slip · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 deep V neckline, high thigh slit · 장면 칸 첫머리 detail

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 거실 | her living room with a deep sofa, floor cushions and a low table |
| 역할 | — |  |
| 의상 | 게임 코스프레 · 란제리 | a daring adult cosplay of a pandaren monk from World of Warcraft — the costume's recognisable colours and parts, cut as a lace bralette and high-waisted briefs with garter straps |
| 몸 자세 · 구도 | 의자에 앉기 · full_body · 옆모습 | seated on a chair |
| 손 · 소품 동작 | prop · prop · 자수 틀 · 수를 놓는다 | stitches into a small embroidery hoop with fabric in it |

옷 종류 crop_top · 옷 색 — · 게임 코스프레 월드 오브 워크래프트 · a pandaren monk(계획기가 정함) · 란제리 · 1회차 · 드러내기 plunging neckline, cropped hem · 장면 칸 첫머리 place

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 공연장 대기실 | a backstage dressing room with a bulb-lit mirror, a vanity table and costume racks |
| 역할 | — |  |
| 의상 | 수영복 · 홀터 비키니 | a halter bikini with a neck tie and an underbust band |
| 몸 자세 · 구도 | 벽에 기대 서기 · waist_up · 옆모습 | standing, leaning back against a wall |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 bikini · 옷 색 카멜 · 초콜릿 (camel and chocolate brown) · 드러내기 sweetheart neckline, high-cut leg · 장면 칸 첫머리 detail

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 포켓몬 세계 부엌 | a sunny home kitchen in a Pokémon-world town, bowls of berries on the counter |
| 역할 | — |  |
| 의상 | 저녁 드레스 · 슬립 위 실크 로브 | a silk robe over an evening slip |
| 몸 자세 · 구도 | 서기 · face_close · 정면 | standing |
| 손 · 소품 동작 | v_sign · out |  |

옷 종류 robe + slip · 옷 색 세이지 · 올리브 (sage and olive green) · 드러내기 deep V neckline, backless · 장면 칸 첫머리 action

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 물가 연구 기지 | a calm lake pier and shoreline research base with a small moored boat |
| 역할 | — |  |
| 의상 | 란제리풍 · 크바야 응용 레이스 | a kebaya-inspired sheer lace top with floral embroidery over a fitted camisole |
| 몸 자세 · 구도 | 가장자리에 걸터앉기 · three_quarter · 정면 | perched on a ledge or edge |
| 손 · 소품 동작 | edge_brace_both · edge_brace_both |  |

옷 종류 tank · 옷 색 옐로 · 머스터드 (butter yellow and mustard) · 드러내기 plunging neckline, bare midriff · 장면 칸 첫머리 light

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 그루밍 매트 있는 방 | a sunny room with a grooming mat, a towel and a small brush basket |
| 역할 | — |  |
| 의상 | 모험가 · 정글 탐험가 | a jungle-explorer look — a khaki shirt knotted under the bust with rolled sleeves, cargo shorts, a canvas utility belt and lace-up boots |
| 몸 자세 · 구도 | 옆으로 눕기 · waist_up · 뒤 3/4 | lying on her left side |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 shirt + shorts · 옷 색 카멜 · 초콜릿 (camel and chocolate brown) · 상황 소매를 걷고 단추 하나를 풂 · 드러내기 sweetheart neckline, side cutouts · 장면 칸 첫머리 place

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 실내 암벽 | an indoor climbing wall of coloured holds |
| 역할 | — |  |
| 의상 | 서브컬처 · 스팀펑크 | steampunk — a brocade underbust corset belt over a blouse, a short bustle skirt and brass goggles |
| 몸 자세 · 구도 | 쪼그려 앉기 · environmental · 뒤 3/4 | crouching low on her heels |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 blouse + lingerie_set + skirt · 옷 색 — · 옷 자유 · 드러내기 deep V neckline, strapless top · 장면 칸 첫머리 detail

## ◆ casual90 — 캐릭터만의 컷(서예가 · 노출 bold)

일상 열 장에 더하는 한 장 — 채울 칸이 없다. 막히면 같은 지시문으로 두 번 더(모두 세 번), 그래도 막히면 계획기 `--own --own-level` 로 한 단계 내려 다시 짓는다(IMAGE_RULES 3절 「캐릭터만의 컷」).

| 칸 | 표의 글 |
|---|---|
| 장소 | a calligraphy studio — a long low table with an ink stone, rolls of paper, brush holders, a paper screen window |
| 장면 | she is a calligrapher standing at the table, holding a brush in both hands above fresh paper in deep concentration |
| 의상 | a calligrapher look fitted to her body — a short kimono-style wrap top and a short pleated skirt, bare shoulders and legs, sleeves tied back, a small ink-stone charm at her sash |
| 도구 | a calligraphy brush dipped in ink (sig_both) |
| 자세 추천 | counter_work |
