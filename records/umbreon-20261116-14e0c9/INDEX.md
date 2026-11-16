# 블래키 (0197 · Umbreon) — 지시문 묶음

화풍 `anime_25d_gloss` · 만든 도구 `tools/prompt-pack.cjs build` · 생성기 코드 1d4fc63 · 2026-11-16T07:18:38.376Z

자리마다 `<자리>-prompt.txt` 를 **고치지 않고 그대로** 제출하고, 첨부 칸의 그림을 붙인다. 고칠 것이 있으면 settings.json 을 고쳐 build 를 다시 돌린다.

**① → 멈춤 → 일상컷**(2026-11-11 삼국지 · 원소와 같이). ① 은 **네 장**(첨부 없이 한 장씩) — **두 장은 우리 설계 `light-prompt.txt` 그대로, 두 장은 임의 설계 `light-free.txt`**(설계 주문 — 화풍 · 색 · 머리색 · 체형 · 장갑 폼 · 원작 특징 · 노출 · 구도 · 자세는 우리 것, 큰 실루엣은 목록에서 하나 + 원작에서 딴 제 아이디어 하나, 얼굴 · 눈색(우리 것이든 제 것이든) · 헤어스타일 · 화장 · 표정 · 장면(배경) · 타입 효과는 맡은 쪽이 지어 제 지시문을 쓴다, 둘째 장은 첫째와 확실히 다르게(자세는 같게)). 네 장을 「우리 설계 1 · 2 / GPT 설계 1 · 2」 로 붙여 보이고 **멈추고 묻는다** — 고르기 전엔 일상컷으로 넘어가지 않고 ① 도 올리지 않는다. 고른 장만 올리고 그 장을 붙여 일상컷을 그린다. 임의 설계 장이면 기록 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`)을 남긴다.

**일상컷 옷 자유 컷 두 장** — 계획에 「옷 자유」 로 적힌 컷 가운데 「장면 자유」 가 아닌 한 장은 Outfit 줄이 「노출 의상을 네가 지어라」 다 — 이 묶음의 `outfit-catalog.md`(우리가 쓰는 옷 전부)를 읽고 **거기 없는 옷**을 지어 그 줄에만 써 넣는다(실제로 넘긴 글은 기록에).

**일상컷 자유 장면 두 장**(2026-11-11) — 계획에 「장면 자유」(옷 자유 가운데 한 장) · 「갈래 · 상황 자유」 로 적힌 컷은 SCENE 칸이 설계 주문이다: **장소 · 활동 · 자세 · 구도 · 의상을 맡은 쪽이 짓는다** — 캐릭터의 특징에서 출발해 예상하지 못했지만 자연스럽게 어울리는 일상의 한 순간, 참신함은 장식보다 상황과 행동에서, 이 묶음의 다른 일상컷 · 이 세션에서 그린 컷과 비슷한 장면은 피한다. 장면 자유는 `outfit-catalog.md` 에 **없는 노출 의상**, 갈래 · 상황 자유는 필수 갈래(성인 롤플레이 · 수영복 · 란제리풍) 하나를 골라 **없는 옷** + 끝의 상황 목록에 **없는 노출 상황**. SCENE 밖의 칸(얼굴 · 화풍 · 체형 · 인체 · 옷 갈아입기 · 각도)과 표정 · 노출 강도 · 원작 영향도 줄은 우리 것 그대로 — 그 위에서 제 지시문을 써 그린다. 기록에 `generation.design: "gpt_free"` 와 실제로 넘긴 지시문(`generation.free_prompt`).

**일상컷 게임 코스프레 한 장**(2026-11-15 — 필수, 상황 노출 자리) — 계획에 「게임 코스프레」 로 적힌 컷의 Outfit 줄은 게임 · 캐릭터 이름이 든 코스프레 글이다(실제 작품 이름을 쓰는 유일한 갈래). **캐릭터 이름이 적힌 줄은 그대로 그린다** — 주인공 하나 게임, 등장인물 많은 게임도 계획기가 캐릭터를 정한다(2026-11-16 — 세 공방이 그린 것 · 예약한 것과 안 겹치게, 목록을 다 쓰면 2회차). 기록 `generation.cosplay` 는 그 줄의 캐릭터 · 재단. **옛 계획에만**(2026-11-16 전에 짠 계획 — Outfit 줄 맨 앞이 「…」 인 1회차 pick 칸): 되면 먼저 계획기로 그 칸만 다시 짠다 — `node tools/casual-plan.cjs <카드> --recosplay --plan <계획 파일> --dir <이 폴더> --reserve --push`(장소 · 다른 칸은 그대로, 그 자리 지시문을 다시 쓴다). 그대로 그릴 때만 **맡은 쪽이 캐릭터를 고른다** — 괄호 안 「이미 쓴」 목록에 없는 그 게임의 캐릭터 하나를 골라, 「…」 자리에 캐릭터 이름 + 그 의상의 알아볼 색 · 조각 + 괄호 안 재단 글을 쓰고 괄호 주문은 지운다(그 줄만 — 다른 줄은 그대로). 고를 캐릭터가 더 없으면(다 썼거나 알아볼 만한 캐릭터가 없으면) 새로 지어내지 말고 **같은 자리의 `<자리>-again-prompt.txt`**(계획기가 쓴 캐릭터 가운데 덜 입은 하나 · 아직 안 입은 재단을 정해 둔 2회차 지시문)를 그대로 그린다 — 기록 `generation.cosplay` 는 그 지시문의 캐릭터 · 재단. 그 파일이 없으면(쓴 캐릭터가 아직 없다) 1회차로 고른다. 그래도 막히면 그 컷을 다시 짠다: `node tools/casual-plan.cjs <카드> --session <같은 세션> --keep <카드>:<다른 컷 번호> --cosplay-full <게임 열쇠> --reserve --push`. 그린 뒤 기록에 `generation.cosplay: { "game": "<게임 열쇠>", "character": "<그린 캐릭터 영어 이름 — 1회차는 채운 이름>", "cut": "<재단 열쇠>" }`(세 공방이 이 칸으로 쓴 캐릭터를 센다)와 실제로 넘긴 글(`submitted`).

**프롬프트 임의 수정 금지 — 이미지 모델에도 똑같다(2026-11-08).** IMAGE_RULES.md 1절의 변경 사유(settings 고친 뒤 build · 막혔을 때 계획기 다시 계획 · 같은 지시문 재생성 · 사용자가 시킨 부분 고치기) 말고는 낱말 하나도 고치지 않는다. image_gen 에도 이 글 그대로 넘기고(`submitted` 0 일 때만) 고쳐 쓰지 말고 그대로 그리게 한다.

**노출은 세션이 줄이지 않는다.** 노출 · 의상 줄을 빼거나 누그러뜨리거나 고정값(강도 strong · 노출 bold)을 미리 낮추지 않는다 — 실제로 막혔을 때만 IMAGE_RULES.md 3절 7 순서(같은 지시문 한 번 → 노출 한 단계씩 settings exposure · exposure_why → 계획기로 장면 다시). 검수 `qa.json` 에 컷마다 `exposure`(match · weaker · stronger + 근거).
기록에는 `<자리>-ui.json`(생성기 저장값과 같은 꼴)과 지시문을 둔다 — 관리기를 쓰면 `python3 tools/image-runner.py intent --card 197 --slot <자리> --prompt <이 폴더>/<자리>-prompt.txt --ui <이 폴더>/<자리>-ui.json`.

| 차례 | 자리 | 첨부 | 지시문 | 낱말 | sha256(앞 12) | 올릴 파일 |
|---|---|---|---|---|---|---|
| ① | light | 없음 | `light-prompt.txt` | 908 | `9e253fa87ca5` | `블래키_light_anime_25d_gloss_f.webp` |
| ② | casual1 | ① 블래키_light_anime_25d_gloss_f.webp | `casual1-prompt.txt` | 1169 | `4dffd4d33abe` | `블래키_anime_25d_gloss_f_casual1.webp` |
| ③ | casual2 | ① 블래키_light_anime_25d_gloss_f.webp | `casual2-prompt.txt` | 1157 | `04574cb139ad` | `블래키_anime_25d_gloss_f_casual2.webp` |
| ④ | casual3 | ① 블래키_light_anime_25d_gloss_f.webp | `casual3-prompt.txt` | 1148 | `ed4dfef1563d` | `블래키_anime_25d_gloss_f_casual3.webp` |
| ⑤ | casual4 | ① 블래키_light_anime_25d_gloss_f.webp | `casual4-prompt.txt` | 1101 | `52886b60b571` | `블래키_anime_25d_gloss_f_casual4.webp` |
| ⑥ | casual5 | ① 블래키_light_anime_25d_gloss_f.webp | `casual5-prompt.txt` | 1133 | `dbf3e14893e3` | `블래키_anime_25d_gloss_f_casual5.webp` |
| ⑦ | casual6 | ① 블래키_light_anime_25d_gloss_f.webp | `casual6-prompt.txt` | 1212 | `8731fcb24559` | `블래키_anime_25d_gloss_f_casual6.webp` |
| ⑧ | casual7 | ① 블래키_light_anime_25d_gloss_f.webp | `casual7-prompt.txt` | 1217 | `84f2a0919821` | `블래키_anime_25d_gloss_f_casual7.webp` |
| ⑨ | casual8 | ① 블래키_light_anime_25d_gloss_f.webp | `casual8-prompt.txt` | 1084 | `f324369be034` | `블래키_anime_25d_gloss_f_casual8.webp` |
| ⑩ | casual9 | ① 블래키_light_anime_25d_gloss_f.webp | `casual9-prompt.txt` | 1185 | `a6a7218e64ae` | `블래키_anime_25d_gloss_f_casual9.webp` |
| ⑪ | casual10 | ① 블래키_light_anime_25d_gloss_f.webp | `casual10-prompt.txt` | 1147 | `b636cb479e16` | `블래키_anime_25d_gloss_f_casual10.webp` |
| ◆ | casual90 | ① 블래키_light_anime_25d_gloss_f.webp | `casual90-prompt.txt` | 1071 | `0b7efad84d7e` | `블래키_anime_25d_gloss_f_casual90.webp` |

## ② casual1 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 전망대 | a hilltop lookout over a wide valley |
| 역할 | — |  |
| 의상 | 수영복 · 컷아웃 원피스 | a fully lined one-piece swimsuit with large cut-outs at the sides of the waist |
| 몸 자세 · 구도 | 난간·창턱에 기대 서기 · waist_up · 옆모습 | standing at a waist-high railing or sill |
| 손 · 소품 동작 | prop · rail · 우산 · 우산을 쓴다 | holds an umbrella open over her shoulder |

옷 종류 swimsuit · 옷 색 코랄 · 오렌지 (coral and soft orange) · 드러내기 plunging neckline, high-cut leg · 장면 칸 첫머리 detail

## ③ casual2 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 마을 열매 시장 | a village market stall piled with fresh berries |
| 역할 | — |  |
| 의상 | 휴양지 차림 · 랩 점프슈트(짧은) | a wrap-front holiday romper with a deep V neckline and a tie belt |
| 몸 자세 · 구도 | 위로 손 뻗기 · full_body · 옆모습 | standing close to a high shelf or line, reaching up to it |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 jumpsuit · 옷 색 핑크 · 로즈 (rose pink and blush) · 상황 젖은 옷 — 비 · 물 튐 · 드러내기 sweetheart neckline, cutout waist · 장면 칸 첫머리 place

## ④ casual3 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 대회 무대 | a contest or tournament stage under spotlights |
| 역할 | — |  |
| 의상 | 게임 코스프레 · 트임 롱드레스 | a daring adult cosplay of Mario from Super Mario Bros. — Mario's outfit — a red cap with a plain white circle badge, a red top, blue overalls with big yellow buttons, white gloves and brown boots, cut as a floor-length gown with a thigh-high slit |
| 몸 자세 · 구도 | 서기 · full_body · 뒤 3/4 | standing |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 dress · 옷 색 — · 게임 코스프레 슈퍼 마리오 브라더스 · Mario(마리오) · 트임 롱드레스 · 1회차 · 드러내기 deep V neckline, backless · 장면 칸 첫머리 light

## ⑤ casual4 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 현관 | the entryway of her home with a shoe bench, coat hooks and a long mirror |
| 역할 | — |  |
| 의상 | 란제리풍 · 보디수트 | a lingerie bodysuit with a scooped neckline, wide straps and lace side panels |
| 몸 자세 · 구도 | 바닥에 앉기 · three_quarter · 3/4 정면 | sitting on the ground |
| 손 · 소품 동작 | chin_knee · floor_brace |  |

옷 종류 bodysuit + lingerie_set · 옷 색 그레이 · 실버 (dove grey and silver) · 드러내기 plunging neckline, halter neck · 장면 칸 첫머리 action

## ⑥ casual5 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 옥상 파티 | a city rooftop party under string lights |
| 역할 | — |  |
| 의상 | 포켓몬 코스튬 · 크롭 투피스형 | a daring adult costume version of {costume}, cut as a cropped top and a micro skirt that bare the midriff |
| 몸 자세 · 구도 | 가장자리에 걸터앉기 · chest_up · 3/4 정면 | perched on a ledge or edge |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 crop_top + skirt · 옷 색 — · 드러내기 sweetheart neckline, mini length · 장면 칸 첫머리 place

## ⑦ casual6 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 포켓몬 세계 안 | inside the Pokémon world, as if she simply lives there |
| 장소 | 그늘진 잔디밭 | a shaded lawn with a picnic blanket under a broad tree |
| 역할 | — |  |
| 의상 | 동탄룩 · 튜브탑 + 하이웨이스트 레깅스 | a tight tube top under an open cropped cardigan with glossy high-waisted leggings that outline the hips and legs |
| 몸 자세 · 구도 | 엎드리기 · environmental · 3/4 정면 | lying on her front |
| 손 · 소품 동작 | AUTO · AUTO |  |

옷 종류 cardigan + leggings · 옷 색 — · 갈래 · 상황 자유(자유 장면) · 드러내기 deep V neckline, side cutouts · 장면 칸 첫머리 detail

## ⑧ casual7 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 육상 트랙 | a running track with lane lines and a grandstand |
| 역할 | — |  |
| 의상 | 평상복 · 자동 — 계열 안에서 장면에 맞게 | everyday clothes that suit the place and activity |
| 몸 자세 · 구도 | 서기 · face_close · 정면 | standing |
| 손 · 소품 동작 | shush · out |  |

옷 종류 shirt + shorts · 옷 색 세이지 · 올리브 (sage and olive green) · 드러내기 plunging neckline, one-shoulder cut · 장면 칸 첫머리 light

## ⑨ casual8 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 지금 현실 | present-day real world |
| 장소 | 수리 가게 작업대 | a small repair kiosk with a cluttered workbench, a low stool, tools hanging on the wall and an open shutter onto the street |
| 역할 | — |  |
| 의상 | 역할극·직업 의상 · 카지노 딜러 | a casino dealer costume with a fitted waistcoat, bow tie and cuffs |
| 몸 자세 · 구도 | 무릎 꿇기 · three_quarter · 뒤 3/4 | kneeling on the ground |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 vest · 옷 색 스카이 · 네이비 (sky blue and navy) · 드러내기 sweetheart neckline, cropped hem · 장면 칸 첫머리 action

## ⑩ casual9 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 무대·환상 | a stylised stage, editorial or fantasy setting not bound to a real year |
| 장소 | 정글 유적 | overgrown jungle temple ruins — mossy stone steps, hanging vines and shafts of light through the canopy |
| 역할 | — |  |
| 의상 | 무대·판타지 의상 · 마법사 | a sorceress costume — an off-shoulder velvet robe gown with a jewelled belt and a crystal staff prop |
| 몸 자세 · 구도 | 벽에 기대 서기 · chest_up · 3/4 정면 | standing, leaning back against a wall |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 dress + robe · 옷 색 — · 옷 자유 · 드러내기 deep V neckline, high thigh slit · 장면 칸 첫머리 action

## ⑪ casual10 — 고른 장면(버전2)

| 칸 | 고른 것 | 지시문 문장 |
|---|---|---|
| 시대 | 첫 등장 무렵 현실 | the real world around the year her Pokémon first appeared |
| 장소 | 박물관 갈라 | a grand museum hall with marble statues at night |
| 역할 | — |  |
| 의상 | 웨딩 · 브라이덜 레이스 | a white lace bridal lingerie set with a short veil |
| 몸 자세 · 구도 | 서기 · waist_up · 뒤 3/4 | standing |
| 손 · 소품 동작 | natural · natural |  |

옷 종류 lingerie_set · 옷 색 — · 장면 자유(자유 장면) · 드러내기 plunging neckline, bare midriff · 장면 칸 첫머리 light

## ◆ casual90 — 캐릭터만의 컷(카페 야간 바 전문 · 노출 bold)

일상 열 장에 더하는 한 장 — 채울 칸이 없다. 막히면 같은 지시문으로 두 번 더(모두 세 번), 그래도 막히면 계획기 `--own --own-level` 로 한 단계 내려 다시 짓는다(IMAGE_RULES 3절 「캐릭터만의 컷」).

| 칸 | 표의 글 |
|---|---|
| 장소 | a cozy café — a wooden counter, an espresso machine, glass pastry cases and hanging pendant lamps |
| 장면 | she is the night-bar specialist perched sideways on a stool, polishing a small cup on the counter with both hands |
| 의상 | a barista look fitted to her body — a short café apron over a fitted tank top and short skirt, bare shoulders and legs, a set of golden ring marks on her sleeves |
| 도구 | — |
| 자세 추천 | bench_fix |
