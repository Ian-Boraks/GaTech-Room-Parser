# GaTech-Room-Parser [![Run on Repl.it](https://repl.it/badge/github/Ian-Boraks/GaTech-Room-Parser)](https://repl.it/github/Ian-Boraks/GaTech-Room-Parser)

Used for displaying the number of beds left for GaTech housing.

The data is collected from https://housing.gatech.edu/available-rooms using an API call to https://housing.gatech.edu/rooms/FreeRooms.json?_=1655904358700 .

If you want a JS tool similar to this that can be ran straight in your browser, [click me](https://gist.github.com/VR314/6c4d05bd8cdce60d4a2bd01ff3634464). This tool was created by [VR314](https://github.com/VR314).

---

To set up the config, use the following command line arguments:

Gender:

> `-g <Male, Female, Neutral, All>`

Capacity (Room Type):

> `-c <Double, Triple, Quad, Suite, 2 person, 4 person, 6 person, All>`

bed_empty (Beds in room for -e and -er to be true):
>   `-C <int>`


List Empty Rooms:
>   1. `-e`   (will list just the empty room count)
>   2. `-er`  (will list both the count and the room names)

List Bed Names:

> `-b`

Output to a HTML File:

> `-fo`

Run Silently (Use w/ -csv):

> `-s`

---

Example outputs:

```
Updated on: 2022-06-22 18:50:03
Using Config: {'gender': 'All', 'capacity': 'All', 'beds': False, 'csv': False, 'silent': False}

Dorm                        Beds Left
------------------------  -----------
Armstrong                         103
Brown                              50
Eighth St East (Honors)            90
Eighth St South (Honors)           93
Field                               6
Fitten                             10
Freeman                            66
Fulmer                             47
Hanson                             39
Harrison                           74
Hefner                            100
Hopkins                             5
Montag                             77
Smith                             268
Woodruff North                    232
Woodruff South                    219
```

```
Updated on: 2022-06-22 18:50:03
Using Config: {'gender': 'All', 'capacity': 'All', 'beds': True, 'csv': False, 'silent': False}

Dorm         Beds Left
---------  -----------
Armstrong          103
Rooms: [ARM101a, ARM101b, ARM102a, ARM102b, ARM103a, ARM103b, ARM104a, ARM104b, ARM106a, ARM106b, ARM107a, ARM107b, ARM108a, ARM108b, ARM109a, ARM109b, ARM110a, ARM110b, ARM111a, ARM111b, ARM112a, ARM112b, ARM113a, ARM113b, ARM114a, ARM114b, ARM116a, ARM116b, ARM117a, ARM117b, ARM118a, ARM118b, ARM119a, ARM119b, ARM201a, ARM201b, ARM202a, ARM202b, ARM203a, ARM203b, ARM204a, ARM204b, ARM206a, ARM206b, ARM207a, ARM207b, ARM208a, ARM208b, ARM209a, ARM209b, ARM210a, ARM210b, ARM211a, ARM211b, ARM212a, ARM212b, ARM213a, ARM213b, ARM214a, ARM214b, ARM216a, ARM216b, ARM217a, ARM217b, ARM218a, ARM218b, ARM220a, ARM220b, ARM301a, ARM301b, ARM302a, ARM302b, ARM303a, ARM303b, ARM304a, ARM304b, ARM306a, ARM306b, ARM307a, ARM307b, ARM308a, ARM308b, ARM309a, ARM309b, ARM310a, ARM310b, ARM311a, ARM311b, ARM312a, ARM312b, ARM313a, ARM313b, ARM314a, ARM314b, ARM315b, ARM316a, ARM316b, ARM317a, ARM317b, ARM318a, ARM318b, ARM320a, ARM320b]

Dorm      Beds Left
------  -----------
Brown            50
Rooms: [BRN102a, BRN102b, BRN103a, BRN103b, BRN104a, BRN104b, BRN105a, BRN105b, BRN106a, BRN106b, BRN107a, BRN107b, BRN109a, BRN109b, BRN110a, BRN110b, BRN111a, BRN111b, BRN113a, BRN113b, BRN114b, BRN209b, BRN214b, BRN217b, BRN301a, BRN301b, BRN302a, BRN302b, BRN304a, BRN304b, BRN305a, BRN305b, BRN306a, BRN306b, BRN307a, BRN307b, BRN308a, BRN308b, BRN309a, BRN309b, BRN310a, BRN310b, BRN311a, BRN311b, BRN312a, BRN312b, BRN313a, BRN313b, BRN314a, BRN314b]

Dorm                       Beds Left
-----------------------  -----------
Eighth St East (Honors)           90
Rooms: [ESE104A, ESE104B, ESE108A, ESE108B, ESE108C, ESE108D, ESE109A, ESE109C, ESE109D, ESE113A, ESE113B, ESE113C, ESE113D, ESE116A, ESE116B, ESE116C, ESE116D, ESE118A, ESE118B, ESE118C, ESE118D, ESE202A, ESE202B, ESE202C, ESE202D, ESE202E, ESE202F, ESE205A, ESE205B, ESE205C, ESE205D, ESE208A, ESE208B, ESE208C, ESE208D, ESE209A, ESE209B, ESE209C, ESE209D, ESE213A, ESE213B, ESE213C, ESE213D, ESE217A, ESE217B, ESE217C, ESE217D, ESE218A, ESE218B, ESE218C, ESE218D, ESE218E, ESE218F, ESE302A, ESE302B, ESE302C, ESE302D, ESE302E, ESE302F, ESE304A, ESE304B, ESE305A, ESE305B, ESE305C, ESE305D, ESE308B, ESE308C, ESE308D, ESE311A, ESE311B, ESE311C, ESE311D, ESE313A, ESE313B, ESE313C, ESE313D, ESE315A, ESE315B, ESE315C, ESE315D, ESE316A, ESE316B, ESE316C, ESE316D, ESE318A, ESE318B, ESE318C, ESE318D, ESE318E, ESE318F]

Dorm                        Beds Left
------------------------  -----------
Eighth St South (Honors)           93
Rooms: [ESS105A, ESS105B, ESS106A, ESS106C, ESS106D, ESS108A, ESS108B, ESS108C, ESS108D, ESS111A, ESS111B, ESS111C, ESS111D, ESS112A, ESS112B, ESS112C, ESS112D, ESS114A, ESS114B, ESS114C, ESS114D, ESS201A, ESS201B, ESS201C, ESS201D, ESS201E, ESS201F, ESS203A, ESS203B, ESS203C, ESS203D, ESS204A, ESS204B, ESS204C, ESS204D, ESS208A, ESS208B, ESS208C, ESS208D, ESS210A, ESS210B, ESS210C, ESS210D, ESS211A, ESS211B, ESS211C, ESS211D, ESS213A, ESS213B, ESS213C, ESS213D, ESS213E, ESS213F, ESS214A, ESS214B, ESS214C, ESS214D, ESS301A, ESS301B, ESS301C, ESS301D, ESS301E, ESS301F, ESS303A, ESS303B, ESS303C, ESS303D, ESS304A, ESS304B, ESS304C, ESS304D, ESS306A, ESS306B, ESS306C, ESS306D, ESS308A, ESS308B, ESS308C, ESS308D, ESS310A, ESS310B, ESS310C, ESS310D, ESS311A, ESS311B, ESS311C, ESS311D, ESS313A, ESS313B, ESS313C, ESS313D, ESS313E, ESS313F]

Dorm      Beds Left
------  -----------
Field             6
Rooms: [FLD113b, FLD213b, FLD401c, FLD401d, FLD413b, FLD416b]

Dorm      Beds Left
------  -----------
Fitten           10
Rooms: [FIT103a, FIT103b, FIT107a, FIT107b, FIT108a, FIT108b, FIT109a, FIT109b, FIT111a, FIT111b]

Dorm       Beds Left
-------  -----------
Freeman           66
Rooms: [FRE108b, FRE110b, FRE114a, FRE114b, FRE116a, FRE116b, FRE118a, FRE118b, FRE201a, FRE201b, FRE202a, FRE202b, FRE205a, FRE205b, FRE209a, FRE209b, FRE210a, FRE210b, FRE213a, FRE213b, FRE214a, FRE214b, FRE216a, FRE216b, FRE217a, FRE217b, FRE219a, FRE219b, FRE220a, FRE220b, FRE301a, FRE301b, FRE302a, FRE302b, FRE303a, FRE303b, FRE305a, FRE305b, FRE306a, FRE306b, FRE307a, FRE307b, FRE308a, FRE308b, FRE309a, FRE309b, FRE311a, FRE311b, FRE312a, FRE312b, FRE313a, FRE313b, FRE314a, FRE314b, FRE315a, FRE315b, FRE316a, FRE316b, FRE317a, FRE317b, FRE318a, FRE318b, FRE319a, FRE319b, FRE320a, FRE320b]

Dorm      Beds Left
------  -----------
Fulmer           47
Rooms: [FUL202b, FUL203a, FUL203b, FUL205a, FUL205b, FUL206a, FUL206b, FUL209a, FUL209b, FUL210a, FUL210b, FUL211a, FUL211b, FUL212a, FUL212b, FUL213a, FUL213b, FUL215a, FUL215b, FUL301a, FUL301b, FUL302a, FUL302b, FUL303a, FUL303b, FUL304a, FUL304b, FUL305a, FUL305b, FUL306a, FUL306b, FUL307a, FUL307b, FUL308a, FUL308b, FUL310a, FUL310b, FUL311a, FUL311b, FUL312a, FUL312b, FUL313a, FUL313b, FUL314a, FUL314b, FUL315a, FUL315b]

Dorm      Beds Left
------  -----------
Hanson           39
Rooms: [HAN301a, HAN301b, HAN311a, HAN311b, HAN312a, HAN312b, HAN313b, HAN314a, HAN314b, HAN315a, HAN315b, HAN401a, HAN401b, HAN402a, HAN402b, HAN403a, HAN403b, HAN404a, HAN404b, HAN405a, HAN405b, HAN406a, HAN406b, HAN408a, HAN408b, HAN409a, HAN409b, HAN410a, HAN410b, HAN411a, HAN411b, HAN412a, HAN412b, HAN413a, HAN413b, HAN414a, HAN414b, HAN415a, HAN415b]

Dorm        Beds Left
--------  -----------
Harrison           74
Rooms: [HRN002a, HRN002b, HRN002c, HRN002d, HRN004a, HRN004b, HRN005a, HRN005b, HRN006a, HRN006b, HRN007a, HRN007b, HRN008a, HRN008b, HRN008c, HRN008d, HRN010a, HRN010b, HRN011b, HRN102b, HRN105a, HRN105b, HRN105c, HRN105d, HRN108a, HRN108b, HRN108c, HRN108d, HRN111a, HRN111b, HRN114a, HRN114b, HRN114c, HRN114d, HRN117a, HRN117b, HRN117c, HRN117d, HRN120a, HRN120b, HRN207a, HRN207b, HRN207c, HRN207d, HRN210a, HRN210b, HRN210c, HRN210d, HRN216a, HRN216b, HRN216c, HRN216d, HRN219c, HRN219d, HRN304b, HRN305a, HRN305b, HRN307a, HRN307b, HRN307c, HRN307d, HRN310a, HRN310b, HRN310c, HRN310d, HRN313a, HRN313b, HRN316d, HRN319a, HRN319b, HRN319c, HRN319d, HRN323a, HRN323b]

Dorm      Beds Left
------  -----------
Hefner          100
Rooms: [HEF102a, HEF102b, HEF103a, HEF103b, HEF104a, HEF104b, HEF105a, HEF105b, HEF107a, HEF107b, HEF108a, HEF108b, HEF109a, HEF109b, HEF110a, HEF110b, HEF111a, HEF111b, HEF112a, HEF112b, HEF113a, HEF113b, HEF114a, HEF114b, HEF115a, HEF115b, HEF116a, HEF116b, HEF117a, HEF117b, HEF118a, HEF118b, HEF201a, HEF201b, HEF202a, HEF202b, HEF203a, HEF203b, HEF204a, HEF204b, HEF205a, HEF205b, HEF207a, HEF207b, HEF208a, HEF208b, HEF209a, HEF209b, HEF210a, HEF210b, HEF211a, HEF211b, HEF212a, HEF212b, HEF213a, HEF213b, HEF214a, HEF214b, HEF215a, HEF215b, HEF216a, HEF216b, HEF217a, HEF217b, HEF218a, HEF218b, HEF219a, HEF219b, HEF302a, HEF302b, HEF303a, HEF303b, HEF304a, HEF304b, HEF305a, HEF305b, HEF307a, HEF307b, HEF308a, HEF308b, HEF309a, HEF309b, HEF311a, HEF311b, HEF312a, HEF312b, HEF313a, HEF313b, HEF314a, HEF314b, HEF315a, HEF315b, HEF316a, HEF316b, HEF317a, HEF317b, HEF318a, HEF318b, HEF319a, HEF319b]

Dorm       Beds Left
-------  -----------
Hopkins            5
Rooms: [HOP209b, HOP301c, HOP301d, HOP401c, HOP401d]

Dorm      Beds Left
------  -----------
Montag           77
Rooms: [MON101a, MON101b, MON107a, MON107b, MON109a, MON109b, MON110a, MON110b, MON111a, MON111b, MON112b, MON113a, MON113b, MON117b, MON201a, MON201b, MON202a, MON202b, MON203a, MON203b, MON205a, MON205b, MON207a, MON207b, MON208a, MON208b, MON209a, MON209b, MON211a, MON211b, MON212a, MON212b, MON213a, MON213b, MON214a, MON214b, MON215b, MON216a, MON216b, MON217a, MON217b, MON219a, MON219b, MON220a, MON220b, MON301a, MON301b, MON302a, MON302b, MON303a, MON303b, MON306a, MON306b, MON307a, MON307b, MON308a, MON308b, MON309a, MON309b, MON310a, MON310b, MON311a, MON311b, MON312a, MON312b, MON313a, MON313b, MON316a, MON316b, MON317a, MON317b, MON318a, MON318b, MON319a, MON319b, MON320a, MON320b]

Dorm      Beds Left
------  -----------
Smith           268
Rooms: [SMT103a, SMT103b, SMT105a, SMT105b, SMT107a, SMT107b, SMT109a, SMT109b, SMT111a, SMT111b, SMT112a, SMT112b, SMT113a, SMT113b, SMT114a, SMT114b, SMT115a, SMT115b, SMT116a, SMT116b, SMT117a, SMT117b, SMT118a, SMT118b, SMT126a, SMT126b, SMT127a, SMT127b, SMT128a, SMT128b, SMT129a, SMT129b, SMT129c, SMT129d, SMT130a, SMT130b, SMT130c, SMT130d, SMT201a, SMT201b, SMT201c, SMT201d, SMT202a, SMT202b, SMT202c, SMT202d, SMT203a, SMT203b, SMT204a, SMT204b, SMT206a, SMT206b, SMT207a, SMT207b, SMT209a, SMT209b, SMT210a, SMT210b, SMT210c, SMT210d, SMT212a, SMT212b, SMT214a, SMT214b, SMT215a, SMT215b, SMT216a, SMT216b, SMT217a, SMT217b, SMT218a, SMT218b, SMT219a, SMT219b, SMT220a, SMT220b, SMT221a, SMT221b, SMT223a, SMT223b, SMT224a, SMT224b, SMT225a, SMT225b, SMT226a, SMT226b, SMT230a, SMT230b, SMT231a, SMT231b, SMT232a, SMT232b, SMT232c, SMT234a, SMT234b, SMT235a, SMT235b, SMT236a, SMT236b, SMT238a, SMT238b, SMT238c, SMT238d, SMT239a, SMT239b, SMT239c, SMT239d, SMT301a, SMT301b, SMT301c, SMT301d, SMT302a, SMT302b, SMT302c, SMT302d, SMT303a, SMT303b, SMT304a, SMT304b, SMT307a, SMT307b, SMT309a, SMT309b, SMT310a, SMT310b, SMT310c, SMT310d, SMT311a, SMT311b, SMT319a, SMT319b, SMT320a, SMT320b, SMT321a, SMT321b, SMT322a, SMT322b, SMT323a, SMT323b, SMT324a, SMT324b, SMT325a, SMT325b, SMT327a, SMT327b, SMT328a, SMT328b, SMT329a, SMT329b, SMT330a, SMT330b, SMT331a, SMT331b, SMT332a, SMT332b, SMT333a, SMT333b, SMT334a, SMT334b, SMT337a, SMT337b, SMT338a, SMT338b, SMT339a, SMT339b, SMT339c, SMT342a, SMT342b, SMT343a, SMT343b, SMT344a, SMT344b, SMT345a, SMT345b, SMT345c, SMT345d, SMT346a, SMT346b, SMT346c, SMT346d, SMT401a, SMT401b, SMT401c, SMT401d, SMT402a, SMT402b, SMT402c, SMT402d, SMT403a, SMT403b, SMT405a, SMT405b, SMT406a, SMT406b, SMT406c, SMT407a, SMT407b, SMT409a, SMT409b, SMT410a, SMT410b, SMT410c, SMT410d, SMT411a, SMT411b, SMT413a, SMT413b, SMT414a, SMT414b, SMT415a, SMT415b, SMT417a, SMT417b, SMT418a, SMT418b, SMT420a, SMT420b, SMT421a, SMT421b, SMT422a, SMT422b, SMT423a, SMT423b, SMT424a, SMT424b, SMT425a, SMT425b, SMT426a, SMT426b, SMT427a, SMT427b, SMT428a, SMT428b, SMT429a, SMT429b, SMT431a, SMT431b, SMT432a, SMT432b, SMT433a, SMT433b, SMT434a, SMT434b, SMT435a, SMT435b, SMT438a, SMT438b, SMT439a, SMT439b, SMT440a, SMT440b, SMT440c, SMT442a, SMT442b, SMT443a, SMT443b, SMT444a, SMT444b, SMT445a, SMT445b, SMT446a, SMT446b, SMT446c, SMT446d, SMT447a, SMT447b, SMT447c, SMT447d]

Dorm              Beds Left
--------------  -----------
Woodruff North          232
Rooms: [WDN101Bb, WDN101Bb, WDN103Ba, WDN103Bb, WDN106Aa, WDN106Ab, WDN106Ba, WDN106Bb, WDN108Aa, WDN108Ab, WDN108Ab, WDN108Ba, WDN108Bb, WDN201Aa, WDN201Ab, WDN201Ba, WDN201Bb, WDN203Ba, WDN203Ba, WDN203Bb, WDN204Ba, WDN204Bb, WDN205Ba, WDN206Aa, WDN206Ab, WDN206Ba, WDN206Bb, WDN207Aa, WDN207Ab, WDN207Ba, WDN207Bb, WDN208Aa, WDN208Ab, WDN209Aa, WDN209Ab, WDN209Ba, WDN209Bb, WDN210Ba, WDN210Bb, WDN213Aa, WDN213Ab, WDN213Ba, WDN213Bb, WDN214Aa, WDN214Ab, WDN214Ba, WDN214Bb, WDN215Aa, WDN215Ab, WDN215Ba, WDN215Bb, WDN217Aa, WDN217Ab, WDN217Ba, WDN217Bb, WDN219Aa, WDN219Ab, WDN219Ba, WDN219Bb, WDN301Aa, WDN301Ab, WDN301Ba, WDN301Bb, WDN303Ba, WDN303Bb, WDN304Aa, WDN304Ab, WDN304Ba, WDN304Bb, WDN305Ab, WDN305Ba, WDN305Bb, WDN306Aa, WDN306Ba, WDN306Bb, WDN307Aa, WDN307Ab, WDN307Ba, WDN307Bb, WDN308Ab, WDN308Ba, WDN308Bb, WDN309Aa, WDN309Ab, WDN309Ba, WDN309Bb, WDN310Bb, WDN310Bb, WDN313Aa, WDN313Ab, WDN313Ba, WDN313Bb, WDN314Aa, WDN314Ab, WDN314Ba, WDN314Bb, WDN315Aa, WDN315Ab, WDN315Ba, WDN315Bb, WDN316Aa, WDN316Ab, WDN316Ba, WDN316Bb, WDN317Aa, WDN317Ab, WDN317Ba, WDN317Bb, WDN319Aa, WDN319Ab, WDN319Ba, WDN319Bb, WDN401Aa, WDN401Ab, WDN401Ba, WDN401Bb, WDN403Ba, WDN403Bb, WDN404Aa, WDN404Ab, WDN404Ba, WDN404Bb, WDN405Aa, WDN405Ab, WDN405Ba, WDN405Bb, WDN406Aa, WDN406Ab, WDN406Ba, WDN406Bb, WDN407Ba, WDN407Bb, WDN408Aa, WDN408Ab, WDN408Ba, WDN408Bb, WDN409Aa, WDN409Ab, WDN409Ba, WDN409Bb, WDN410Ba, WDN410Bb, WDN413Aa, WDN413Ab, WDN413Ba, WDN413Bb, WDN414Aa, WDN414Ab, WDN414Ba, WDN414Bb, WDN415Aa, WDN415Ab, WDN415Ba, WDN415Bb, WDN416Ba, WDN416Bb, WDN417Aa, WDN417Ab, WDN417Ba, WDN417Bb, WDN418Aa, WDN418Ab, WDN418Ba, WDN418Bb, WDN419Aa, WDN419Ab, WDN419Ba, WDN419Bb, WDN420Aa, WDN420Ab, WDN420Ba, WDN420Bb, WDN501Aa, WDN501Ab, WDN503Ba, WDN503Bb, WDN504Aa, WDN504Ab, WDN504Ba, WDN504Bb, WDN505Ba, WDN505Bb, WDN506Aa, WDN506Ab, WDN506Ba, WDN506Bb, WDN507Aa, WDN507Ab, WDN507Ba, WDN507Bb, WDN508Aa, WDN508Ab, WDN508Ba, WDN508Bb, WDN509Aa, WDN509Ab, WDN509Ba, WDN509Bb, WDN510Ba, WDN510Bb, WDN513Aa, WDN513Ab, WDN513Ba, WDN513Bb, WDN514Aa, WDN514Ab, WDN514Ba, WDN514Bb, WDN515Aa, WDN515Ab, WDN515Ba, WDN515Bb, WDN516Aa, WDN516Ab, WDN516Ba, WDN516Bb, WDN517Aa, WDN517Ab, WDN517Ba, WDN517Bb, WDN518Aa, WDN518Ab, WDN518Ba, WDN518Bb, WDN519Aa, WDN519Ab, WDN519Ba, WDN519Bb, WDN520Aa, WDN520Ab, WDN520Ba, WDN520Bb]

Dorm              Beds Left
--------------  -----------
Woodruff South          219
Rooms: [WDS103Bb, WDS104Aa, WDS104Ab, WDS104Ba, WDS105Ab, WDS106Aa, WDS106Ab, WDS106Ba, WDS106Bb, WDS108Aa, WDS108Ab, WDS108Ba, WDS108Bb, WDS201Aa, WDS201Ab, WDS201Ba, WDS201Bb, WDS203Ba, WDS203Bb, WDS204Ab, WDS204Ab, WDS206Aa, WDS206Ab, WDS206Ba, WDS206Bb, WDS207Aa, WDS207Ab, WDS207Ba, WDS207Bb, WDS208Ab, WDS208Ba, WDS208Bb, WDS209Aa, WDS209Ab, WDS209Ba, WDS209Bb, WDS210Ba, WDS210Bb, WDS213Ba, WDS213Bb, WDS214Aa, WDS214Ab, WDS217Aa, WDS217Ab, WDS217Ba, WDS217Bb, WDS219Aa, WDS219Ab, WDS219Ba, WDS219Bb, WDS301Ba, WDS301Bb, WDS303Ba, WDS303Bb, WDS304Aa, WDS304Ab, WDS304Ba, WDS304Bb, WDS305Aa, WDS305Ab, WDS305Ba, WDS305Bb, WDS306Aa, WDS306Ab, WDS306Ba, WDS306Bb, WDS307Aa, WDS307Ab, WDS307Ba, WDS307Bb, WDS308Aa, WDS308Ab, WDS308Ba, WDS308Bb, WDS309Aa, WDS309Ab, WDS309Ba, WDS309Bb, WDS310Bb, WDS313Aa, WDS313Ab, WDS313Ba, WDS313Bb, WDS314Aa, WDS314Ab, WDS314Ba, WDS314Bb, WDS315Aa, WDS315Ab, WDS315Ba, WDS315Bb, WDS316Aa, WDS316Ab, WDS316Ba, WDS316Bb, WDS317Aa, WDS317Ab, WDS317Ba, WDS317Bb, WDS319Aa, WDS319Ab, WDS319Ba, WDS319Bb, WDS401Aa, WDS401Ab, WDS401Ba, WDS401Bb, WDS403Ba, WDS403Bb, WDS405Aa, WDS405Ab, WDS406Aa, WDS406Ab, WDS406Ba, WDS406Bb, WDS407Aa, WDS407Ab, WDS407Ba, WDS407Bb, WDS408Aa, WDS408Ab, WDS408Ba, WDS408Bb, WDS410Ba, WDS410Bb, WDS413Aa, WDS413Ab, WDS413Ba, WDS413Bb, WDS414Aa, WDS414Ab, WDS414Ba, WDS414Bb, WDS415Aa, WDS415Ab, WDS415Ba, WDS415Bb, WDS416Aa, WDS416Ab, WDS416Ba, WDS416Bb, WDS417Aa, WDS417Ab, WDS417Ba, WDS417Bb, WDS418Aa, WDS418Ab, WDS418Ba, WDS418Bb, WDS418Bb, WDS419Aa, WDS419Ab, WDS419Ba, WDS419Bb, WDS420Aa, WDS420Ab, WDS420Ba, WDS420Bb, WDS501Ba, WDS501Bb, WDS503Ba, WDS503Bb, WDS503Bb, WDS504Aa, WDS504Ab, WDS504Ba, WDS504Bb, WDS505Aa, WDS505Ab, WDS505Ba, WDS505Bb, WDS506Aa, WDS506Ab, WDS506Ba, WDS506Bb, WDS507Aa, WDS507Ab, WDS507Ba, WDS507Bb, WDS508Aa, WDS508Ab, WDS508Ba, WDS508Bb, WDS509Aa, WDS509Ab, WDS509Ba, WDS509Bb, WDS510Ba, WDS510Bb, WDS513Aa, WDS513Ab, WDS513Ba, WDS513Bb, WDS514Aa, WDS514Ab, WDS514Ba, WDS514Bb, WDS515Aa, WDS515Ab, WDS515Ba, WDS515Bb, WDS516Aa, WDS516Ab, WDS516Ba, WDS516Bb, WDS517Aa, WDS517Ab, WDS517Ba, WDS517Bb, WDS518Ba, WDS518Bb, WDS519Aa, WDS519Ab, WDS519Ba, WDS519Bb, WDS520Aa, WDS520Ab, WDS520Ba, WDS520Bb]
```
