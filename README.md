ARC-Seal: i=1; a=rsa-sha256; s=arcselector10001; d=microsoft.com; cv=none;
 b=xkvByS0G0R9y+FLJmXtHVhLPfU0boa8lWtyLtPFnWhhpdZK2vv1yxSgP8XketmOaUm+Ck6LY6CRQvNGPnxmaXVAnOU97zxRhBWli37XxFHDtndwgc88ojS//n7cD9bU66UPLR6FfN9r3YlBeGU8AcgnZeN+48PuNlBzvQhhz8s1RGEJCYqtjVXNt9F80fWvDRo2okH6vtfy6mbVe57IvN698uvI8BWOlWYsjq1SPbP4QwLHXcIViMr5yn+LfLXCVshj7n2VUz+TqLLRLOoCAC1FcW11DiWjANKcBbGQqmGXKfiuV5X6YE1u+JdRNNDZ1GKa3/4SU2g2nkMfz/DEHSQ==
ARC-Message-Signature: i=1; a=rsa-sha256; c=relaxed/relaxed; d=microsoft.com;
 s=arcselector10001;
 h=From:Date:Subject:Message-ID:Content-Type:MIME-Version:X-MS-Exchange-AntiSpam-MessageData-ChunkCount:X-MS-Exchange-AntiSpam-MessageData-0:X-MS-Exchange-AntiSpam-MessageData-1;
 bh=oiwiTKanRjdFkOuJleCovTAD3KUm7GwHOzJG7VXQCCY=;
 b=FMd7jDwwlDr+jbhdhMbzLYa1+kYPUWVeVrjFejjOuKkVUZML0Ntsul1Wxv74mKjVSL2sZK8iqXANe4UiP/+Oo2j/o812RD9vKW4Ymkx3LmGmf6Vf0g8KyT+ynHlB+eAQAScwRVaEy3ENvvoJydhQwjQQM1+Xx3xiuO+1ENVpU57SIUc1FmbYUCCfjyt/WwCgxizotm0AV4h5UJ7m9FLt8zqhuQ9EaFKGji3dXzinHStFzue8+tjaPcECs9IE52oP7p5PA+4J8kvI5taJO2G8MsnYjfdU1kM9AI1DeumBnICrzFg0WDv8DFE9FVajAELneiGWYVHhpdUTsTRGLTKpGA==
ARC-Authentication-Results: i=1; mx.microsoft.com 1; spf=none; dmarc=none;
 dkim=none; arc=none
DKIM-Signature: v=1; a=rsa-sha256; c=relaxed/relaxed; d=outlook.com;
 s=selector1;
 h=From:Date:Subject:Message-ID:Content-Type:MIME-Version:X-MS-Exchange-SenderADCheck;
 bh=oiwiTKanRjdFkOuJleCovTAD3KUm7GwHOzJG7VXQCCY=;
 b=hn8HW+Ku+ztbomudHt5rWt05PLIjYUfbjhSH+kKpVZ5rwU094cLp/nP1D6AuOOtVd9c3RwfQLh3VgUgAH9f/mtruMM7WXsGQoGd84ifu+BtwIJiu+uh+94MS+iAJdYHJMkieo9r82OeA8XNsOxGeW9o3eVkrJMbHWOjnlCBFeguuAK2FXOWxjdFHuZYjZZC0pNjtvmQKgEpRWD/+Bcg977lwMwrmhfaQdhOK3tmu4uhC8zFkaDOp9kKLyoAQU+FOAJ31w75mGfvSwBOvZCSVx912upsB2oepVZOrAASqK4KahCqw76zvVrPK3BCPIOY/jhUIMFna1Cib0RuIzqVHXQ==
Received: from BY1PR84MB3910.NAMPRD84.PROD.OUTLOOK.COM (2603:10b6:a03:4b2::8)
 by PH0PR84MB2220.NAMPRD84.PROD.OUTLOOK.COM (2603:10b6:510:166::18) with
 Microsoft SMTP Server (version=TLS1_2,
 cipher=TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384) id 15.20.8069.18; Thu, 17 Oct
 2024 10:35:02 +0000
Received: from BY1PR84MB3910.NAMPRD84.PROD.OUTLOOK.COM
 ([fe80::aa78:f035:3b7e:7485]) by BY1PR84MB3910.NAMPRD84.PROD.OUTLOOK.COM
 ([fe80::aa78:f035:3b7e:7485%4]) with mapi id 15.20.8048.020; Thu, 17 Oct 2024
 10:35:02 +0000
From: Nathan LaMoreaux <nathandlamoreaux@outlook.com>
To: "05shifter_stakes@icloud.com" <05shifter_stakes@icloud.com>
Subject:
Thread-Index: AQHbIIAmY8Xi3sz9iUaXnZ6j3iUZxg==
Date: Thu, 17 Oct 2024 10:35:01 +0000
Message-ID: <BY1PR84MB39104BDF18D6A5C05D23958BD0472@BY1PR84MB3910.NAMPRD84.PROD.OUTLOOK.COM>
Accept-Language: en-US
Content-Language: en-US
X-MS-Has-Attach:
X-MS-TNEF-Correlator:
x-ms-reactions: allow
x-ms-publictraffictype: Email
x-ms-traffictypediagnostic: BY1PR84MB3910:EE_|PH0PR84MB2220:EE_
x-ms-office365-filtering-correlation-id: 91818d74-b755-4158-17a9-08dcee975b57
x-microsoft-antispam: BCL:0;ARA:14566002|8062599003|8060799006|14030799003|37102599003|15080799006|461199028|12050799009|19110799003|9400799024|4302099013|440099028|3412199025|1602099012|102099032|10035399004;
x-microsoft-antispam-message-info: =?us-ascii?Q?obwB1BIQ7aE93kM+sbKYFGaGN1MQSS/hyf4BmKpQeD6+hZwkqdLIJ8PBPoXo?=
 =?us-ascii?Q?o2z3MqWho7wGwyvu1p/tf8I80s4HLvGns3FdNpVeiY4VkwAA0XyLLSpBEx8R?=
 =?us-ascii?Q?obdlsuQCB17lxmIQjvqT6DliuY/uHt4Y/+sFpxPWfEE+iRw729D5dTxvSnr3?=
 =?us-ascii?Q?yn40zJBWhwd0yYNsGEK413zVXE55SVPtq2L4e0SBYvr9IgA4Ohs1eXpHd9zG?=
 =?us-ascii?Q?Y8l44eX3yl67YrhihY1if9TNQb0ouRi18ugyluLbkiaoty6rDXHpTodl8A9P?=
 =?us-ascii?Q?C2b5RA4g6WRzwyVCUDs27yRJTtPKG1dhtnxQN2v0L7+4plo7ycssIteNf7RA?=
 =?us-ascii?Q?H79oFJno7WfIOOc4iRC/zrtS+PKHULSM/rTzvKkPfBHJM8tooriOyOgxFuul?=
 =?us-ascii?Q?P3oi77AnHsbkBKRXy/Gn230npHzfJWrPOxCNkmorFNWHaG4RlxABpeDywhJb?=
 =?us-ascii?Q?Xjfjvk1BHZKLjS+8/tcmdO8TrhpjxSan4cSefNbk0JnZfa+Oj9ADMScfAH4V?=
 =?us-ascii?Q?7xZGJvPEroGW6MqXUUzjuaoNZ7TqiMCFYG/4MqWmTigk+KbLQC6u9N/ZQOr4?=
 =?us-ascii?Q?cVavqinHMXuoeozGo0YWkAaYAgEtnmgNOfdN/+fuH+8pboXlC73MMniHosdr?=
 =?us-ascii?Q?U4/3DI1+vDmA8T0ofyliIQDW0ZxtiCY4CsAnGHyOg0Hv8eRR3QfZQBub++Xa?=
 =?us-ascii?Q?WxbZzN0HdWSixukTbJNJePFE3CuvyZP2B3jx2eEqPOAok77knHWuQrCXcaBf?=
 =?us-ascii?Q?23gDX7JgDr63pTPvG3lmuT7+wLkkbV5zgtTnzU56rnADmphI/KE+RcweoSiy?=
 =?us-ascii?Q?5a/H2TE03zRNNWC4KXj4czFUvtxDSTqWGl7lNHFF7amjk+cQkI+yCE8CXEhU?=
 =?us-ascii?Q?L6Hx860KpxBK4WjAEyAgPajB2CBfcZgMnDRfXhrCuGnojht5Pq+TX3rRKk9m?=
 =?us-ascii?Q?XwpjBmYypug7AYEO5z0sW78a5CN1GZlAEOXacY8GoiKlo0Dmvdr9TMawaJm1?=
 =?us-ascii?Q?hxIjS406mPO5IfEErtLgmgMPDA=3D=3D?=
x-ms-exchange-antispam-messagedata-chunkcount: 1
x-ms-exchange-antispam-messagedata-0: =?us-ascii?Q?UUYItFeCUcSarIGVauLy7Nhlz4CSxHy5qESYCCsZRaZVXLUAClgEv7yhDGwf?=
 =?us-ascii?Q?M32iNy2loRNLrbxaotQ7CxN7gF0DABSO5wshjQFi+HAJd/D5QmHtwHHAe/ve?=
 =?us-ascii?Q?sIZYqS/5fHrzzvULm0q7myywaxYo8TwNBziPeH6bDV9RHdhhdXfgRINn2ILe?=
 =?us-ascii?Q?GAmQjGavICtkeu6bzZHlbswsAHP0QsN1i5KB0WcEbe+XqB/LHv8Mlwf3Cz8h?=
 =?us-ascii?Q?EzRrmtT3hqHM1/7XH0+7sVi+sMAKcPUAJ2ef+QLLiF5XWGlVPO9kTWntT1ua?=
 =?us-ascii?Q?s2eBFtJjU1K7lO9S7BBNUvOCPJOTI6z6zGBi+sHT4NHL3Fjh9za58r6VSL5/?=
 =?us-ascii?Q?9QACT5A77CtQ1AE4YbuFjS7GUzz9qOeJewNkalzvyTEQ9OwjwQUZsRAL+uNM?=
 =?us-ascii?Q?74pmgZoa6Wx5azX+ZLR75XMNrfNmbX5ZLB4ngEbR4L2LNo+KkLMVzeHh5R3F?=
 =?us-ascii?Q?PRvim/uWysd/4jSRBWCMF3axCALqpWwS/14vh9G2YRDtoP/aLTbMcWcTzSmq?=
 =?us-ascii?Q?kGuMY6WzZKUpwUJSDlB44Ut0my9YtqCsqlvubXr3M09jGcA6kd4FRpdWoCC0?=
 =?us-ascii?Q?vfUUVzaBRKSvnbU7uNGnIrr4dv/juT2hEI2Y2emigcIZVYNZq11SSp+Xk9p8?=
 =?us-ascii?Q?ayqRpppwsTD3EBaomMf9b7U09dhIGWcDFS+NLyasxToYmngHX5sKVC9ystW3?=
 =?us-ascii?Q?pCfjXC+PKfUSdJUjWLwR6OHLbUavLaWCfxRbGOkiYuC7M45gdestoA6FHCzX?=
 =?us-ascii?Q?l27H5PdBR9kdTOFdrCki1/QR4TRFAvwyI5qCRaRpGkbZMNhpt7NJqm6GiFSu?=
 =?us-ascii?Q?aR3rr4QPVJM39r1rxVU13gX8gPxomHtXauiAaBoF57G+mA+IjnLbST2WEnyd?=
 =?us-ascii?Q?LczcQsiTl3CfQUbBarc8BtmS67jyljUxmOZsn66Iyh9GSUOVyqJUMWQahK5Q?=
 =?us-ascii?Q?5NQKKAlCTzSOYoixEsNR0eE+xF5mwX7ZKGqrsf5GGUIcaMzHQyRgdkrW+/Xq?=
 =?us-ascii?Q?rI912FwnN7XjtPpFk9L1OKZJ3Vv3sY7FYxVbRS/N/s71RWdICuMNz205OLVx?=
 =?us-ascii?Q?dWTWfiCr16N/Nrp6ODEvYtuLAOq6K30ZPMhodGTEg/qs2lInB15JZjpYC4rJ?=
 =?us-ascii?Q?QNDCrk8JtMntLsp9CWdxOY+nn7Qy0h1AMj+5eFyYOq9QiLOXQfMBzAh38lxp?=
 =?us-ascii?Q?6oQ/CHNCvIpI5WMsl0qHs0MOrMgx9f/mlbgaXfJT1+IC1VhPbFEG9Xbs412G?=
 =?us-ascii?Q?+W2FzVplfwsgjpaymP4mYuDGuOPmZVK6EahMlKDK4w=3D=3D?=
Content-Type: multipart/alternative;
	boundary="_000_BY1PR84MB39104BDF18D6A5C05D23958BD0472BY1PR84MB3910NAMP_"
X-OriginatorOrg: outlook.com
X-MS-Exchange-CrossTenant-AuthAs: Internal
X-MS-Exchange-CrossTenant-AuthSource: BY1PR84MB3910.NAMPRD84.PROD.OUTLOOK.COM
X-MS-Exchange-CrossTenant-RMS-PersistedConsumerOrg: 00000000-0000-0000-0000-000000000000
X-MS-Exchange-CrossTenant-Network-Message-Id: 91818d74-b755-4158-17a9-08dcee975b57
X-MS-Exchange-CrossTenant-originalarrivaltime: 17 Oct 2024 10:35:01.9219
 (UTC)
X-MS-Exchange-CrossTenant-fromentityheader: Hosted
X-MS-Exchange-CrossTenant-id: 84df9e7f-e9f6-40af-b435-aaaaaaaaaaaa
X-MS-Exchange-CrossTenant-rms-persistedconsumerorg: 00000000-0000-0000-0000-000000000000
X-MS-Exchange-Transport-CrossTenantHeadersStamped: PH0PR84MB2220
MIME-Version: 1.0

--_000_BY1PR84MB39104BDF18D6A5C05D23958BD0472BY1PR84MB3910NAMP_
Content-Type: text/plain; charset="us-ascii"
Content-Transfer-Encoding: quoted-printable



Get Outlook for iOS<https://aka.ms/o0ukef>

--_000_BY1PR84MB39104BDF18D6A5C05D23958BD0472BY1PR84MB3910NAMP_
Content-Type: text/html; charset="us-ascii"
Content-Transfer-Encoding: quoted-printable

<html><head>
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Dus-ascii"=
>
</head>
<body>
<div dir=3D"ltr">
<div dir=3D"ltr"><br>
</div>
<div id=3D"ms-outlook-mobile-signature">
<div><br>
</div>
Get <a href=3D"https://aka.ms/o0ukef">Outlook for iOS</a></div>
</div>
</body>
</html>

--_000_BY1PR84MB39104BDF18D6A5C05D23958BD0472BY1PR84MB3910NAMP_--
