Linguistics & NLP
================


------------------------------------------------------------------------

# Introduction

-   자연어처리

    -   자연어의 의미를 분석하여 컴퓨터가 처리할 수 있도록 하는 일

    -   자연어 이해, 자연어 생성, 음성인식, 음성합성, 기계번역 등

    -   examples

        -   정보검색, 음성인식, 번역, 감성분석, 요약 …

-   응용언어학과 자연어처리의 **관계**는?

    -   컴퓨터가 이해하도록 언어를 처리하는 과정에서 해당 언어의 특성을
        잘 알고 있어야 적절한 피쳐선택, 전처리 등을 통해 효율이 훨씬
        올라갈 수 있을 것

-   NLP past and present

    -   Knowledge\_based(rule-based)
    -   Statistical approach + Machine learning
    -   Deep learning

-   The current state of NLP

    -   자연어이해 HotpotQA, KorQuAD

    -   문장생성 GPT-3, chatbot

~~But~~  
~~동음이의어(훈장, medal’s words), 한눈을 팔다(sell one eye),
오다리(five-legged) …~~  
~~대화형 Agent, 서울의 수도가 어디야?, 어제보다 더워?~~

------------------------------------------------------------------------

# Natural language processing

<div class="figure" style="text-align: center">

<img src="C:/rdata/NLP_linguistic/pngfiles/set.png" alt="Natural language processing" width="980" />
<p class="caption">
Natural language processing
</p>

</div>

-   Basic steps of NLP
    -   Sentence splitting
    -   Tokenization
    -   Morphological analysis
    -   Part-of-speech tagging
    -   Shallow parsing
    -   Named entity recognition
    -   Syntactic parsing
    -   (Semantic Role Labeling)
    -   Semantic / Pragmatic analysis

------------------------------------------------------------------------

# What is Language?

We lived in a world of language. The possession of language
distinguishes humans from other animals. What does it mean to “know” a
language?  
\* Linguistic competence of linguistic knowledge : **mental grammar**  
\* mental grammar : internalized grammar that exists in the minds of
speakers

------------------------------------------------------------------------

# What is linguistic Knowledge?

When you know a language, you can speak and be understood by others who
know that language.  
When you know a language, you have the capactiy to produce sounds that
signify certain meanings and to understand or interpret the sounds
produced by others.

-   In summary
    1.  knowledge of **the sound system** : knowing sounds are in that
        language and what sounds are not, knowing which sounds may start
        a word, end a word, and follow each other.
    2.  knowledge of **Words** : knowing certain sequences of sounds
        signify certain concepts or meanings. The relationship between
        speech sounds and the meanings they represent is an
        **arbitrary** one.  
        &gt;&gt; Arbitrary Relation of Form and Meaning  
        The words of a particular language have the meanings they do
        only by **convention**.  
        (e.g. 돼지의 음성어 “꿀꿀”은 각 국마다 다르게 표현한다. form과
        meaning사이의 관계가 자의적이며 만들어 낸 것)
    3.  Knowledge of **Sentences and Non-sentences** : The number of
        sentences in a language is infinite.  
        knowing a language means being able to produce new sentences
        never spoken before and to understand sentences never heard
        before &gt;&gt; Creativity.  
        Our knowledge of a language determines which strings of words
        are well-formed sentences and which are not.  
        문장은 무한히 생성해낼 수 있으나, 그 방법은 유한하다.

------------------------------------------------------------------------

# What is Grammar?

-   Descriptive Grammar (언어학자에 의해 기술된 문법)
-   Prescriptive Grammars (규칙으로 정한 것)
-   **Universal Grammar** (보편 문법)
    -   인간이 보편적으로 이미 가지고 있는 모든 언어에 대한 문법.
        general grammar(모든 언어), special grammar(구체적인 언어 형태).

------------------------------------------------------------------------

# Can computers learn human language?

위 내용에 따르면, 컴퓨터가 자연어를 이해하려면 언어에 대한 지식들이
있어야하고 linguistic competence가 있어야 하는데?

<div class="figure" style="text-align: center">

<img src="C:/rdata/NLP_linguistic/pngfiles/turing.png" alt="Turing test(*Alan M. Turing 1912-1954*)" width="503" />
<p class="caption">
Turing test(*Alan M. Turing 1912-1954*)
</p>

</div>

------------------------------------------------------------------------

# Morphology : the words of language

Words are an important part of linguistic knowledge and constitute a
component of our mental grammars.  
We all have a mental dictionary of all the words we know, which includes
the following information :  
- Pronunciation (발음)  
- Meaning  
- Orthography (spelling)  
- Grammatical category (품사)

------------------------------------------------------------------------

## Content Words and Function words

-   Content words : 실제로 의미를 가지고 있는 단어 (nouns, verbs,
    adjectives, etc.) &gt;&gt; Open class : 계속 새로운 타입의 content
    words가 add될 수 있다.
-   Function words : 기능적인(grammatical) 의미를 하는 단어.
    (articles(관사 등), prepostitions, conjuctions, etc.) &gt;&gt;
    closed class : 새로운 타입이 add되기 쉽지 않다.
    -   mental grammar는 이를 구별하여 인식한다.

------------------------------------------------------------------------

## Morphemes : 형태소

-   Morphology : 단어의 구조(structure)와 형성해나가는 규칙(rule)에 대한
    학문 (e.g. cats, cat/s와 같은 rules)
-   Morpheme : the minimal units of meaning, and morphemes can be words
    on their own, and/or can often be combined with other morphemes to
    make words (e.g. the word *books* has two morphemes, *book(N)* +
    *-s(plural marker)*)

------------------------------------------------------------------------

## Bound and Free Morphemes

-   **Free morphemes(자립형태소)** can stand alone. (e.g. love), Free +
    Free 로 새로운 단어가 만들어지기도 함.
-   **Bound(affix) morphemes(구속형태소)** cannot stand along. 접사나
    구속어근처럼 다른 언어 형식에 결합되어 쓰이는 형태소(ex : -ish, un-)
    -   Prefixes : 앞에 붙는 것 (e.g. un-)
    -   Suffixex : 뒤에 붙는 것 (e.g. -ness)
    -   Infixes : inserted inside a root. (사이)
    -   Circumfixes : the beggining and the end of a root. (앞뒤)

------------------------------------------------------------------------

# Roots and Stems in Morphology

-   Roots : base. (unloveable, un-**love**-able)
-   Stems : once an affix has been attached to a root, (root + one
    morpheme, e.g. un-*loveable*)
-   Bound roots(구속어근) : 혼자 쓸 수 없는 roots. (e.g. -ceive.
    receive, conceive, preceive)

------------------------------------------------------------------------

# Rules of Word Formation : 단어 형성 규칙

-   Derivational morphemes : 의미와 root의 품사정보를 바꿈. (e.g. -ly,
    love + -ly, 품사와 의미를 바꿈)
-   Inflectional morphemes : similar to function words. it have only
    grammatical function, 항상 suffixes로 존재하며 개수가 한정적임.
    productive 함. (e.g. -s, -ed, -ing, -est)

------------------------------------------------------------------------

# Hierarchical Structure of Words

Morphemes are added to a base in a bixed order which reflects the
structure of a word.  
(e.g. unsystematic, un- + system + -atic, system + -atic을 하고 나서
un을 붙여야 함.)  
이 계층적구조가 존재하는 이유는, -atic은 명사에만 붙을 수 있고, un은
형용사에만 붙을 수 있으므로 이런 순서와 계층적구조가 필요하다.  
`unlockable` 같은 경우를 살펴보면, ‘un-’ 은 Adjective(lock + -able)에도,
Verb(lock)에도 붙을 수 있다. 전자로 계층구조를 잡으면 `'잠글 수 없는'`의
뜻을 가지며, 후자는 `'풀 수 있는'`으로 해석된다. &gt;&gt; ambiguous  
이 모호함은 context나 앞 뒤의 Hint 등으로 해결해야 한다.

<div class="figure" style="text-align: center">

<img src="C:/rdata/NLP_linguistic/pngfiles/unlockable.png" alt="two meaning of unlockable" width="100%" />
<p class="caption">
two meaning of unlockable
</p>

</div>

------------------------------------------------------------------------

# Rule Productivity

Derivational affixes are `productive` to different extents. (e.g. -able,
un-)

### Exceptions and Suppletions

-   Not all words undergo regular morphological processes. (e.g. feet,
    went, sing, children)  
-   When new words enter the language, regular morphological rules
    generally apply to them. (e.g. geek -&gt; geeks(not geeken))  
-   Borrowed words(차용어) may retain borrowed morphology. (e.g. Latin
    *datum*, and data)
-   Some morphemes have no phonological shape at all. (e.g. hit+past,
    sheep+plural)
-   When a verb is derived from a noun, even if it is pronounced the
    same as an irregular verb, the regular rules apply to it. 명사로도
    동사로도 쓰이는 단어 중 명사형에서 파생돼서 생긴 새로운 동사는
    기존의 룰을 따름.(e.g. *ring* / *rang*(벨이 울리는),
    ringed(둘러쌓인.., derived from a noun))
-   When a noun is used in a compound in which its meaning is lost, its
    plural follows the regular rules. (e.g. flatfoot / flatfeet,
    flatfoots)

### Other Morphological Processes

-   Back-formations : new words can be created through **misanalysis**
    of morpheme boundaries.  
    (e.g. editor(먼저 나온 단어) → edit / television(먼저 나온 단어) →
    televise)

-   Acronym : 초성을 따서 만든 단어 (e.g. NASA, BTW, UCLA)

-   Abbreviation / Clipping : a shortened form of a word or phrase.
    (e.g. bike/bicycle, gas/gasoline)

-   Eponym : Some people’s names are turned into everyday words.
    (e.g. *Murphy’s Law*)

-   Blends : words in which two words may be combined, but parts of the
    words that are combined are deleted. (e.g. smog(smoke + fog),
    bromance(brother + romance))

-   Compounds : joining two or more words together to make a new word.
    phrase(명사 구)와 비슷하지만 보통 띄어쓰기가 없는 경우가 많음.
    (e.g. cathouse, landlord)

------------------------------------------------------------------------

# One word or several words?

-   Idioms(관용어)
    -   A hot potato
    -   Piece of cake
-   Multi-token words
    -   New York
    -   Rock n roll

------------------------------------------------------------------------

# Sentence splitting

만약 다음과 같은 문장들이 있다고 하자.

Three years after its artificial-intelligence engine Watson made its
high-profile win on Jeopardy!, IBM is adapting the technology as it
seeks practical commercial uses, an IBM executive explained yesterday at
EmTech, a conference organized by MIT Technology Review. Rhodin said IBM
is refining Watson to make it more adept at providing the correct answer
to a specific question in a specific domain?for example, by learning
from previous queries. IBM has also been working with USAA, a company
that provides financial services to U.S. military personnel.
Mr. Sherwood said reaction to Sea Containers’ proposal has been “very
positive.” In New York Stock Exchange compositetrading yesterday, Sea
Containers closed at $62.625, up 62.5 cents. “I said, ‘what’re you?
Crazy?’”said Sadowsky. IL-33 is known to induce the production of
Th2-associated cytokines (e.g. IL-5 and IL-13).

이 문장을 **split**하고 싶다면 어떻게 할 것인가? 마침표 기준으로
나누어도 쉽지 않을 것이 예상된다. 문장 끝이 항상 마침표도 아니며,
마침표가 다른 의미로 쓰이는 경우도 있기 때문이다.

------------------------------------------------------------------------

# Word tokenization

영어는 space 단위로 문장을 나누면 간단하게 tokenization이 가능하다. 물론
경우에 따라 정확하지 않을 수 있다(Idiom이나 축약형). 이 때 중의성 등이
발생할 수 있다. 이 외에도 하이픈 등에서 여러 문제가 발생할 가능성이 없진
않으나 비교적 한글보다는 간단한 tokenization이 가능하다.

## Morphological analysis in korean

`나는 학교에 간다.`라는 문장을 tokenization을 한다고 하면 조금 더 복잡한
형태소 분석이 필요하다. 이를 살펴보면 이 또한 중의성도 있을 수 있다. 또
오타에 대한 문제가 생길 수도 있다.

<div class="figure" style="text-align: center">

<img src="C:/rdata/NLP_linguistic/pngfiles/koreantoken.png" alt="tokenization of korean" width="100%" />
<p class="caption">
tokenization of korean
</p>

</div>

## How to resolve typing mistakes?

오타에 대한 문제를 해결하기 위해선 `Levenshtein distance` 알고리즘이
유용하게 쓰일 수 있다. 다음 예시를 보고 이해할 수 있다. 혹은 `편집거리`
라고도 부른다. 편집거리 (edit distance, Levenshtein metric) 는 두
문자열에서 하나의 문자열을 다른 문자열과 똑같게 만들기 위해서 최소로
필요로 하는 편집 회수(문자 추가, 제거, 위치 변경)를 계산한다.

<img src="C:/rdata/NLP_linguistic/pngfiles/edit_distance.png" width="100%" style="display: block; margin: auto;" />

``` r
# 기본 패키지 사용
adist("shawn henry","shan hennyy")
```

    ##      [,1]
    ## [1,]    3

``` r
# stringdist package 사용
library(stringdist)
stringdist(c("shawn henry"), c("shan hennyy", "show hurry"))
```

    ## [1] 3 4

``` r
# make matrix
stringdistmatrix(c("foo","bar","boo","baz"))
```

    ##   1 2 3
    ## 2 3    
    ## 3 1 2  
    ## 4 3 1 2

``` r
# 유사한 것 찾기
amatch(c("hello"),c("hillu","hala","hallo", "hi"),maxDist=2)
```

    ## [1] 3

------------------------------------------------------------------------

------------------------------------------------------------------------

# Syntax (구문, 문법)

유한한 규칙의 문법으로 무한한개수의 문장을 생성할 수 있다. 또한 처음보는
문장을 생성, 이해할 수 있다.

## What the Syntax Rules Do

word + word = phrase  
phrase + phrase = sentence  
맞는 어순으로 문장을 만들어 낼 수 있도록 함. 한국은 SOV순이며, 영어는
SVO 순.

-   대통령은 새 대법관을 지명했다.
-   새 대법관을 대통령은 지명했다.

또한 의미도 달라질 수 있다.  
- *I mean what I say vs. I say what i mean.*  
- 나는 망원경을 들고 있는 남자를 보았다 `vs.` 망원경을 들고 있는 나는
남자들 보았다.  
또한 syntax rule은 *grammatical relations of a sentence*를 특정
지어주기도 한다.  
나아가 Syntax rule은 **constraints**를 정의한다. (e.g. 주격조사, 동사에
따른 목적격의 결정 등)

Syntax를 어떻게 해석하냐에 따라 의미가 달라질 수 있으며, 이 경우
tree(hierarchical)이 있어야 ambiguity를 해결할 수 있다.

<div class="figure" style="text-align: center">

<img src="C:/rdata/NLP_linguistic/pngfiles/omw.png" alt="old men and women" width="100%" />
<p class="caption">
old men and women
</p>

</div>

lexical ambiguity는 context없이는 해결하기 힘들다.(e.g. this makes you
smart)

------------------------------------------------------------------------

# What Grammaticality is **not** based on

“무도회에서 분홍색 양말을 신은 거대한 귀뚜라미가 춤을 추었다.” 이런
문장이 있다고 했을 때, 문법적으로는 완벽하지만 진실인지 아닌지, 의미가
있는지 없는지는 확인해봐야 한다. 따라서 문법은 진실 여부와 의미 유무는
기반하고 있지 않다.

------------------------------------------------------------------------

# Sentence Structure

S-V-O, N-V-N 등으로 일차원으로 문장구조를 기술할 수 있다. 만약
morpheme이 여러개로 이루어져있거나, 합성이 있다면 1차원이 아닌 tree
diagram으로 문장구조를 기술해야 중의성을 해결할 수 있다.

------------------------------------------------------------------------

# Constituents and Constituency Tests

-   Constituents are the natural groupings in a sentence.
    -   \[\[the\] \[child\]\] \[\[found\] \[\[a\] \[puppy\]\]

1.  stand alone test
2.  replacement by pronoun or do
3.  move as a unit

------------------------------------------------------------------------

# Syntactic Categories

A syntactic category is a family of expressions that can substitute for
one another without loss of grammaticality.

## NP

-   **the child** found a puppy.  
-   **A police officer** found a puppy.  
-   **Your neighbor** found a puppy.

## VP

-   The child **found a puppy**.  
-   The child **ate the cake**.  
-   The child **slept**.

## 그 외

#### Phrasal categories

-   NP (명사구): men, the man, the man with a telescope  
-   VP (동사구): sees, always sees, rarely sees the man, often sees the
    man with a telescope, know who you are, slept on the bed  
-   PP (전치사구): over, nearly over, over the hill  
-   AdjP (형용사구): happy, very happy, very happy about winning  
-   AdvP (부사구): brightly, more brightly, more brightly than the Sun

#### Lexical categories

-   Noun (명사): puppy, girl, soup, happiness, pillow  
-   Verb (동사): find, run, sleep, realize, see, want  
-   Preposition (전치사): up, down, across, into, from, with  
-   Adjective (형용사): red, big, candid, lucky, large  
-   Adverb (부사): again, carefully, luckily, very, fairly

#### functional categories

-   Auxiliary (조동사): verbs such as have, and be, and modals such as
    may, can, will, shall, must
-   Determiners (한정사): the, a, this, that, those, each, every

• English : Noun, Pronoun, Verb, Adjective, Adverb, Interjection,
Preposition, Conjunction.  
• Korean : 명사, 대명사, 동사, 형용사, 부사, 대명사, 감탄사, 조사, 수사,
관형사

------------------------------------------------------------------------

# Penn Treebank Tagset

<div class="figure" style="text-align: center">

<img src="C:/rdata/NLP_linguistic/pngfiles/tagset_eng.png" alt="Penn treebank tagset" width="100%" />
<p class="caption">
Penn treebank tagset
</p>

</div>

------------------------------------------------------------------------

# Korean POS tagging

kkma, hannanum, simplepos 등 다양한 오픈소스 존재.

------------------------------------------------------------------------

# Phrase Structure Trees

The italicized word(s) is the head of every phrase. Every phrase is
determined by its head.

-   The phrasal category that may occur next to a head and elaborates on
    the meaning of the head is a complement.  
-   The core of every phrase is its head.(except NP)
-   Elements preceding the head are specifiers.

------------------------------------------------------------------------

# Selection

동사의 종류에 따라서 동사가 명사나 부사를 요구하거나,
제약조건(constraints)를 요구하기도 한다. 자세하겐 동사가 의미적으로
추가적인 것을 요구하거나, 문법적인 것만을 요구하기도 한다.  
- C-selection  
- S-selection

------------------------------------------------------------------------

# Structure Ambiguities

The following sentence has two meanings : *The boy saw the man with the
telescope.*  
The meanings are :  
– 1. The boy used the telescope to see the man.  
– 2. The boy saw the man who had a telescope.  
Each of these meanings can be represented by a different phrase
structure tree.

### Local ambiguities

*the girl told the story cried.*, 이 문장을 왼쪽에서부터 읽어보면 바로
이해가 되지 않고 다시 한 번 읽어봐야 이해가 됨.

------------------------------------------------------------------------

# Dependency grammar

phrase structure grammar로 보는 것보다 Dependency grammar로 보는 것이
조금은 trend인듯함.  
• It is based on the dependency relation.  
• A dependency structure is determined by the relation between a word (a
head) and its dependents.  
• It is well suited for the analysis of languages with free word
order.  
• Governor (지배소)  
• Dependent (의존소)

<div class="figure" style="text-align: center">

<img src="C:/rdata/NLP_linguistic/pngfiles/dependency.png" alt="grammar dependency vs. phrase structure" width="100%" />
<p class="caption">
grammar dependency vs. phrase structure
</p>

</div>

<div class="figure" style="text-align: center">

<img src="C:/rdata/NLP_linguistic/pngfiles/dep2.png" alt="dependency rule" width="100%" />
<p class="caption">
dependency rule
</p>

</div>

But,Korean  
• Free in word order  
• Omission  
+ ungrammatical sentences on the internet

------------------------------------------------------------------------

# Semantics (& Pragmatics)

## The Meaning of Language

-   when you know a language, you know :
    -   a word(sentence) is meaningful or not
    -   a word(sentence) has two meanings
    -   two words(sentences) have the same meanings
    -   two words(sentences) have opposite meanings
    -   what words refer to (sentences is true or false)

## What Speaker Know about Sentence Meaning :

### Truth

If you know the meaning of a sentence, you can determine under what
conditions it is true or false.  
You don’t need to know whether or not a sentence is true of false to
understand it.  
Most sentences are true or false depending on the situation. But some
sentences are always true(false).  
사람 대 사람으로 얘기할 때는 shared knowledge나 상황에 의존하고 있는
것이 분명히 있지만, 컴퓨터가 인식을 해야할 땐?

### Entailment and Related Notions

또한 모든 sentences에는 Entailment(함의)가 있고, paraphrases
sentences(entail relationship)나, contradictory realatons관계는 어떻게
인식을 시켜야 하는가?

### Ambiguity

-   Syntatic ambiguity (구조적 중의성) (e.g. *the boy saw the man with
    the telescope*)
-   Lexical ambiguity (어휘적 중의성) (e.g. *smart*(똑똑하다, 얼얼하다))

## Compositional Semantics

우리가 처음 본 문장을 해석할 줄 아는 이유는 구조적으로 어떻게 해석해야
할 지를 알 기 때문이다. 또 각각의 단어가 가지고 있는 의미를 알고 있기
때문에 그 각각의 의미를 구조적으로 넣어 이해하기 때문이다.

## When Compositionality Goes Awry :

### Anomaly(변칙)

-   An anomalous sentence
    -   *Colorless green ideas sleep furiously.*(WHAT??)
    -   이 문장은 구조적으로 괜찮지만 contains semantic violations하다.

### Metaphor

-   (e.g. *A grief ago*, *Walls have ears.*)

### Idioms

they must be listed in a mental lexicon!

-   (e.g. *drop the ball*, *put his foot in his mouth*)

## Lexical Semantics :

### Reference

Referent(지시대상) : the real-world objectt designated by a word  
- Jack, the happy swimmer, my friend, and that guy can all have the same
referent in the sentence Jack swims.  
- Jack = the happy swimmer = my friend = that guy

### Sense

Sense (의미): an element of meaning separate from reference and more
enduring

The same reference but different senses

-   Barack Obama  
-   The President (미합중국의 수장)  
-   Michelle Obama’s husband

## Lexical Relations :

### Synonyms(동의어)

e.g. sofa = couch, apathetic = indifferent

### Antonyms(반의어)

e.g. alive/dead, present/absent → comlementary antonyms  
e.g. big/small, hot/cold → Gradable antonyms  
e.g. give/receive, buy/sell → Relational antonyms

그 외 :

-   Homonyms(동철동음이의어, e.g. bank(은행,둑))  
-   Homographs(동철이의어, e.g. bow(인사하다, 활))  
-   Homophones(동음이의어, e.g. bear and bare)  
-   Polysemy(다의어, e.g. diamond : the geometric shape; abaseball
    field)

## Lexical Relations

-   *Hyponym* and *hypernym* involve the relationship between a general
    term and specific instances of that term

### WordNet

A large lexical database of English words. Nouns, verbs, adjectives, and
adverbs are grouped into sets of cognitive synonyms called ‘synsets’,
each expressing a distinct concept. Synsets are interlinked using
conceptual-semantic and lexical relations such as hyponymy

<div class="figure" style="text-align: center">

<img src="C:/rdata/NLP_linguistic/pngfiles/book.png" alt="book" width="100%" />
<p class="caption">
book
</p>

</div>

### MindNet

Automatically created database of lexico-semantic relations (MS)

<div class="figure" style="text-align: center">

<img src="C:/rdata/NLP_linguistic/pngfiles/mind.png" alt="mindnet" width="100%" />
<p class="caption">
mindnet
</p>

</div>

-   Other linguistic database
    -   PropBank
    -   FrameNet

# Semantic features

The conceptual elements that are part of the meanings of words and
sentences. Antonyms is that they share all but one semantic feature.

-   (e.g. Noun, \[female feature\] hen, aunt, girl, woman)
-   (e.g. Verb, \[cause to\] darken, kill, uglify)

# Thematic Roles

Thematic\[Ɵ\] roles (의미역) express the relation between the arguments
of the verb and the situation the verb describes.

-   Agent: the ‘doer’ of the action
-   Theme: the ‘undergoer’ of the action
-   Goal: the endpoint of a change in location or possession
-   Source: where the action originates
-   Instrument: the means used to accomplish an action
-   Experiencer: one receiving sensory input

# Pragmatics

Pragmatics (화용) is concerned with our understanding of language in
context.

– Linguistic context: the discourse that precedes the phrase or sentence
to be interpreted – Situational context: everything nonlinguistic in the
environment of the discourse

-   오늘 덥지 않아?
-   어제까지 날씨가 선선했다는 대화가 오간 상황
-   현재 겨울인 경우
-   차안에서의 대화인 경우
-   길을 걸으면서 하는 대화인 경우

# Deixis

Deixis refers to words and expression whose reference depend on the
situational context.

-   Person deixis
-   Time deixis
-   Place deixis

사용예시

-   Arnold Schwarzenegger really likes it in Venice. On December 11,
    2012, there was a boat parade in the canals in Venice. On December
    12, 2012, an art festival will be held. The art festival on December
    12, 2012 will be extremely fun.  
-   I really like it in Venice. Today, there was a boat parade in the
    canals here. Tomorrow an art festival will be held. It will be
    extremely fun.

# Pronouns and Linguistic Context

Pronouns get their meaning from other NPs in the sentence or discourse.
Reflexive pronouns always depend on an antecedent in the same clause for
its meaning. Regular pronouns cannot refer to an antecedent in the same
clause.

# Referent

• Can I borrow your Shakespeare? • Shakespeare takes up the whole bottom
shelf.

# Implicatures

Implicatures (함축) are inferences that may be drawn from an utterance
based on context.

-   SUE: Does Mary have a boyfriend?  
-   BILL: She’s been driving to Santa Barbara every weekend.

Bill asserts that Mary drives to Santa Barbara every weekend and
implicates that she has a boyfriend living in Santa Barbara.

# Maxims of Conversation

-   Maxims of conversation are conversational conventions that govern
    discourse
    -   Maxim of Quality: Truth
    -   Do not say what you believe to be false.
    -   Do not say that for which you lack adequate evidence.
-   Maxim of Quantity: Information
    -   Make your contribution as informative as is required for the
        current purposes of the exchange.
    -   Do not make your contribution more informative than is required.
-   Maxim of Relation: Relevance
    -   Be relevant.
-   Maxim of Manner: Clarity
    -   Avoid obscurity of expression.
    -   Avoid ambiguity.
    -   Avoid unnecessary wordiness.
    -   Be orderly

# Presupposition (전제)

• Have you stopped hugging your border collie?  
• Takes some more tea.  
• Have another beer.  
• The present King of France is bald

# Speech Acts

-   The study of speech acts describes how people do things with
    language.  
-   Performative verbs: verbs that accomplish an action when they are
    uttered.
    -   Some performative verbs: bet, challenge, dare, fine, nominate,
        promise, resign
    -   A test for performativity: performative verbs usually sound good
        when you add I hereby to the sentence :
        -   I hereby resign
        -   ?I hereby know you
