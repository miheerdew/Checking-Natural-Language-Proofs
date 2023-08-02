# Checking Natural Language Proofs

The task of reviewing a natural language proof in mathematics can be difficult as it requires verifying numerous mental calculations. On the other hand, formal language proofs can automatically be verified by using computers. Can we use large language modelling (LLM) tools to verify that a natural langauge proof is correct? Such a system would be helpful to review mathematical papers, student homework, etc. The problem of checking proofs ought to be easier than the problem of automatic theorem proving. 

This also touches on an aspect that is of general importance for adaptation of A.I. : how do we build A.I. tools that we can trust? In our case, how can we trust that the verdict on proof/exam/homework provided by an LLM based system is indeed correct? The problem of checking natural langauge proofs could be a great play-ground to investigate this, as there is an objective/formal notion of whether a statement is true or not. 

One approach for checking natural lanaguge proofs could involve translating natural langauge proofs to formal langauge proofs. But  how do we trust that the translation is correct? The issue of trust can perhaps be addressed by creating a modular system in which the tranlation module is indepedently applied to different parts of the proof (e.g. Lemmas), and the end result combined and verified via the formal system. Further there could be a way for humans to randomly inspect parts of the system to see that it is functioning well (see [probabilistically Checkable proofs](https://en.wikipedia.org/wiki/Probabilistically_checkable_proof)). Finally, asking GPT to reproduce intermidiate steps in a proof it generates ([see this video](https://youtu.be/hJP5GqnTrNo?t=767)) has shown to improve its accuracy. We could do the same, and perhaps also verify the intermediate steps that it works out using the formal system?   

Also, how do we take the error messages from the formal lanaguge system and translate them back into natural language to explain why the proof is incorrect? 

## Subproblems

- [ ] Can we design a system that can find potential errors in a proof? For instance, we could start with system that just proof-reads english text (no mathematics). 
- [ ] Can we design a system to translate Natural Lanaguage proofs to Machine Language proof
- [ ] https://www.timeshighereducation.com/campus/simple-hack-chatgptproof-assignments-using-google-drive


# Relevant Resources 

1. [LeanDojo: Theorem Proving with Retrieval-Augmented Language Models](https://arxiv.org/pdf/2306.15626.pdf)
2. https://medium.com/@xiupp2005/integrating-chatgpt-with-proof-assistant-56a49347a549
3. https://proofassistants.stackexchange.com/questions/2053/make-chatgpt-write-formal-proof-from-natural-language-proof
4. https://github.com/princeton-nlp/NLProofS, https://arxiv.org/pdf/2205.12443v1.pdf
5. https://math.stackexchange.com/questions/403163/natural-language-proof-assistant
6. https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00503/113022/ProoFVer-Natural-Logic-Theorem-Proving-for-Fact
7. https://mathscholar.org/2023/02/can-chatgpt-prove-math-theorems/
8. https://arxiv.org/pdf/2301.13867.pdf

