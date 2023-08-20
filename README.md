# modded_geth_TxPool_Comparison
last tests of modded geth vs default geth


# Process:

- 4 nodes : 2 modded (1 USA / 1 EUR), 2 default ( EUR only) - same settings for all 4.
- same txpool fetcher running on each nodes.
- chasing USDT tx on PCS router.

```
-------------------------------------------------------------------

Server server1 file: 1.usa.modded.txt
Server server2 file: 2.eur.modded.txt
Server server3 file: 3.eur.default.txt
Server server4 file: 4.eur.default.txt

Server Position Summary:

                | 1st Place  | 2nd Place  | 3rd Place | 4th Place | 5th Place | 6th Place
-----------------------------------------------------------------------------------------
server1         |        102 |         49 |        30 |         0 |         0 |         0
server2         |         74 |         89 |        12 |         0 |         0 |         0
server3         |          0 |          1 |        32 |       125 |         0 |         0
server4         |          5 |         38 |        88 |        23 |         0 |         0
-----------------------------------------------------------------------------------------

Server Positions Summary (percentages in each position):

                |    1st     |    2nd     |    3rd    |    4th    |    5th    |    6th
----------------|------------|------------|-----------|-----------|-----------|----------
server1         |   56.35%   |   27.07%   |   16.57%  |    0.00%  |    0.00%  |    0.00%
server2         |   40.88%   |   49.17%   |    6.63%  |    0.00%  |    0.00%  |    0.00%
server3         |    0.00%   |    0.55%   |   17.68%  |   69.06%  |    0.00%  |    0.00%
server4         |    2.76%   |   20.99%   |   48.62%  |   12.71%  |    0.00%  |    0.00%
-----------------------------------------------------------------------------------------
```





```
Transaction Hash                                                     Server Time Differences
--------------------------------------------------------------------
0x4b76f8a692f8421e55ca8f18bd195720fa78593eff7ccdd3097a14cc486e5a37 |      0 server1  |
0x2a24127257ed5e129e325f484569e6935ef398387ec0df10a3d93d62860bb271 |      0 server1  |
0x41318372b24fe91311ebe5bd5a6561ebae191806638d6043fad5eaf6abdd57e2 |      0 server1  |
0xa670bc53073ac982cccd60d1d96cdeec5753eeb6baf8ef4f67095c73ca989702 |      0 server1  |    +26 server2  |    +28 server4  |    +86 server3  |
0x589cb5603cb3df2955f07610f4e677969402f744d45f431323d5155677a9ad71 |      0 server1  |    +44 server4  |    +48 server2  |   +603 server3  |
0x0db4ef94d3d613e99fe29727ed680dfbb1cdab34ac45ed552535b89de1a2110f |      0 server1  |    +50 server2  |    +55 server4  |   +107 server3  |
0xa027122e33beb1b2f1d2ec737aa79949be4c16bbdba66129db1abcb23472e849 |      0 server1  |    +44 server2  |    +44 server4  |    +96 server3  |
0x733f312de8a1983b8257d69ce7a296f173124d8e2b48d8ff41ab12eccfd2fc67 |      0 server2  |     +1 server4  |    +19 server1  |   +561 server3  |
0xffcf401113fc2141f8b20eed06f3ebc8cc75a6929fe56af38d1892e859253f3c |      0 server2  |    +16 server1  |
0xb0ddf2e5d1d0f44e1e7828598fc090a0399ad7317119ff3a3ee76fb7f6bf8eb9 |      0 server2  |    +13 server1  |    +50 server3  |
0x54c39f64685952831a10f735f4ac38d32b625e203162bb8eeabfb136bb678958 |      0 server1  |    +28 server2  |    +37 server4  |    +65 server3  |
0x8b0ef625672ab50397c3f390373f595c62fb2dba65eee60014475e894195414e |      0 server1  |    +38 server4  |    +39 server2  |   +243 server3  |
0xcfd66a4938ace6a45247d81ce8c5e0b7138b8f74b450ed1c9c71b2bc90444894 |      0 server1  |    +44 server2  |   +168 server3  |   +545 server4  |
0xcc30449dd8a71188336d690a368e2a18c67cf1027f18a3658f11e8bb2f0eb58b |      0 server1  |    +46 server2  |    +51 server4  |    +74 server3  |
0x22ae04366004ff6fdb5e85b9c70184f32b79cfed77b08f102cc372dd227385dc |      0 server1  |    +38 server2  |    +53 server4  |    +81 server3  |
0x437fff087222026be1abe141ab3fa9a0ef5835112ddc1bed279f648ecdeaa8ac |      0 server1  |    +24 server4  |    +26 server2  |    +48 server3  |
0x5420780aa49a871e359e18d518560827b491968df33f5470564faf0ed0ee5b99 |      0 server2  |    +22 server1  |    +59 server3  |   +450 server4  |
0xf5883830ea610946138fdb6d4b3b3acd638de8221821e994671c018dab927309 |      0 server2  |     +5 server4  |    +38 server1  |    +50 server3  |
0x0b8a9b9715752445eeecbe7f48d304a7c6eb175ca879964ef950ed7e853103a9 |      0 server1  |    +48 server2  |    +66 server4  |    +77 server3  |
0x9fe35b0239d5c0dbfc61eabe104cc08739ece9bc2a27fcc2211efbf332b8c5d4 |      0 server2  |    +19 server1  |
0xcf152abdf00617463ecc6a7ed96b429d1642ffff60cedf8a051170f5108415d1 |      0 server1  |    +46 server2  |    +51 server4  |   +114 server3  |
0x3df70765430e6bfd95f23d555f6123b54932ceb9ba6a18661e2603efcee8ed2c |      0 server2  |    +25 server1  |    +34 server3  |    +87 server4  |
0x5601fce56cf4a471ad6f78488f09387af30b1ecbc680cbaef313c8bf6fa907d9 |      0 server1  |    +19 server2  |    +40 server4  |    +84 server3  |
0x8aaa247677876f58374f1219813f25c48be709047122625d161db65b41817f9a |      0 server2  |    +20 server1  |    +71 server3  |    +74 server4  |
0xaf36383f5a874656c00f58c8e71c2a7db6e048f5e3c6f95beadc5a717b87580f |      0 server1  |    +44 server4  |    +46 server2  |    +76 server3  |
0x605de18b039aa8c905f6726c109c592b85111a75794154aa3ae7fe09b001464d |      0 server1  |
0x80f133b6576911f444f4c05c5120e36ddb1d5fea01e0218400cd95e6b8fe0a55 |      0 server2  |    +25 server4  |    +40 server1  |   +766 server3  |
0xfe99860b490ab2564384f523dd20a260dea489b15ce9f0deaca108a350a19ba0 |      0 server1  |    +44 server2  |    +48 server4  |   +389 server3  |
0x6b4ede290db9c8aa31d5091237811b62c42060e9bdb73fb5366ec121519fbc34 |      0 server1  |    +48 server2  |    +53 server4  |   +122 server3  |
0x9f1fd9174e26b252d893a3f1728ae2993379e98dd43a1dd6b64293ee3994fc29 |      0 server1  |    +33 server2  |    +40 server4  |   +103 server3  |
0xc4e43c3cad8ff74098c326aad7c2e2d8df7d6464c070619bbc15c3dbcdb88eb1 |      0 server1  |    +30 server4  |    +32 server2  |    +81 server3  |
0x76d51d4fbff719f7c4fbf423cfe0899e6444a6f76f008ff423be272b38eaf339 |      0 server1  |    +36 server2  |    +42 server4  |    +66 server3  |
0xb37c1f73b350301edbc9c51590265eeeddb7015150bcb79c60f7a1a1074a099f |      0 server1  |    +43 server4  |    +45 server2  |   +109 server3  |
0xdd1e4cf5c103009583ced7fc1ffb9a113a8b36efc46dbe7f81ec10e56173e047 |      0 server1  |    +40 server2  |    +45 server4  |    +70 server3  |
0xa6c8147ac46c886d0f5c756c7e334b8591432f1e9be8fb0802a4c8a9c2c59a72 |      0 server1  |    +47 server4  |    +48 server2  |    +79 server3  |
0xef12ee2daf7071e8c410bfa1b6997e02924295fe9dbe0d9598e7353fed87e753 |      0 server1  |    +48 server2  |    +74 server4  |   +109 server3  |
0xc3fd3d334250cfcf505081aef3cf812686e62c297cf699a444fcd05a2afd9110 |      0 server1  |    +40 server2  |    +55 server4  |    +68 server3  |
0x4a704f448b255e5792c6c7e8ef40b5e2e13e5b3fc1cb23d5b707b1188006c942 |      0 server1  |    +44 server2  |    +47 server4  |    +73 server3  |
0xd361d754b2b08972d67f7445dcde3c357352537fc728718188176453aabdbddc |      0 server1  |    +16 server2  |    +16 server4  |    +97 server3  |
0xffbb258a549f138f8dd85e24b5be1309901d8078d89c776ab0798257d8d67ff5 |      0 server1  |    +44 server2  |   +117 server3  |   +543 server4  |
0xeeb339ba6474423d57b0caa151f8c8f03c05f4af674cf89b62b6f918b13e58ee |      0 server1  |    +41 server2  |    +54 server4  |   +107 server3  |
0xe2e6d6026dea78bcf8ad9f2d7d6398e1a4e84f5e54639576f14a9c73238b08dd |      0 server1  |    +50 server2  |    +51 server4  |   +837 server3  |
0x39ea6c8ca4a1449f1306c7d7e50fc687efc5d7c380424281b00971950ef5cff9 |      0 server2  |     +1 server4  |    +19 server1  |    +40 server3  |
0xa321c04eebdb91d68e46519a7fc014cbda718b878c9ccb5852201b547f5eba28 |      0 server1  |    +48 server2  |    +49 server4  |   +109 server3  |
0x082d0b0a8048eebea1fe6e956f4da1820308d91bc06674286d2f55be1cbedc66 |      0 server2  |    +12 server1  |    +32 server3  |
0xadf2426b7a3f2ee18a1a9fd8385baa55badcf1d468f68c338a61ca82b46bab83 |      0 server4  |     +2 server2  |    +16 server1  |
0xb84783050d6d757f4eebc4d66bda1ee8a2e658730bed77d468f046c15181f68e |      0 server2  |    +17 server1  |
0xa52987668f033b7ff2d0662aa9876de72cde3e935f9061d3bd462e9ca4244faf |      0 server2  |    +26 server1  |    +43 server3  |    +96 server4  |
0xa20b2a0113080d1a06998710a2c9deaf801d12175a12f82c8bdf220699ff3700 |      0 server2  |     +3 server4  |    +19 server1  |    +98 server3  |
0x0441c28783c5af9d343ce73cfd30534faf4314d77e33659f4e2c39a7d5235d92 |      0 server1  |    +11 server2  |    +15 server4  |    +63 server3  |
0x4df9fb2c7ded6850ac162760bcaa975fef1abbd53be0f3dbd23fa0b90f21da8e |      0 server1  |    +47 server2  |    +53 server4  |    +98 server3  |
0x146639b3e6095db17bc50db958f9cdd4e1bd91fc0469c7633c4036462a3db9d7 |      0 server1  |    +45 server2  |
0x70a9e5c094ff3b699836fee025acc5370cfab18dab4384fe51d0ac18b0bb8501 |      0 server1  |    +95 server3  |
0xfcecf7d5b294c9ab045c37c0c13d8cd6981e86cd3dac5d6e84523004e2cc0fb7 |      0 server1  |    +19 server2  |    +56 server4  |    +72 server3  |
0x0f1438eba730ee1e0b8e73b471f6381c97518242549575d91641ed1e15e28223 |      0 server1  |    +46 server2  |    +51 server4  |   +106 server3  |
0x38cd2422043d7d3fe538e61dce8e8ab928c5f2eca8f898ceba98261666d86cc3 |      0 server1  |    +32 server2  |    +36 server4  |   +245 server3  |
0x16202373d604bedfb2b2bc0acd30ae45155f1ce005659ca459d70fc88edadfa6 |      0 server1  |    +49 server2  |    +62 server4  |    +78 server3  |
0x5aa48469a98de57e8b319f6a182475f12c86ddea274c4ff13cd745034949c33a |      0 server2  |    +18 server1  |    +62 server4  |   +482 server3  |
0x153236fcfab8995974b9fb99087ea3761d20b5ae2abccac08ea98cfdd20a179d |      0 server2  |    +23 server1  |    +56 server3  |   +677 server4  |
0xf35f654f8226b6b522baad8faed7a58fd23f49097ca4f8277f719243d6850553 |      0 server1  |    +39 server2  |    +59 server4  |   +100 server3  |
0x4735e951438d4f52cd3fa7753ca6322abd6082ca28678392b66a008c32b8fea5 |      0 server2  |    +20 server1  |    +77 server3  |
0xd1d99081750ddaf57a4ef41707ef16d250c9abed2e0d19373fccf514006b7435 |      0 server2  |    +11 server1  |    +65 server4  |   +125 server3  |
0xaec95df24083220822a2d8f97adf3bff8798bf21cc783b2e6659067f2a533d2f |      0 server1  |    +37 server2  |    +56 server4  |    +70 server3  |
0x34db60b3966eeedc2ffffb9584607a8290425fdc4adf6b4fcf911f41bccba19e |      0 server1  |    +46 server2  |    +60 server4  |   +251 server3  |
0xfaac14c61408ee598ef2e7bcc4a24da5c0f584d220fa49830eeba9148f7c6c42 |      0 server2  |    +17 server1  |    +58 server3  |    +74 server4  |
0x2d946604c3db5b4238312a4cd67ca9cdc930d3654dec9fa013cf02865db426df |      0 server2  |    +12 server1  |
0x1c60dea7c1a82c4f9cbfb3903cf19789de4803dd7a32ba675e86c47ddfbaee91 |      0 server2  |    +43 server1  |    +52 server3  |    +98 server4  |
0x6e9135411fe04869bd256157d4bb98aa3c7a7eac7696f1507a1468366d586596 |      0 server2  |    +45 server1  |   +103 server4  |   +269 server3  |
0x858cd244593dc3fa691cc463b67c61f25229092102f83f451e18eda0d56e4589 |      0 server1  |    +39 server2  |    +51 server4  |   +102 server3  |
0x07f067bf36c664d00f53422a419e52adaccfc76fad0108cf14d78347a0f99b88 |      0 server1  |    +29 server2  |    +42 server4  |    +67 server3  |
0x41aca86f8098cdbcfa6b7ed637a22abc4a1b10a82a6f9afd481ac1f7a9978d0a |      0 server1  |    +54 server2  |    +62 server4  |   +129 server3  |
0x90f16b157bae37589c35d96d6704d1532c6c2845e14a497624a81eb7d1fc152c |      0 server1  |    +45 server2  |    +46 server4  |   +104 server3  |
0x09bd83c9cdb6bb4e9293cdef90926a3ff22b77b1e667a89cd2d5969867b565d2 |      0 server1  |    +42 server2  |    +74 server4  |   +128 server3  |
0xed90caf1982266fa8c168390e536fac80dc4beaa4714cfa1590830efa61a8ad5 |      0 server1  |    +43 server2  |    +45 server4  |    +72 server3  |
0x666e15981139e60b15eecca808e071f3d54e9a6fb3747287f01ae39e0c37da8a |      0 server1  |    +32 server2  |    +61 server4  |    +82 server3  |
0x03778a9faebd0aa029da112b8c18c9902c235706972a70f4785f4c0c9effbed4 |      0 server1  |    +40 server2  |    +67 server4  |    +75 server3  |
0x9c8832cfff8e5dffab38a30b5ca48819365d29ceb1232028d6cd81aa1dac5cc2 |      0 server2  |    +16 server1  |
0x72a2ee64167c13acc9da5b45f1607ee03973c36de7ce2acd99d0f04630fefa95 |      0 server2  |    +23 server1  |
0xcdd773a570448c96836b7aca6f5a21e3f76850e26fa9030afc74032516f39d4b |      0 server2  |    +39 server1  |    +67 server3  |   +100 server4  |
0xbe8ab7d48aacfb365452ad4ec6d0527f5a1784756cf40cd314ecc38444cb4330 |      0 server1  |    +38 server2  |   +107 server3  |   +431 server4  |
0xfaa822faedf5fcbe8b2c418785cba63afef29f304ef8a72893e63b3b64967256 |      0 server1  |    +39 server2  |    +40 server4  |   +116 server3  |
0x4e8b98a3ad17872a72201f1b23ba86415985ab063e4149f1250a8dcbb26d61ad |      0 server1  |    +48 server2  |   +106 server3  |   +548 server4  |
0xf9bca164632fe1483243f4e132d112f5e1f8cedaadf2b77b504426642e5d4647 |      0 server2  |    +33 server1  |    +56 server3  |    +84 server4  |
0x2205d62af39fa136b59f330054e8faccb2138f5699b29c4dd650b2b064107273 |      0 server2  |    +39 server1  |    +98 server4  |   +261 server3  |
0x8a971ce2c068878d41a828b13ccef58ecb6ba089c77abb18bbe24d03a3091c74 |      0 server2  |     +2 server4  |    +19 server1  |    +35 server3  |
0xa001fe0c276bf69695f7a2a8e592f1cc2ae4b710d395c0def66c273c3f615449 |      0 server2  |     +7 server4  |    +39 server1  |    +77 server3  |
0x3517d6342a5f3ffbbe3bf10e920a700616c58fef8f9f2de7e7ba0625d33e39b0 |      0 server2  |    +18 server1  |    +64 server4  |   +495 server3  |
0xc5b2064e8e9ca963ce68c7e61843c9e584fc0e9fd16ecf0f490487d3f1efae8d |      0 server1  |    +41 server2  |    +42 server4  |   +772 server3  |
0xa9c5771fb7716f7527735959ae6f3d4f603751a0f6298527527ab0d0306d43b6 |      0 server1  |    +44 server2  |    +46 server4  |   +108 server3  |
0x4c24a71aebaddaa980d65bc3e1a38646482bf3e168407492125649fac3e7ea12 |      0 server1  |    +46 server2  |    +53 server4  |   +830 server3  |
0x7871c4c72a35cd0f4a896e67b26282bc7f5b86bbdb255629bffec33a138ecdb7 |      0 server2  |     +3 server4  |    +18 server1  |
0x7457c9c2be108477f1d1fa2276a6e9e6003edea8c194d5447b51dc2ada5163bf |      0 server2  |    +19 server1  |    +32 server3  |    +69 server4  |
0xac9de197380338ffad175856ef9722c6cd92de242a8c807ee22eb06975500e5e |      0 server1  |    +48 server2  |    +53 server4  |   +202 server3  |
0xc015377c59dd799f59d7f9affe2303100604bcc7b8987e09f1fc5537a2183b6f |      0 server1  |    +38 server4  |    +40 server2  |
0x54de2c2d2dbe8fb4db4e3eaf956c18520b3a0bcc3df2746ed82c6d4b43971b9f |      0 server1  |    +30 server2  |    +57 server4  |    +89 server3  |
0xb2cab9d9a35e45b6ed8c96d92a3ee2e75cc45da562524a01f2463b5790aeb863 |      0 server2  |    +18 server1  |   +508 server4  |
0x1afbbf444e8b61a1ab0c1f6cfa8fdb6c45f227da1a558c4efa082d53b2583d42 |      0 server2  |    +20 server1  |   +555 server4  |
0xbc05227a260c6a1d785ca7c6967e2589880ecd8744d7d831d417b44c8caaee31 |      0 server1  |    +47 server2  |    +50 server4  |    +79 server3  |
0x40403d3df4b8b86ae854b0a9fe834e20ee6d6c2bf73e5b2dde5a231807d08945 |      0 server4  |     +2 server2  |    +22 server1  |    +78 server3  |
0x576699ae0eb46dbe0134406ab107991cf34485a9da97ea813dc80cf84fbb7e8f |      0 server2  |     +3 server4  |    +19 server1  |   +113 server3  |
0x2a56a54d268a4f631253e21f3b8075692756e98b1a5aab72acfdfa7f2a8d4deb |      0 server1  |    +49 server2  |   +126 server4  |   +207 server3  |
0x7a8313145be77170d97897165d0c82563bd4cb08d7b596c8ff40206d4f261b13 |      0 server2  |      0 server4  |    +17 server1  |    +34 server3  |
0xb0c894bec3f9858e8537d692640f6a123cd0c50f7a79ecbb7270882e3939281e |      0 server1  |    +44 server2  |    +54 server4  |   +187 server3  |
0xbf65ce8d94a6a640e63c246e0b1b68f150d671b001cb5fee299e50a1a898d448 |      0 server1  |    +49 server2  |    +52 server4  |   +114 server3  |
0xd95a4873097c0321f194da5fc20cec3fa86dc25c8c35a4c3d8db443d89f8a0a6 |      0 server2  |    +27 server4  |    +40 server1  |   +249 server3  |
0xf267c161575d74f2e1d49c2bec3730ca1f852d8c11c0924ad3e9aabf1e6587f4 |      0 server1  |    +46 server2  |    +71 server4  |    +79 server3  |
0xee33f85ce4c211e904eab628b2bcb6599899f54cffba50f24a29a87609419f37 |      0 server2  |    +15 server1  |    +69 server4  |   +529 server3  |
0x07e66a43b9d38f142d65fa20206e690fd6aeafe5ed3cde2b4130bee05f5d0fe2 |      0 server1  |    +49 server2  |    +55 server4  |   +119 server3  |
0x620049bf16fa15cc4e0ec52442ffa9bdd46e78353e144275e0d6623450aebf15 |      0 server2  |    +12 server1  |    +49 server3  |
0x3ca861fbfaf58d29a4af09c961b2768ce3a6166f6b46195389b63033c67a1f12 |      0 server1  |    +48 server2  |   +123 server3  |   +561 server4  |
0x6d353966ab75b78eab09acff577d61e46ef1cce4bdbd4fde6fa6582bfc68ed09 |      0 server2  |    +21 server1  |    +75 server4  |   +139 server3  |
0x05d7442f0f83fb9219b23d34742fd02453157fa208e7e1f5bdf1fa1126906bfc |      0 server2  |    +19 server1  |    +80 server4  |   +534 server3  |
0xf5a164dee9a41c8ee320b414df053e02c5c7a4ed6096ab167acd58db07f4129f |      0 server1  |    +48 server2  |    +52 server4  |   +125 server3  |
0x30a3832363125934f21c51f685d9545427bc0fc2cb66d0fb9fc1460193af9dec |      0 server1  |    +47 server2  |    +47 server4  |    +79 server3  |
0x0791c6ce3360a7dc3f1bf8b9d3d17b2254d9f13e4ecec3c37f75304b842b95fd |      0 server1  |    +32 server2  |    +37 server4  |   +801 server3  |
0xc9660fe31fc780449c5df4c29c294e52fc06b0278c56ba3d433912d009a16d3d |      0 server2  |     +3 server4  |    +20 server1  |   +245 server3  |
0x4d9fab806331c30a489629a55073f672cc7266ed0f1e9fd43560615d87db0203 |      0 server2  |    +28 server1  |    +56 server3  |    +88 server4  |
0xcaca9464a67a41479986ff34e4b6e294e4147f60e8ce69f45aae55a7add20fff |      0 server1  |    +49 server2  |    +53 server4  |    +81 server3  |
0x705dda3b1d4542d8866fa75a8cd11d82c7f9a06ce36b8ddbb619c5561580addf |      0 server2  |     +3 server4  |    +20 server1  |    +72 server3  |
0x0870af93e4ba3c85432854b3c4ae8eb6a8cb74c04b8ed5c7a7bf41f0c777e6f4 |      0 server1  |    +46 server2  |    +56 server4  |   +610 server3  |
0x1da01c4d9796989e9cc02ba39eaff5b6ee10c48b0835afadbb75d3804778fc60 |      0 server1  |    +37 server2  |   +127 server3  |   +542 server4  |
0x60e141000257526bbd8d0cba7fc132dba13dd68584a07c555d128c042811d77c |      0 server1  |    +49 server2  |    +57 server4  |   +234 server3  |
0xda2a67373a2ad283caafc28c641d358bdade1daf3ce2b897ccfb31686685f6c3 |      0 server2  |    +19 server1  |    +77 server4  |   +110 server3  |
0x259859c4a0dbf807e623ec56517143381533663515b9b4eda876347a950dd331 |      0 server1  |    +48 server4  |    +49 server2  |    +81 server3  |
0xb921dbffcba65ef2bc5273e789c8d49173c14bb510fc9c4094fbb20e8f17d5c2 |      0 server2  |    +26 server1  |
0xafceb9cad320c9ff630f875910d8ea48da7d6d9518acbfebb64760940a471527 |      0 server2  |    +26 server1  |
0x4f5b3289779cde33bd7e77b4f8eac8b3dfba6863fd8c7946d9cf84d8f70bb024 |      0 server2  |     +7 server4  |    +42 server1  |    +57 server3  |
0x14c2bc6761b452f31d309fb3169440f869beb390e9ed68ec890cee132b1ea645 |      0 server1  |     +3 server2  |
0x9ab0322a29383afecafb4f9383ed844c75b3701d6a94a4dca334a2928747fc82 |      0 server1  |    +43 server2  |    +81 server3  |   +519 server4  |
0xc3a11b453b24a1dc6136d0167fff904f322f7e9b99f331dd2a86f168e6c84f82 |      0 server1  |    +44 server4  |    +46 server2  |   +116 server3  |
0x216c67ad9300d319aae7ef7f346fca21824be921c9856343cac4a10bbd224ca5 |      0 server2  |     +1 server4  |    +37 server1  |    +57 server3  |
0xac7b2068024715891317b327eec23b98fd8d6392153b063fe359a56c9ebd4e04 |      0 server2  |    +37 server1  |   +104 server4  |   +670 server3  |
0xb0a69fed3bb5ed5339db54c8e0a7e1c4df6a77701b83d03f0b991a9957e741be |      0 server1  |    +13 server2  |    +14 server4  |   +637 server3  |
0xe310fef60344190c4d7ff6af4fa3fcee8fc79d428b0c4fabf016639eacac7b37 |      0 server1  |    +47 server2  |    +55 server4  |   +832 server3  |
0x06593a329f0db1c72e8f685ea36004d967217e7d9131203c141db2a731c5c13b |      0 server2  |     +3 server4  |    +19 server1  |    +35 server3  |
0x45e11ce2c2e01e2ad4f71a61eecae0736633ff1b64f2c4f0da3633869073d4de |      0 server2  |     +5 server4  |    +19 server1  |    +84 server3  |
0x146e2c131d82f9c1c543b9bf83902264ce608f86489207589384953bf71ef13f |      0 server1  |    +48 server2  |    +48 server4  |   +838 server3  |
0x0b221bb33897f3f71789c8b1db069d2c6ccd423ddcd214053d53dcf46d21ba32 |      0 server2  |    +30 server1  |    +61 server3  |
0x7b0efe4ebe59d7551a5095dbdee58686de16a20313f58fd009ee073125dc0b11 |      0 server2  |    +45 server1  |   +302 server4  |   +561 server3  |
0x9ae32295140f9c86ec9122dbc6ff6cbcc49adc32c0fc9affcd1b3bcf1199dcdf |      0 server2  |    +45 server1  |   +302 server4  |   +563 server3  |
0x14d7fc4f0c4363161c444066bb42f4b414d602bf58e4e3a108a48a1438dc4b79 |      0 server1  |    +37 server2  |    +44 server4  |    +70 server3  |
0x90272d864abe70637111e745a029ee7bf82d9c4041d89bd99154ba19a816c7b9 |      0 server2  |     +1 server4  |    +19 server1  |    +36 server3  |
0x4f365428f71b4ab6f397b3543fe7166fc1f46d40c618713987b2b7b58e9625ca |      0 server2  |    +20 server1  |    +40 server3  |    +79 server4  |
0x0d0af8b8cb6ce784d0bb7e2b3b019750ec250cb75561518a3d11c01ad5d96561 |      0 server2  |    +20 server1  |    +34 server3  |    +76 server4  |
0xc9a830b28cb5a794fd1bec769df0c04054c6fa0f261f08136c2f4bf2f88fca5d |      0 server2  |     +5 server4  |    +18 server1  |    +32 server3  |
0x2d85fb6a0adb79534a79b2dcfcbf5cd10b29252264372211a66a3c81204df3ff |      0 server2  |     +1 server4  |    +26 server1  |   +727 server3  |
0x56c3367d6e5a36348563cf1c47fcd25892c009c0b5c6561fdd12ea25389261bc |      0 server1  |    +44 server2  |    +58 server4  |   +969 server3  |
0x70d161eb1512febcc5ec23444979a0f5b31acd77c8f483ee93388248dbb21284 |      0 server2  |     +9 server4  |    +10 server1  |    +37 server3  |
0xbe068b79b817137f8a4d1d76aaeb4068e7f2a3ef69e3e1a23d78e920ebeccba5 |      0 server2  |     +6 server4  |    +13 server1  |   +111 server3  |
0xa1be9b3c80386b65430b54032c0f52ea632b9ca6b9bcacb8e3d1505fc09896d7 |      0 server4  |     +1 server2  |    +19 server1  |   +756 server3  |
0x74cff2f9da8392b14a2b5bee9ce54f09279ce8688bc96d7b8f06ecc8a26d049a |      0 server2  |    +13 server1  |
0x5c5ff0b80a4fe7d89508c32622abd536dfafebf70515346a125156c00505ce30 |      0 server1  |    +46 server2  |   +125 server3  |   +544 server4  |
0x60777c0319ae3d2813a5c9017978bd12d2f1e3b5d7eb6d13c33c8f9b43a88ae0 |      0 server1  |    +42 server2  |   +583 server3  |
0x04e0e9496731eef21b93ab0510efa3a1f63f89a2ed643f2210f9c8849d22cd8f |      0 server2  |    +31 server4  |    +41 server1  |   +256 server3  |
0x75ff428d17734a74bf87cf830eb329525c4c3152d6d45b0979ada8be78b626f2 |      0 server1  |    +22 server2  |    +65 server4  |    +83 server3  |
0x71c352e8c0c33517c8f9ffcec83be46f75d8996442e74f35c84cf701334087b0 |      0 server1  |    +35 server4  |    +37 server2  |   +166 server3  |
0x406baad8eb6ba583580395b39b20e3af0ca8979e11a7162df4b1b75cfea3db8d |      0 server2  |     +5 server4  |    +19 server1  |    +38 server3  |
0x68455819c5f09df9ade9543878d5904d7daec73e349594fa74c7d6baa95e5786 |      0 server1  |    +38 server2  |    +39 server4  |    +72 server3  |
0x34f241d94af91b3721156cedec19a2cbbe70be731de5cc522135be9626c99b94 |      0 server4  |     +7 server1  |   +456 server3  |
0x674a06d34bc0ef8424906e57cc918a6c5b015bc1c8bb7c5ecd8db4b5634eeab6 |      0 server1  |    +35 server2  |    +60 server4  |    +93 server3  |
0xcf89235231313af24749f460976e8145a76b6f7f2147f1581b7b9097cee42935 |      0 server1  |    +46 server2  |    +49 server4  |   +103 server3  |
0x913ef33f5462c13c52fcf6c053b851949ceb5e89920dfb9b8bf80b1d86bb547e |      0 server2  |    +18 server1  |    +35 server3  |    +74 server4  |
0xf6cf96c6e0d3384d63b87d9fdb740611d7804c388b155eee620a26d61dbbb1ce |      0 server1  |    +48 server2  |    +85 server3  |   +502 server4  |
0x6446881dd314fdfb6b8eeffa45114c4ec1a7a1bc48c8fd16e6a9673d7841b596 |      0 server2  |     +9 server1  |
0xe79cfa0b0800d9be6ef013c8bd82e7022ec410eccddb17a08e587d9964802d7a |      0 server2  |    +15 server1  |
0x98ec67bc96dfd98be0f213f242d2f205aabe4f1dc497873b4cbb8546795e2e41 |      0 server1  |    +42 server2  |    +56 server4  |   +242 server3  |
0x598814001bbeed299c855aac9ee5986e8575c773285ccba377559368dc6f266a |      0 server2  |     +7 server1  |
0x3e14d1c572df7a247d572c630b9f139a68cbfbd869026bbb21d6c8fdddf34817 |      0 server1  |    +44 server2  |    +44 server4  |   +579 server3  |
0xcf440823141c7eeac45ba57a728c53438bbb97f08277d026efd04e30a3a479d5 |      0 server1  |    +40 server2  |    +84 server4  |   +614 server3  |
0xf5c955eb465d2a9ebd6a70f2bd4fd8055a5c4034cabbb046320c5d8788bfdae6 |      0 server2  |     +5 server4  |    +17 server1  |    +61 server3  |
0x902c25d8c479f34853977fab72c57c111bb4e52d1a5eadc2278d5d7259bd2a0d |      0 server1  |    +47 server4  |    +48 server2  |   +101 server3  |
0x9e9d552bf0ab8e5af63706e044dbddfddc92e2d92b995a6af5c79feed1fed6ec |      0 server4  |     +2 server2  |    +22 server1  |    +38 server3  |
0x57cee42813f2bc4c1de3994397bb42708ee9b2cc84008c31cefb69dcef05a2db |      0 server2  |    +21 server1  |    +37 server3  |
0x3d81c60694ad3993db3783190c87947e86fdc20f8d1c70526a697cc6b64dfacf |      0 server1  |    +41 server2  |    +52 server4  |   +123 server3  |
0x8c351842e7de5a7506c738ee6b5f8b7c8ff4edaf97e04f2ff5961e591496f6ff |      0 server1  |    +40 server2  |    +40 server4  |    +76 server3  |
0x5a238354ff5a2f52e4d787d2c8e264721d279491943fbaf99beef8688cb2e0d9 |      0 server1  |    +45 server2  |    +45 server4  |    +83 server3  |
0x8d57b9a7393bbd689efd41357dc0174211c8b1dc18c15a51685fd5dc1cd94db5 |      0 server2  |    +20 server1  |    +64 server4  |   +518 server3  |
0x417bbc36a62e22d35b63fdec5e6dd368bb54b0daa012b4fe120ab6c812e21835 |      0 server2  |     +2 server4  |    +40 server1  |   +544 server3  |
0xbfbd2bdb601c3ff60e827efb8db42b588d5b193935593f56cb839dd83a29edc2 |      0 server1  |    +32 server2  |    +34 server4  |    +79 server3  |
0xd88b401f0e438736fca3dccfd6228eb61db3ea0000b22b552388175c870d6faf |      0 server2  |    +24 server1  |    +82 server3  |
0x64c1223442cf4fbee250b375c8b8c51cbe610cc0a229fca91bd7cf4f895a4d7e |      0 server1  |    +46 server2  |    +64 server4  |    +82 server3  |

```


Log file created: /home/script/nodecompare-main/log/2023-08-20T22-44-18.862Z.log


