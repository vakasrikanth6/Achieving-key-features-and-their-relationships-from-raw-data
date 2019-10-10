# Achieving-key-features-and-their-relationships-fromm-raw-data

For example, if we have requirements of huge rows regarding bank payment data we can fairly assume that the clusters formed might be a group of descriptors talking about a specific mode of payment, One such cluster maybe a “credit card” cluster. This cluster which is taking about credit-card is one of the functionality of a requirement specification which can be further mined for features. Having this idea in mind, we create an approach which can mine for features in these clusters thereby extracting good set of features.We achieve this tasks with the help of NLTK libraries and POStags

we know a descriptor is nothing but a sentence containing a set of words and relations between words from our data, we take this descriptors and we classify the words of them as to which parts of speech they belong to. Likewise, we do it for all the words of a sentence, all the sentences of a cluster and for all the clusters formed from our clustering process. We make use of the following Parts of speech tags

[NN] Noun,
[NNP] Proper Noun,
[JJ] Adjective,
[VB] Verb,
[CC] Coordinating conjunction RB Adverb ,
[CD] Cardinal number NNS Noun plural, 
[DT] Determiner PDT Predeterminer,
[IN]Preposition or conjunction NNP Proper noun, singular
[JJ]Adjective VB Verb, base form
[MD] Modal verb VBG Verb, gerund, participle
[NN] Noun, singular or mass VBN Verb, past participle.



This approach is formulated keeping in mind how a human might extract certain features from a set of sentences when he reads it. If a paragraph is given to an individual to read and formulate a one line summary, the indicidual often carries his task by collecting information regarding each and ever sentence as he reads through. The brain collectively organizes the important keywords and key phrases which it reads on the flow, and once after completion of the whole paragraphs, the brain tends to mix those important words and formulate a sentence to give a one line summary. Keeping this approach in mind we tend to treat each clusters as a paragraph and thereby focus on extracting important words from these clusters which defines the characteristics or properties of this cluster and also defines certain additional features present in them. The one keyword which can define the whole cluster can act as a root node also termed as a abstract feature and the other extracted keywords which are termed important and also add value to the cluster can act as their child nodes also termed as features. Using the parts of speech tag and named entity approach we achieve all of these tasks. Few of the POStags used in our work is defined as follows

• Noun pairs[NN-NN] • Adjective-Noun pairs[JJ-NN] • Nouns[NN] • Proper-nouns[NNP] • Combination of noun and adjective pairs [NN-JJ]
