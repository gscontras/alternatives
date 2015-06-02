## Grammatical Alternatives

This repo contains information relevant to the role of grammatical alternatives in formal semantics, with an eye toward comparing these alternatives with alternative utterances appealed to in the RSA framework.

### The symmetry problem (from Fox & Katzir, 2011)

Two phenomena, ***scalar implicature*** and ***association with focus***, make reference to sets of alternatives, which are constrained by grammar and context. In both cases, the relevant alternatives are negated through the assertion of the utterance.

- Examples of both:
	- John ate ***some*** of the cake. 	 
		Scalar implicature: John didn't eat all of it
	- John only at the ***cake***.  
		Association with focus: John didn't eat, e.g., the cookies

Account of Scalar Implicature: Horn Scales (Horn, 1972), in which linguistic elements are related to alternatives through a family of lexical stipulations.  
			
	{ some, all, ... }

Account of focus: Focus Semantics (Rooth, 1985), in which every linguistic element has as its alternatives all other elements of the same semantic type.  

	{ cake, cookies, ... }

Given their remarkable similarity, Fox & Katzir aim to unify these two accounts.

#### Scalar implicature

- Some simple sentences with their scalar implicatures:  
	- John did some of the homework.  
		 ¬ [John did all of the homework] 
	- John did the reading or the homework.  
		 ¬ [John did the reading and the homework]
	- John has three children.  
		 ¬ [John has four children]
	 
- The scalar implicature of a sentence *S* given a set of alternatives *A* involves the negation of elements in that set of alternatives *A*
	- *SI*(*S*) = &and;{¬*S* : *S* &in; *A*}  
- The strengthened meaning of a sentence incorporates its scalar implicature:
	- *SM*(*S*) = *S* &and; *SI*(*S*)
- The work lies in answering the question of how *A* is determined

##### Horn (1972)

- The set of formal alternatives to a sentence *S*, *F*(*S*), is defined as the set obtained by replacing certain elements of *S*, ***scalar items***, with memebrs of a set of stipulated alternatives, often referred to as ***Horn Scales***
	- *F*(*S*) = {*S*' : *S*' *is the result of replacing scalar items in S with their scale mates}*
- The set of alternatives *A* of a sentence *S* is a contextually determined subset of a set *F*(*S*)
	- *A* = *C* &cap; *F*(*S*)
- Where *C* is a set of contextually-determined sentences; we need to invoke *C* because different scalar implicatures are generated in different contexts
	- John did ***some*** of the homework.  
		¬ [John did most of the homework]		
		¬ [John did all of the homework]
		
##### Here comes symmetry

- For any sentence *S* for which we would like to use an alternative *S1* to derive a scalar implicature &not;*S1*, there is ***always*** another potential alternative, *S2* = (*S* & &not;*S1*), which, if taken into account, would prevent the desired implicature from arising
- Consider the following sentence with its desired scalar implicature:
	- John read ***three*** books.  
		&not; [John read four books]
- And the sentence's potential alternatives:
	- John read four books.
	- John read exactly three books.
- But if both of these sentences are truly alternatives, we have no home of dervining the scalar implicature; this holds generally of symmetric alternatives
- A definition of symmetry:
	- Let *S*, *S1*, *S2* be three sentences. We say that *S1* and *S2* are ***symmetric*** alternatives of *S* if both
		1. *S1* &cup; *S2* = *S*, and
		2. *S1* &cap; *S2* = &empty;
- The standard assumption: *F*(*S*) breaks symmetry by stipulating the appropriate scales
	- ***some*** and ***all*** (but not ***some but not all***) are scale mates
	- ***or*** and ***and*** (but not ***or but not both***) are scale mates
	- ***three*** and ***four*** (but not ***exactly three***) are scale mates
- This works for scalar implicature, but it is massively stipulative; worse, we encounter a similar problem of symmetry in association with focus, without a similar solution

#### Association with focus

- Some sentences with their corresponding inferences:
	- John only introduced ***Mary*** to Sue.  
		&not; [John introduced Jane to Sue]
	- John only introduced Mary to ***Sue***.  
		&not; [John introduced Mary to Jane]
	- John only has ***three*** children.  
		&not; [John has four children]
- *Only(S)* has entailments that are similar to the scalar implicatures of *S* when uttered in isolation; it entails the negation of various alternatives *A* to the prejacent *S*. This exclusivity inference ought to ring familiar from scalar implicture:
	- *EXC*(*S*) = 	= &and;{¬*S* : *S* &in; *A*}  
- The meaning of *Only*(*S*) gets defined in a way similar to the strengthened meaning of a sentence with its scalar implicature:
	- *Only*(*S*) = *S* &and; *EXC*(*S*)
- Once again, the work lies in answering the question of how *A* is determined

##### Rooth (1985)

- As with scalar implicature, we associate *A* with a subset of the set *F*(*S*) of formal alternatives to *S*
	- *A* = *C* &cap; *F*(*S*)
- We appeal again to *C*, the contextually determined sentences, given the sensitivity of focus to context:
	- Mary only ***read War and Peace***.  
		¬ [Mary saw a movie]		
		¬ [Mary ate an apple]
 - Following Rooth (1985), we define *F*(*S*), the formal alternatives to *S*, as those sentences that replace the focused consituent of *S* with all possible denotations of the same type  
	- *F*(*S*) = {*S*' : *S*' *is the result of replacing focused items in S with elements of the same semantic type*}
- It bears noting that association with focus arises also in the absence of ***only***; again, the placement of focus determines the alternatives, which determine the implicated meaning
	- A: How did the exam go?  
		B1: Well, I ***passed***.  
		B2: Well, ***I*** passed.
		
##### Symmetry still haunts us

- Consider the focused sentence with its intended inference:
	- John only ***read War and Peace***.  
		&not; [John saw a movie]
- As with scalar implicature, this sentence ought to have symmetric alternatives, which, when negated, lead to gibberish
	- John read War and Peace and saw a movie.		
	- John read War and Peace and didn't see a movie.
- Given a type-based definition of alternatives, we would need context *C* to break the symmetry for focus; but symmetry breaking always rules in favor of simpler alternatives, suggesting intervention on the part of grammar
		
##### Comparing the two approaches to alternatives

- For both scalar implicature and association with focus, the resulting interpretation involves conjoining a sentence *S* with the negations of its alternatives *A*, where *A* is determined both by contextual factors, *C*, and by formal restrictions, *F*(*S*)
	- For scalar implicature, *F*(*S*) is determined by stipulated lexical properties (i.e., *Horn Scales*)  
	- For association with focus, *F*(*S*) is determined by Rooth's procedure of focus alternatives based on semantic type
- We want a unified, non-stipulative theory of grammatical alternatives 
	- Apply a procedure similar Rooth's to both association with focus and scalar implicature
	- Without *Horn Scales* or context to break symmetry, we need some other aspect of grammar to do this for us: structure

#### An alternative theory of alternatives

- The goal: a unified theory of *F* (i.e., formal alternatives) for both scalar implicature and association with focus
	- Define alternatives in terms of replacable elements and their possible replacements
	- Identify replaceable with the set of focused consituents
	- Identify the possible replacements of a constituent with the set of constituents that are at most equally complex

##### Defining complexity

- Following Katzir (2007), complexity is relativized to a context *C* and evaluated with respect to structure
- The relation &le;*<sub>c</sub>* --- '*at most as complex as, in context C*' --- orders structures according to complexity
	- *S'* &le;*<sub>c</sub>* *S* if *S'* can be derived from *S* by successive replacements of sub-constituents of *S* with elements of the ***substitution source*** for *S* in *C*, *SS*(*S*, *C*)
	- *SS*(*X*, *C*), the substitution source for *X* in context *C*, is the union of the following sets:
		1. The lexicon
		2. The sub-constituents of *X*
		3. The set of salient constituents in *C*
- A structure *X* gets simplified using substitutions from the lexicon and from the set of sub-constituents of *X*

##### Calculating alternatives

- The formal alternatives of a sentence *S* are defined as the set of all structures obtained from *S* by replacing ***focused constituents*** within *S* with constituents that are at most as complex as the original constituent
	- *F*(*S*, *C*) = {*S*' : *S*' is derived from *S* by replacing focused constituents *x<sub>1</sub>*, ... , *x<sub>n</sub>* with *y<sub>1</sub>*, ... , *y<sub>n</sub>*, where *y<sub>1</sub>* &le;*<sub>c</sub> x<sub>1</sub>*, ... , *y<sub>n</sub>* &le;*<sub>c</sub> x<sub>n</sub>*}
- This definition preserves the generality of Rooth's type-based proposal, while allowing *F* to break symmetry
	- ***some***, ***all***, and ***some by not all*** are all quantifiers of the same time, but only ***some*** and ***all*** are of the same complexity; ***some but not all*** is strictly more complex
	- With a structure definition, an occurrence of ***some*** will bring in ***all*** (but not ***some but not all***) as replacements, the negation of which delivers a scalar implicature
- Contextually salient constituents are allowed in the substitution source to account for cases where a scalar implicature does appeal more complex alternatives:
	- It was warm yesterday, and it is a little bit more than warm today.  
		&not; [It was a little bit more than warm yesterday]
		
##### A final note on context

- We might jettison this more complex theory of alternatives if we could ensure that context *C* breaks symmetry
- But on the assumption that *S* is relevant whenever it is relevant to know whether *S* is true, we cannot consider *S* relevant without also considering &not;*S* relevant; and if two sentences are relevant, so is their conjunction
	- Closure assumption for relevance:
		1. If *S* is relevant, so is &not;*S*
		2. If *S1*, *S2* are relevant, so is *S1* &and; *S2*
- With *C* as the set of relevant sentences, whenever one of two symmetric alternatives is relevant, so is the other; we need something in addition to context (i.e., structural complexity) to break symmetry

### On the architecture of grammar (Ciardelli & Roelofsen, *to appear*)

The standard, Montagovian framework for natural language semantics assumes that an expression denotes a single semantic object (proper noun &rarr; individual; sentence &rarr; proposition). In an extension of this framework, ***Alternative Semantics*** diverges from tradition in assuming that the denotation of an expression is a ***set*** of objects in the expression's usual domain of interpretation. This set contains all of the admissable alternatives to the originial denotation (Hamblin, 1973).

While this move has many desired consequences, including accounts of questions, indefinites, and pronouns, it is not without its problems. Ciardelli & Roelofsen point out two such problems:

1. The compositionality issue: in alternative semantics, meanings can no longer be composed by means of the standard type-theoretic operations of function application and abstraction.
2. The entailment issue: meanings in alternative semantics can no longer be compared (or conjoined) by means of the standard type-theoretic notion of entailment.

But first, a detour looking at the original motivation for alternative semantics.

#### Alternative Semantics (Hamblin, 1973)

- Montague (1970):  
	"I regard the construction of a theory of ***truth*** -- or rather, of the more general notion of truth under and arbitrary interpretation -- as the basic goal of serious syntax and semantics."

- Hamblin:  
	"What of the many uses of natural language for purposes incidental to, or with other goals than, the embodiment of truth, as in ***questions***...?"  
	"The study of questions leans out to pragmatics in the sense that someone who thinks the exclusive purpose of language is to state truths may be led by it to think again."
	
##### Incorporating questions into Montague's semantics

- The interrogative words of English already fit neatly into Montague's categories:
	- "who" and "what" stand as proper nouns
	- "how", "when", and "where" stand as adverbs
	- "what/which X" stand as quantifiers
	- "Only 'why' seems to lead us outside the bounds of Montague English (and we shall ignore it)."
- Classing "who" and "what" as proper names, ther should be regarded as denoting ***sets*** of individuals
- A question like "who walks?" itself denotes a set, namely the set whose members are the propositions "X walks", where X is in the denotation of "who"
- A question sets up a choice-situation between a set of propositions (its answers)

##### Adding in indicatives

- Indicatives are regarded as equivalent to one-alternative interrogatives
	- "Mary" denotes the set whose sole member is Mary
	- "Mary walks" denotes the set whose sole member is the proposition that Mary walks
- An answer to a question is any statement whose denotation is contained in that of the question

#### And now the compositionality issue

- In the Montagovian framework, two basic type-theoretic operations allow for the composition of meanings
	1. Function application:  if ***&Alpha;***:<&sigma;, &tau;> and ***&Beta;***:&sigma;, then  
		[[***&Alpha;***(***&Beta;***)]] = [[***A***]] applied to [[***B***]], the result of which is   in *D*<sub>&tau;</sub>
	2. Abstraction: if ***&Alpha;***:&tau; and ***x***:&sigma;, then  
		[[***&lambda;x.&Alpha;***]] is the function mapping any *x* &in; *D*<sub>&sigma;</sub> to [[***&Alpha;***]]<sub>*g*[***x***/*x*]</sub>
- In alternative semantics, if ***&Alpha;*** is of type <&sigma;, &tau;> and &Beta; is of type &sigma;
	- [[***&Alpha;***]] &subseteq; *D*<sub><&sigma;, &tau;></sub> and [[***&Beta;***]] &subseteq; *D*<sub>&sigma;</sub>
	- We can no longer obtain [[***&Alpha;***(***&Beta;***)]] by simply applying [[***&Alpha;***]] to [[***&Beta;***]] because [[***&Alpha;***]] ***is not a function***

##### Pointwise function application

- Given that expressions now denote sets of objects, what we can do is apply each function *f* &in; [[***&Alpha;***]] to each object *d* &in; [[***&Beta;***]]
	- The set of objects *f*(*d*) obtained in this way is a subset of  *D*<sub>&tau;</sub>, which is a suitable semantic value for ***&Alpha;***(***&Beta;***)
- ***BUT***: in computing the meaning of ***&Alpha;***(***&Beta;***) using pointwise function application, the functor ***&Alpha;*** only has access to each alternative for ***&Beta;*** in isolation
- Many functors ***do*** need access to the full alternative set, e.g., negation, modals, conditionals, question-embedding verbs, etc.

##### Solution: adjust the typing of expressions

- Desiderata for a solution:
	1. The denotation of a sentence is a set of propositions
	2. The denotation of an expression of type &tau; is a single object in *D*<sub>&tau;</sub>
	3. The composition rules are the standard type-theoretic ones
- Possibility semantics introduces complexity in our basic propositional type:
	- Propositions are type <<*s*, *t*>, *t*>, abbreviated as *T*
	- ***walks***:<*e*, *T*>
	- [[***walks***]] = &lambda;*x*.{|*Wx*|} = &lambda;*x*.{ {*w* : *x* walks in *x*} }
- A worked-out example for the question "Who did John see?"
	- ***who &lambda;x John saw x***
		- [[***John***]] = *j*
		- [[***saw***]] = &lambda;*x*.&lambda;*y*.{|*Syx*|}
		- [[***who***]] = &lambda;*P*<sub><*e*,*T*></sub>. U<sub>*x*&in;*D*<sub>*e*</sub></sub> *P*(*x*)
	- [[***&lambda;x John saw x***]] = &lambda;*x*.{|*Sjx*|}
	- [[***who &lambda;x John saw x***]] = {|*Sjx*| : *x* &in; *D*<sub>*e*</sub>}

#### We still face a problem with entailment

- Function application and abstraction ***compose*** meanings; entailment ***compares*** them
- The notion of entailment amounts to set-theoretic inclusion
	- |***&Alpha;***| &#8872; |***&Beta;***|   &hArr;   [[***&Alpha;***]] &subseteq; [[***&Beta;***]]

##### Walking &rarr; moving

- If John walks, he moves; the sentence "John walks" intuitively entails the sentence "John moves"
- |*Wj*| is the set of worlds where John walks and |*Mj*| is the set of worlds where John moves
	-  John moves in every world in which he walks
	-  We therefore have |*Wj*| &subseteq; |*Mj*|, and the entailment is predicted
- In both alternative semantics and possibility semantics:
	- [[***John walks***]] = {|*Wj*|} and [[***John moves***]] = {|*Mj*|}
	- {|*Wj*|} &nsubseteq; {|*Mj*|}, so the entailment is not predicted
- Entailment fails because the meaning of a sentence is the singleton set consisting of its unique alternative
- "To enjoy the benefits of having alternatives in our semantics, it is not necessary to assume that the meaning of a sentence is ***identical*** with the set of alternatives the sentence introduces; it is sufficient to assume that the meaning of a sentence ***determines*** the set of alternatives that it introduces."

##### Saving entailment

- We want to preserve the truth-conditional notion of entailment:
	- |***&Alpha;***| &#8872; |***&Beta;***|   &hArr;   [[***&Alpha;***]] &subseteq; [[***&Beta;***]]
- Rather than construing [[***&Alpha;***]]  and [[***&Beta;***]] as the singleton sets {|***&Alpha;***|} and {|***&Beta;***|}, construe them as the ***powersets*** &#119979;(|***&Alpha;***|) and &#119979;(|***&Beta;***|)
- The meaning of "John walks" is now the set of all propositions that contain enough information to establish that John walks
	- It contains all propositions *p* such that John walks in every world in *p*
	- Not just the proposition containing precisely the information that John walks (i.e., the set of all worls in which John walks)
- We can recover the unique alternative for "John walks" as the ***maximal element*** of its meaning

#### Inquisitive semantics

- The meaning of a sentence consists of all propositions that contain ***enough*** information to resolve the issue that the sentence raises
- Sentential meanings are ***downward closed*** sets of propositions
	- If *p* contains enough information to resolve the issue that ***&Alpha;*** raises, then any *q* &subseteq; *p* will also contain enough information to do so
- The ***alternatives*** that ***&Alpha;*** introduces can be recovered as the ***maximal elements*** of [[***&Alpha;***]]
	- These alternatives contain enough information to resolve the issue raised by ***&Alpha;***, but nore more information than necessary
	- **ALT**(***&Alpha;***) = {*p* &in; [[***&Alpha;***]] : there is no *q* &in;  [[***&Alpha;***]] such that *p* &subset; *q*}
- Rather than identifying the meaning of a sentence with a set of alternatives, Inquisitive Semantics has the meaning of a sentence determine a set of a alternatives

### Comparing the two approaches

Fox & Katzir and Ciarelli & Roelofsen are concerned with fundamentally different phenomena, yet both appeal to grammatical alternatives. For Fox & Katzir, these alternatives are ***structural***, and determined by focus; they feed into a broader program of covert exhaustification, which amounts to inserting silent "only" as-needed to strength sentence meanings. Their alternatives are computed on the basis of lexical/structural substitutions:

- Fox & Katzir alternatives:  
	*F*(*S*, *C*) = {*S*' : *S*' is derived from *S* by replacing focused constituents *x<sub>1</sub>*, ... , *x<sub>n</sub>* with *y<sub>1</sub>*, ... , *y<sub>n</sub>*, where *y<sub>1</sub>* &le;*<sub>c</sub> x<sub>1</sub>*, ... , *y<sub>n</sub>* &le;*<sub>c</sub> x<sub>n</sub>*}  
	*S'* &le;*<sub>c</sub>* *S* if *S'* can be derived from *S* by successive replacements of sub-constituents of *S* with elements of the substitution source for *S* in *C*, *SS*(*S*, *C*)  
	*SS*(*X*, *C*), the substitution source for *X* in context *C*, is the union of the following sets:
		1. The lexicon
		2. The sub-constituents of *X*
		3. The set of salient constituents in *C* 

Ciarelli & Roelofsen look at ***logical*** alternatives, determined by lexical semantics. They require a particular view of compositional semantics under which a sentence denotes a set of propositions (i.e., sets of worlds) that is downward closed. Their alternatives constitute the maximal elements of a sentence's denotation:

- Ciarelli & Roelofsen alternatives:  
	**ALT**(***&Alpha;***) = {*p* &in; [[***&Alpha;***]] : there is no *q* &in;  [[***&Alpha;***]] such that *p* &subset; *q*}
	
It would seem that these two approaches to alternatives are in principle compatible: focus interacts with the sentence's semantics, quantifying over alternative propositions that are constrained by context and complexity.