---
layout: entry
title:  'Sandbox'
---

~~~ sdparse
Mary/NNP got/VBD the/DT red/JJ dress and I got the blue
nsubj(got-2,Mary)
det(dress,the-3)
amod(dress,red)
dobj(got-2,dress)
cc(got-2,and)
conj(got-2,got-8)
nsubj(got-8,I)
dobj(got-8,blue)
det(blue,the-9)
~~~

~~~ sdparse
Mary got the red dress and I got the blue
nsubj(got-2,Mary)
det(dress,the-3)
amod(dress,red)
dobj(got-2,dress)
cc(got-2,and)
nsubj(got-8,I)
conj(got-2,got-8)
remnant(red,blue)
remnant(the-3,the-9)
~~~

<div class="sd-parse">
Alternative syntax
</div>

<div class="sd-parse" tabs="yes">
Dynamic visualization (click "edit!")
</div>

<div class="conllx-parse" tabs="yes">
1   CoNLL-X   CoNLL-X   NNP   _    _    2    NMOD    _    _
2   example   example   NN    _    _    0    ROOT    _    _
</div>

<div class="conllu-parse" tabs="yes">
1   CoNLL-U   CoNLL-U   NNP   _    _    2    nmod    _    _
2   example   example   NN    _    _    0    root    _    _
</div>

<div class="conllu-parse" tabs="yes">
# sentence-label S1
1   CoNLL-U   CoNLL-U   NNP   _    _    2    nmod    _    _
2   example   example   NN    _    _    0    root    _    _
</div>

<div class="ann-annotation" tabs="yes">
.ann annotation example
</div>

~~~ sdparse
Parse with errors
det(no-such, token)
~~~

Right-to-left text (Hebrew, SD format)

~~~ sdparse
דני/NOUN ראה/VERB סרט/NOUN
nsubj(ראה, דני)
dobj(ראה, סרט)
~~~

Same sentence in CoNLL-U:

~~~ conllu
1     דני       _        NOUN    _      _     2      nsubj _ _
2     ראה       _        VERB    _      _     0      root  _ _
3     סרט       _        NOUN    _      _     2      dobj  _ _
~~~

Arabic (CoNLL-U):

~~~ conllu
1     وَ       _        NOUN    _      _     2      nsubj _ _
2     لاحَظَ       _        VERB    _      _     0      root  _ _
3     التَقْرِيرُ       _        NOUN    _      _     2      dobj  _ _
~~~

----------
