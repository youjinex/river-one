# 더 리버 원에 쓴 외부 재료
게임 안 크레딧 화면은 src/credits.js. 새 재료를 넣으면 여기와 그 파일에 같이 적음.
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
- 안방 라운지 체어(11/2): mid_century_lounge_chair = Poly Haven CC0(shrink_glb 512, 0.5). 시네마 영화는 11/3 아래 '홈시네마 영화' 줄로 바뀜.
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
  - sunbed.glb = "Beach Chair Sunbed low Low-poly 3D model" by cvato5555, CC BY 4.0, https://sketchfab.com/3d-models/da9838a86f594664b1dc4dba7edf1fe2 (천을 아이보리로 바꿈. 11/3 오후에 뺌: 배처럼 보이고 사람이 아래로 들어가서 tower.js의 코드 선베드로 바꿈)

## 음악 (11/3, 파일에 넣지 않고 스트리밍, src/music.js)
- 쇼팽 녹턴, 왈츠, 전주곡: Musopen 쇼팽 전집, CC0, https://archive.org/details/musopen-chopin
- 캐롤 판: "Starlifter and Roots in Blue" 2020 (United States Air Force Band of Mid-America) 11곡, 미국 정부 저작물이라 퍼블릭 도메인, Wikimedia Commons 파일명 `<곡명> (2020) - Starlifter and Roots in Blue - United States Air Force Band of Mid-America.mp3`
- 합창 캐롤 판: Silent Night, Silent Night (1990), Carols of the Season (Singing Sergeants, United States Air Force Band), 퍼블릭 도메인, Wikimedia Commons. Jingle Bells (Calm), Deck the Halls A (Kevin MacLeod), CC BY 3.0
- 보사노바와 2층 라운지 음악: Bossa Antigua, Casa Bossa Nova, BossaBossa, Backbay Lounge, Airport Lounge, Gymnopedie No. 1, 2, 3 (Kevin MacLeod, incompetech.com), CC BY 3.0, Wikimedia Commons
- 힙합 판(11/4 교체, 랩 곡 위주. Free Music Archive 장르 태그 Hip-Hop, rap 확인. 공용 사본을 mp3 변환본으로 스트리밍):
  - Kellee Maize, "Signs", CC BY 3.0, 공용 https://commons.wikimedia.org/wiki/File:Kellee_Maize_-_04_-_04_Signs.ogg, 원 출처 https://freemusicarchive.org/music/Kellee_Maize/Aligned_Archetype/04__Kellee_Maize__Signs__Aligned_Archetype__FrostWirecom
  - GHATS, "Mind Over Matter", CC BY 4.0, 공용 https://commons.wikimedia.org/wiki/File:GHATS_-_MIND_OVER_MATTER.wav, 원 출처: 작가가 공용에 직접 올림
  - K3N, "One Million Ways", CC BY 4.0, 공용 https://commons.wikimedia.org/wiki/File:K3N_-_One_Million_Ways.ogg, 원 출처 https://freemusicarchive.org/music/K3N_X/One_Million_Ways/One_Million_Ways
  - Hi-Rez (Prod. Instinctz Beats), "Better Place", CC BY 4.0, 공용 https://commons.wikimedia.org/wiki/File:Hi-Rez_-_04_-_Better_Place_Prod_by_Instinctz_Beats.ogg, 원 출처 https://freemusicarchive.org/music/Hi-Rez/Lost_Time/04_Hi_Rez_Better_Place_Lost_Time_2013_FROSTWIRE_FROSTCLICK_CREATIVE_COMMONS
  - Black Ant, "Underdog", CC BY 3.0, 공용 https://commons.wikimedia.org/wiki/File:Black_Ant_-_14_-_Underdog.mp3, 원 출처 https://freemusicarchive.org/music/Black_Ant/Free_Beats_Sel_3/
  - CuzOH! Black feat. Wordsmith, "Stronger Living", CC BY 4.0, 공용 https://commons.wikimedia.org/wiki/File:CuzOH_Black_Feat_Wordsmith_-_05_-_Stronger_Living_Feat_Wordsmith.ogg, 원 출처 https://freemusicarchive.org/music/CuzOH_Black_Feat_Wordsmith/FrostWire_Creative_Commons_Mixtape_Volume_4/05_Wordsmith_Stronger_Living_The_Backstage_EP_FROSTCLICK_FROSTWIRE_CREATIVE_COMMONS_MIXTAPE_VOL_4
  - Nangdo, "Rattan Joint", CC BY 4.0, 공용 https://commons.wikimedia.org/wiki/File:Nangdo_-_Rattan_Joint.ogg, 원 출처 https://freemusicarchive.org/music/Nangdo/Chrome/05_Rattan_Joint
  - Kellee Maize, "Mothership", CC BY 3.0, 공용 https://commons.wikimedia.org/wiki/File:Kellee_Maize_-_05_-_05_Mothership.ogg, 원 출처 https://freemusicarchive.org/music/Kellee_Maize/Aligned_Archetype/05__Kellee_Maize__Mothership__Aligned_Archetype__FrostWirecom
  - Jules, "Gone", CC BY 4.0, 공용 https://commons.wikimedia.org/wiki/File:Jules_-_Jules_01_Gone.ogg, 원 출처 https://freemusicarchive.org/music/Jules/Gone_1676/Jules_01_Gone
  - 빼낸 옛 곡: Broke For Free "Simple Hop", JBlanked "Beat Cook Up 1, 3, 5", Purrple Cat 3곡(힙합 같지 않다는 말로 교체)
  - ccMixter는 다른 사이트에서의 재생을 403으로 막고, archive.org의 힙합은 대부분 NC-ND라 뺌
- 합창 판(11/4): 미 공군 밴드 Singing Sergeants, 미국 정부 저작물이라 퍼블릭 도메인(music.af.mil Public Domain Music). 곡도 보호기간이 끝났거나 공군 단원 작곡:
  - U.S. Air Force Band Singing Sergeants, "셰넌도어", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Shenandoah_-_Singing_Sergeants_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
  - U.S. Air Force Band Singing Sergeants, "Soave sia il vento", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:%22Soave_Sia_Il_Vento%22_from_Cosi_Fan_Tutte_-_Singing_Sergeants_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
  - U.S. Air Force Band Singing Sergeants, "무정한 마음", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Core_%27ngrato_-_Singing_Sergeants_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
  - U.S. Air Force Band Singing Sergeants, "Raisins and Almonds", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Raisins_and_Almonds_-_Singing_Sergeants_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
  - U.S. Air Force Band Singing Sergeants, "Fresh Powder", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Fresh_Powder_-_Singing_Sergeants_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
  - U.S. Air Force Band Singing Sergeants, "Skip to My Lou", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Skip_to_My_Lou_-_Singing_Sergeants_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
- 재즈 보컬 판(11/4):
  - Pierce Murphy, "If You Won’t Choose Me", CC BY 4.0, 공용 https://commons.wikimedia.org/wiki/File:Pierce_Murphy_-_01_-_If_You_Wont_Choose_Me.ogg, 원 출처 https://freemusicarchive.org/music/Pierce_Murphy/This_Isnt_Magic_It_Is_Just_Music/Pierce_Murphy_-_This_Isnt_Magic_It_Is_Just_Music-_A_Demo_-_01_If_You_Wont_Choose_Me
  - U.S. Air Force Band, "Amazing Grace", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Amazing_Grace_(USAFB_jazz_vocal).ogg, 원 출처 http://www.usafband.af.mil/ensembles/BandEnsSongs.asp?Ensemble=-1&Genre=6
  - Pierce Murphy, "Just Give It Time", CC BY 4.0, 공용 https://commons.wikimedia.org/wiki/File:Pierce_Murphy_-_02_-_Just_Give_It_Time.ogg, 원 출처 https://freemusicarchive.org/music/Pierce_Murphy/This_Isnt_Magic_It_Is_Just_Music/Pierce_Murphy_-_This_Isnt_Magic_It_Is_Just_Music-_A_Demo_-_07_Just_Give_It_Time
  - Frédéric Lardon feat. Laura Palmée, "Dans le love", CC0, 공용 https://commons.wikimedia.org/wiki/File:Frederic_Lardon_feat_Laura_Palme_-_09_-_Dans_le_love.ogg, 원 출처 https://freemusicarchive.org/music/Frederic_Lardon_feat_Laura_Palme/Korgi/Frederic_Lardon_feat_Laura_Palme_-_Korgi_-_09_Dans_le_love
  - Pierce Murphy, "Will You Whisper", CC BY 4.0, 공용 https://commons.wikimedia.org/wiki/File:Pierce_Murphy_-_06_-_Will_You_Whisper.ogg, 원 출처 https://freemusicarchive.org/music/Pierce_Murphy/This_Isnt_Magic_It_Is_Just_Music/Pierce_Murphy_-_This_Isnt_Magic_It_Is_Just_Music-_A_Demo_-_11_Will_You_Whisper
  - Pierce Murphy, "Try To Be Nice", CC BY 4.0, 공용 https://commons.wikimedia.org/wiki/File:Pierce_Murphy_-_03_-_Try_To_Be_Nice.ogg, 원 출처 https://freemusicarchive.org/music/Pierce_Murphy/This_Isnt_Magic_It_Is_Just_Music/Pierce_Murphy_-_This_Isnt_Magic_It_Is_Just_Music-_A_Demo_-_08_Try_To_Be_Nice
  - Frédéric Lardon feat. Laura Palmée, "Dans la campagne", CC0, 공용 https://commons.wikimedia.org/wiki/File:Frederic_Lardon_feat_Laura_Palme_-_05_-_Dans_la_campagne.ogg, 원 출처 https://freemusicarchive.org/music/Frederic_Lardon_feat_Laura_Palme/Korgi/Frederic_Lardon_feat_Laura_Palme_-_Korgi_-_05_Dans_la_campagne
- 빅밴드 판(11/4): 미 공군 Airmen of Note(퍼블릭 도메인)와 미 육군 Army Blues(CC0). Stardust(1927)와 아리랑은 곡도 보호기간이 끝났고 나머지는 단원 작곡:
  - U.S. Air Force Band Airmen of Note, "Sheridan Square", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Sheridan_Square_-_Airmen_of_Note_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
  - U.S. Army Blues, "Stardust", CC0, 공용 https://commons.wikimedia.org/wiki/File:US_Army_Blues_-_05_-_Stardust.ogg, 원 출처 https://freemusicarchive.org/music/US_Army_Blues/Live_At_Blues_Alley/0_-_05_-_The_US_Army_Blues_-_Stardust
  - U.S. Air Force Band Airmen of Note, "Uno Mas", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Uno_Mas_-_Airmen_of_Note_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
  - U.S. Air Force Band Airmen of Note, "아리랑", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Arirang_-_Airmen_of_Note_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
  - U.S. Air Force Band Airmen of Note, "Blues for Mundy", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Blues_for_Mundy_-_Airmen_of_Note_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
  - U.S. Air Force Band Airmen of Note, "It’s a Brand New Day", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:It%27s_a_Brand_New_Day_-_Airmen_of_Note_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
  - U.S. Air Force Band Airmen of Note, "Small Note Boogaloo", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Small_Note_Boogaloo_-_Airmen_of_Note_-_United_States_Air_Force_Band.mp3, 원 출처 https://www.music.af.mil/Multimedia/Music/Public-Domain-Music/
- 시티팝은 CC BY나 퍼블릭 도메인 녹음을 찾지 못해 넣지 않음
- 지하 1층 라운지 음악(11/3 저녁, 위키미디어 공용에서 스트리밍): Kevin MacLeod(incompetech.com) "Disco Lounge", "Club Diver", "Ether Disco", "Carpe Diem", "Electro Cabello", CC BY 3.0, 공용 파일명 `<곡명> (ISRC ...).mp3`. Tentacles "Lavanda (We Are Not Dj's Nu Disco Remix)", CC BY 4.0, 공용 파일 Tentacles_-_06_-_Lavanda_We_Are_Not_Djs_Nu_Disco_Remix.ogg(mp3 변환본으로 재생). 주소는 src/music.js의 CLUB
- 3층 라이브러리 음악(11/4, 서가 쪽에서만, src/music.js LIBRARY). Musopen 녹음은 Musopen이 퍼블릭 도메인이나 CC0로 내놓은 것, 미 육군 밴드는 미국 정부 저작물. 곡은 모두 보호기간이 끝남:
  - 차이콥스키 곡, Musopen Symphony Orchestra 연주, "Symphony No. 6 “Pathétique” II", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Tchaikovsky,_Symphony_No._6_in_B_minor,_Op._74,_%27Pathetique%27_-_II._Allegro_con_gracia.ogg
  - 보로딘 곡, Musopen String Quartet 연주, "String Quartet No. 2 III. Notturno", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Borodin_-_String_Quartet_No._2_in_D_major_-_III._Notturno._Andante_(Musopen_String_Quartet).flac
  - 차이콥스키 곡, Musopen 연주, "Piano Concerto No. 1 II. Andantino", CC0, 공용 https://commons.wikimedia.org/wiki/File:Tchaikovsky,_Concerto_No.1_in_B-flat_minor_Op.23,_II._Andantino.ogg
  - 드보르자크 곡, Musopen String Quartet 연주, "String Quartet No. 12 “American” II. Lento", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Dvo%C5%99%C3%A1k_-_String_Quartet_No._12_in_F_major,_Op._96_%27American%27_-_II._Lento_(Musopen_String_Quartet).flac
  - 수크 곡, Musopen String Quartet 연주, "Meditation on the Old Czech Chorale, Op. 35a", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Josef_Suk_-_Meditation_Op_35a.ogg
  - 차이콥스키 곡, U.S. Army Band Strings 연주, "Souvenir de Florence III", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Tchaikovsky_-_Souvenir_de_Florence,_mvt-3_-_US_Army_Band.oga
  - 그리그 곡, Musopen Symphony Orchestra 연주, "Peer Gynt: Morning Mood", 퍼블릭 도메인, 공용 https://commons.wikimedia.org/wiki/File:Musopen_-_Morning.ogg
  - 브람스 곡, Musopen Symphony Orchestra 연주, "Symphony No. 3 III. Poco allegretto", CC0, 공용 https://commons.wikimedia.org/wiki/File:Brahms,_Symphony_No._3_in_F_Major,_Op._90_-_III._Poco_allegretto.ogg
  - 차이콥스키 사계는 사람이 연주한 자유 이용 녹음을 공용과 archive.org에서 찾지 못함(공용 것은 MIDI 렌더링, CC BY-SA)
- 갤러리 벤치 음악(11/4, galseat에 앉았을 때만, src/music.js GALLERY): 바흐 골드베르크 변주곡, Kimiko Ishizaka 연주(Open Goldberg Variations), CC0:
  - Kimiko Ishizaka, "Aria", CC0, 공용 https://commons.wikimedia.org/wiki/File:Kimiko_Ishizaka_-_J.S._Bach-_-Open-_Goldberg_Variations,_BWV_988_(Piano)_-_01_Aria.mp3
  - Kimiko Ishizaka, "Variatio 3", CC0, 공용 https://commons.wikimedia.org/wiki/File:Kimiko_Ishizaka_-_J.S._Bach-_-Open-_Goldberg_Variations,_BWV_988_(Piano)_-_04_Variatio_3_a_1_Clav._Canone_all_Unisuono.mp3
  - Kimiko Ishizaka, "Variatio 13", CC0, 공용 https://commons.wikimedia.org/wiki/File:Kimiko_Ishizaka_-_J.S._Bach-_-Open-_Goldberg_Variations,_BWV_988_(Piano)_-_14_Variatio_13_a_2_Clav.mp3
  - Kimiko Ishizaka, "Variatio 15", CC0, 공용 https://commons.wikimedia.org/wiki/File:Kimiko_Ishizaka_-_J.S._Bach-_-Open-_Goldberg_Variations,_BWV_988_(Piano)_-_16_Variatio_15_a_1_Clav._Canone_alla_Quinta.mp3
  - Kimiko Ishizaka, "Variatio 21", CC0, 공용 https://commons.wikimedia.org/wiki/File:Kimiko_Ishizaka_-_J.S._Bach-_-Open-_Goldberg_Variations,_BWV_988_(Piano)_-_22_Variatio_21_Canone_alla_Settima.mp3
  - Kimiko Ishizaka, "Variatio 25", CC0, 공용 https://commons.wikimedia.org/wiki/File:Kimiko_Ishizaka_-_J.S._Bach-_-Open-_Goldberg_Variations,_BWV_988_(Piano)_-_26_Variatio_25_a_2_Clav.mp3
  - Kimiko Ishizaka, "Aria da Capo", CC0, 공용 https://commons.wikimedia.org/wiki/File:Kimiko_Ishizaka_-_J.S._Bach-_-Open-_Goldberg_Variations,_BWV_988_(Piano)_-_31_Aria_da_Capo_%C3%A8_Fine.mp3
- 곡 자체도 모두 보호기간이 끝났음: Silent Night(1818), Jingle Bells(1857), O Holy Night(1847), Auld Lang Syne, Satie(1888). 재생 주소는 src/music.js에 전부 있음
- 한강 산책로와 점프 공원(11/3, Poly Haven CC0): 재질 concrete_pavers(보행로 블록), granite_wall(호안), rubber_tiles(놀이터 고무 바닥, tex512.mjs). 모델 modular_street_seating(벤치), metal_trash_can, wooden_picnic_table, rock_07(징검돌, 회색으로 물들임), rock_09·boulder_01(내려받았으나 미사용, boulder는 2MB라 뺌), tree_stump_01/02(발판), planter_box_01(허들), old_tyre(slim_model.mjs). 원본은 sim/_ph/
- 점프 공원과 편의점 소품(11/3, Poly Pizza, sim/_dl/polypizza2, slim_model.mjs). 전부 CC BY 3.0이라 출시물에 크레딧 필요:
  - bike_a.glb = "Bicycle" by Poly by Google, poly.pizza/m/19VoUuA2pcN
  - bike_b.glb = "Bicycle" by Poly by Google, poly.pizza/m/b6USSQA731J
  - bike_rack.glb = "Bike Rack" by J-Toastie, poly.pizza/m/DzsJ2LPVKZ
  - parasol.glb = "Parasol" by Zsky, poly.pizza/m/FLEbO2jluO
  - store.glb = "Store" by Mrhadley, poly.pizza/m/TJwNAgLlrS
  - vending.glb = "Vending Machine" by Don Carson, poly.pizza/m/0CX6wj64Swu
  - slide.glb = "Slide" by Poly by Google, poly.pizza/m/dDe3njWPbg0
  - junglegym.glb = "Jungle gym" by Poly by Google, poly.pizza/m/0-7U_RTHzKT
  - swing.glb = "Swing set" by Poly by Google, poly.pizza/m/e-IJdcqZH4p
  - seesaw.glb = "Seesaw" by Poly by Google, poly.pizza/m/8Ha-8ms-TJb

## 갤러리와 카페 그림(11/3)
그림 파일은 첫 로딩 재료에 넣지 않음. assets/art/{s,l}/*.webp → 빌드가 dist/gallery와 reports/gallery로 복사 → 층에 들어갈 때 받음. 원본 목록 art_list.json, 받기 gen_art_dl.mjs, 가공 gen_art.py.
작가는 모두 1955년 이전 사망이고(가장 늦은 사람은 뭉크 1944) 작품은 그 전에 완성됨. 아래는 작품별 받은 곳과 표시.
- sunrise: 클로드 모네, 인상, 해돋이, 1872. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Monet_-_Impression,_Sunrise.jpg
- parasol: 클로드 모네, 파라솔을 든 여인, 1875. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Claude_Monet,_Woman_with_a_Parasol_-_Madame_Monet_and_Her_Son,_1875,_NGA_61379.jpg
- adresse: 클로드 모네, 생타드레스의 정원, 1867. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Garden_at_Sainte-Adresse_MET_DT48.jpg
- grenouillere: 클로드 모네, 라 그르누예르, 1869. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:La_Grenouill%C3%A8re_MET_DT833.jpg
- poppies: 클로드 모네, 아르장퇴유 근처의 양귀비밭, 1875. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Poppy_Fields_near_Argenteuil_MET_DT1034.jpg
- stacks: 클로드 모네, 건초더미, 여름의 끝, 1891. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Claude_Monet_-_Stacks_of_Wheat_(End_of_Summer)_-_1985.1103_-_Art_Institute_of_Chicago.jpg
- normandy: 클로드 모네, 노르망디 열차의 도착, 1877. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Claude_Monet_-_Arrival_of_the_Normandy_Train,_Gare_Saint-Lazare_-_Google_Art_Project.jpg
- rouen: 클로드 모네, 루앙 대성당, 정문, 1894. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Rouen_Cathedral-_The_Portal_(Sunlight)_MET_DT2185.jpg
- fourtrees: 클로드 모네, 네 그루 나무, 1891. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:The_Four_Trees_MET_DT832.jpg
- magpie: 클로드 모네, 까치, 1869. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Claude_Monet_-_The_Magpie_-_Google_Art_Project.jpg
- kerchief: 클로드 모네, 빨간 스카프, 1873. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1958.39
- pourville: 클로드 모네, 푸르빌의 썰물, 1882. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1947.196
- antibes: 클로드 모네, 앙티브의 정원사 집, 1888. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1916.1044
- lilies_b: 클로드 모네, 수련, 1926. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1960.81
- lilies_d: 클로드 모네, 수련, 1906. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Claude_Monet_-_Water_Lilies_-_1906,_Ryerson.jpg
- lilies_e: 클로드 모네, 수련 연못, 1899. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Claude_Monet,_The_Water-Lily_Pond_(National_Gallery,_London).jpg
- bridge: 클로드 모네, 수련 연못 위의 다리, 1899. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Bridge_over_a_Pond_of_Water_Lilies_MET_DT1854.jpg
- footbridge: 클로드 모네, 일본식 다리, 1899. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Claude_Monet,_The_Japanese_Footbridge,_1899,_NGA_74796.jpg
- c1: 클로드 모네, 봄, 꽃 핀 과일나무, 1873. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Spring_(Fruit_Trees_in_Bloom)_MET_DT1902.jpg
- c2: 클로드 모네, 지베르니 근처 센강의 아침, 1897. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Morning_on_the_Seine_near_Giverny_MET_DT1903.jpg
- c3: 클로드 모네, 봄꽃, 1864. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1953.155
- venus: 산드로 보티첼리, 비너스의 탄생, 1485. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Sandro_Botticelli_-_La_nascita_di_Venere_-_Google_Art_Project_-_edited.jpg
- liberty: 외젠 들라크루아, 민중을 이끄는 자유의 여신, 1830. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Eug%C3%A8ne_Delacroix_-_La_libert%C3%A9_guidant_le_peuple.jpg
- nightwatch: 렘브란트 판 레인, 야경, 1642. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:The_Night_Watch_-_HD.jpg
- meninas: 디에고 벨라스케스, 시녀들, 1656. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Las_Meninas,_by_Diego_Vel%C3%A1zquez,_from_Prado_in_Google_Earth.jpg
- jatte: 조르주 쇠라, 그랑드 자트 섬의 일요일 오후, 1886. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Georges_Seurat_-_A_Sunday_on_La_Grande_Jatte_--_1884_-_Google_Art_Project.jpg
- starry: 빈센트 반 고흐, 별이 빛나는 밤, 1889. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Van_Gogh_-_Starry_Night_-_Google_Art_Project.jpg
- mona: 레오나르도 다 빈치, 모나리자, 1519. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Mona_Lisa,_by_Leonardo_da_Vinci,_from_C2RMF_retouched.jpg
- pearl: 요하네스 페르메이르, 진주 귀걸이를 한 소녀, 1665. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:1665_Girl_with_a_Pearl_Earring.jpg
- milkmaid: 요하네스 페르메이르, 우유 따르는 여인, 1660. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Johannes_Vermeer_-_Het_melkmeisje_-_Google_Art_Project.jpg
- pitcher: 요하네스 페르메이르, 물병을 든 젊은 여인, 1662. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Young_Woman_with_a_Water_Pitcher_MET_DP353257.jpg
- aristotle: 렘브란트 판 레인, 호메로스 흉상을 바라보는 아리스토텔레스, 1653. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Aristotle_with_a_Bust_of_Homer_MET_DP319026.jpg
- harvest: 피터르 브뤼헐, 수확하는 사람들, 1565. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Pieter_Bruegel_the_Elder-_The_Harvesters_-_Google_Art_Project.jpg
- hals: 프란스 할스, 즐거운 술꾼, 1629. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Frans_Hals_002.jpg
- roosterman: 프란스 할스, 틸레만 로스테르만의 초상, 1634. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1999.173
- rembeard: 렘브란트 판 레인, 모자를 쓴 수염 난 남자, 1658. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1950.252
- windmill: 야코프 판 라위스달, 풍차가 있는 풍경, 1646. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1967.19
- beyeren: 아브라함 판 베이예런, 은 주전자와 햄, 과일, 1663. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1960.80
- delft: 요하네스 페르메이르, 델프트 풍경, 1661. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:View_of_Delft,_by_Johannes_Vermeer.jpg
- balance: 요하네스 페르메이르, 저울을 든 여인, 1664. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Johannes_Vermeer_-_Woman_Holding_a_Balance_-_Google_Art_Project.jpg
- artpaint: 요하네스 페르메이르, 회화의 기술, 1667. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Jan_Vermeer_-_The_Art_of_Painting_-_Google_Art_Project.jpg
- musicians: 카라바조, 음악가들, 1597. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:The_Musicians_MET_DP-687-001.jpg
- andrew: 카라바조, 성 안드레아의 순교, 1607. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1976.2
- calabazas: 디에고 벨라스케스, 칼라바사스의 초상, 1632. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1965.15
- burning: 윌리엄 터너, 국회의사당의 화재, 1835. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1942.647
- dance: 에드가 드가, 발레 수업, 1874. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:The_Dance_Class_MET_DT46.jpg
- frieze: 에드가 드가, 춤추는 사람들, 1895. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1946.83
- boating: 에두아르 마네, 보트 놀이, 1874. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Boating_MET_DT45.jpg
- cards: 폴 세잔, 카드놀이 하는 사람들, 1892. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:The_Card_Players_MET_DP231550.jpg
- paris: 귀스타브 카유보트, 파리의 거리, 비 오는 날, 1877. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Gustave_Caillebotte_-_Paris_Street;_Rainy_Day_-_Google_Art_Project.jpg
- sisters: 피에르 오귀스트 르누아르, 두 자매, 1881. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Pierre-Auguste_Renoir_-_Two_Sisters_(On_the_Terrace)_-_Google_Art_Project.jpg
- lunch: 피에르 오귀스트 르누아르, 뱃놀이 일행의 점심, 1881. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Pierre-Auguste_Renoir_-_Luncheon_of_the_Boating_Party_-_Google_Art_Project.jpg
- moulin: 피에르 오귀스트 르누아르, 물랭 드 라 갈레트의 무도회, 1876. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Auguste_Renoir_-_Dance_at_Le_Moulin_de_la_Galette_-_Google_Art_ProjectFXD.jpg
- bathchild: 메리 커샛, 아이의 목욕, 1893. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Mary_Cassatt_-_The_Child%27s_Bath_-_Google_Art_Project.jpg
- sainte: 폴 세잔, 생트빅투아르산, 1904. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1958.21
- madamex: 존 싱어 사전트, 마담 X, 1884. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Madame_X_(Madame_Pierre_Gautreau),_John_Singer_Sargent,_1884_(unfree_frame_crop).jpg
- tahiti: 폴 고갱, 아베 마리아, 1891. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Ia_Orana_Maria_(Hail_Mary)_MET_DT1025.jpg
- kiss: 구스타프 클림트, 키스, 1908. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:The_Kiss_-_Gustav_Klimt_-_Google_Cultural_Institute.jpg
- scream: 에드바르 뭉크, 절규, 1893. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Edvard_Munch_-_The_Scream_-_NG.M.00939_-_National_Museum_of_Art,_Architecture_and_Design.jpg
- bedroom: 빈센트 반 고흐, 침실, 1889. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Vincent_van_Gogh_-_The_Bedroom_-_Google_Art_Project.jpg
- cypress: 빈센트 반 고흐, 사이프러스가 있는 밀밭, 1889. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Wheat_Field_with_Cypresses_MET_DT1567.jpg
- irises: 빈센트 반 고흐, 붓꽃, 1890. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Irises_MET_DP346474.jpg
- sunflowers: 빈센트 반 고흐, 해바라기, 1888. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Vincent_van_Gogh_-_Sunflowers_(1888,_National_Gallery_London).jpg
- strawhat: 빈센트 반 고흐, 밀짚모자를 쓴 자화상, 1887. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Vincent_van_Gogh_-_Self-portrait_with_straw_hat_-_Google_Art_Project.jpg
- terrace: 빈센트 반 고흐, 밤의 카페 테라스, 1888. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Van_Gogh_-_Terrace_of_a_Caf%C3%A9_at_Night_(Place_du_Forum)_1888.jpg
- menders: 빈센트 반 고흐, 길을 고치는 사람들, 1889. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1947.209
- poplars: 빈센트 반 고흐, 포플러 두 그루, 1889. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1958.32
- suwa: 우타가와 히로시게, 스와 호수, 1850. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1985.259
- sumida: 우타가와 히로시게, 스미다강의 밤, 1850. CC0. Cleveland Museum of Art Open Access, https://clevelandart.org/art/1920.274
- socrates: 자크 루이 다비드, 소크라테스의 죽음, 1787. CC0. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:The_Death_of_Socrates_MET_DT40.jpg
- temeraire: 윌리엄 터너, 전함 테메레르, 1839. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:The_Fighting_Temeraire,_JMW_Turner,_National_Gallery.jpg
- wanderer: 카스파르 다비트 프리드리히, 안개 바다 위의 방랑자, 1818. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Caspar_David_Friedrich_-_Wanderer_above_the_Sea_of_Fog.jpeg
- gleaners: 장 프랑수아 밀레, 이삭 줍는 여인들, 1857. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Jean-Fran%C3%A7ois_Millet_-_Gleaners_-_Google_Art_Project.jpg
- ermine: 레오나르도 다 빈치, 흰 담비를 안은 여인, 1490. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Lady_with_an_Ermine_-_Leonardo_da_Vinci_-_Google_Art_Project.jpg
- athens: 라파엘로 산치오, 아테네 학당, 1511. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Raphael_School_of_Athens.jpg
- odalisque: 장 오귀스트 도미니크 앵그르, 그랑드 오달리스크, 1814. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Ingre,_Grande_Odalisque.jpg
- swing: 장 오노레 프라고나르, 그네, 1767. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Fragonard,_The_Swing.jpg
- babel: 피터르 브뤼헐, 바벨탑, 1563. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Pieter_Bruegel_the_Elder_-_The_Tower_of_Babel_(Vienna)_-_Google_Art_Project_-_edited.jpg
- arnolfini: 얀 반 에이크, 아르놀피니 부부의 초상, 1434. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Van_Eyck_-_Arnolfini_Portrait.jpg
- whistler: 제임스 휘슬러, 화가의 어머니, 1871. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Whistlers_Mother_high_res.jpg
- wave: 가쓰시카 호쿠사이, 가나가와 해변의 높은 파도 아래, 1831. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Great_Wave_off_Kanagawa2.jpg
- redfuji: 가쓰시카 호쿠사이, 붉은 후지산, 1831. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Katsushika_Hokusai_-_Fine_Wind,_Clear_Morning_(Gaif%C5%AB_kaisei)_-_Google_Art_Project.jpg
- shower: 우타가와 히로시게, 오하시 다리의 소나기, 1857. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Hiroshige,_Sudden_shower_over_Shin-%C5%8Chashi_bridge_and_Atake,_1857.jpg
- plum: 우타가와 히로시게, 가메이도의 매화 정원, 1857. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Ando_Hiroshige_-_Plum_Garden,_Kameido_-_Google_Art_Project.jpg
- beauties: 기타가와 우타마로, 당대 세 미인, 1793. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Utamaro1.jpg
- inwang: 정선, 인왕제색도, 1751. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Inwangjesaekdo.jpg
- geumgang: 정선, 금강전도, 1734. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Geumgangjeondo.jpg
- lilies_a: 클로드 모네, 수련, 1926. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Claude_Monet_-_Water_Lilies_-_Google_Art_Project_(431238).jpg
- lilies_c: 클로드 모네, 수련, 1926. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Claude_Monet,_Water_Lilies,_ca._1915-1926.jpg
- miindo: 신윤복, 미인도, 1805. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Shin_Yun-bok_-_A_Beautiful_Woman_-_Google_Art_Project.jpg
- ssireum: 김홍도, 씨름, 1780. Public domain. Wikimedia Commons, https://commons.wikimedia.org/wiki/File:Danwon-Ssireum.jpg
- 거실 턴테이블(11/3): turntable.glb = "Yamaha TT-300 Record Player" by AleixoAlonso, CC BY 4.0, https://sketchfab.com/3d-models/3577a2a1a0c24218bd5d768beccf218e (유진님 계정으로 1k GLB를 받아 slim_model.mjs 0.55, 텍스처 512. 부품을 나눠 플래터와 톤암을 움직임, 판과 라벨은 코드로 얹음. CC0 턴테이블은 Poly Haven, Poly Pizza, Sketchfab에 쓸 만한 것이 없었음)
- 홈시네마 영화(11/3, 샤레이드 뺌): 파일을 넣지 않고 위키미디어 커먼스 변환본(480p VP9, 안 되면 360p MP4)을 바로 재생, 포스터는 커먼스 장면 썸네일(330px, seek). 인터넷이 없거나 막히면 원래의 빛 화면. 출시물에 크레딧 필요:
  - 〈빅 벅 버니〉 Big Buck Bunny (2008), Blender Foundation, CC BY 3.0, commons.wikimedia.org/wiki/File:Big_Buck_Bunny_4K.webm
  - 〈신텔〉 Sintel (2010), Blender Foundation, CC BY 3.0, commons.wikimedia.org/wiki/File:Sintel_movie_4K.webm
  - 〈스프링〉 Spring (2019), Andy Goralczyk / Blender Studio, CC BY 4.0, commons.wikimedia.org/wiki/File:Spring_-_Blender_Open_Movie.webm
  - 〈티어스 오브 스틸〉 Tears of Steel (2012), Blender Foundation, CC BY 3.0, commons.wikimedia.org/wiki/File:Tears_of_Steel_1080p.webm
  - 〈윙 잇!〉 WING IT! (2023), Blender Studio, CC BY 4.0, commons.wikimedia.org/wiki/File:WING_IT!_-_Blender_Open_Movie-full_movie.webm
  - 〈커피 런〉 Coffee Run (2020), Blender Studio, CC BY 4.0, commons.wikimedia.org/wiki/File:Coffee_Run_-_Blender_Open_Movie-full_movie.webm
  - 〈카미난데스 3: 라미고스〉 Caminandes 3: Llamigos (2016), Blender Foundation, CC BY 3.0, commons.wikimedia.org/wiki/File:Caminandes_3_-_Llamigos_-_Blender_Animated_Short.webm
  - 후보였지만 뺀 것: Charge(총격), Sprite Fright(호러 코미디), Cosmos Laundromat(자살 시도로 시작), Elephants Dream(난해), Caminandes 2(CC BY-SA)

## 나무 잎(11/3)
- leaf_atlas.webp = Poly Haven "Searsia Lucida"(https://polyhaven.com/a/searsia_lucida) CC0의 잎과 껍질 텍스처(1k PNG를 512 WebP로, 69KB). src/topiary.js가 이 잎으로 회양목, 월계수, 올리브 잎 판과 잎마다 기울기를 담은 노멀 판을 실행 중에 그려 씀. 로비 앞, 옥상, 47층 테라스 나무가 이 재료 하나를 같이 씀. 새 파일 추가 없음.

## 온실 꽃과 잎(11/4, Poly Haven CC0)
- anthurium_botany_01.glb(343KB), calathea_orbifolia_01.glb(166KB), periwinkle_plant.glb(149KB): Poly Haven 모델(https://polyhaven.com/a/anthurium_botany_01, /calathea_orbifolia_01, /periwinkle_plant) CC0. 세트 파일에서 한 그루만 pick_nodes.mjs로 남기고 shrink_glb.mjs(텍스처 512)로 줄임. 첫 로딩 재료가 약 0.66MB 늘어남.
- 수국 꽃송이와 장미는 파일 없이 src/topiary.js가 그려 씀. 걸이 화분과 덩굴 잎은 기존 leaf_atlas.
