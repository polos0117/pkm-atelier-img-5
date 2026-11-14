# 브케인 (0155 · Cyndaquil) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 59e8a94 · 2026-11-14T12:00:37.402Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(설계 주문 — 화풍 · 색 · 머리색 · 체형 · 장갑 폼 · 원작 특징 · 노출 · 구도 · 자세는 우리 것, 큰 실루엣은 목록에서 하나 + 원작에서 딴 제 아이디어 하나, 얼굴 · 눈색(우리 것이든 제 것이든) · 헤어스타일 · 화장 · 표정 · 장면(배경) · 타입 효과는 맡은 쪽이 지어 제 지시문을 쓴다, 둘째 장은 첫째와 확실히 다르게(자세는 같게)). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 155 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 올릴 파일 |
|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 887 | `d88f302a20c5` | `브케인_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 브케인_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1144 | `3bc4e791fe07` | `브케인_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 브케인_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1198 | `8704676a759a` | `브케인_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 브케인_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1072 | `b75ab9deba34` | `브케인_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 브케인_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1153 | `9d2df8b70036` | `브케인_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 브케인_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1116 | `3135d67a721e` | `브케인_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 브케인_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1160 | `fba46acdbf29` | `브케인_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 브케인_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1140 | `89135191af1d` | `브케인_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 브케인_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1085 | `3a15a512038a` | `브케인_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 브케인_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1203 | `e43f0facf52e` | `브케인_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 브케인_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1062 | `2571633af106` | `브케인_anime_25d_gloss_f_casual10.webp` |
| ◆ | casual90 | ① 브케인_light_anime_25d_gloss_f.webp | `casual90-prompt.txt` | 1060 | `d9622fbb2989` | `브케인_anime_25d_gloss_f_casual90.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 화실·공방 | an art or pottery studio of easels, clay and paint-splattered tables |
| 역할 | — |  |
| 의상 | 직업복 · 사육 작업복 | work overalls over a fitted tank top and rubber boots |
| 몸 자세 · 구도 | 서기 · waist_up · 뒤 3/4 | standing |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 overalls + tank · 옷 색 — · 장면 자유(자유 장면) · 드러내기 sweetheart neckline, halter neck · 장면 칸 첫머리 action

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 밤 택시 | the back seat of a taxi at night, city lights streaking past |
| 역할 | — |  |
| 의상 | 할로윈 코스튬 · 검은 고양이 | a black cat costume — a glossy black strapless bodysuit, sheer black tights, a cat-ear headband, a curling tail and a bell choker |
| 몸 자세 · 구도 | 서기 · chest_up · 정면 | standing |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 bodysuit + leggings · 옷 색 블랙 · 차콜 (black with charcoal accents) · 상황 젖은 옷 — 비 · 물 튐 · 드러내기 deep V neckline, bare midriff · 장면 칸 첫머리 detail

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 롤러장 | a roller rink under coloured lights |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 승무원풍 | a retro flight-attendant-inspired costume with a fitted jacket, scarf and original airline-style trim |
| 몸 자세 · 구도 | 작업대에 몸 숙이기 · full_body · 뒤 3/4 | standing at a work surface, upper body leaning slightly forward over it, hips back and weight on both feet |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 jacket · 옷 색 스카이 · 네이비 (sky blue and navy) · 드러내기 plunging neckline, cutout waist · 장면 칸 첫머리 light

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 박물관 갈라 | a grand museum hall with marble statues at night |
| 역할 | — |  |
| 의상 | 레트로 · 자동 — 계열 안에서 장면에 맞게 | a period look from a past decade |
| 몸 자세 · 구도 | 스툴·벤치에 옆으로 걸터앉기 · face_close · 3/4 정면 | seated sideways on a stool or bench, her torso turned toward the camera |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 swimsuit · 옷 색 세이지 · 올리브 (sage and olive green) · 드러내기 sweetheart neckline, strapless top · 장면 칸 첫머리 place

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 해변 | a sunny beach with wet sand and shallow surf |
| 역할 | — |  |
| 의상 | 란제리풍 · 나이트 로브 + 란제리 | a lingerie set under an open silk night robe with a tied sash |
| 몸 자세 · 구도 | 서기 · three_quarter · 뒤 3/4 | standing |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 lingerie_set + robe · 옷 색 민트 · 틸 (mint and teal) · 드러내기 deep V neckline, side cutouts · 장면 칸 첫머리 action

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 주방 | her home kitchen with a counter, open shelves and hanging pans |
| 역할 | — |  |
| 의상 | 수영복 · 트라이앵글 비키니 | a triangle bikini with slider cups and tie-side bottoms |
| 몸 자세 · 구도 | 스툴·벤치에 옆으로 걸터앉기 · waist_up · 3/4 정면 | seated sideways on a stool or bench, her torso turned toward the camera |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 bikini · 옷 색 카멜 · 초콜릿 (camel and chocolate brown) · 드러내기 plunging neckline, high-cut leg · 장면 칸 첫머리 detail

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 온천 마을 족욕 | a hot-spring town footbath under a wooden roof |
| 역할 | — |  |
| 의상 | 저녁 드레스 · 슬립 드레스 | a thin-strapped satin slip dress that flows along the body |
| 몸 자세 · 구도 | 스툴·벤치에 옆으로 걸터앉기 · face_close · 정면 | seated sideways on a stool or bench, her torso turned toward the camera |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 dress + slip · 옷 색 아이보리 · 크림 (ivory and warm cream) · 드러내기 sweetheart neckline, backless · 장면 칸 첫머리 place

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 마을 열매 시장 | a village market stall piled with fresh berries |
| 역할 | — |  |
| 의상 | 모험가 · 정글 탐험가 | a jungle-explorer look — a khaki shirt knotted under the bust with rolled sleeves, cargo shorts, a canvas utility belt and lace-up boots |
| 몸 자세 · 구도 | 서기 · environmental · 정면 | standing |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 shirt + shorts · 옷 색 — · 옷 자유 · 드러내기 deep V neckline, off-shoulder neckline · 장면 칸 첫머리 light

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 콘테스트장 | a Pokémon Contest hall with a decorated stage, ribbon displays and audience seats |
| 역할 | — |  |
| 의상 | 운동복 · 골프웨어 — 폴로 + 플리츠 미니스커트 | a fitted golf polo with a pleated mini skirt and a visor |
| 몸 자세 · 구도 | 무릎 꿇기 · environmental · 3/4 정면 | kneeling on the ground |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 skirt · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 plunging neckline, mini length · 장면 칸 첫머리 detail

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 버스 정류장 | a bus shelter on a quiet street, a narrow bench, a glass side panel and the road beyond |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 크롭 투피스형 | a daring adult costume version of {costume}, cut as a cropped top and a micro skirt that bare the midriff |
| 몸 자세 · 구도 | 한쪽 무릎 꿇기 · three_quarter · 정면 | kneeling on one knee, the other foot planted flat in front of her |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 crop_top + skirt · 옷 색 — · 드러내기 sweetheart neckline, one-shoulder cut · 장면 칸 첫머리 place

## ◆ casual90 — 캐릭터만의 컷(피자 가게 견습 · 노출 bold)

일상 열 장에 더하는 한 장 — 채울 칸이 없다. 막히면 같은 지시문으로 두 번 더(모두 세 번), 그래도 막히면 계획기 `--own --own-level` 로 한 단계 내려 다시 짓는다(IMAGE_RULES 3절 「캐릭터만의 컷」).

| 칸 | 표의 글 |
|---|---|
| 장소 | a wood-fired pizza kitchen — a domed brick oven with glowing embers, a dough table dusted with flour, stacked firewood, hanging copper pans |
| 장면 | she is an apprentice pizza cook holding the long peel in both hands, nervously sliding a pizza toward the oven |
| 의상 | a pizza cook look fitted to her body — a flour-dusted apron over a fitted sleeveless top and short shorts, bare arms and legs, hair tied up, a plain paper cook's cap |
| 도구 | a long wooden pizza peel with a pizza (sig_both) |
| 자세 추천 | camera_shot |
