---
layout: entry
title: UD Examples
---
This repository is for producing example visualizations for UD graphs

<div class="conllu-parse" tabs="yes" width="800px" id="xsubj">
# visual-style  8 6 nsubj:xsubj color:blue
1 La  _ _ _ _ 2 det _ _
2 mamma _ _ _ _ 4 nsubj _ _
3 ha  _ _ _ _ 4 aux _ _
4 chiesto _ _ _ _ 0 root _ _
5 a _ _ _ _ 6 case  _ _
6 Maria _ _ _ _ 4 obl 8:nsubj:xsubj _
7 di  _ _ _ _ 8 case  _ _
8 comprare  _ _ _ _ 4 xcomp _ _
9 il  _ _ _ _ 10  det _ _
10  pane  _ _ _ _ 8 obj _ _
11  . _ _ _ _ 4 punct _ _
</div>

<div class="conllu-parse" tabs="yes" width="800px" id="dep propagation">
# visual-style  5 2 nsubj color:blue
# visual-style  5 6 obj color:blue
1 La  _ _ _ _ 2 det _ _
2 libreria _ _ _ _ 3 nsubj 5:nsubj _
3 compra  _ _ _ _ 0 root _ _
4 e _ _ _ _ 5 cc _ _
5 vende _ _ _ _ 3 conj  _ _
6 libri _ _ _ _ 3 obj  5:obj  _
7 usati  _ _ _ _ 6 amod  _ _
8 . _ _ _ _ 3 punct _ _
</div>

<div class="conllu-parse" tabs="yes" width="800px" id="dep propagation">
# visual-style  3 6 obj color:blue
1 La  _ _ _ _ 2 det _ _
2 libreria _ _ _ _ 3 nsubj _ _
3 vende  _ _ _ _ 0 root _ _
4 libri _ _ _ _ 3 obj _ _
5 e _ _ _ _ 6 cc  _ _
6 riviste _ _ _ _ 4 conj  3:obj _
. _ _ _ _ 3 punct _ _
</div>


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
# visual-style 13 15 obl:in color:blue
# visual-style 13 19 obl:agent color:blue
# visual-style 13 3 conj:e color:blue
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
11	,	,	PUNCT	FF	_	15	punct	_	_
12	e	e	CCONJ	CC	_	15	cc	13:cc	_
13	E12.1	adottare	VERB	V	Gender=Masc|Number=Plur|Tense=Past|VerbForm=Part  3 conj:e	_	_
14	in	in	ADP	E	_	15	case	_	_
15	ambito	ambito	NOUN	S	Gender=Masc|Number=Sing	13	obl:in	_	_
16	internazionale	internazionale	ADJ	A	Number=Sing	15	amod	_	_
17	da	da	ADP	E	_	19	case	_	_
18	l'	il	DET	RD	Definite=Def|Number=Sing|PronType=Art	19	det	_
19	ITU	ITU	PROPN	SP	_	13	obl:agent	_	SpaceAfter=No
20	.	.	PUNCT	FS	_	3	punct	_	_

</div>
