# 더 리버 원에 쓴 외부 재료
전부 Poly Haven(polyhaven.com) CC0. 출처 표기 의무 없음, 상업 사용 가능.
- 재질(512 WebP로 줄임): marble_01, white_plaster_02, natural_walnut_veneer, smoked_walnut_veneer, rough_linen, velour_velvet
- 모델(meshopt + WebP 1024/512): Ottoman_01, ceramic_vase_01, modern_ceiling_lamp_01, potted_plant_02, potted_plant_04, wine_bottles_01
- 모델 2차(sim/shrink_glb.mjs로 텍스처 512, 메시 단순화 후 meshopt): dining_chair_02, modern_wooden_cabinet, fancy_picture_frame_01, hanging_picture_frame_01, ornate_mirror_01, tea_set_01, vintage_electric_kettle, wooden_display_shelves_01, desk_lamp_arm_01
- 한강 물 노멀: three.js 예제 waternormals.jpg(MIT, three.js authors) → water_nor.webp 1024. Poly Haven이 아닌 유일한 재료
- 별: HYG 4.1(astronexus, CC BY-SA 4.0, 히파르코스 기반) 등급 8 이하의 실제 좌표. sim/gen_stars.mjs가 src/stars.js로 묶음. 이미지 아님, 출시물 크레딧 필요
- HDRI: qwantani_dusk_2_puresky 1k
빌드 때 scripts/gen_assets.py가 src/assets.js(base64)로 묶음.
- 차: ferrari.glb = three.js 예제의 Ferrari 458 Italia, 만든 이 vicent091036 (Sketchfab, CC BY 4.0, https://sketchfab.com/models/57bf6cc56931426e87494f554df1dab6). 출시물엔 이 줄을 크레딧에 넣을 것
- 주차장 슈퍼카 7대와 로비 오브제 4종 (Sketchfab, 11/2에 유진님 계정으로 받음, sim/slim_model.mjs로 실내 제거·단순화·텍스처 256~512 WebP·meshopt). 출시물엔 아래 줄을 크레딧에 넣을 것. NC는 비상업 조건
  - aventador.glb = "Lamborghini Aventador SVJ SDC ( FREE )" by SDC PERFORMANCE™️, CC BY 4.0, https://sketchfab.com/3d-models/784e4656aca649cca55d6b18740a19b2
  - revuelto.glb = "Free Lamborghini Revuelto" by ALIEEEN, CC BY 4.0, https://sketchfab.com/3d-models/cf52245eb68f48daa909c7ad2a8deaa3
  - gt3.glb = "2022 Porsche 911 GT3 Touring (992)" by Ddiaz Design, CC BY-NC-SA 4.0, https://sketchfab.com/3d-models/a76364a3d50c4d78912a28250cb57be5 (내 차로도 씀)
  - roadster.glb = "Tesla Roadster" by Mona x Supercars, CC BY 4.0, https://sketchfab.com/3d-models/6ad8555df20f4f56985de23a587998cb
  - taycan.glb = "2020 Porsche Taycan Turbo S" by OUTPISTON, CC BY-NC-SA 4.0, https://sketchfab.com/3d-models/3657f54c69c242f09fae93104bb20120
  - cybertruck.glb = "Tesla Cybertruck" by A Certain Duck, CC BY 4.0, https://sketchfab.com/3d-models/1ab0c3f248fa47019c4311abce9731a0
  - targa.glb = "2021 Porsche 911 Targa 4S (992)" by Ddiaz Design, CC BY-NC-SA 4.0, https://sketchfab.com/3d-models/8981d73373bd4d92bb429c5621f0f50d
  - flowers.glb = "flowers with the vase" by Musaev H.N., CC BY 4.0, https://sketchfab.com/3d-models/0f58352d377840cdbeef0bd71b24aff6
  - orchid.glb = "Orchidea" by Antonio Rossini, CC BY 4.0, https://sketchfab.com/3d-models/9e351f19b3ba4910b7d15954e49ae178
  - lilies.glb = "Vase with lilies _ Metashape" by Moshe Caine, CC BY 4.0, https://sketchfab.com/3d-models/67a08a5b930e46c4b5805a3887adcf06
  - bird.glb = "Bird In Space sculpture Brâncuși" by FarnazShahriari_, CC BY 4.0, https://sketchfab.com/3d-models/6f86e6d65ce64619bf013f6a6ee7ebef
  - ferrari.glb은 11/2에 뺌(내 차를 GT3로 바꿈, 용량 때문). 원본은 assets/candidates/ferrari.glb
- 가전·오브제 9종 (Sketchfab, 11/2, slim_model.mjs): marzocco.glb = "La Marzocco Coffee Machine" by Akeelah (CC BY), mixer.glb = "KitchenAid Stand mixer" by MelissaVerdonck (CC BY), toaster.glb = "Smeg Toaster" by The Fresh Lab (CC BY), winefridge.glb = "Wine fridge 39 metal" by Rustam T (CC BY), beoplay.glb = "Bang & Olufsen Beoplay A9" by JAMES SA (CC BY), tv.glb = "Sony BRAVIA XR-77A80L OLED TV" by eltayerkebulan (CC BY), candle.glb = "Scented Candle" by Brownbreadrender (CC BY), bath.glb = "Angelo Freestanding Bath" by tissinouk (CC BY), shower.glb = "Rain Shower Head" by Rita Santos (CC BY). uid는 sim/_dl/<이름>/license.txt. 욕조·샤워기는 욕실이 생기면 놓을 것(아직 미배치)
- 강변도로(11/2, Poly Haven CC0): 재질 asphalt_02, leafy_grass, gravelly_sand(1k → 512 WebP, sim/tex512.mjs). 모델 island_tree_02, island_tree_01, tree_small_02(sim/slim_tree.mjs: 잎 카드 1~2%만 남기고 3.6~4.4배 키움, 줄기·가지 단순화, 잎 512·껍질 256 WebP), shrub_02(slim_model.mjs). 원본은 sim/_ph/
- 거실 소파(11/2): dune.glb = "Dune_sofa_ARobj" by qasimroy, CC BY 4.0, https://sketchfab.com/3d-models/be4fe0bcfc2e4138b63effbd3f756252 (텍스처 떼고 slim_model.mjs). 천 재질 curly_teddy_natural = Poly Haven CC0(tex512.mjs). 곡선 소파는 코드로 만듦(penthouse.js curvedSofa).
- 식탁·창가 원탁·서재 의자(11/2): tulip.glb = "saarinen tulip chair" by Grapxly, CC BY 4.0(작가 표시 NoAI: 생성형 AI 데이터셋·입력 사용 금지), https://sketchfab.com/3d-models/bc48eb1d27794a7baa8b2009aff5590e (텍스처 떼고 slim_model.mjs 0.07).
- 주방 가전(11/2): ovenstack.glb = "Oven, Microwave and Winecooler" by lutz_westerfeld, CC BY 4.0, https://sketchfab.com/3d-models/60ffe27b68dd4f9cb9f79b7b61350311 (와인쿨러와 앞면 제작자 글자 지움, 0.6). hob.glb = "Bosch Series 6 Induction Hob With Extractor" by 3dvisualisierung, CC BY 4.0, https://sketchfab.com/3d-models/87ba25dddee44f6da9dc35bac1bfd015 (0.7, 화면엔 브랜드 표시 없음).
- 안방 라운지 체어(11/2): mid_century_lounge_chair = Poly Haven CC0(shrink_glb 512, 0.5). 시네마 영화는 파일을 넣지 않고 위키미디어에서 재생: 〈샤레이드〉(Stanley Donen, 1963, 퍼블릭 도메인), 〈신텔〉(Blender Foundation, CC BY 3.0), 〈스프링〉(Blender Studio, CC BY 4.0). 인터넷이 없거나 막히면 원래의 빛 화면으로 돌아감.
- 3층 라이브러리와 온실(11/2, Poly Haven CC0): book_encyclopedia_set_01(낱장 면 빼고 표지만, 책등 아틀라스는 서가 인스턴스에도 씀), Chandelier_01, GreenChair_01, ClassicConsole_01, marble_bust_01, pachira_d(pachira_aquatica_01의 가장 큰 그루), fern_b(fern_02의 한 포기). sim/pick_nodes.mjs로 고른 뒤 slim_model.mjs. 원본은 sim/_ph/
- 테라스(11/3, Poly Haven CC0): grass_tuft.glb = grass_medium_01, fern.glb = fern_02 (slim_model, slim_tree).
- 도로 차와 강 위 배(11/3, Poly Pizza, slim_model로 줄임): CC0 = v_suv.glb "SUV" by Quaternius (poly.pizza/m/xsMtZhBkxL), b_sail.glb "Sail Boat" by Quaternius (poly.pizza/m/BgSZXwmm7k). CC BY 3.0 = v_sedan.glb "Car" by Quaternius (poly.pizza/m/HQ0hvRM2XR), v_pickup.glb "Mitsubishi L200" by Muhammad Reyhan (poly.pizza/m/4qjS9tFhsJg), b_ferry.glb "Boat" by Poly by Google (poly.pizza/m/c2SYxaiPfF3), b_cruise.glb "Cruise ship" by Poly by Google (poly.pizza/m/dgLCxDWhnZQ), b_liner.glb "Cruise liner" by Poly by Google (poly.pizza/m/cPiY_8RZMHE), b_motor.glb "Boat" by Poly by Google (poly.pizza/m/8vekojz4Abf)
- 오리배(11/3): b_swan.glb = "Swanboat" by yuma727, CC BY 4.0, https://sketchfab.com/3d-models/swanboat-a80e756ed56e4df8a24800c349f1d878 (유진님 계정으로 받음. 왕관과 페달을 빼고 선체를 파랑, 좌석을 노랑으로 바꾸고 눈의 흰 점을 지운 뒤 면 수를 줄임, sim/_dl/swanboat)

## 서재 책 본문
빌드에 내장되어 인터넷 없이 열림. `node gen_books.mjs <원문 폴더>` → `src/text/books.js`(한자 읽기표 hanja.json), 본문 글꼴은 고운바탕(SIL OFL) 부분 글꼴 `gen_bookfont.py` → `src/text/bookfont.js`.
한국 저작권: 1962년 이전 사망 작가는 보호기간 만료(2013년 70년 연장 대상 아님). 원문은 한국어 위키문헌(ko.wikisource.org), 영어는 Project Gutenberg(머리말과 꼬리말을 뺀 본문).

| 작가 | 사망 | 넣은 작품 | 판본 |
|---|---|---|---|
| 김소월 | 1934 | 진달래꽃(1925) 124편 | 위키문헌 현대어 표기 |
| 한용운 | 1944 | 님의 침묵(1926) 94편 | 위키문헌 현대어 표기 |
| 윤동주 | 1945 | 하늘과 바람과 별과 시 72편 | 1948, 1955년판. 한자만 한글로, 읍니다는 습니다로, 나머지 표기는 원본 그대로 |
| 이육사 | 1944 | 육사시집(1946)에서 16편 | 위키문헌 |
| 정지용 | 1950 | 향수, 창, 바다(오늘의 시에만) | 위키문헌 |
| 이장희 | 1929 | 봄은 고양이로다(오늘의 시에만) | 위키문헌 |
| 현진건 | 1943 | 운수 좋은 날, B사감과 러브레터 | 위키문헌 |
| 이효석 | 1942 | 메밀꽃 필 무렵 | 위키문헌 |
| 김유정 | 1937 | 봄봄, 동백꽃, 금 따는 콩밭 | 위키문헌 |
| 이상 | 1937 | 날개, 권태, 산촌여정 | 위키문헌 |
| 김동인 | 1951 | 감자, 배따라기 | 위키문헌 |
| 나도향 | 1926 | 그믐달 | 위키문헌 |
| F. Scott Fitzgerald | 1940 | The Great Gatsby(1925), Gutenberg 64317 | |
| O. Henry | 1910 | The Gift of the Magi(1905), Gutenberg 7256 | |
| Oscar Wilde | 1900 | The Happy Prince, The Selfish Giant(1888), Gutenberg 902 | |
| Edgar Allan Poe | 1849 | The Tell-Tale Heart(1843), Gutenberg 2148 | |
| Charlotte Perkins Gilman | 1935 | The Yellow Wallpaper(1892), Gutenberg 1952 | |
| William Shakespeare | 1616 | Sonnets(1609), Gutenberg 1041 | |

뺀 것: 염상섭(1963 사망, 한국에서 보호 중), 백석(1996), 주요한(1979), Robert Frost(1963, 미국은 만료지만 한국은 보호 중), 김영랑(1950, 만료지만 위키문헌에 1935년 원문 표기만 있어 읽기 어려움).
- 4층 헬스장과 수영장 선베드(11/3, Sketchfab, 유진님 계정으로 1k GLB를 받음, sim/slim_model.mjs로 단순화, 텍스처 WebP 512(원판 256), meshopt). 공개할 때 아래 크레딧을 표기해야 함:
  - treadmill.glb = "Treadmill Machine" by Sousinho, CC BY 4.0(작가 표시 NoAI: 생성형 AI 학습에 쓰지 말 것), https://sketchfab.com/3d-models/faed3a2a275b4fd68089e1d8bdfb7f89
  - squatrack.glb = "Squat Rack With Bar" by Sousinho, CC BY 4.0(NoAI), https://sketchfab.com/3d-models/8e3109a049274de2941e7a2e014aa10d
  - flatbench.glb = "Flat Bench" by Sousinho, CC BY 4.0(NoAI), https://sketchfab.com/3d-models/b56ab6e2b50246c88c7f72a4f16fc857
  - inclinebench.glb = "Incline Bench" by Sousinho, CC BY 4.0(NoAI), https://sketchfab.com/3d-models/bdc274649c234c188d2d4f4c732acb1c
  - plates.glb = "Weightlifting Bumper Plates" by Sousinho, CC BY 4.0(NoAI), https://sketchfab.com/3d-models/221e92f466114ffc99c1bc9c86a4ad17
  - weightroom.glb = "Weight Room Set 2" by Tytan, CC BY 4.0, https://sketchfab.com/3d-models/fa481412927e43dfbeab9f6da464c15b
  - sunbed.glb = "Beach Chair Sunbed low Low-poly 3D model" by cvato5555, CC BY 4.0, https://sketchfab.com/3d-models/da9838a86f594664b1dc4dba7edf1fe2 (천을 아이보리로 바꿈: CC BY 수정 표시)
