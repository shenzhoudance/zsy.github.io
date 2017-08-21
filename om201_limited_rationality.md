### 怎样接球？
当篮球迎面飞来，你会怎样接球？如何保证飞来的篮球，都能被接住?和没有经过训练的普通人相比，那些有经验的运动员是如何接球？

### 超凡模型与接球

#### 1.超凡模型

超凡模型基于主观期望效用理论。认为存在全知全能的人类。

在篮球运动中，运动员需要接住空中的来球。如果把运动员替换为机器人，我们希望机器人能够完美得接住来球，那我们可以做哪些努力？我们可以尝试向机器人程序里，输入球的原始速率和角度，也许还要输入风力和风向，甚至要考虑到球的旋转。在完成这些输入后，我们期待机器人能够精确计算出落球的位置，并在恰当时间内，赶到那个位置，接住来球。完美的情况下，无论来球从哪个方向来，机器人每次都能接住来球。

这个拥有完美接球记录的机器人，遵循的便是**超凡模型**

#### 2.超凡模型的缺陷

**不存在无懈可击的归纳规律**。「任何一个看见过白天鹅的人，都不能保证下一次看到的天鹅不是黑的」。根据贝叶斯公式，在第一件事发生后，我们可以根据条件概率算出，在第一件事发生后的基础上第二件事的概率，然后这种概率性的陈述，却永远没办法保证，第二件事一定会发生。「构成归纳之基础的事件，通常需要借助某些工具，而这些工具本身却出处隐含着理论假设」。任何一台显微镜都包含着最基本的光学原理。

**「是什么」无法得到「应该如何」**。「尽管理性是我们在探寻实现目标的响应手段时的强大工具，但它却无法对目标本身提供任何帮助。」这点在人工智能上体现尤为突出。讨论人工智能是什么并没有给计算机科学带来巨大进步，而注重操作主义的图灵却发明了「图灵测试」，让一位象棋对手对阵另一位「选手」，在比赛结束后，人们才发现另一外「选手」居然是台电脑。图灵由此开创了「人工智能应该如何」的先例。生活这样的案例也随处可见。当年你走进美术馆，想体验「什么是油画」时，最终往往会被淹没在琳琅满目的画作之中，然后给自己一个简单的结论，「油画就是很多颜色的画」。而当你在美术馆看到一位认真专注的临摹者，且这位临摹者使用的工具居然不是油画笔，而是十五块一支的多色圆珠笔，你就会明白「油画原来可以用圆珠笔临摹」。

**哥德尔不完备性**。「一个逻辑体系无论多么完善，总会存在某些命题，仅仅通过对输入项的合理变换无法得出最终结果。」

「如何我们用理性来探寻和选择行动方案，那么有关输入项至少应该包括：一组“应该怎样”的命题或欲实现的价值，一组“是什么”的命题或关于拟采取行动所处环境的基本事实。」「任何试图用“逻辑”来判断“应该怎样”和“是什么”命题的合理性的尝试，必然会重新回到一组新的“应该怎样”和“是什么”的命题。」


### 行为模型与接球

#### 1.篮球与行为模型

与超凡模型的接球方法不同，行为模型团队认为，即使再出色的篮球运动员，也不会先练习风速/作用力/角度等物理问题后，再去打球。当你再回到那个接球的场景中，你会发现现实中，这个完美的机器人并没有被制造出来。球场上能够接住球的，还是那些被层层挑选出来的人类。

行为模型团队注意到，那些出色的篮球远动员，进行的各种接球练习可以大约总结为，保持跑动，以便他们的眼睛与篮球的角度保持恒定。在恒定的角度下，接球就变得容易得多。

行为模型团队开发的机器人被编制的变量只有两个，保持跑动与保持机器人与篮球角度恒定。剩下的就交给运气。知识与计算的有限性未必是一种缺陷。
 
工具可能是简单的，但在特定的范围内，却是有效的。企图完美分析出各种变量的程度，也许只能一直停留在分析阶段，却永远都接不球。并不存在使用于所有情境的万能魔法锤。但简捷性能保证做出快速、节俭和准确的决策


#### 2.寂寥世界（a nearly empty world）

西蒙說「即便在信息爆炸的今天，我们依然生活在一个寂寥世界 。我们生活的世界或许可以称为寂寥世界：它有着数百万个变量，它们在理论上可以相互影响，但在现实生活的绝大多数情形中则不会。」

正如虽然万物之间都存在相互牵引，而有些物体的牵引总比其他物体大得多。但我们并不会被空气拖入天空，却会被地心固定于地面。就像，我们在做决策时，虽然理论上万事万物都对决策产生影响，但真正能产生效果的却只有寥寥几个。

### 什么是有限理性

#### 1.有限理性的工作机制

「为了在有限制的现实社会中采取切合实际的行动，一个生物体需要通过某种方式来集中注意力，以避免过于分心，并在特定时间里把注意力集中到需要高度关注的事情上。」

**冷认知与热认知（情感的作用）**新手在解决问题过程中，搜索往往是沉闷而缓慢的，相对不容易激发强烈的情感，可称之为“冷认知”；而专家在解决问题时，由于相对熟悉环境，往往容易唤起情况的共鸣，它是一种“热认知”。

为了在有限制的现实社会中采取切合实际的行动，较优的方法便是，把注意力集中到需要高度关注的事情上。 而将注意力集中的最理想工具是，情感。
 
“热认知”与情感密切相关。「情感的功能，是我们所处的环境中选择出特定对象，作为我们关注的目标」。「情感一旦被激发出来就不会消失，且之道某种介入之前，人们不会转而关注其他问题。」情感有时候会使得有关问题，成为我们脑海中挥之不去的烦恼，但也能激发我们解决问题的灵感。

大多数学习者在情感强烈的状态下，专注时间更长，且思考程度更深。在研究军事社会学论著时，《战争与和平》可能比普通论著更容易让学习者留下深刻持久的印象。当然，值得注意的是，采用富有情感的人文书籍进行学习时，也要重视它们在科学上的可靠性，二者缺一不可。

  
**替代性选择机制**很多问题并不能被理想得解决，我们在分解问题的过程中，很大一部分时间是花在寻找更好的替代方案。

比如，在人工智能科学中，为了模拟人类大脑识别文字的过程，科学家并没有完全分析透彻神经回路结构。相反，他们将识别文字过程，简化为识别笔划过程，机器只要识别了一个字母中的特征性笔画，就能计算出，这个字母可能是B或D或O的概率，然后按照最大可能概率，给出识别结果。
  
**根据真实情况进一步推论**「这种能力有助于人们简化与当前决策有关环境的认识，进而进行常识性推理」。

花费大量精力寻找替代方案的过程中，我们不仅搜索已存在的真实信息，更多得还要根据这些信息，来推论，或者说想象，我们可以用这些信息达到什么目标。这种推论或者想象的能力，是为了让大脑做减法，简化那些陌生的场景。而正由于，我们执行的动作是推论或想象，我们能预估的后果，始终是有限制的。

#### 2.有限理性的定义

西蒙首创了“有限理性“这个术语，并首次使用一把剪刀来比喻有限理性，它的一个刀片是现实人类的”认知局限性“，另一个刀片是”环境结构“。
头脑只有有限的时间、知识和其他资源，但它能够通过利用环境结构而获得成功。 仅仅研究一个刀片是不够的，两个刀片联动才能裁剪东西。

**有限理性的原因**西蒙說「首先，你的决策不是生活中广泛领域的问题的综合性选择，而是通常关注某些特定的具体事件」。比如在买车时，你看你会考虑到车的排量，配置，型号等因素，也会考虑到家中孩子数量，需要购置小型或中型的车。但你很可能不会再考虑，买这辆车对明年的家庭理财计划是否有影响，或者这辆车后续维护费用等。

西蒙說「其次，当你进行某一具体决策时，无论它有多么重要，你都不可能对它在未来的具体详情了然于胸」对于你的生活方式和未来境况，你了解的不过是一个大致的概貌，也许不久会发生一两项重大改变，甚至会出现一些突发情况。诚如上述所言，你在考虑是否购买一辆汽车时，你只是对汽车的用途、你的收入水平、其它要求以及是否考虑在另一个城市找一份新工作等，有一个大致的概念。但你不可能预见到每一种可能性。

西蒙說「不同领域的决策会唤起不同的价值观，而关注点的变化则会使得选择出现很大的不一致性。」比如，在买车前，你可能沉浸在自驾游的美好设想里，却不忽略了你也可以用购车款带全家出国旅行也能创造美好回忆的可能。西蒙說「最后，你为购买汽车决策所付出的所有努力，大部分将耗费在了解现实情况、唤起相关价值观等方面，而实际选择也许只需花费一点点时间而已。」

### 直觉模型

「直觉模型认为，人们得以正确决策的原因，主要在于拥有良好的直觉或判断力。」简洁优美得解决问题，依靠的是理性分析，还是创造性直觉？「人类思维是否具有分析性思维和直觉性思维两种完全不同的方式？我们所谓的创造力，是否主要取决于后者？」

#### 1.左脑与右脑（直觉模型的传统研究角度）

  人们曾经从大脑功能定位角度分析，人类解决问题到底依靠何种思维。比较流行的一种说法是「左脑与右脑理论」。「大脑左侧善于分析，但迟缓平淡，缺乏想象力。左侧大脑的推理类似行为模型模式。」「右脑是人类储存想象力和创造力的地方。」

虽然，有很多证据表明大脑半球存在分工，「但没有任何证据表明，任何一个大脑半球能够在正常情况下独立完成人类任何复杂的智力活动。」大部分证据表明，任何包含着获取信息、处理信息和利用信息的复杂思维活动，通常都会按照不同的比例和不同的方式，同时用到我们的两个大脑半球。」

相比于大脑功能定位角度，社会学家更倾向于用直觉性思维来讨论「直觉」或「创造力」。 
  
#### 2.直觉与识别（直觉模型的现代研究角度）

  「什么是直觉?一种常见的现象是，有时候人们会忽然想到问题的答案，从而拥有一种强烈程度各异的“啊哈！”经验。」

国际象棋大师，在看到棋局的五秒或十秒后，已经拥有第一冲动的走法。虽然，他不会立即就走出这一步，可能还需要十分钟或半小时去确认，一般而言，这第一冲动的走法80%情况下，的确是最优方案。象棋大师能够拥有第一冲动的最优方案，在于他已经能够「识别」上万棋局的经验。
  正如每个行业的专家，在成为专家的过程中，他们对本专业的术语已经积累了大量丰富的经验。很多局面对他们而言就像老朋友一样熟悉。因此，正如你会判断你的老朋友是否值得你借钱给他一样简单，专家也能轻松判断其专业内，某个局面应该如何掌控。
  
#### 3.直觉模型与行为模型

行为模型类似于搜索过程，被大量陌生所包围，其过程是痛苦而缓慢的；直觉模型类似于识别过程，周遭都是熟悉事物，其识别过程不仅迅速且准确。 新手的痛苦在于，「专家接住直觉就可以解决问题，新手往往需要经历一种痛苦的搜索过程。」 这是因为，专家在过去的搜索中，已积累了大量知识。而我们也要意识到，「绝大多数的问题，既包括新奇的成分又包括书写的方面，其解决有赖于直觉和搜索的合作。」


### 最优与满意

#### 1.有限理性的三个模型

**超凡模型**「它假定天地之间有一个进行综合性决策的英雄式人物」「超凡模型也许是上帝的思考方式，但确实不宜视为人类的思考模式。」
  
**行为模型**「它假设人类理性是一种非常有限的理性，深受有关境遇和人类计算能力的限制。」 行为模型解释了，「人类作为拥有有限计算能力的生物体，在面对复杂又寂寥的世界中」，如何做出适应性选择，并得以成功生存的理论。
  
**直觉模型**直觉模型强调的是，「人类的技能是通过经验积累和识别而获得的」，并且在积累经验过程中，人类情感将帮助人们将注意力集中于特定的问题上。

#### 2.最优与满意
最优，是指选择所有可能行动方案中的绝对最佳方案，抑或是指选择给定信息条件下我能够确定的最佳方案。

满意，却是局部的最优。