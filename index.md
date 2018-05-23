---
layout: entry
title: UD Examples
---
This repository is for producing example visualizations for UD graphs

### <i>"Il governo sono io, non Walesa e presto vedrò il leader sovietico"</i>

<div class="conllu-parse" tabs="yes" id="tut-2947">
# visual-style 11 5 nsubj color:blue
# visual-style 3 8 nsubj color:blue
1	"	"	PUNCT	FB	_	3	punct	_	SpaceAfter=No
2	Il	il	DET	RD	Definite=Def|Gender=Masc|Number=Sing|PronType=Art	3	det	_	_
3	governo	governo	NOUN	S	Gender=Masc|Number=Sing	0	root	_	_
4	sono	essere	AUX	V	Mood=Ind|Number=Sing|Person=1|Tense=Pres|VerbForm=Fin	3	cop	_	_
5	io	io	PRON	PE	Number=Sing|Person=1|PronType=Prs	3	nsubj	11:nsubj	Propagate=Yes|SpaceAfter=No
6	,	,	PUNCT	FF	_	7	punct	_	_
7	non	non	ADV	BN	PronType=Neg	8	advmod	_	_
8	Walesa	Walesa	PROPN	SP	_	5	conj	3:nsubj	_
9	e	e	CCONJ	CC	_	11	cc	_	_
10	presto	presto	ADV	B	_	11	advmod	_	_
11	vedrò	vedere	VERB	V	Mood=Ind|Number=Sing|Person=1|Tense=Fut|VerbForm=Fin	3	conj	_	_
12	il	il	DET	RD	Definite=Def|Gender=Masc|Number=Sing|PronType=Art	13	det	_	_
13	leader	leader	NOUN	S	Gender=Masc	11	obj	_	_
14	sovietico	sovietico	ADJ	A	Gender=Masc|Number=Sing	13	amod	_	SpaceAfter=No
15	"	"	PUNCT	FB	_	3	punct	_	SpaceAfter=No
</div>

### <i>Sono stati adottati negli Stati Uniti dall'IEEE, e in ambito internazionale dall'ITU.</i>

<div class="conllu-parse" tabs="yes" id="tut-3427">
# visual-style 13 12 cc color:blue
# visual-style 13 14 obl:in color:blue
# visual-style 13 18 obl: color:blue
1	Sono	essere	AUX	VA	Mood=Ind|Number=Plur|Person=3|Tense=Pres|VerbForm=Fin	3	aux	_	_
2	stati	essere	AUX	VA	Gender=Masc|Number=Plur|Tense=Past|VerbForm=Part	3	aux:pass	_	_
3	adottati	adottare	VERB	V	Gender=Masc|Number=Plur|Tense=Past|VerbForm=Part	0	root	_	_
4	in	in	ADP	E	_	6	case	_	_
5	gli	il	DET	RD	Definite=Def|Gender=Masc|Number=Plur|PronType=Art	6	det	_	_
6	Stati	Stati	PROPN	SP	_	3	obl:in	_	_
7	Uniti	Uniti	PROPN	SP	_	6	flat:name	_	_
8	da	da	ADP	E	_	10	case	_	_
9	l'	il	DET	RD	Definite=Def|Number=Sing|PronType=Art	10	det	_	_
10	IEEE	IEEE	PROPN	SP	_	3	obl:agent	_	SpaceAfter=No
11	,	,	PUNCT	FF	_	14	punct	_	_
12	e	e	CCONJ	CC	_	14	cc	13:cc	_
13  E12.1	adottare	VERB	V	Gender=Masc|Number=Plur|Tense=Past|VerbForm=Part  3 conj:e	_	_
14	in	in	ADP	E	_	14	case	_	_
15	ambito	ambito	NOUN	S	Gender=Masc|Number=Sing	3	conj:e	13:obl:in	_
16	internazionale	internazionale	ADJ	A	Number=Sing	14	amod	_	_
17	da	da	ADP	E	_	18	case	_	_
18	l'	il	DET	RD	Definite=Def|Number=Sing|PronType=Art	18	_	_
19	ITU	ITU	PROPN	SP	_	13	obl:agent	_	SpaceAfter=No
20	.	.	PUNCT	FS	_	3	punct	_	_

</div>
