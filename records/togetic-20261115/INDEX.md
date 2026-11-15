# 토게틱 (0176 · Togetic) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 302be16 · 2026-11-15T14:01:13.525Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(설계 주문 — 화풍 · 색 · 머리색 · 체형 · 장갑 폼 · 원작 특징 · 노출 · 구도 · 자세는 우리 것, 큰 실루엣은 목록에서 하나 + 원작에서 딴 제 아이디어 하나, 얼굴 · 눈색(우리 것이든 제 것이든) · 헤어스타일 · 화장 · 표정 · 장면(배경) · 타입 효과는 맡은 쪽이 지어 제 지시문을 쓴다, 둘째 장은 첫째와 확실히 다르게(자세는 같게)). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**일상컷 게임 코스프레 한 장**(2026-11-15 — 필수, 상황 노출 자리) — 계획에 「게임 코스프레」 로 적힌 컷의 Outfit 줄은 게임 · 캐릭터 이름이 든 코스프레 글이다(실제 작품 이름을 쓰는 유일한 갈래). 주인공 하나 게임 · 2회차(캐릭터 이름이 적힌 줄)는 그대로 그린다. **등장인물 많은 게임 1회차**(Outfit 줄 맨 앞이 「…」)는 **맡은 쪽이 캐릭터를 고른다** — 괄호 안 「이미 쓴」 목록에 없는 그 게임의 캐릭터 하나를 골라, 「…」 자리에 캐릭터 이름 + 그 의상의 알아볼 색 · 조각 + 괄호 안 재단 글을 쓰고 괄호 주문은 지운다(그 줄만 — 다른 줄은 그대로). 고를 캐릭터가 더 없으면(다 썼거나 알아볼 만한 캐릭터가 없으면) 새로 지어내지 말고 **같은 자리의 `<자리>-again-prompt.txt`**(계획기가 쓴 캐릭터 가운데 덜 입은 하나 · 아직 안 입은 재단을 정해 둔 2회차 지시문)를 그대로 그린다 — 기록 `generation.cosplay` 는 그 지시문의 캐릭터 · 재단. 그 파일이 없으면(쓴 캐릭터가 아직 없다) 1회차로 고른다. 그래도 막히면 그 컷을 다시 짠다: `node tools/casual-plan.cjs <카드> --session <같은 세션> --keep <카드>:<다른 컷 번호> --cosplay-full <게임 열쇠> --reserve --push`. 그린 뒤 기록에 `generation.cosplay: { "game": "<게임 열쇠>", "character": "<그린 캐릭터 영어 이름 — 1회차는 채운 이름>", "cut": "<재단 열쇠>" }`(세 공방이 이 칸으로 쓴 캐릭터를 센다)와 실제로 넘긴 글(`submitted`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 176 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 올릴 파일 |
|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 945 | `a5ae78cbd3c4` | `토게틱_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 토게틱_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1152 | `9db281e60fdc` | `토게틱_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 토게틱_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1175 | `cf891969de16` | `토게틱_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 토게틱_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1192 | `8ef70d3ce2d1` | `토게틱_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 토게틱_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1214 | `b2622acbdb08` | `토게틱_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 토게틱_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1173 | `7763b6edec52` | `토게틱_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 토게틱_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1144 | `47c73d6dbaeb` | `토게틱_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 토게틱_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1129 | `a3e5b96d25d6` | `토게틱_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 토게틱_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1127 | `b1fcb6b22a98` | `토게틱_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 토게틱_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1112 | `13dcfc766bb8` | `토게틱_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 토게틱_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1116 | `3ff6925ee37d` | `토게틱_anime_25d_gloss_f_casual10.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 포켓몬 보호구역 | a Pokémon reserve with habitat gates, shaded water bowls and spacious planted enclosures |
| 역할 | 포켓몬 보호구역 관리인 | a Pokémon reserve caretaker |
| 의상 | 평상복 · 롱코트 + 머플러 | a long wool coat and a knitted scarf |
| 몸 자세 · 구도 | 무릎 꿇기 · three_quarter · 옆모습 | kneeling on the ground |
| 손 · 소품 동작 | prop · prop · 물통 · 물통으로 물그릇을 채운다 | refills a shaded water bowl from a water jug |

옷 종류 coat · 옷 색 — · 장면 자유(자유 장면) · 드러내기 deep V neckline, bare midriff · 장면 칸 첫머리 light

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 전망대 | a hilltop lookout over a wide valley |
| 역할 | — |  |
| 의상 | 수영복 · 트라이앵글 비키니 | a triangle bikini with slider cups and tie-side bottoms |
| 몸 자세 · 구도 | 작업대에 몸 숙이기 · waist_up · 3/4 정면 | standing at a work surface, upper body leaning slightly forward over it, hips back and weight on both feet |
| 손 · 소품 동작 | prop · prop · 종이 지도 · 지도를 두 손으로 펼친다 | unfolds a folded paper map in both hands in front of her |

옷 종류 bikini · 옷 색 핑크 · 로즈 (rose pink and blush) · 드러내기 sweetheart neckline, high-cut leg · 장면 칸 첫머리 detail

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 재즈바 | a dim jazz bar with a grand piano |
| 역할 | — |  |
| 의상 | 무대·판타지 의상 · 별의 여신 | a star goddess costume — a midnight-blue gown scattered with crystal stars and a crescent headpiece |
| 몸 자세 · 구도 | 서기 · face_close · 3/4 정면 | standing |
| 손 · 소품 동작 | cheek · out |  |

옷 종류 dress · 옷 색 스카이 · 네이비 (sky blue and navy) · 드러내기 plunging neckline, backless · 장면 칸 첫머리 action

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 조용한 정원 | a quiet garden with a feeding bowl set on the grass |
| 역할 | — |  |
| 의상 | 운동복 · 스키웨어 — 몸에 붙는 스키 수트 | a sleek fitted one-piece ski suit with goggles pushed up on her head |
| 몸 자세 · 구도 | 한쪽 무릎 꿇기 · full_body · 3/4 정면 | kneeling on one knee, the other foot planted flat in front of her |
| 손 · 소품 동작 | prop · floor_brace · 나무열매 간식 · 동료에게 간식을 내민다 | offers a small berry treat to her companion |

옷 종류 swimsuit · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 deep V neckline, halter neck · 장면 칸 첫머리 place

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 양궁장 | an archery range of targets on a green field |
| 역할 | — |  |
| 의상 | 레트로 · 자동 — 계열 안에서 장면에 맞게 | a period look from a past decade |
| 몸 자세 · 구도 | 서기 · face_close · 정면 | standing |
| 손 · 소품 동작 | shush · out |  |

옷 종류 jumpsuit · 옷 색 블랙 · 차콜 (black with charcoal accents) · 드러내기 sweetheart neckline, off-shoulder neckline · 장면 칸 첫머리 place

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 베이커리 작업실 | a small bakery workroom with a floury wooden worktable and warm ovens |
| 역할 | — |  |
| 의상 | 서브컬처 · 자동 — 계열 안에서 장면에 맞게 | a subculture street look |
| 몸 자세 · 구도 | 벽에 기대 서기 · chest_up · 3/4 정면 | standing, leaning back against a wall |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 blouse + lingerie_set + skirt · 옷 색 — · 옷 자유 · 드러내기 plunging neckline, cutout waist · 장면 칸 첫머리 detail

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 무대·환상 | a stylised stage, editorial or fantasy setting not bound to a real year |
| 장소 | 화보 스튜디오 | an editorial photo studio with a seamless backdrop and dramatic lights |
| 역할 | — |  |
| 의상 | 게임 코스프레 · 크롭 투피스 | a daring adult cosplay of the Chosen Undead in Elite Knight armour from Dark Souls — the Elite Knight armour — a fitted steel breastplate, a short faded rust-red tabard, steel pauldrons, gauntlets and greaves, with a frayed cloth scarf, cut as a cropped top and a micro skirt or hot pants that bare the midriff |
| 몸 자세 · 구도 | 한 발 올려 서기 · full_body · 3/4 정면 | standing with one foot up on a step, the other leg straight |
| 손 · 소품 동작 | hip · natural |  |

옷 종류 crop_top + skirt + trousers · 옷 색 — · 게임 코스프레 다크 소울 · the Chosen Undead in Elite Knight armour(선택받은 불사자(상급 기사)) · 크롭 투피스 · 1회차 · 드러내기 deep V neckline, cropped hem · 장면 칸 첫머리 action

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 댄스 무대 | a lit dance stage or milonga floor |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 바디수트형 | a daring adult costume version of {costume}, cut as a high-cut bodysuit with sheer thigh-high tights |
| 몸 자세 · 구도 | 한쪽 무릎 꿇기 · chest_up · 정면 | kneeling on one knee, the other foot planted flat in front of her |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 bodysuit + leggings · 옷 색 — · 드러내기 sweetheart neckline, open back · 장면 칸 첫머리 light

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 운전석 | the driver's seat of a small car parked on a quiet street, the steering wheel in front of her, the windscreen and side window bright |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 메이드 코스튬 | a black-and-white maid costume with a structured bodice, puffed sleeves and a full apron |
| 몸 자세 · 구도 | 의자에 앉기 · environmental · 3/4 정면 | seated on a chair |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 apron · 옷 색 아이보리 · 크림 (ivory and warm cream) · 드러내기 plunging neckline, side cutouts · 장면 칸 첫머리 detail

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 현관 | the entryway of her home with a shoe bench, coat hooks and a long mirror |
| 역할 | — |  |
| 의상 | 란제리풍 · 실크 파자마 세트 | a silk pajama set — a short satin camisole with lace trim and matching tap shorts, the long-sleeved pajama shirt worn open over it |
| 몸 자세 · 구도 | 쪼그려 앉기 · three_quarter · 뒤 3/4 | crouching low on her heels |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 shirt + shorts + tank · 옷 색 코랄 · 오렌지 (coral and soft orange) · 드러내기 deep V neckline, mini length · 장면 칸 첫머리 light
