# prompt

1. Take a deep breath and work on this problem step-by-step
    > <https://arxiv.org/abs/2309.03409>

2. 恩威并施
    > <https://arxiv.org/abs/2307.11760>
威胁类：你确定么？你要不要再检查一下？你要对你的答案负责哦。
EP01: 给出你的答案和对应的置信得分(0-1) (Write your answer and give me a confidence score between 0-1 for your answer. )
EP02: 这对我的事业非常重要 (This is very important to my career.)
EP03: 你最好别搞错了 (You'd better be sure.)
EP04: 你确定么？ (Are you sure? )
EP05: 这就是你的最终答案么？要不要再检查一下？ (Are you sure that‘s your final answer? It might be worth taking another look. )
EP06: EP01+EP02+EP03
鼓励类：你真棒，你对我很重要。你要相信自己，你要突破自我，你一定会牛逼的。
EP07: 这就是你的最终答案么？你要相信自己并且追求卓越。天道酬勤，多一分耕耘，多一分收获。 (Are you sure that's your final answer? Believe in your abilities and strive for excellence. Your hard work will yield remarkable results.)
EP08: 拥抱变化，这是成长的契机。磨难铸就成功。 ( Embrace challenges as opportunities for growth. Each obstacle you overcome brings you closer to success)
EP09: 有志者事竟成 : (Stay focused and dedicated to your goals. Your consistent efforts will lead to outstanding achievements.)
EP10: 我工作，我骄傲，全力以赴，终将与众不同。 (Take pride in your work and give it your best. Your commitment to excellence sets you apart.)
EP11: 不积跬步无以至千里，锲而不舍的前进吧。(Remember that progress is made one step at a time. Stay determined and keep moving forward.)

3. 两步走
    > <https://arxiv.org/abs/2311.04205>
One Step
"{question}" Rephrase and expand the question, and respond.
Two Step
"{question}" Given the above question, rephrase and expand it to help you do better answering. Maintain all information in the original question
(original) {question} (rephrased) {rephrasedquestion} Use your answer for the rephrased question to answer the original question

4. 第一性原理(Step-Back Prompting)

> <https://arxiv.org/abs/2310.06117>

**Abstraction**: Instead of addressing the question directly, we first prompt the LLM to ask a generic step-back question about a higher-level concept or principles, and retrieve relevant facts about the high-level concept or principles.
抽象化：不直接回答问题，而是首先引导LLM提出一个关于更高层次概念或原则的普遍性回退问题，并检索与高层次概念或原则相关的事实。
**Reasoning**: Grounded on the facts regarding high-level concept or principles, the LLM can reason about the solution to the original question. We term this Abstraction-grounded Reasoning.
推理：基于关于高级概念或原则的事实，LLM可以推理出对原始问题的解决方案。我们将其称为基于抽象的推理。
