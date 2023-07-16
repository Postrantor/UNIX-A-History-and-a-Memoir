---
tip: translate by openai@2023-07-14 17:09:31
...

## **Preface**

"One of the comforting things about old memories is their tendency to take on a rosy glow. The memory fixes on what was good and what lasted, and on the joy of helping to create the improvements that made life better."

> "回忆让人宽慰的一点是它们往往会带着一种玫瑰色的光芒。记忆会停留在好的事情和持久的事情上，以及帮助创造让生活变得更好的改善的喜悦上。"

Dennis Ritchie, "The Evolution of the Unix Time-sharing System,"

October 1984

Since its creation in a Bell Labs attic in 1969, the Unix operating system has spread far beyond anything that its creators could possibly have imagined. It has led to the development of much innovative software, influenced myriad programmers, and changed the entire path of computer technology.

> 自 1969 年在贝尔实验室阁楼里创建以来，Unix 操作系统已经远远超出了其创造者所能想象的范围。它促进了许多创新软件的开发，影响了无数程序员，改变了整个计算机技术的发展道路。

Unix and its derivatives aren't widely known outside a particular technical community, but they are at the heart of any number of systems that are part of everyone's world. Google, Facebook, Amazon, and plenty of other services are powered by Linux, a Unix-like operating system that I'll talk about later on. If you have a cell phone or have a Mac, it runs some version of Unix. If you have gadgets like Alexa at home or navigation software in your car, they're powered by Unix-like systems too. If you're bombarded by advertising whenever you browse the web, Unix systems are behind it, and of course the tracking that knows what you're doing so you can be more accurately bombarded is likely to be based on Unix as well.

> Unix 及其衍生物并不为特定的技术社区所熟知，但它们是每个人的世界中任何数量系统的核心。谷歌、Facebook、亚马逊等大量服务都由 Linux(一种类 Unix 的操作系统，稍后会讨论)提供支持。如果你有手机或 Mac，它们都运行某种版本的 Unix。如果你家里有 Alexa 这类设备或车载导航软件，它们也是由类 Unix 系统提供支持。如果你在浏览网页时被广告轰炸，Unix 系统就在背后，当然，知道你在做什么，以便更精确地轰炸你的跟踪也很可能基于 Unix。

Unix was created more than 50 years ago by two people, along with a small group of collaborators and camp followers. Through a sequence of lucky accidents, I was present at the creation, though certainly not responsible for any of it. At most I can take credit for a modest amount of useful software and, thanks to first-rate co-authors, some books that have helped

> Unix 在 50 多年前由两个人以及一小群合作者和追随者创建。通过一系列的幸运的意外，我出席了有关创造的活动，尽管自己绝不能为此负责。我最多可以为一些有用的软件和几本由一流的合作作者共同撰写的书籍获得一点荣誉，这些书籍也帮助了很多人。

## PREFACE

people to learn more about Unix and its languages, tools and philosophy.

This book is part history and part memoir, a look at the origins of Unix and an attempt to explain what Unix is, how it came about, and why it matters. The book is certainly not a scholarly work, however---there are no footnotes---and it has become less history and more memoir than I had originally planned.

> 这本书既是历史，又是回忆录，它**探索了 Unix 的起源，试图解释 Unix 是什么、它是如何产生的，以及它为什么重要**。当然，这本书不是学术著作——没有脚注——它比我最初计划的更多的是回忆录，而不是历史。

The book is written for anyone with an interest in computing or the history of inventions. It includes a certain amount of technical material, but I've tried to provide sufficient explanation that even if you don't hav e much background, you can appreciate the basic ideas and see why they might be important. You can safely skip over anything that seems too complicated, however, so there's no need to read every word. If you are a programmer, some of the explanations may seem pretty obvious and over-simplified, but with luck some of the historical insights will be useful, and the stories that go with it might be new and interesting to you.

> 这本书是为所有对计算机或发明史感兴趣的人编写的。它包含了一定数量的技术材料，但我已尽力提供足够的解释，即使您没有太多背景知识，您也可以理解基本的想法，并看到它们为什么可能很重要。但是，您可以安全地跳过任何似乎太复杂的内容，因此没有必要阅读每一个字。如果您是程序员，那么一些解释可能会显得很明显，而且过于简单化，但希望其中的一些历史见解会有所帮助，而且伴随的故事可能对您来说是新鲜有趣的。

Although I have tried to be accurate, there are sure to be places where my memory is imperfect. Furthermore, the interviews, personal reminiscences, oral histories, books and papers that I've relied on are not always consistent with my own memories or with each other in their accounts of who did what and when.

> 尽管我努力做到准确，但肯定会有我的记忆不完善的地方。此外，我所依赖的采访、个人回忆、口述历史、书籍和文件，并不总是与我自己的记忆或彼此的记载(关于谁做了什么以及何时)一致。

Fortunately, many of those involved in the early days are still alive and have helped to straighten me out. They too may suffer from memory lapses and rose-colored glasses but any errors that remain are my fault, at least until I can safely blame them on someone else.

> 幸运的是，参与早期工作的许多人仍然健在，他们帮助我把事情弄清楚。他们也可能有记忆缺漏和美化的倾向，但是任何错误都是我的错，至少在我可以安全地将责任归咎于其他人之前是我的错。

My main purpose in writing is to tell some of the wonderful stories of an especially productive and formative time in the history of computing. It's important to understand the evolution of the technology that we use and take for granted. The decisions that shaped how that technology developed and thus defined the paths that we took were made by real people, working under the pressures and constraints of the time. The more we know about the history, the more we can appreciate the inventive genius that led to Unix and perhaps better understand why modern computer systems are as they are. If nothing else, choices that might seem wrong-headed or perverse today can often be seen as natural consequences of what was understood and could be accomplished with the resources available at the time.

> 我写作的主要目的是讲述一些关于计算机历史中特别富有成果和形成性的时期的精彩故事。了解我们使用和认为理所当然的技术的演变是很重要的。影响技术发展并定义我们所走的路径的决定是由当时承受着压力和限制的真实的人们做出的。我们了解的历史越多，我们就越能够欣赏到导致 Unix 的发明天才，也许能够更好地理解为什么现代计算机系统是如此。如果没有其他的选择，今天看起来有些错误或变态的选择往往可以被看作是当时可以理解和实现的资源的自然结果。

The story is about more than just the Unix operating system, though that's the core. It also includes the C programming language, one of the most widely used of all languages, and at the heart of the systems that run the Internet and the services that use it. Other languages began life at Bell Labs with Unix too, notably C++, which is also widely used. Microsoft Office tools like Word, Excel or Powerpoint are written in C++, as are most of the browsers you might be using. A dozen or two of the core tools that programmers use daily and simply take for granted were written in the early days of Unix and are still part of every programmer's toolkit, often much the same as they were 40 or 50 years ago.

> 故事不仅仅是关于 Unix 操作系统，尽管这是核心内容。它还包括 C 编程语言，这是最广泛使用的语言之一，也是运行互联网和使用它的服务的系统的核心。其他语言也在贝尔实验室的 Unix 系统上诞生，特别是 C++，它也被广泛使用。微软办公套件也是如此，Word、Excel 或 Powerpoint 等工具都是用 C++编写的，大多数你正在使用的浏览器也是如此。在 Unix 早期编写的十几个或二十个核心工具，现在仍然是程序员每天都会使用的工具，而且和 40 或 50 年前的情况几乎一样。

Computer science theory plays a vital role as well, often enabling immensely practical tools. Hardware research explored design tools, integrated circuits, computer architecture, and unusual special-purpose devices.

> 计算机科学理论也起着至关重要的作用，往往可以提供非常实用的工具。硬件研究探索了设计工具、集成电路、计算机体系结构和特殊用途的设备。

The interplay among all of these activities often led to unexpected inventions, and was one of the reasons why the whole enterprise was so productive across so many different fields.

> 所有这些活动之间的相互作用经常会导致意想不到的发明，这也是为什么整个企业在许多不同领域都如此高效率的原因之一。

There is also an interesting and relevant story about how technological innovation happens. Bell Labs, where Unix began, was a remarkable institution that produced many good ideas and capitalized on them. It was the origin of many world-changing inventions, and there are lessons to be learned from how it worked.

> 也有一个有趣而相关的故事，讲述了技术创新是如何发生的。Unix 开始的贝尔实验室是一个了不起的机构，它产生了许多好的想法，并利用了它们。它是许多世界变革性发明的起源，我们可以从它的工作方式中学习到很多东西。

The Unix story certainly offers many insights into how to design and build software, and how to use computers effectively, which I have tried to highlight along the way. As a simple but characteristic example, the Unix philosophy of software tools made it possible to combine existing programs to accomplish a wide variety of tasks without having to write new software.

> Unix 的故事无疑提供了许多关于如何设计和构建软件以及如何有效使用计算机的见解，我在此过程中也尝试着强调了这些。作为一个简单但具有特色的例子，Unix 软件工具的哲学使得可以结合现有的程序完成各种任务，而无需编写新的软件。

It's a programming instance of an old strategy: divide and conquer. By breaking bigger tasks into smaller ones, each one becomes more manageable, and the pieces can be combined in unexpected ways.

> 这是**一个古老策略的编程实例：分而治之**。通过将大任务分解成更小的任务，每个任务都变得更容易管理，而这些部分可以以意想不到的方式组合起来。

Finally, although Unix was the most visible software from Bell Labs, it was by no means the only contribution to computing. The Computing Science Research Center, the fabled "Center 1127," or just "1127," was unusually productive for two or three decades. Its work was inspired by Unix and used Unix as a base, but the contributions go well beyond that. Members of 1127 wrote important books that for years have been core texts in computer science and references for programmers. Center 1127 was an exceptionally influential industrial computer science research laboratory, one of the most productive of comparably sized groups at the time or subsequently.

> 最后，尽管 Unix 是贝尔实验室最引人注目的软件，但它绝不是唯一对计算机有贡献的软件。著名的“1127 中心”或“1127”的计算科学研究中心在二三十年间表现异常活跃。它的工作受 Unix 启发，并以 Unix 为基础，但其贡献远远超出此。1127 中心的成员编写了重要的书籍，这些书籍多年来一直是计算机科学的核心教科书，也是程序员的参考资料。1127 中心是一个极具影响力的工业计算机科学研究实验室，是当时或随后同规模小组中最富有成效的之一。

Why was Unix and the surrounding environment so successful? How did a two-person experiment grow into something that literally changed the world? Was this a singular event, so unlikely that nothing like it could ever happen again? On the larger question of whether such influential results can be planned, I'll say more at the end of the book. For now, it seems to me that Unix owes its success to an accidental combination of factors: two exceptional people, an excellent supporting cast, talented and enlightened management, stable funding in a corporation that took a very long view, and an unfettered environment for exploration no matter how unconventional. Its adoption was facilitated by rapidly advancing technology where hardware kept getting smaller, cheaper and faster at an exponential rate.

> 为什么 Unix 及其周边环境如此成功？两个人的实验如何发展成改变世界的东西？这是一个特殊的事件，如此不可能再次发生？就这样影响深远的结果是否可以计划的更大问题，我将在本书末尾说明。到目前为止，Unix 似乎要归功于一个意外的组合因素：两个杰出的人，一个出色的支持团队，有才华和开明的人。
> 管理、在一家公司里提供稳定的资金，以及一个不受限制的探索环境，无论多么不寻常。随着硬件越来越小、越来越便宜且速度越来越快，以指数率增长，它的采用得到了促进。

The early years of Unix were for me and many others at Bell Labs won-drously productive and fun. I hope that this book will help you sense some of the joy of creation, and indeed of making life better, that Dennis Ritchie described in the epigraph above.

> 早期的 Unix 对我和贝尔实验室的许多其他人来说是一段神奇的、富有成效的乐趣时光。我希望本书能帮助你感受到丹尼斯·里奇在上面引文中所描述的创造的喜悦，乃至改善生活的喜悦。

## **Acknowledgments**

One of the unexpected pleasures of writing this book has been to reconnect with so many friends and colleagues, who have generously shared their memories and some great stories. It is hard to express just how valuable that has been. I hav en't been able to include all of the stories, but I have greatly enjoyed hearing them, and I am in debt to the many remarkable people that I have been fortunate enough to work with.

> 一写这本书的意外乐趣之一，是重新与许多朋友和同事联系起来，他们慷慨地分享了他们的回忆和一些很棒的故事。很难表达这有多么宝贵。我没有能够包括所有的故事，但我非常喜欢听到它们，我感激我幸运能够与许多杰出的人一起工作。

Biographical material is scattered throughout the book, with major sections on the three main people without whom Unix would not have happened---Ken Thompson, Dennis Ritchie and Doug McIlroy. Ken and Doug have provided invaluable feedback on the book, though they are in no way responsible for anything I've gotten wrong or inadvertently misrepresented. I have also received valuable comments and suggestions from Dennis's brothers John and Bill; his nephew Sam provided detailed comments on several drafts.

> 在书中散布着传记资料，关于没有哪三个主要人物就不可能有 Unix 的发生——肯·汤普森、丹尼斯·里奇和道格·麦克尔罗伊。肯和道格对这本书提供了宝贵的反馈，尽管他们并不对我所犯的任何错误或无意中曲解的内容负责。我也从丹尼斯的兄弟约翰和比尔那里收到宝贵的意见和建议；他的侄子山姆对几个草稿提供了详细的意见。

As he has done so many times before, Jon Bentley gav e me invaluable insights, helpful suggestions for organization and emphasis, numerous anec-dotes, and detailed comments on writing, over at least half a dozen drafts. I am enormously indebted to Jon once again.

> 当他像以前那样做了很多次之后，乔恩·本特利给了我宝贵的见解、有用的组织和重点建议、许多轶事以及对写作的详细评论，至少超过六个草稿。我再次深深地感谢乔恩。

Gerard Holzmann provided advice, archival material and many original photographs that have helped to make the book more visually interesting.

> Gerard Holzmann 提供的建议、档案资料和许多原始照片有助于使这本书变得更加有视觉吸引力。

Paul Kernighan read multiple drafts and spotted myriad typos. He also suggested some excellent titles, though in the end I regretfully decided not to use _A History of the Unix-speaking Peoples._

> 保罗·克尔尼根阅读了多份草稿，发现了众多错别字。他还提出了一些很棒的标题，但最后我遗憾地决定不使用《Unix 说话民族的历史》。

Al Aho, Mike Bianchi, Stu Feldman, Steve Johnson, Michael Lesk, John Linderman, John Mashey, Peter Neumann, Rob Pike, Howard Trickey and Peter Weinberger provided critical reading and stories of early Unix days, many of which I have quoted or paraphrased.

> 阿霍、迈克·比安奇、斯图·费尔德曼、史蒂夫·约翰逊、迈克尔·莱斯克、约翰·林德曼、约翰·马谢伊、彼得·纽曼、罗布·派克、霍华德·特里基和彼得·温伯格提供了关于早期 Unix 时代的关键阅读和故事，我引用或改写了其中许多。

I also received many helpful comments and other contributions from Michael Bachand, David Brock, Grace Emlin, Maia Hamin, Bill Joy, Mark Kernighan, Meg Kernighan, William McGrath, Peter McIlroy, Arnold Robbins, Jonah Sinowitz, Bjarne Stroustrup, Warren Toomey and Janet Vertesi.

> 我还从 Michael Bachand、David Brock、Grace Emlin、Maia Hamin、Bill Joy、Mark Kernighan、Meg Kernighan、William McGrath、Peter McIlroy、Arnold Robbins、Jonah Sinowitz、Bjarne Stroustrup、Warren Toomey 和 Janet Vertesi 那里得到了许多有用的评论和其他贡献。

I am deeply grateful for all of the generous assistance, but I am responsible for any errors or misinterpretations. Many other people have contributed to Unix in important ways over the past fifty years, and I apologize to anyone whose work has been slighted.

> 我深深感谢所有慷慨的帮助，但我对任何错误或误解负有责任。在过去的五十年里，许多其他人为 Unix 做出了重要贡献，我向任何受到轻视的人表示歉意。

# Chapter 1

**Bell Labs**

"One Policy, One System, Universal Service"

AT&T's mission statement, 1907

"At first sight, when one comes upon it in its surprisingly rural setting, the Bell Telephone Laboratories' main New Jersey site looks like a large and up-to-date factory, which in a sense it is. But it is a factory for ideas, and so its production lines are invisible."

> 当人们第一次看到它，它位于意想不到的乡村环境中，贝尔电话实验室的新泽西主要地点看上去像一个大型现代化的工厂，从某种意义上来说，它是一个工厂。但它是一个创意工厂，因此它的生产线是看不见的。

Arthur Clarke, _Voice Across the Sea_, 1974

quoted in _The Idea Factory_ by Jon Gertner, 2012

To understand how Unix happened, we have to understand Bell Labs, especially how it worked and the creative environment that it provided.

> 要了解 Unix 是如何发生的，我们必须了解贝尔实验室，特别是它的工作方式和它提供的创造性环境。

AT&T, the American Telephone and Telegraph Company, grew out of combining a host of local telephone companies from across the United States. Early in its history, AT&T realized that it needed a research organization that would systematically address the scientific and engineering problems that the company encountered as it tried to provide a national telephone system. In 1925, it created a research and development subsidiary, Bell Telephone Laboratories, to attack these problems. Although the full name was regularly abbreviated to Bell Labs or BTL or merely "the Labs," telephony was always the central concern.

> AT&T，美国电话电报公司，源于美国各地的当地电话公司的合并。早期，AT&T 意识到它需要一个研究机构，可以系统地解决该公司在尝试提供全国电话系统时遇到的科学和工程问题。1925 年，它成立了一家研发子公司，贝尔电话实验室，来解决这些问题。尽管全称经常被缩写为贝尔实验室或 BTL 或仅仅“实验室”，但电话业务始终是核心关注点。

Bell Labs was originally located at 463 West Street in New York City, but at the beginning of the Second World War, many of its activities moved out of New York. AT&T was heavily involved in the war effort, providing expertise on a wide variety of important military problems---communications systems, of course, but also fire-control computers for anti-aircraft guns, radar, and cryptography. Part of this work was done in suburban and rural New

> 贝尔实验室最初位于纽约市西街 463 号，但在第二次世界大战开始时，许多活动都离开了纽约。 AT＆T 在战争中发挥了重要作用，为各种重要的军事问题提供专业知识-当然是通信系统，但还有防空炮的火控计算机，雷达和密码学。其中一部分工作是在郊区和农村完成的。

> []{#index_split_000.html#p16}![](./index-16_1.jpg){.calibre4}
> **Figure 1.1:** From New York City to Murray Hill, New Jersey

Jersey, 20 miles (33 km) west of New York. The largest site was in an area called Murray Hill, which was part of the small towns of New Providence and Berkeley Heights.

> 纽泽西，距纽约西部 20 英里(33 公里)。最大的遗址位于一个叫墨里山的地方，这是新普罗维登斯和伯克利高地的一部分。

Figure 1.1 shows the general lay of the land; 463 West Street is on the Hudson River, a short distance north of the 9A highway marker. Bell Labs at Murray Hill straddles the boundary between New Providence and Berkeley Heights, just north of Interstate 78. Both locations are marked on the map with dots.

> 图 1.1 显示了地形的大致样子；463 西街位于哈德逊河北边，距离 9A 公路标志不远。Murray Hill 的贝尔实验室位于新普罗维登斯和伯克利高地之间的边界上，位于 78 号州际公路北边。两个地点都标有点。

More and more Bell Labs activities shifted to Murray Hill, and the Labs left West Street entirely in 1966. By the 1960s, Murray Hill housed over 3,000 people, at least 1,000 with PhDs in technical fields like physics, chemistry, mathematics, and various flavors of engineering.

> 随着越来越多的贝尔实验室活动转移到默里山，1966 年实验室完全离开了西街。到 1960 年代，默里山已经容纳了 3000 多人，至少有 1000 人拥有物理、化学、数学和各种工程学科的博士学位。

Figure 1.2 is an aerial photo of the Murray Hill complex in 1961. There were three main buildings. Building 1 is to the lower right in the picture, 2 is to the upper left, and 3 is the square one with an open courtyard. Before it was blocked by the addition of two new buildings in the 1970s, there was a single uninterrupted quarter-mile (400 m) corridor from one end of Building 1 to the other end of Building 2.

> 图 1.2 是 1961 年莫里山综合体的一张航拍照片。有三栋主要建筑。建筑 1 位于图片的右下角，2 位于左上角，3 是一座带有开放庭院的正方形建筑。在 1970 年代新增加的两栋建筑封堵之前，从建筑 1 的一端到建筑 2 的另一端有一条长达四分之一英里(400 米)的连续走廊。

I spent over 30 years in Building 2, from an internship in 1967 until I retired in 2000. My offices were in the side wings marked with dots, on the fifth (top) floor. For future reference, Stair 9 in this picture is at the absolute far end of Building 2, and Stair 8 is one wing closer to the center. For most of the early years, the Unix room was in the sixth floor attic between stairways 8 and 9.

> 我在 2 号楼待了 30 多年，从 1967 年的实习开始到 2000 年退休。我的办公室在标有点的侧翼，在五楼(顶层)。供将来参考，这张图片中的 9 号楼梯位于 2 号楼的最远端，8 号楼梯更靠近中心。在早期的大部分时间里，Unix 室位于八号楼梯和九号楼梯之间的六楼阁楼里。

Figure 1.3 shows a Google satellite image of Bell Labs in 2019. Buildings 6 (towards the lower left, with the marker) and 7 (towards the upper right) were added in the early 1970s, and for some years after 1996, Building 6 was the headquarters of Lucent Technologies. It's intriguing how much corporate history is captured in the labels that Google has assigned: "Bell Labs" as a marker, Lucent Bell Labs on the exit driveway, Alcatel-Lucent Bell Labs on the entry, and Nokia Bell Labs at the apex of the managerial pyramid in Building 6.

> 图 1.3 显示了 2019 年谷歌卫星图像中的贝尔实验室。 楼 6(朝左下方，标记)和 7(朝右上方)是在 1970 年代初建成的，1996 年之后的一些年，楼 6 是路华科技的总部。 谷歌分配的标签所捕获的公司历史令人着迷：“贝尔实验室”作为标记，路华贝尔实验室在出口车道上，阿尔卡特朗讯贝尔实验室在入口处，诺基亚贝尔实验室位于楼 6 的管理顶峰。

I'm not qualified to write a detailed history of the Labs, but fortunately that's already been done well by other writers. I particularly like Jon Gertner's _The Idea Factory_, which focuses on the physical sciences, and James Gleick's _The Information_ is excellent for information science. The volumi-nous (seven volumes and nearly 5,000 pages) official Bell Labs publication called _A History of Science and Engineering in the Bell System_ is thorough, authoritative, and in my sampling, always interesting.

> 我没有资格写一部详细的实验室历史，但幸运的是，这已经被其他作家写得很好。我特别喜欢乔恩·格特纳(Jon Gertner)的《理念工厂》，专注于物理科学，而詹姆斯·格里克(James Gleick)的《信息》(The Information)对信息科学非常出色。由贝尔实验室(Bell Labs)出版的 7 卷近 5000 页的官方出版物《贝尔系统科学与工程史》(A History of Science and Engineering in the Bell System)详尽、权威，我抽样看来总是很有趣。

> []{#index_split_000.html#p18}![](./index-18_1.jpg){.calibre4}
> **Figure 1.2:** Bell Labs in 1961 (Courtesy of Bell Labs)

## **1.1 Physical sciences at Bell Labs**

During its early years, most research at Bell Labs involved physics, chemistry, materials, and communications systems. Researchers had exceptional freedom to pursue their own interests, but the environment was so rich in relevant problems that it wasn't hard to explore in areas that were both scientifi-cally interesting and potentially useful to the Bell System and to the world at large.

> 在其早期，贝尔实验室的大部分研究都涉及物理学、化学、材料和通信系统。研究人员拥有追求自己兴趣的非凡自由，但这个环境富含相关问题，所以在既具有科学意义又可能对贝尔系统和整个世界有益的领域进行探索并不困难。

Bell Labs was responsible for a remarkable number of scientific and technological advances that changed the world. Foremost among them was the transistor, inv ented in 1947 by John Bardeen, Walter Brattain and William Shockley, who were trying to improve amplifiers for long-distance telephone circuits. The transistor resulted from fundamental research into the properties of semiconductor materials, driven by a need for devices that would be more physically robust and less energy-hungry than vacuum tubes, which in the 1940s were the only way to make communications equipment and, incidentally, to build the earliest computers.

> 贝尔实验室为世界发生巨大变化的许多科学技术进步负责。最重要的是 1947 年由约翰·巴迪恩，沃尔特·布拉顿和威廉·肖克利发明的晶体管，当时他们正试图改善长途电话电路的放大器。晶体管源于对半导体材料性质的基础研究，其背后的驱动力是需要比 1940 年代真空管更加物理稳定和能耗更低的设备，真空管当时是建立最早的计算机和通信设备的唯一方式。

The invention of the transistor was recognized with a Nobel Prize in physics in 1956, one of nine Nobel prizes that have been awarded to scientists for work done at least in part at Bell Labs. Other major inventions included negative feedback amplifiers, solar cells, lasers, cell phones, communications satellites and charge-coupled devices (which make the camera in your phone work).

> 发明的晶体管在 1956 年获得诺贝尔物理学奖，这是因贝尔实验室的工作而获得的九项诺贝尔奖之一。其他重大发明还包括反馈放大器、太阳能电池、激光器、手机、通信卫星和电容耦合器(使您的手机中的相机可以正常工作)。

Very roughly, in the 1960s through 1980s there were 3,000 people in the research area of Bell Labs (mostly at Murray Hill), and 15,000 to 25,000 in development groups in multiple locations that designed equipment and systems for the Bell System, often using results from the research area. That's a lot of people. Who paid for them all?

> 大致来说，在 1960 年代至 1980 年代，贝尔实验室的研究领域有 3000 人(主要在 Murray Hill)，而在多个地点的开发小组有 15000 到 25000 人，他们为贝尔系统设计设备和系统，通常使用研究领域的结果。这些人有很多。谁为他们支付费用？

AT&T was effectively a monopoly, since it provided telephone service to most of the United States, but its ability to exploit its monopoly power was constrained. It was regulated by federal and state bodies that controlled the prices that it could charge for its various services, and it was not allowed to enter businesses that were not directly related to providing telephone services.

> AT&T 有效地是一个垄断，因为它为美国大部分地区提供电话服务，但是它利用垄断力量的能力受到限制。它受到联邦和州政府的监管，这些政府控制它为各种服务收取的价格，并且不允许它进入与提供电话服务无关的业务。

This regulatory regime worked well for many years. AT&T was required to provide service to everyone ("universal service") no matter how remote or unprofitable. As compensation, it got a stable and predictable overall rate of return.

> 这种监管制度多年来运行良好。AT&T 被要求为所有人提供服务(“普遍服务”)，无论是多么偏远或不利可图。作为补偿，它获得了稳定可预见的整体回报率。

As part of this arrangement, AT&T directed a small fraction of its revenue to Bell Labs, with the express purpose of improving communications

> 作为这项安排的一部分，AT&T 将其收入的一小部分指向贝尔实验室，目的是为了改善通信。

> []{#index_split_000.html#p20}![](./index-20_1.jpg){.calibre4}
> **Figure 1.3:** Bell Labs in 2019; Building 6 is towards the lower left

services. In effect, Bell Labs was paid for by a modest tax on every phone call in the country. According to a paper by A. Michael Noll, AT&T spent about 2.8 percent of its revenues on research and development, with about 0.3 percent on basic research. I'm not sure how well this would work today, but for decades, the arrangement led to a steady flow of improvements to the phone system and a significant number of fundamental scientific discoveries.

> 根据 A. Michael Noll 的论文，AT＆T 将其收入的约 2.8％用于研发，其中约 0.3％用于基础研究。实际上，贝尔实验室是由全国每个电话通话征收的一笔微薄税款支付的。我不确定这种安排在今天是否有效，但几十年来，这种安排导致电话系统的稳步改进以及大量基本科学发现。

Stable funding was a crucial factor for research. It meant that AT&T could take a long-term view and Bell Labs researchers had the freedom to explore areas that might not have a near-term payoff and perhaps never would. That's a contrast with today's world, in which planning often seems to look ahead only a few months, and much effort is spent on speculating about financial results for the next quarter.

> 稳定的资金是研究的关键因素。这意味着 AT＆T 可以长期观察，贝尔实验室的研究人员可以自由地探索可能没有近期回报的领域，也许永远不会。这与当今世界形成鲜明对比，在这个世界中，计划通常只有几个月的时间才能展现出来，并且在猜测下一个季度的财务业绩上花费了很多努力。

> 可以采取长期视角，贝尔实验室的研究人员有自由探索可能不会在短期内带来回报，甚至永远不会带来回报的领域。这与当今的世界形成了鲜明的对比，当今的计划往往只展望未来几个月，而大量的精力花费在推测下一季度的财务结果上。

## **1.2 Communications and computer science**

Bell Labs was naturally a pioneer in designing, building and improving communications systems, a blanket term that covered everything from the design of consumer hardware like telephones through to the infrastructure of switching systems, microwave transmission towers, and fiber optic cables.

> 贝尔实验室自然是设计、构建和改进通信系统的先驱，这一覆盖范围从设计消费硬件(如电话)到交换系统、微波传输塔和光纤电缆的基础设施都包括在内。

Sometimes this breadth of practical concerns could even lead to advances in basic science. For example, in 1964 Arno Penzias and Robert Wilson were trying to figure out what was causing unwanted noise in the antenna that Bell Labs was using to detect radio signals bounced off Echo balloon satellites. They eventually deduced that the noise came from the background radiation that was the residue of the cosmic Big Bang at the beginning of the universe. This discovery led to the 1978 Nobel Prize in physics for Penzias and Wilson. (Arno says that "Most people get Nobels for things they were looking for. We got one for something we were trying to get rid of.") Another part of the Bell Labs mission was to develop a deep mathematical understanding of how communications systems worked. The most important result was Claude Shannon's creation of information theory, which was in part motivated by his study of cryptography during World War II. His 1948

> 有时，这种实用问题的广度甚至可能导致基础科学的进步。例如，1964 年，Arno Penzias 和 Robert Wilson 试图弄清楚是什么在贝尔实验室用来探测反射气球卫星的无线电信号的天线上产生了不想要的噪声。他们最终推断出，噪声来自宇宙大爆炸开始时留下的背景辐射。这一发现为 Penzias 和 Wilson 获得了 1978 年的诺贝尔物理学奖。(阿诺说：“大多数人获得诺贝尔奖是因为他们正在寻找的东西。我们获得了一个我们正在试图摆脱的东西。”)贝尔实验室的另一个任务是深入研究通信系统的工作原理。**最重要的结果是 Claude Shannon 创立的信息论**，其部分动机源于他在二战期间研究密码学的研究。他于 1948 年发表了他的著作。

paper "A Mathematical Theory of Communication," published in the _Bell_ _System Technical Journal_, explained the fundamental properties and limitations on how much information could be sent through a communications system. Shannon worked at Murray Hill from the early 1940s to 1956, then returned to teach at MIT, where he had been a graduate student. He died in 2001 at the age of 84.

> 《通信的数学理论》一文发表在《贝尔系统技术杂志》上，解释了通信系统可以传输信息的基本特性和局限性。从 20 世纪 40 年代初起，肖恩就在 Murray Hill 工作，直到 1956 年，然后回到麻省理工学院任教，他曾在那里就读研究生。2001 年，他去世，享年 84 岁。

As computers became more powerful and less expensive, computer use expanded to include more data analysis, along with extensive modeling and simulation of physical systems and processes. Bell Labs had been involved with computers and computing since the 1930s, and had computer centers with big central computers by the late 1950s.

> 随着计算机变得更加强大和便宜，计算机的使用范围扩大到包括更多的数据分析，以及广泛的建模。
> 模擬物理系統和過程。貝爾實驗室自 1930 年代以來一直參與計算機和計算，到 1950 年代後期，已經有了大型中央計算機的計算中心。

In the early 1960s, a computer science research group was formed by splitting some people out of mathematics research, along with some of the staff who operated the large central computer at Murray Hill. The resulting amalgam was called the Computing Science Research Center, and although for a brief period it still ran computer services for all of Murray Hill, it was part of the research division, not a service function. In 1970 the group that managed the computer facilities was moved into a separate organization.

> 1960 年初，一个计算机科学研究小组从数学研究中分离出一些人，加上一些在 Murray Hill 运行大型中央计算机的工作人员，形成了一个混合组织，称为计算科学研究中心，虽然它在短暂的时期仍然为 Murray Hill 的所有计算机服务，但它是研究部门的一部分，而不是服务功能。 1970 年，管理计算机设施的小组被转移到一个单独的组织中。

## **1.3 BWK at BTL**

This section contains a fair amount of personal history, which I hope will give you some idea of the lucky accidents that led me to computing as a career, and to Bell Labs as an unequaled place to pursue it.

> 这一部分包含了相当多的个人历史，我希望它能给你一些关于我如何偶然选择计算机作为职业，以及贝尔实验室作为一个无与伦比的职业发展场所的想法。

I was born in Toronto, and went to the University of Toronto. I was in a program called Engineering Physics (later renamed to Engineering Science), a catch-all program for those who didn't really know what they wanted to focus on. I graduated in 1964, which was in the early days of computing: I saw my first computer when I was in my third year at university. There was only one big computer for the whole university, an IBM 7094, which was pretty much top of the line. It had 32K (32,768) 36-bit words of magnetic core memory (today we would say 128K bytes), and some secondary storage in the form of big mechanical disk drives. It cost literally three million US dollars at the time and it lived in a large air-conditioned room, tended by professional operators; ordinary people (and especially students) did not get anywhere near it.

> 我出生在多伦多，上的是多伦多大学。我在一个叫做工程物理(后来改名为工程科学)的项目里，这是一个为那些不知道自己想要专注于什么的人设计的抓住所有机会的项目。我 1964 年毕业，那时计算机还处于早期发展阶段：我在大学三年级的时候看到了我的第一台计算机。整个大学只有一台大型计算机，一台 IBM 7094，这几乎是最顶级的。它有 32K(32,768)36 位字的磁芯存储(今天我们可以说是 128K 字节)，以及一些以大型机械磁盘驱动器为形式的辅助存储。它的价格实际上是 300 万美元，它住在一个空调室里，由专业操作员照顾；普通人(特别是学生)都无法接近它。

As a result, I did little computing as an undergraduate, though I did try to learn the Fortran programming language. For anyone who has ever struggled to write their first program, I can sympathize. I studied Daniel McCracken's excellent book on Fortran II and had the rules down pat, but I couldn't figure out how to write that first program, a conceptual barrier that many people seem to encounter.

> 结果，我在本科期间做了很少的计算，尽管我尝试学习 Fortran 编程语言。对于任何曾经努力写自己的第一个程序的人，我能够同情。我学习了 Daniel McCracken 关于 Fortran II 的出色的书籍，并掌握了规则，但我无法弄清楚如何编写第一个程序，这是许多人似乎遇到的概念障碍。

In the summer before my final year of college, I landed a job at Imperial Oil in Toronto, in a group that developed optimization software for refineries.
(Imperial Oil was partly owned by Standard Oil of New Jersey, which became Exxon in 1972.)

> 在我大学最后一年的夏天，我在多伦多的帝国石油公司找到了一份工作，在那里开发用于炼油厂的优化软件。
> 帝国石油部分由新泽西标准石油公司拥有，该公司于 1972 年更名为埃克森石油公司。

In retrospect, I was well below average as an intern. I spent the entire summer trying to write a giant Cobol program for analyzing refinery data. I don't recall its precise purpose, but I know for sure that it never worked. I didn't really know how to program, Cobol provided little support for good program organization, and structured programming had not been invented, so my code was an endless series of IF statements that branched off somewhere to do something once I had figured out what that something should be.

> 回想起来，我作为实习生的表现远远低于平均水平。整个夏天我都在试图编写一个用于分析炼油数据的巨大 Cobol 程序。
> 我不记得它的确切目的，但我可以肯定它从来没有运作过。我并不是很懂编程，Cobol 提供的程序组织支持极其有限，而结构化编程还没有被发明，所以我的代码就是一个没完没了的 IF 语句，一旦我弄清楚应该做什么，它们就会支线到某处去做那些事情。

I also tried to get Fortran programs running on Imperial's IBM 7010, since I sort of knew Fortran, certainly better than I knew Cobol, and Fortran would have been better suited for data analysis. It was only after weeks of fighting JCL, IBM's Job Control Language, that I deduced that there was no Fortran compiler on the 7010, but the JCL error messages were so inscrutable that no one else had figured that out either.

> 我也试着在帝国公司的 IBM 7010 上运行 Fortran 程序，因为我比较懂 Fortran，肯定比我懂 Cobol 好，而且 Fortran 更适合数据分析。经过几个星期与 IBM 的作业控制语言(JCL)作斗争后，我推断 7010 上没有 Fortran 编译器，但 JCL 错误信息如此晦涩难懂，以至于没有其他人也没有发现这一点。

When I returned to school for my senior year after this somewhat frustrating summer, I was still strongly interested in computing. There were no formal courses on computer science, but I did write my senior thesis on artificial intelligence, a hot topic at the time. Theorem provers, programs to play chess and checkers, and machine translation of natural languages all seemed like they were within reach, just requiring a bit of programming.

> 当我在这个有些令人沮丧的夏天回到学校上大四的时候，我仍然对计算机技术非常感兴趣。学校没有计算机科学的正式课程，但我确实写了我的毕业论文关于当时很热门的人工智能。证明定理的程序、下棋和跳棋的程序以及自然语言的机器翻译似乎都在可以实现的范围之内，只需要一点点编程。

After graduating in 1964, I had no clue what to do next, so like many students I put off the decision by going to graduate school. I applied to half a dozen schools in the United States (not common among Canadians at the time), and by good luck was accepted by several, including MIT and Princeton. Princeton said that the normal time to complete a PhD was three years, while MIT said it would probably take sev en years. Princeton offered a full fellowship; MIT said I would have to be a research assistant for 30 hours a week. The decision seemed pretty clear-cut, and a good friend, Al Aho, who had been a year ahead of me at Toronto, was already at Princeton, so off I went. It turned out to be an incredibly fortunate choice.

> 1964 年毕业后，我不知道接下来该做什么，所以像许多学生一样推迟了这个决定，去读研究生。我申请了美国的六所学校(当时在加拿大不多见)，幸运的是，我被其中几所，包括麻省理工学院和普林斯顿大学录取了。普林斯顿说正常情况下获得博士学位需要三年，而麻省理工说可能需要七年。普林斯顿提供了全额奖学金；麻省理工说我每周要做 30 个小时的研究助理。决定似乎很明确，我在多伦多大学一年级的好朋友阿尔·阿霍(Al Aho)已经在普林斯顿了，所以我就去了。结果是一个意外的好决定。

In 1966, I got lucky again, with a summer internship at MIT, thanks in part to the fact that another Princeton grad student, Lee Varian, had done a great job there in 1965. I spent the summer using CTSS, the Compatible Time-Sharing System, writing programs in MAD (Michigan Algorithm Decoder, a dialect of Algol 58) to build tools for a new operating system called Multics, which we'll come to in Chapter 2. (Multics was originally spelled MULTICS, but the lower-case version is less visually jarring; as with UNIX versus Unix and some other all-caps words, I'll use the nicer-looking form even though it's not historically accurate.) My nominal boss at MIT was Professor Fernando Corbató, "Corby" to ev eryone, a wonderful gentleman, the creator of CTSS, and the person in charge of Multics. Corby won the Turing Award in 1990 for his fundamental work on time-sharing systems. He died in July 2019 at the age of 93.

> 1966 年，我又一次运气不错，在麻省理工学院有一个暑期实习，这部分要归功于另一位普林斯顿大学研究生李·瓦里安(Lee Varian)，他在 1965 年在那里做得很出色。我花了这个暑假使用兼容时间共享系统(CTSS)，用密歇根算法解码器(MAD)(一种算法 58 的方言)编写程序，为一个叫做 Multics 的新操作系统构建工具，我们将在第 2 章中讨论它。(Multics 最初拼写为 MULTICS，但小写版本看起来更舒服；与 UNIX 与 Unix 以及一些其他大写字母一样，即使它不是历史上准确的，我也会选择更好看的形式。)我在 MIT 的名义上的老板是费尔南多·科尔巴托(Fernando Corbató)，每个人都叫他“Corby”，一个很棒的绅士，CTSS 的创造者，也是 Multics 的负责人。科尔巴托在 1990 年因其关于时间共享系统的基础工作获得了图灵奖。他于 2019 年 7 月去世，享年 93 岁。

In addition to leading the design and implementation of CTSS and Multics, Corby was the inventor of passwords for computer access. There had been little need for such a thing with batch computing, but some security mechanism was necessary to protect private files on a time-sharing computer with a shared file system.

> 除了领导 CTSS 和 Multics 的设计和实施外，Corby 还是电脑访问密码的发明者。在批处理计算中，这种东西几乎没有什么需要，但是在共享文件系统的时间共享计算机上，有必要有一些安全机制来保护私人文件。

I still remember both of the short pronounceable passwords that were automatically generated for me while I was at MIT in the summer of 1966.

> 我仍然记得 1966 年夏天我在麻省理工学院时被自动生成的两个短而易记的密码。

Tw o passwords were needed, not one, because one day during the summer a mixup caused the file that stored the passwords to be exchanged with the file that held the login message of the day. Since passwords were stored unen-crypted, everyone who logged in got to see everyone else's passwords.

> 需要两个密码，而不是一个，因为夏天的一天，混乱导致存储密码的文件与存储每日登录消息的文件交换了。由于密码未加密，每个登录的人都可以看到其他人的密码。

My office, which I remember as being unshared, belonged to Professor Joseph Weizenbaum, but he was away for the summer. Early in 1966, Weizenbaum had published a description of Eliza, a program that simulated a dialog with a Rogerian psychologist. Eliza was one of the first attempts at using natural language to interact with a computer. It was surprisingly effective, at least when first encountered, and I enjoyed showing it off to visitors.

> 我记得的办公室是没有分享的，属于约瑟夫·魏曾鲍姆教授，但他夏天不在。1966 年初，魏曾鲍姆发表了一篇关于 Eliza 的描述，Eliza 是一个模拟罗杰斯心理学家对话的程序。Eliza 是最早尝试使用自然语言与计算机交互的尝试之一，它出人意料地有效，至少当第一次遇到时是如此，我喜欢向访客展示它。

There are plenty of Eliza simulators on the web today; it's still entertaining to play with them for a few minutes, though their weaknesses quickly become evident.

> 今天网上有很多伊莉莎模拟器；虽然它们的弱点很快就会显现出来，但玩它们几分钟仍然很有趣。

ELIZA: Please tell me what's been bothering you.
YOU: I'm trying to write a book about Unix.
ELIZA: Is it because you are trying to write a book about unix that you came to me?
YOU: Yes.
ELIZA: You are sure.
YOU: Yes.
ELIZA: You seem to be quite positive.
YOU: Yes.
ELIZA: I see.

In the summer of 1967, I got the ultimate piece of good luck: an internship at Bell Labs in Murray Hill, in the Computing Science Research Center, working for Doug McIlroy (Figure 1.4). Doug suggested that I explore some problem in evaluating memory allocators, one of his long-term interests. In the best intern tradition, I bumbled around and eventually did something completely different, creating a library of functions that made it convenient to do list processing in Fortran programs. I spent the summer writing tight assembly language for the then-current big computer at Murray Hill, a GE

> 1967 年夏天，我得到了最棒的好运：在 Murray Hill 的贝尔实验室的计算科学研究中心实习，为 Doug McIlroy(图 1.4)工作。**Doug 建议我研究评估内存分配器的一些问题**，这是他长期关注的话题之一。最好的实习生传统是，我摸索着最终做了一些完全不同的事情，创建了一个使用 Fortran 程序进行列表处理变得方便的函数库。我花了整个夏天编写 Murray Hill 当时最大的电脑 GE 的紧凑的汇编语言。

635, which was in effect a cleaned-up and more orderly IBM 7094, but also a simpler version of the GE 645 that had been specially designed for Multics.

> 635 是一台清理并组织更加有序的 IBM 7094，也是为 Multics 专门设计的 GE 645 的简化版。

That's pretty much the last time I wrote assembly language, but even though what I was doing was fundamentally misguided, it was a blast and it hooked me completely on programming.

> 那大概是我最后一次编写汇编语言了，尽管如此。
> 我做的事基本上是错误的，但是还是很有趣，完全把我吸引到了编程中去。

> []{#index_split_000.html#p25}![](./index-25_1.jpg){.calibre4}
> **Figure 1.4:** Doug McIlroy, ∼1981 (Courtesy of Gerard Holzmann) **1.4 Office space** Sometimes geography is destiny.

My office as an intern in 1967 was on the fifth floor of Building 2, on a corridor off Stair 8. On my first day on the job, I was sitting in my office (the good old days when even an intern could luck into a private office), wonder-ing what to do, when an older guy appeared in my doorway at 11AM, and said "Hi, I'm Dick \[unintelligible\]. Let's go to lunch."

> 1967 年我作为实习生的办公室在 2 号楼的五楼，在 8 号楼梯的走廊上。我上班的第一天，我坐在我的办公室里(那些好日子，即使是实习生也能够得到一间私人办公室)，不知道该做什么，这时一个年纪大一点的家伙 11 点出现在我的门口，说：“嗨，我是迪克[无法辨认]。让我们去吃午饭吧。”

OK, I thought, why not? I don't remember anything at all about the lunch, but I do remember that afterwards, Dick \[unintelligible\] went off somewhere else, and I sneaked along the corridor to read the name tag on his door. Richard Hamming! My friendly next-door neighbor was famous, the inventor of error-correcting codes, and the author of the textbook for a numerical analysis course that I had just taken.

> 好吧，我想，为什么不呢？我完全不记得午餐的事情了，但是我记得之后，Dick \[无法理解\] 又走到别的地方去了，我溜到走廊里看他的门牌上写的名字。Richard Hamming！我友好的隔壁邻居是个有名的人，纠错码的发明者，也是我刚刚上完的数值分析课程的教科书的作者。

Dick (Figure 1.5) became a good friend. He was a man of strong opinions and not afraid to express them, which I think put off some people, but I enjoyed his company and over the years profited a great deal from his advice.

> 狄克(见图 1.5)成了一个好朋友。他有着坚定的观点，也不怕表达出来，这可能让一些人有些反感，但我很喜欢他的陪伴，多年来他的建议给了我很大的帮助。

He was a department head, but there were no people in his department, which seemed odd. He told me that he had worked hard to achieve this combination of suitable title without responsibility, something that I came to appreciate only much later when I became a department head with a dozen people in my department.

> 他是一个部门主管，但他的部门里没有人，这似乎很奇怪。他告诉我，他努力工作，获得了这种合适的头衔而没有责任，这是我所了解到的。
> 当我成为一个拥有十几个人的部门负责人时，才更加意识到这一点。

[]{#index_split_000.html#p26}![](./index-26_1.jpg){.calibre4}
**Figure 1.5:**

Dick Hamming, ∼1975, in his trademark plaid jacket (Wikipedia) I was there in the summer of 1968 when he learned that he had won the ACM Turing Award, which today is considered the computer science equivalent of a Nobel prize. Dick's sardonic reaction: since the Nobel prize was at that time was worth \$100,000 and the Turing award was worth \$2,000, he said that he had won 2 percent of a Nobel prize. (This was the third Turing aw ard; the first two went to Alan Perlis and Maurice Wilkes, also pioneers of computing.) Dick was cited for his work on numerical methods, automatic coding systems, and error-detecting and error-correcting codes.

> 狄克·哈明(Dick Hamming)，1975 年前后，以他标志性的格子夹克(Wikipedia)而闻名。1968 年夏天，他得知自己赢得了 ACM 图灵奖，如今被视为计算机科学界的诺贝尔奖。狄克讽刺地说：当时诺贝尔奖的价值是 10 万美元，而图灵奖的价值只有 2000 美元，所以他赢得的只是诺贝尔奖的 2%。(这是第三次颁发图灵奖；第一两次分别授予计算机先驱艾伦·佩里斯(Alan Perlis)和莫里斯·威克斯(Maurice Wilkes)。)狄克因其数值方法、自动编码系统以及检测和纠正错误码的研究而被提名。

Dick was the person who started me writing books, which has turned out to be a good thing. He had a fairly low opinion of most programmers, who he felt were poorly trained if at all. I can still hear him saying

> 狄克是让我开始写书的人，这结果是件好事。他对大多数程序员的看法相当低，他觉得他们如果接受过培训的话，培训质量也不怎么样。我仍然能听到他说：

"We giv e them a dictionary and grammar rules, and we say, 'Kid, you're now a great programmer.' "

> 我们给他们一本字典和语法规则，然后我们对他们说：“孩子，你现在是一个伟大的程序员了。”

He felt that programming should be taught as writing was taught. There should be a notion of style that separated poor code from good code, and programmers should be taught how to write well and appreciate good style.

> 他觉得编程应该像教授写作一样被教授。应该有一种区分糟糕代码和优秀代码的风格观念，程序员应该被教授如何写出优秀的代码以及欣赏优秀的风格。

He and I disagreed on how this might be accomplished, but his idea was sound, and it led directly to my first book, _The Elements of Programming_ _Style_, which I published in 1974 with P. J. "Bill" Plauger, who was at the time in the adjacent office. Bill and I emulated Strunk and White's _The_

> 他和我对如何实现这个想法意见不同，但他的想法是正确的，这直接导致了我的第一本书《编程元素》(The Elements of Programming Style)，1974 年我和当时在隔壁办公室的 P. J. “比尔”普劳格(Bill Plauger)一起出版了这本书。比尔和我模仿了斯特伦克和怀特的《简明英语》(The Elements of Style)。

_Elements of Style_ by showing a sequence of poorly written examples, and explaining how to improve each of them.

> _《风格要素》通过展示一系列写得不好的例子，并解释如何改进每一个例子来帮助我们。_

Our first example came from a book that Dick had showed me. He came into my office one day carrying a numerical analysis text, all up in arms about how bad the numerical parts were. I saw only an awful chunk of Fortran:

> 我们的第一个例子来自了一本迪克给我展示的书。他有一天走进我的办公室，手里拿着一本数值分析的书，对书中的数值部分大为不满。我只看到一大块可怕的 Fortran 代码：

```
DO 14 I=1,N
DO 14 J=1,N
14 V(I,J)=(I/J)\*(J/I)
```

If you're not a Fortran programmer, let me explain. The code consists of two nested DO loops, both ending at the line which has the label 14. Each loop steps its index variable from the lower limit to the upper limit, so in the outer loop I steps from 1 to N, and for each value of I, in the inner loop J steps from 1 to N. The variable V is an array of N rows and N columns; I loops over the rows and for each row, J loops over the columns.

> 如果你不是一位 Fortran 程序员，让我来解释一下。这段代码由两个嵌套的 DO 循环组成，都以标签 14 的行结束。每个循环都会令其索引变量从下限到上限变化，所以外循环中 I 从 1 变化到 N，对于每个 I 的值，内循环中 J 也会从 1 变化到 M。
> 从 1 到 N 的步骤。变量 V 是一个 N 行 N 列的数组；我遍历行，对于每一行，J 遍历列。

This specific pair of loops thus creates an N by N matrix with 1's on its diagonal and 0's everywhere else, like this when N is 5: 1 0 0 0 0

> 这对循环特别地创造了一个 N 乘 N 的矩阵，对角线上为 1，其他位置为 0，当 N 为 5 时，如下：1 0 0 0 0。

```
0 1 0 0 0
0 0 1 0 0
0 0 0 1 0
0 0 0 0 1
```

The code relies on the fact that integer division in Fortran truncates any frac-tional part, so if I is not equal to J, one of the divisions will produce 0, but if I equals J (as it does on the diagonal), the result will be 1.

> 代码依赖于 Fortran 中整数除法会截断任何小数部分的事实，因此如果 I 不等于 J，其中一个除法将产生 0，但如果 I 等于 J(如对角线上的情况)，结果将为 1。

This all seemed way too clever to me, and misplaced cleverness is a bad idea in programming.

> 这对我来说太过聪明了，而**在编程中使用不当的聪明手段是个坏主意**。

Rewriting it in a straightforward and obvious way leads to a clearer version: each time through the outer loop, the inner loop sets every element of row I to 0, and then the outer loop sets the diagonal element V(I,I) to 1: C

> **把它用一种直白明了的方式重写，可以得到一个更清晰的版本**：每次通过外层循环，内层循环将行 I 的每个元素设置为 0，然后外层循环将对角元素 V(I,I)设置为 1：C

```
MAKE V AN IDENTITY MATRIX
DO 14 I = 1,N
DO 12 J = 1,N
12 V(I,J) = 0.0
14 V(I,I) = 1.0
```

This also led to our first rule of programming style: _**Write clearly---don't be too clever.**_

> 这也导致了我们编程风格的第一条规则：_写得清楚，不要太聪明_。

Dick retired from Bell Labs in 1976 and went to the Naval Postgraduate School in Monterey, California, where he taught until his death early in 1998 at the age of 82. The story goes that one of his courses there was known to students as "Hamming on Hamming," which suggests an awkward parallel with this section of the book.

> Dick 于 1976 年从贝尔实验室退休，前往加利福尼亚蒙特雷的海军研究生学校，一直任教直到 1998 年初去世。
> 在 82 岁的时候，有一个传说，他在那里的一门课程被学生们称为“Hamming on Hamming”，这与本书的这一部分似乎有着尴尬的平行。

Dick thought hard all the time about what he was doing and why. He often said that "The purpose of computing is insight, not numbers," and he ev en had a tie with that written on it (in Chinese). One of his early insights was that computing would come to account for half the work at Bell Labs.

> 狄克总是认真思考他正在做什么以及为什么。他经常说 **“计算的目的是洞察力，而不是数字”**，甚至在他的领带上写了这句话。他早期的一个洞见是，计算机将占据贝尔实验室工作的一半。

None of his colleagues agreed, but in fact his estimate soon proved too conservative. He used to say that Friday afternoons were for thinking great thoughts, so he sat back and thought, though he was always welcoming to visitors like me at any time.

> 没有一个同事同意他的估计，但事实上他的估计很快就被证明太保守了。他常说**星期五下午是用来思考伟大想法的时间**，所以他坐下来思考，尽管他总是乐意接待像我这样的访客。

A few years after his retirement, Dick gav e an insightful talk that distilled his advice on how to hav e a successful career, called "[You and Your Research](https://www.youtube.com/watch?v=a1zDuOPkMSw)," which you can find on the web. He gav e the first version of that talk at Bellcore in March 1986; Ken Thompson drove me there so we could hear it. I've been recommending the talk to students for decades---it really is worthwhile to read the transcript, or to watch one of the video versions.

> 几年退休后，Dick 给出了一次深刻的演讲，概括了他关于如何取得成功职业生涯的建议，这次演讲叫做“**你和你的研究**”，你可以在网上找到它。他在 1986 年 3 月在 Bellcore 首次发表了这次演讲，Ken Thompson 开车带我去听它。几十年来，我一直在向学生推荐这次演讲——阅读讲稿或观看视频版本真的很值得。

Right across the hall from me in the summer of 1967 was Vic Vyssotsky (Figure 1.6), another incredibly smart and talented programmer. Vic was in charge of the Bell Labs part of Multics, a partner with Corby, but he still managed to find time to talk almost daily to a lowly intern. Vic pressed me into teaching a Fortran class to physicists and chemists who needed to learn how to program. The experience of teaching non-programmers turned out to be good fun. It got me over any fear of public speaking and made it easy to get into a variety of teaching gigs later on.

> 1967 年夏天，在我的隔壁就是 Vic Vyssotsky(图 1.6)，另一位非常聪明和有才华的程序员。Vic 负责 Bell Labs 的 Multics 部分，是 Corby 的合作伙伴，但他仍然设法每天找时间和一个低级实习生谈话。Vic 把我安排成了一个给物理学家和化学家上的 Fortran 课程的老师，他们需要学习如何编程。教非程序员的经历最终成了一件有趣的事情。这让我克服了任何演讲的恐惧，也使我以后容易进入各种教学工作。

Shortly afterwards, Vic moved to another Bell Labs location where he worked on the Safeguard anti-missile defense system.

> 不久之后，Vic 搬到另一个贝尔实验室位置，在那里他致力于 Safeguard 反导弹防御系统的研究。

He eventually returned to Murray Hill and became the executive director responsible for computer science research, and thus was my boss a couple of levels up.

> 他回到穆雷山，成为负责计算机科学研究的执行总监，因此他是我上级几个层级的老板。

By the spring of 1968, I had started to work on a problem for my PhD thesis, one suggested by my advisor, Peter Weiner. The problem was called _graph partitioning_: giv en a set of nodes connected by edges, find a way to separate the nodes into two groups of equal size such that the number of edges that connect a node in one group to a node in the other group is as small as possible. Figure 1.7 shows an example: any other partition of the nodes into two groups of five requires more than two edges between the two sets.

> 我的导师 Peter Weiner 建议的论文的主题是图分割：给定一组由边连接的节点，找到一种方法将节点分成两组，每组大小相等，将一组中的节点与另一组中的节点相连的边的数量尽可能少。 图 1.7 显示了一个例子：将节点分成两组五个要求超过两条边。

[]{#index_split_000.html#p29}![](./index-29_1.jpg){.calibre4}
**Figure 1.6:**
**Figure 1.7:**

Graph partitioning example

This was ostensibly based on a practical problem: how to assign parts of a program to memory pages such that when the program was run, the amount of swapping of program pages into and out of memory would be minimized.

> 这宣称基于一个实际问题：**如何将程序的部分分配到内存页面，以便在运行程序时，将程序页面交换到内存中和从内存中交换的数量将被最小化**。

The nodes represented blocks of code, the edges represented possible transi-tions from one block to another, and each edge could have a weight that measured the frequency of the transition and thus how costly it would be if the two blocks were in different pages.

> 节点代表代码块，边代表从一个块到另一个块的可能转换，每条边可以有一个权重，衡量转换的频率，从而如果这两个块在不同页面上，就会有多大的成本。

It was an artificial problem in a way, but it was a plausible abstraction of something real, and there were other concrete problems that shared this abstract model. For example, how should components be laid out on circuit boards to minimize the expensive wiring that connected one circuit board to another? Less plausibly, how might we assign employees to floors of a building to keep people on the same floor as the people they talk to most often?

> 这在某种程度上是一个人为制造的问题，但它是一个现实问题的合理抽象，而且还有其他具体问题也具有这种抽象模型。例如，应该如何布置电路板上的元件，以最小化连接一块电路板到另一块电路板的昂贵的线缆？不太合理的是，我们如何将员工分配到楼层，以使人们与他们最常联系的人员处于同一楼层？

This was enough justification for a PhD thesis topic, but I wasn't making much progress. When I returned to the Labs for a second internship in the summer of 1968, I described the problem to Shen Lin (Figure 1.8), who had recently developed the most effective known algorithm for the classic Traveling Salesman problem: given a set of cities, find the shortest route that visits each city exactly once, and then returns home.

> 这足以为博士论文题目提供充分的理由，但我的进展不大。1968 年夏天我第二次回到实验室实习时，我向沈林(见图 1.8)描述了这个问题，他最近发展出最有效的**经典旅行商问题算法**：给定一组城市，找到一条最短的路线，每个城市只访问一次，然后返回家。

Shen came up with an approach for graph partitioning that looked promising, though there was no assurance that it would produce the best possible answers, and I figured out how to implement it efficiently. I did experiments on a large number of graphs to assess how well the algorithm worked in practice. It seemed highly effective, but we never discovered a way to guarantee an optimum solution. I also found a couple of interesting special-case graphs where I could devise algorithms that were both fast and guaranteed to produce optimal solutions. The combination of results was enough for a thesis, and by the end of the summer I had everything I needed. I wrote it up over the fall, and had my final oral exam late in January 1969. (Princeton's optimistic estimate of three years had turned into four and a half.) A week later, I started work in the Computing Science Research Center at Bell Labs. I nev er had an interview; the Labs sent me an offer sometime in the fall, though with a caveat: my thesis had to be finished. Sam Morgan, the director of the Center and thus my boss two lev els up, told me, "We don't hire PhD dropouts." Finishing the thesis was definitely a good thing; I got another letter in December saying that I had received a substantial raise, well before I reported for work!

> 谢恩提出了一种图分割的方法，看起来很有希望，虽然不能保证一定能得到最佳答案，我想出了如何有效地实现它。我在大量的图上进行了实验，以评估该算法的实际效果。它似乎非常有效，但我们从未发现一种方法可以保证获得最优解。我还发现了一些有趣的特殊案例图，我可以设计出既快速又可以保证获得最优解的算法。这些结果足以构成一篇论文，到夏天结束时，我已经拥有了一切所需。我在秋季完成了写作，并于 1969 年 1 月进行了最终口试。(普林斯顿乐观估计的三年变成了四年半。)一周后，我开始在贝尔实验室计算科学研究中心工作。我从未参加过面试；实验室给我发了一封信，大约在秋季，但是有一个条件：我的论文必须完成。中心主任，也就是我的上级两级老板萨姆·摩根告诉我：“我们不雇佣博士辍学生。”完成论文绝对是一件好事；我在 12 月收到了另一封信，说我收到了一大笔加薪，还没有上班呢！

As an aside, although Shen and I didn't know it at the time, there was a reason why we were unable to find an efficient graph-partitioning algorithm that would always find the best possible answer. Others had been puzzling over the inherent difficulty of combinatorial optimization problems like graph partitioning, and had discovered some interesting general relationships.

> 虽然当时我和沈不知道，但作为一个附带的信息，我们无法找到一个总能找到最佳答案的有效图分割算法的原因是什么。其他人一直在思考像图分割这样的组合优化问题的固有困难，并发现了一些有趣的一般关系。

In a remarkable 1971 result, Stephen Cook, a mathematician and computer scientist at the University of Toronto, showed that many of these challenging problems, including graph partitioning, are equivalent, in the sense that if we could find an efficient algorithm (that is, something better than trying all possible solutions) for one of them, that would enable us to find efficient algorithms for all of them. It's still an open problem in computer science whether such problems are truly hard, but the betting is that they are.

> 1971 年，多伦多大学的数学家和计算机科学家斯蒂芬·库克取得了一项了不起的成果，他表明，包括图分割在内的许多具有挑战性的问题是等价的，也就是说，如果我们能够为其中一个问题找到一种有效的算法(也就是比尝试所有可能的解决方案更好的东西)，那么我们就可以为所有问题找到有效的算法。计算机科学中是否真的存在这样的问题仍然是一个悬而未决的问题，但是大家都认为它们是困难的。

Cook received the 1982 Turing Award for this work.

When I got to Bell Labs as a permanent employee in 1969, no one told me what I should work on. This was standard practice: people were introduced to other people, encouraged to wander around, and left to find their own

> 当我在 1969 年成为贝尔实验室的永久员工时，没有人告诉我应该做什么。这是标准做法：向其他人介绍，鼓励漫游，然后让他们自己找到自己的方向。

[]{#index_split_000.html#p31}![](./index-31_1.jpg){.calibre4}
**Figure 1.8:**

Shen Lin, ∼1970 (Courtesy of Bell Labs) research topics and collaborators. In retrospect, this seems like it must have been daunting, but I don't recall any concern on my part. There was so much going on that it wasn't hard to find something to explore or someone to work with, and after two summers I already knew people and some of the current projects.

> 沈林，约 1970 年(由贝尔实验室提供)的研究课题和合作者。回想起来，这似乎是一个艰巨的任务，但我不记得有任何担忧。当时有太多的事情要做，找到一些可以探索的东西或与之合作的人并不困难，两个暑假之后，我已经认识了一些人，并了解了一些当前的项目。

> [!NOTE]
> read here.

This lack of explicit management direction was standard practice.

Projects in 1127 were not assigned by management, but grew from the bottom up, coalescing a group of people who were interested in a topic. The same was true for work with other parts of the Labs: if I was involved with some development group, I might try to entice research colleagues to join me, but they would be volunteers.

> 1127 的项目不是由管理层指派的，而是从底层开始发展起来，聚集了一群对某个话题感兴趣的人。与实验室的其他部分的工作也是如此：如果我参与某个开发小组，我可能会试图诱使研究同事加入我，但他们都是志愿者。

In any case, for a while I continued to work with Shen on combinatorial optimization. Shen was exceptionally insightful on such problems, able to sense a promising line of attack by playing with small examples by hand. He had a new idea for the traveling salesman problem, a technique that greatly improved on his previous algorithm (which was already the best known), and I implemented it in a Fortran program. It worked well, and for many years was the state of the art.

> 在任何情况下，我都继续与沈一起研究组合优化问题。沈在这方面非常有洞察力，能够通过手工玩小例子来感知有前途的攻击线。他有一个新的旅行商问题的想法，这个技术大大改善了他以前的算法(已经是最好的)，我用 Fortran 程序实现了它。它运行良好，多年来一直是最先进的技术。

This kind of work was fun and rewarding, but although I could convert ideas into working code pretty well, I wasn't any good at the algorithmic parts. So I gradually drifted into other areas: document preparation software, specialized programming languages, and a bit of writing.

> 这种工作很有趣而且有回报，但是虽然我可以把想法转化成可以运行的代码，但我在算法方面不太擅长，所以我逐渐漂移到其他领域：文档准备软件、专用编程语言，还有一点写作。

I did come back to work with Shen a couple of other times, including a complex tool for optimizing the design of private networks for AT&T customers. It was good to flip back and forth between comparatively pure computer science and systems that were actually of some use to the company.

> 我确实和沈一起回来工作过几次，包括一个为 AT&T 客户优化私有网络设计的复杂工具。在相对纯粹的计算机科学和实际对公司有用的系统之间来回切换是很好的。

[]{#index_split_000.html#p32}![](./index-32_1.jpg){.calibre4}

18 CHAPTER 1: BELL LABS

**Figure 1.9:**

PR photo, ∼1970 (Courtesy of Bell Labs) The Bell Labs public relations operation was fond of Shen's work on the Trav eling Salesman problem and he figured in a number of advertisements.

> 1970 年左右(贝尔实验室提供)，贝尔实验室的公关部门非常喜欢申先生在旅行推销员问题上的工作，他也出现在许多广告中。

Figure 1.8 is a blurry excerpt from one of them, with me in the corner, and Figure 1.9, from some glossy PR magazine published by the Labs, talks about our work on graph partitioning, perhaps after we obtained a patent for the algorithm.

> 图 1.8 是其中一个模糊的摘录，我在角落里，而图 1.9 来自实验室出版的一本光鲜的公关杂志，谈论我们在图分割方面的工作，也许是在我们获得算法专利后。

Note that, most uncharacteristically, I am wearing a tie. A few years later, Dennis Ritchie and I wrote an article about C for another company magazine, probably the _Western Electric Engineer_. Before publication, we were asked to send pictures of ourselves to accompany the article, which we did. After a few weeks, we were told that the pictures had been lost. No problem, we said, we can send them again. To which the response was "This time, could you wear ties?" We replied with a firm no, and shortly afterwards the magazine was published with our original tie-less pictures, which had miracu-lously been found.

> 注意，我最不像自己的样子，我系了领带。几年后，我和丹尼斯·里奇为另一家公司的杂志写了一篇关于 C 语言的文章，可能是《西电工程师》。在发表之前，我们被要求发送我们自己的照片附在文章上，我们做了。几个星期后，我们被告知照片丢失了。没问题，我们说，我们可以再发一次。对此，回答是“这次，你们能戴领带吗？”我们坚决拒绝，不久之后，杂志以我们原来没有领带的照片发表了，这些照片奇迹般地被发现了。

When I started as a permanent employee, my office was on the fifth floor of Building 2 on a corridor off Stair 9, and I stayed in it for 30 years, a fixed point in a world of change. Over the years, my neighbors across the hall included Ken Thompson, Dennis Ritchie, Bob Morris, Joe Ossanna, and Gerard Holzmann, and eminent visitors like John Lions, Andy Tanenbaum and David Wheeler.

> 当我开始做永久雇员时，我的办公室在 2 号楼的第五层，在 9 号楼梯外的走廊上，我在那里呆了 30 年，在变化的世界中是一个固定的点。这些年来，我的隔壁邻居包括肯·汤普森，丹尼斯·里奇，鲍勃·莫里斯，乔·奥萨纳，杰拉德·霍尔茨曼，以及像约翰·莱昂斯，安迪·坦南鲍姆和大卫·惠勒等杰出的访客。

For the last decade of my time at the Labs, Ken Thompson and Dennis Ritchie's offices were directly across the corridor from mine. Figure 1.10 is a view of Dennis's office, taken in October 2005 from my old office doorway.

> 最后十年我在实验室的时间里，肯·汤普森和丹尼斯·里奇的办公室就在我的办公室对面。图 1.10 是 2005 年 10 月从我的旧办公室门口拍摄的丹尼斯的办公室的照片。

Ken's office was to the left.

Over the years my immediate neighbors included Bill Plauger, Lorinda Cherry, Peter Weinberger and Al Aho. Doug McIlroy, Rob Pike and Jon

> 这些年来，我的直接邻居包括比尔·普劳格、洛林达·樱桃、彼得·温伯格和艾尔·阿霍。道格·麦克罗伊、罗布·派克和乔恩也是我的邻居。

[]{#index_split_000.html#p33}![](./index-33_1.jpg){.calibre4}

CHAPTER 1: BELL LABS

19

**Figure 1.10:**

Dennis Ritchie's office in 2005

Bentley were just a few doors away. It's easier to collaborate with people who are physically close; I've been truly lucky in my neighbors.

> 我家距离 Bentley 只有几个门的距离。与身边的人合作更容易，我的邻居真是太幸运了。

**1.5 137** → **127** → **1127** → **11276**

Who were the players at this time, and what was the environment like? In the early 1970s, there were just over 30 people in Computing Science Research, with perhaps 4 to 6 working on Unix or things closely related to it.

> 在这个时候有哪些玩家，环境是怎样的？在 20 世纪 70 年代初，计算机科学研究有 30 多人，其中有 4 到 6 人在研究 Unix 或与它密切相关的东西。

Figure 1.11 is a montage of part of the Bell Labs internal phone book. It's not yellowed with age; when I arrived, the org chart part was printed on yellow paper, just like the yellow pages in old telephone books.

> 图 1.11 是贝尔实验室内部电话簿的一部分的蒙太奇图片。它没有褪色；当我到达时，组织图部分是用黄纸印刷的，就像旧电话簿中的黄页一样。

The page is from 1969. It shows the Computing Science Research Center under Sam Morgan (Figure 1.12), who was an excellent applied mathematician and an expert in communications theory. Doug McIlroy, who played an enormously important but not widely known role in Unix, managed a group that included Ken Thompson and others who were involved in early Unix, like Rudd Canaday, Bob Morris, Peter Neumann and Joe Ossanna. Elliot Pinson's department included Dennis Ritchie, Sandy Fraser and Steve

> 页面来自 1969 年，它展示了萨姆·摩根(图 1.12)领导下的计算科学研究中心，他是一位出色的应用数学家，也是通信理论专家。道格·麦克罗伊(Doug McIlroy)管理着一个团队，其中包括肯·汤普森(Ken Thompson)和其他参与早期 Unix 的人，比如鲁德·坎纳迪(Rudd Canaday)、鲍勃·莫里斯(Bob Morris)、彼得·纽曼(Peter Neumann)和乔·奥萨纳(Joe Ossanna)。埃利奥特·皮森(Elliot Pinson)的部门包括丹尼斯·里奇(Dennis Ritchie)、桑迪·弗雷泽(Sandy Fraser)和史蒂夫(Steve)。

[]{#index_split_000.html#p34}![](./index-34_1.jpg){.calibre4}

20 CHAPTER 1: BELL LABS

**Figure 1.11:**

Bell Labs phone book, ∼1969 (Courtesy of Gerard Holzmann) Johnson, who were also part of Unix for many years.

> 1969 年的贝尔实验室电话簿(由 Gerard Holzmann 提供)中，约翰逊家族也是 Unix 的长期成员。

Although most researchers had PhDs, no one used "Doctor"; it was first names for everyone. One visible exception about titles was that in the phone book of Figure 1.11, women were either Miss or Mrs, while men were free of marital status indicators. I don't recall exactly when this labeling stopped, but it was certainly gone from the phone book by the early 1980s.

> 尽管大多数研究人员都拥有博士学位，但没有人使用“博士”这个头衔；对所有人来说，都只是名字。关于头衔的一个明显的例外是，在图 1.11 的电话簿中，女性要么是小姐，要么是夫人，而男性则不需要表明婚姻状况。我不记得这种标记何时停止，但在 20 世纪 80 年代初，电话簿上已经没有了。

In the 1960s and 1970s there were few women and people of color in technical positions at Bell Labs; most members of technical staff were white males, and it stayed that way for a long time. In this respect, the Labs was representative of most technical environments at this period in the history of computing.

> 在 1960 年代和 1970 年代，贝尔实验室的技术职位中很少有女性和有色人种；大多数技术人员都是白人男性，而且这种情况一直持续很长时间。在这方面，实验室代表了计算机历史上这段时期大多数技术环境的特征。

During the early 1970s, Bell Labs started three long-running programs that attempted to improve the situation. The Cooperative Research Fellowship Program (CRFP) began in 1972; each year, it funded four years or more of graduate school for about 10 minority students to obtain their PhDs. The Graduate Research Program for Women (GRPW), which started in 1974, provided the same graduate school support for women, perhaps 15 or 20 per year. Sev eral of them worked in Center 1127 and in my department at one

> 在 20 世纪 70 年代初，贝尔实验室启动了三个长期项目，试图改善这种情况。合作研究奖学金计划(CRFP)于 1972 年开始；每年，它为约 10 名少数族裔学生提供四年或更多的研究生学校资助，获得博士学位。女性研究生项目(GRPW)始于 1974 年，为女性提供相同的研究生学校资助，每年可能有 15 到 20 人。他们中的几个人在 1127 中心和我的部门工作。

[]{#index_split_000.html#p35}![](./index-35_1.jpg){.calibre4}

CHAPTER 1: BELL LABS

21

**Figure 1.12:**

Sam Morgan, director of 1127, ∼1981 (Courtesy of Gerard Holzmann) time or another, and most went on to successful careers within Bell Labs, at universities and at other companies. Each year, the Summer Research Program (SRP), also started in 1974, provided fully funded summer internships for roughly 60 undergraduate women and minority students, who were hosted at Murray Hill, Holmdel and sometimes other locations, working one-on-one with a research mentor. I was in charge of SRP for Center 1127 for over 15 years, so I got to meet a lot of nice sharp undergrads, and mentor a few.

> 萨姆·摩根(Sam Morgan)，1127 中心主任，于 1981 年(由杰拉德·霍尔茨曼(Gerard Holzmann)提供)，许多人都曾在某个时候参加过贝尔实验室(Bell Labs)，并取得了成功的职业生涯，在大学和其他公司。1974 年开始的暑期研究计划(SRP)每年为约 60 名女性和少数族裔的大学生提供全额资助的暑期实习，他们在 Murray Hill，Holmdel 和其他地方接受指导，一对一与研究导师合作。我负责 1127 中心的 SRP 超过 15 年，因此我认识了很多可爱的聪明的本科生，并指导了一些人。

These programs were effective in the long run, but the environment was still quite homogeneous during the 1960s and 1970s, and I'm sure that I was oblivious to some of the issues that this raised.

> 这些计划从长远来看是有效的，但在 1960 年和 1970 年代环境仍然相当同质化，我敢肯定我没有察觉到这带来了一些问题。

Bell Labs had a clear managerial hierarchy. At the top was the president, in charge of perhaps 15 to 25 thousand people. Beneath that were areas numbered 10 (research), 20 (development), 50 (telephone switching), 60 (military systems), and so on, each with a vice president. Research itself was divided into physics (11), mathematics and communications systems (13), chemistry (15) and the like, with an executive director for each; it also included legal and patent groups. Mathematics Research was 131, and Computing Science Research was "Center 137," with half a dozen individual departments like 1371. In a major shift, all of this was renumbered a few years later, when we became Center 127, and then during some reorganization, an extra digit was added to the front, and we became 1127, a number that lasted until 2005,

> 贝尔实验室有一个清晰的管理层级结构。最高层是总裁，负责大约 15 到 25000 人。在此之下有 10(研究)、20(开发)、50(电话交换)、60(军事系统)等等各个领域，每个领域都有一位副总裁。研究本身又分为物理(11)、数学和通信系统(13)、化学(15)等，每个领域都有一位执行主任；还包括法律和专利组。数学研究为 131，计算机科学研究为“中心 137”，有半打个部门，如 1371。几年后，这一切都重新编号了，我们变成了中心 127，然后在一些重组中，在前面加了一个数字，我们变成了 1127，这个编号一直持续到 2005 年。

[]{#index_split_000.html#p36}22 CHAPTER 1: BELL LABS

well after I retired in 2000.

There were relatively few lev els in the hierarchy. Researchers like me were "member of technical staff" or MTS, and there were a couple of technical levels below that. MTS in Research normally got a private office, though ev eryone was expected to keep the door open most of the time. There was a supervisor level above this, though 1127 had only a few supervisors over the years. The next level was department head, a person like Doug McIlroy who was responsible for half a dozen to a dozen individual researchers. The level above that was director of a center, who might have half a dozen departments, then executive director, with a handful of centers, and then vice president, who oversaw the executive directors.

> 相对来说，等级层次不多。像我这样的研究人员都是“技术人员”(MTS)，而且还有几个技术级别低于 MTS。研究部门的 MTS 通常有个私人办公室，但是每个人都被期望大部分时间都保持门开着。在这之上还有一个主管级别，不过 1127 在这些年里只有几个主管。接下来是部门负责人，像道格·麦克伊尔罗伊(Doug McIlroy)这样的人负责六到十个单独的研究人员。在这之上是中心主任，可能有半打到十几个部门，然后是执行主任，负责几个中心，最后是副总裁，负责管理执行主任。

Vice presidents reported to the president. Bill Baker, an outstanding chemist, was vice president of research from 1955 until 1973, and president of Bell Labs until 1980. While he was vice president, it was believed that he knew every MTS in research by name and was aware of what they were working on. I think it might well have been true; certainly he always knew what my colleagues and I were up to.

> 副总裁向总统汇报。1955 年至 1973 年，杰出的化学家比尔·贝克担任研究部副总裁，1980 年担任贝尔实验室总裁。在他担任副总裁期间，据信他熟记研究部每一位 MTS 的名字，并知道他们正在做什么。我认为这很有可能是真的；当然，他总是知道我和我的同事们在做什么。

I was a regular MTS until 1981, when I finally succumbed to the pressure to become a department head. Most people went into management reluctantly, because although it was not the end of personal research, it did represent a slowdown, and it came with responsibilities like looking after one's department that could be challenging. Of course the usual arguments were trotted out: "It's inevitable, why not now?" Or, somewhat contradictory,

> 我一直是一名普通的 MTS，直到 1981 年，我终于屈服于成为部门主管的压力。大多数人不情愿地进入管理层，因为虽然它不是个人研究的终点，但它确实代表了一种减速，并且它伴随着像照顾自己部门这样的责任，这可能是具有挑战性的。当然，通常的论点是：“这是不可避免的，为什么不现在？”或者有点矛盾，

"This might be your last chance." Or, "If not you, it will be someone else not as good."

> 这可能是你最后的机会。或者，如果不是你，就会是另一个不太好的人。

For better or worse, I became head of a new department, 11276, with the carefully meaningless name "Computing Structures Research." The department usually had 8 to 10 people with a daunting spectrum of interests: graphics hardware, integrated circuit design tools, document preparation, operating systems, networking, compilers, C++, wireless system design, computational geometry, graph theory, algorithmic complexity, and lots more besides.

> 我不管好坏，成为了一个新部门 11276 的负责人，这个部门的名字叫做“计算结构研究”，听起来毫无意义。这个部门通常有 8 到 10 个人，涉及到各种各样的领域：图形硬件、集成电路设计工具、文档准备、操作系统、网络、编译器、C++、无线系统设计、计算几何、图论、算法复杂性以及其他很多方面。

Understanding what each of them was working on well enough to explain it further up the chain was always a challenge, though it was also rewarding, and a surprising amount of what I learned then has stuck with me.

> 了解每个人正在做什么，足以进一步向上级解释，总是一个挑战，但也很有成就感，我当时学到的东西出乎意料地多，而且记忆犹新。

The management hierarchy was accompanied by a few perks at each level. Some were obvious, like successively bigger offices at director and above. I think there was also a modest salary increase for department heads but it certainly wasn't big enough to be memorable.

> 管理层级附带了每个级别的一些福利。有些很明显，比如主管及以上级别的办公室越来越大。我想部门负责人也有一点点薪水增加，但肯定不够大到让人记住。

Some were more subtle: department heads and up had carpeted offices, while ordinary folk had bare linoleum or vinyl tile. When I was promoted, I

> 一些更微妙：部门负责人及以上的人有地毯铺设的办公室，而普通人只有光滑的油毡或乙烯基瓷砖。当我被提升时，我也拥有了地毯铺设的办公室。

[]{#index_split_000.html#p37}CHAPTER 1: BELL LABS

23

was giv en a glossy printed brochure listing my options for carpet color, office furniture, and the like. I briefly tried a new desk but it was too big and uncomfortable, so I went back to the ancient Steelcase that I had inherited in 1969. And I declined the carpet entirely, since I wasn't enthusiastic about distinctions of rank. Sam Morgan advised me strongly that I should take the carpet. He said that some day I would want the authority that came from having a carpet. I still declined, and the carpet distinction eventually went aw ay.

> 我收到一份光面印刷的小册子，列出了地毯颜色、办公家具等选项。我稍微试了一下新桌子，但是太大而且不舒服，所以我又回到 1969 年继承的古老的 Steelcase 桌子上。我完全拒绝地毯，因为我对身份的区别并不感兴趣。萨姆·摩根强烈建议我应该要地毯。他说有一天我会想要地毯带来的权威。我还是拒绝了，最终地毯的区别也消失了。

The primary annual task for department heads was to assess the work of their department members in an elaborate ritual called "merit review." Once a year each MTS wrote down on one side of one piece of paper a summary of what they had done during the year; in 1127, it was known as an "I am great report," a term that I think originated with Sam Morgan. The department head wrote another piece of paper that summarized and assessed the work, including "areas for improvement," a section that was meant to contain constructive criticism.

> 部门负责人的首要年度任务是通过一种称为“绩效评估”的精心准备的仪式来评估部门成员的工作。每年，每个 MTS 都会在一张纸的一面写下他们一年来所做的总结；在 1127 年，这被称为“我很棒的报告”，我认为这个术语源自萨姆·摩根。部门负责人写另一张纸，总结并评估工作，包括“改进领域”，这一部分旨在包含建设性的批评。

Writing the assessment and feedback was hard work, and there was a strong tendency to leave the areas for improvement part blank, but one year we were told that it had to be filled in; evasions like leaving it empty or saying "N/A" were no longer acceptable. I came up with the phrase "Keep up the good work," and got away with that for a year or two before being told that more critical comments were required, on the grounds that no one was perfect. Fortunately I didn't hav e to do this for a star like Ken Thompson.

> 写评估和反馈是艰苦的工作，而且有一种很强的倾向是不填写改进的领域，但有一年我们被告知必须填写；像空着或者说“N/A”这样的逃避不再可以接受了。我想出了“继续努力”这个短语，在一两年里还能顺利通过，直到被告知需要更多批评性的意见，理由是没有人是完美的。幸运的是，我不用为像肯·汤普森这样的明星做这件事。

What could one have said?

The department heads and the director met to come up with a consensus evaluation for each MTS. This normally took a full-day meeting. It was followed some weeks later by another full-day meeting that determined next year's salaries by allocating each MTS a share of a pot of raise money. These two related evaluations were officially known as merit review and salary review, but I always thought of them as "abstract merit" and "concrete merit."

> 部门负责人和主管开会讨论，为每个 MTS 做出共识评估。这通常需要一整天的会议。几周后，又举行了一个全天会议，通过将每个 MTS 分配一部分涨薪资金来确定明年的薪水。这两个相关的评估正式称为绩效评估和薪酬评估，但我总是把它们称为“抽象绩效”和“具体绩效”。

This process was repeated up the management chain, with an executive director reviewing all the MTS results with directors, and also assessing department heads.

> 这个过程被重复地上报到管理层，一个执行董事会审查所有的 MTS 结果，同时也评估部门负责人。

Although merit review in some centers could be competitive, our reviews were remarkably collegial. Rather than "My people are better than your people," the tone was more like "Don't forget this other good work that your person did."

> 尽管在某些中心进行的绩效评估可能具有竞争性，但我们的评估显得非常友好。与其说“我的人比你的人好”，更像是“别忘了你的人做的其他好事”。

I may be too sanguine, but I think the whole process worked well, because management was technically competent all the way up and everyone had gone through the process at lower levels. The system did not seem to have

> 我也许过于乐观了，但我认为整个过程进行得很顺利，因为管理层在技术上都很有能力，而且每个人都经历了较低层次的过程。系统似乎没有出现什么问题。

[]{#index_split_000.html#p38}24 CHAPTER 1: BELL LABS

much of a bias towards either practice or theory, at least for us in 1127---good programs and good papers were both valued. The absence of proposals or plans for future work was a good thing. One was expected to have roughly a year's worth of accomplishments at the end of the year, but any number of false starts could be ignored, and management took a long view of people who worked on the same thing for multiple years. I think that it also helped that in Research there were very few management levels, so promotion wasn't really on most people's radar most of the time. If one really aspired to be a manager, an org anization outside of Research would likely be a better option.

> 大多数偏向实践或理论的偏见对我们在 1127 来说都是受重视的。缺乏未来工作的提案或计划是件好事。人们期望在年底有大约一年的成就，但任何失败的开始都可以被忽略，管理层对那些长期从事同一件事情的人有着长远的眼光。我认为，研究中管理层很少，因此晋升不是大多数人最常考虑的事情。如果一个人真的渴望成为管理者，那么研究之外的组织可能是一个更好的选择。

It's interesting to compare the Bell Labs evaluation process with how it's done in research universities. In the latter, hiring and especially promotion are strongly influenced by a dozen or more letters solicited from prominent outside researchers who are in the same specialty. This tends to encourage deep expertise in narrow fields, since the goal of a reviewee is to master some field so well that external reviewers can legitimately say "This person is the best person in this sub-field at this stage of his or her career."

> 有趣的是比较贝尔实验室的评估过程与研究大学是如何做的。在后者，招聘和特别是晋升受到来自外部研究人员的十几封书面请求的强烈影响，这些研究人员都处于同一个专业领域。这往往鼓励深入掌握狭窄领域的专业知识，因为考核对象的目标是掌握某一领域的知识，以至于外部评审可以合法地说：“在其职业生涯的这个阶段，此人是该子领域中最好的人选。”

By contrast, Bell Labs created a rank order for every researcher, from the bottom up. Each department head ranked his or her people; those rankings were merged by department heads within a center, and those in turn by the next two lev els, so by the end everyone's approximate position in the whole population was determined.

> 通过对比，贝尔实验室为每个研究人员创建了一个从下到上的等级排序。每个部门主管对自己的人进行排名；这些排名由中心的部门主管合并，然后由下两个级别合并，因此最终每个人在整个人群中的大致位置就被确定了。

A person who did great work in a narrow field might well be ranked highly by his or her immediate management, but no one further up would likely know of the work. Interdisciplinary work, on the other hand, stood out at higher levels because more managers would have seen it. The broader the collaborations, the more managers would know about it. The end result was an organization that strongly favored collaboration and interdisciplinary research. And because the managers who made the decisions had come up through the same process, they were inclined in the same direction.

> 一个在狭窄领域做出伟大成就的人可能会受到其直接管理者的高度评价，但更高层次的人可能不会知道这项工作。另一方面，跨学科的工作会在更高层次引起重视，因为更多的管理者会看到它。合作范围越广，更多的管理者就会知道它。最终的结果是，组织强烈青睐合作和跨学科研究。而且，因为做出决定的管理者也是从同一过程中出来的，他们也倾向于同一方向。

I was a department head for over 15 years, was probably at best an average manager, and was definitely happy to step down. Others successfully resisted promotion for long periods; Dennis Ritchie became a department head well after I did, and Ken Thompson never did.

> 我担任部门主管超过 15 年，可能最多算是一个普通的经理，而且我很乐意让出位置。其他人也长期拒绝晋升；丹尼斯·里奇在我担任部门主管之后才成为一名部门主管，而肯·汤普森从未担任过。

Having now taught at a university for 20 years, I'm still not enthusiastic about sitting in judgment on other people's work. It's necessary, howev er, and sometimes one has to make decisions that do affect people's liv es, like firing someone (which I fortunately never had to do) or failing a student in a course (not common but not unheard of either). One of the good things about the Bell Labs process was that it was based on the shared judgment of other

> 现在在大学教了 20 年了，我仍然不太热衷于评判别人的作品。然而，这是必要的，有时候我们必须做出会影响别人生活的决定，比如解雇某人(幸运的是我从来没有这样做过)或者把某个学生不及格(不常见，但也不是没有发生过)。贝尔实验室的过程有个好处就是它是基于其他人的共同判断的。

[]{#index_split_000.html#p39}CHAPTER 1: BELL LABS

25

people who understood the work. As Doug McIlroy said, "Collegiality was the genius of the system. Nobody's advancement depended on the relationship with just one boss." The process at the Labs wasn't perfect, but it was pretty good and I've certainly heard and read about performance review processes that are far worse.

> 人们理解这项工作。正如道格·麦克伊尔罗伊所说：“同事之间的关系是这个系统的天赋。没有人的进步取决于与某一位老板的关系。” 实验室的过程并不完美，但是还是相当不错的，我也听说过并且阅读过更糟糕的绩效评估流程。

[]{#index_split_000.html#p40} []{#index_split_000.html#p41}Chapter 2

**Proto-Unix (1969)**

"At some point I realized that I was three weeks from an operating system."

> 在某一刻，我意识到距离操作系统只有三个星期。

Ken Thompson, Vintage Computer Festival East, May 4, 2019

The Unix operating system was born in 1969, but it didn't spring into existence out of nothing. It came out of the experiences of several people at Bell Labs who had worked on other operating systems and languages. This chapter tells that story.

> Unix 操作系统于 1969 年诞生，但它并非凭空而来。它源自于贝尔实验室的几位工作人员在其他操作系统和语言上的经验。本章将讲述这个故事。

**2.1 A bit of technical background**

This section is a short primer on the basic technical material that forms the central topics of the book: computers, hardware, software, operating systems, programming, and programming languages. If you're already familiar with these ideas, skip ahead; if not, I hope this will bring you up to speed enough that you can appreciate what it's all about. If you want more detailed explanations aimed at non-technical readers, you might like my _Understanding the Digital World_, though I am not unbiased.

> 这一部分是关于书中核心主题：计算机、硬件、软件、操作系统、编程和编程语言的简短引导。如果你已经熟悉这些概念，请跳过；如果不是，我希望这能让你足够了解它的内容，以便你能够欣赏它。如果你想要针对非技术读者的更详细的解释，你可能会喜欢我的《了解数字世界》，尽管我不是公正的。

A computer is fundamentally not much more than a calculator like the ones that used to be separate gadgets but are now just applications on a phone. Computers can do arithmetic computations exceedingly fast, howev er, billions per second today, though it was significantly less than millions per second in the 1970s.

> 电脑基本上不比过去的独立计算器多多少，它们现在只是手机上的应用程序。电脑可以以极快的速度进行算术计算，如今每秒可以达到数十亿次，尽管在 1970 年代只有数百万次。

A typical computer of the 1960s and 1970s had a repertoire of a few dozen kinds of instructions that it could perform: arithmetic (add, subtract, multiply, divide), read information from primary memory, store information

> 1960 年代和 1970 年代的典型计算机可以执行几十种不同类型的指令：算术运算(加、减、乘、除)、从主存储器中读取信息以及存储信息。

[]{#index_split_000.html#p42}28 CHAPTER 2: PROTO-UNIX

into primary memory, and communicate with devices like disks and anything else that might be connected. Plus one other crucial thing: the repertoire includes instructions that decide which instructions to perform next---thus what the computer will do next---based on the results of previous computations, that is, what it has already done. In that way, a computer controls its own destiny.

> 转移到主存储器中，与磁盘等设备进行通信。另外一个重要的事情是：指令集包括根据先前计算的结果，也就是它已经做了什么，决定下一步执行哪些指令的指令，从而决定计算机的下一步行动。这样，计算机就能控制自己的命运。

Instructions and data are stored in the same primary memory, which is usually called RAM, for "random access memory." If you load a different set of instructions into the RAM, the computer does a different job when it executes them. That's what's happening when you click on an icon for a program like Word or the Chrome browser---it tells the operating system to load the instructions for that program into memory and start to run it.

> 在同一个主存储器中存储指令和数据，通常称为 RAM(随机存取存储器)。如果你将不同的指令加载到 RAM 中，当它们执行时，计算机将做出不同的工作。这就是当你点击 Word 或 Chrome 浏览器图标时发生的事情---它会告诉操作系统将该程序的指令加载到内存中并开始运行它。

Programming is the process of creating the sequences of operations that perform some desired task, using some programming language. It's possible to create the necessary instructions directly, but this is a difficult chore with many clerical details, even for tiny programs, so most of the advances in programming have inv olved creating programming languages that are closer to the way that humans might express a computation. Programs called _compilers_ (which of course have to be written themselves) translate from higher-level languages (closer to human language) ultimately to the individual instructions of a specific kind of computer.

> 编程是使用某种编程语言创建执行某些期望任务的操作序列的过程。可以直接创建必要的指令，但即使是小程序，这也是一项具有许多文书细节的艰巨任务，因此编程的大部分进步都涉及到创建更接近人类表达计算方式的编程语言。称为*编译器*的程序(当然必须自己编写)可以从更高级的语言(更接近人类语言)最终翻译成特定计算机的单独指令。

Finally, an operating system is just a big and complicated program built from the same instructions as ordinary programs like Word or a browser. Its task is to control all the other programs that are trying to run, and to manage interactions with the rest of the computer.

> 最后，操作系统只是一个由像 Word 或浏览器这样的普通程序使用相同指令构建的大而复杂的程序。它的任务是控制所有试图运行的其他程序，并管理与计算机其余部分的交互。

This is pretty abstract, so here's a small concrete example of what programming is. Suppose we want to compute the area of a rectangle from its length and width. We might say in English "the area is the product of the length and width." Writing it on the board in school, a teacher could say that area is computed with this formula:

> 这很抽象，所以这里有一个编程的小具体例子。假设我们想要从长度和宽度计算矩形的面积。我们可以用英语说“面积是长度和宽度的乘积”。在学校的黑板上写下，老师可以说面积是用这个公式计算的：

_area_ = _length_ × _width_ In a higher-level programming language, we would write area = length \* width

> 面积 = 长度 × 宽度。在高级编程语言中，我们可以写作面积 = 长度 × 宽度。

which would be the exact form in most of the popular languages of today. A compiler translates that into a still readable but machine-specific sequence of machine instructions for a computer. That sequence might look like this for a simple hypothetical computer:

> 编译器将其转换为仍然可读但特定于计算机的机器指令序列。对于一台简单的假设计算机，该序列可能如下所示：

[]{#index_split_000.html#p43}CHAPTER 2: PROTO-UNIX 29

load length

multiply width

store area

Finally a program called an _assembler_ converts that sequence of more or less readable instructions into a sequence of machine instructions that can be loaded into the primary memory of a computer; when those instructions are executed, they will compute the area from the given length and width. Of course this glosses over any number of details---how do we specify compiling and loading, how do the length and width get into the computer, how is the area printed, and so on---but it's the essence of the story.

> 最后，一个称为编译器的程序将这系列更多或更少可读的指令转换成可以加载到计算机主存储器中的机器指令序列；当执行这些指令时，它们将根据给定的长度和宽度计算出面积。当然，这略去了许多细节 - 我们如何指定编译和加载，长度和宽度如何进入计算机，面积如何打印等等，但这是故事的本质。

If you prefer to see a working example, here is a complete program in the C programming language that reads a length and width, and prints an area: void main() {

> 如果您更喜欢看到一个工作示例，这里有一个完整的 C 编程语言程序，可以读取长度和宽度，并打印出面积：void main() {

float length, width, area;

scanf(\"%f %f\", &length, &width); area = length \* width;

printf(\"area = %f\\n\", area);

}

This program can be compiled and executed on any computer.

Everyone is familiar at least with the names of modern operating systems like Windows and macOS; cell phones run operating systems like Android and iOS.

> 大家至少都熟悉现代操作系统的名字，比如 Windows 和 macOS；手机运行的操作系统有 Android 和 iOS。

An operating system is a program that controls a computer, sharing the resources among programs that are running. It manages the primary memory, allocating it to running programs as they need it. On a desktop or laptop the operating system lets you run a browser, a word processor, a music player, and perhaps our little area-computation program, all at the same time, switching its attention to each as necessary.

> 操作系统是一种控制计算机的程序，它可以在运行的程序之间共享资源。它管理主存储器，根据运行程序的需要将其分配给它们。在台式机或笔记本电脑上，操作系统可以让您同时运行浏览器、文字处理器、音乐播放器，甚至可能还有我们的小面积计算程序，并根据需要将其注意力转移到每个程序上。

It also controls the display, giving each program screen visibility when requested, and it manages storage devices like disks, so that when you save your Word document, it is preserved so that you can recover it and resume work later on.

> 它还控制显示器，当程序需要时，提供每个程序的屏幕可见性，并管理存储设备，如磁盘，这样当你保存 Word 文档时，它就会被保存下来，以便你可以恢复它并稍后继续工作。

The operating system also coordinates communication with networks like the Internet, so your browser can help you search, check in with friends, shop, and share cat videos, all simultaneously.

> 操作系统还协调与像 Internet 这样的网络的通信，因此您的浏览器可以帮助您同时搜索、与朋友联系、购物和分享猫咪视频。

It's not so obvious to non-programmers, but an operating system also has to protect programs from other programs in case they hav e errors, and it has to protect itself from errant or malicious programs and users.

> 对于非程序员来说，这不是那么明显，但是操作系统也必须保护程序免受其他程序出错的影响，并且必须保护自身免受错误或恶意程序和用户的攻击。

Something similar is going on with the operating systems on phones.

Underneath, there's a lot of action to maintain communications via a mobile

> 在下面，有很多行动来通过移动设备保持通信。

[]{#index_split_000.html#p44}30 CHAPTER 2: PROTO-UNIX

network or Wi-Fi. Phone apps are exactly the same idea as programs like Word, though often different in detail, and they are written in the same programming languages.

> 网络或 Wi-Fi。手机应用程序与像 Word 这样的程序完全一样，尽管在细节上可能有所不同，而且它们是用相同的编程语言编写的。

Operating systems today are big and complicated programs. Life was simpler in the 1960s but relative to the time, they were still big and complicated. Typically a computer manufacturer like IBM or DEC (Digital Equipment Corporation) would provide one or more operating systems for its various kinds of hardware. There was no commonality at all between hardware from different manufacturers and sometimes not even between hardware offerings from the same manufacturer, and thus there was also no commonality among operating systems.

> 今天的操作系统是庞大且复杂的程序。1960 年代的生活更简单，但相对于当时，它们仍然很大且复杂。通常，像 IBM 或 DEC(数字设备公司)这样的计算机制造商会为其各种硬件提供一个或多个操作系统。不同制造商的硬件没有共同之处，有时甚至同一制造商的硬件产品也没有共同之处，因此操作系统也没有共同之处。

To further complicate matters, operating systems were written in assembly language, a human-readable representation of machine instructions, but very detailed and specific to the instruction repertoire of a particular kind of hardware. Each kind of computer had its own assembly language, so the operating systems were big and complicated assembly language programs, each written in the specific language of its own hardware.

> 事情变得更加复杂，操作系统是用汇编语言编写的，这是一种人类可读的机器指令表示形式，但非常详细，且专门针对特定硬件的指令集。每种计算机都有自己的汇编语言，因此操作系统都是大型复杂的汇编语言程序，每个程序都是用其自身硬件的特定语言编写的。

This lack of commonality among systems and the use of incompatible low-level languages greatly hindered progress because it required multiple versions of programs: a program written for one operating system had to be in effect rewritten from scratch to move to a different operating system or architecture. As we shall see, Unix provided an operating system that was the same across all kinds of hardware, and eventually it was itself written in a high-level language, not assembly language, so it could be moved from one kind of computer to another with comparatively little effort.

> 这种系统之间缺乏共性以及使用不兼容的低级语言大大阻碍了进步，因为它需要多个版本的程序：一个为某个操作系统编写的程序实际上必须从头开始重写才能移动到不同的操作系统或架构。正如我们将看到的，Unix 提供了一个跨所有硬件类型相同的操作系统，最终它本身是用高级语言而不是汇编语言编写的，因此可以相对轻松地从一种计算机移动到另一种计算机。

**2.2 CTSS and Multics**

The most innovative operating system of the time was CTSS, the Compatible Time-Sharing System, which was created at MIT in 1964. Most operating systems in that era were "batch processing." Programmers put their programs on punch cards (this was a long time ago!), handed them to an operator, and then waited for the results to be returned, hours or even days later.

> 最具创新性的操作系统当时是 CTSS，即兼容时间共享系统，该系统于 1964 年在麻省理工学院创建。当时大多数操作系统都是“批处理”。程序员将他们的程序放在穿孔卡上(这是很久以前的事了！)，交给操作员，然后等待结果，几小时甚至几天后返回。

Punch cards were made of stiff high-quality paper and could store up to 80 characters, typically a single line of a program, so the 6-line C program above would require 6 cards, and if a change was necessary, the card(s) would have to be replaced. Figure 2.1 shows a standard 80-column card.

> 普查卡是由坚固的高质量纸制成的，可以存储多达 80 个字符，通常是程序的单行，因此上面的 6 行 C 程序需要 6 张卡片，如果需要更改，卡片(s)必须更换。图 2.1 显示了一张标准的 80 列卡片。

By contrast, CTSS programmers used typewriter-like devices ("terminals"

like the Model 33 Teletypes in Figure 3.1 in the next chapter) that were connected directly or by phone lines to a single big computer, an IBM 7094 with

> 就像下一章中图 3.1 中的 33 号模型电传打字机，它们可以直接或通过电话线连接到一台大型计算机 IBM 7094。

[]{#index_split_000.html#p45}![](./index-45_1.jpg){.calibre4}

CHAPTER 2: PROTO-UNIX 31

**Figure 2.1:**

Punch card, 7-3/8 by 3-1/4 in \[187.325 mm by 82.55 mm\]

twice the usual 32K words of memory. The operating system divided its attention among the users who were logged in, switching rapidly from one active user to the next, giving each user the illusion that they had the whole computer at their disposal. This was called "time-sharing," and (speaking from personal experience) it was indescribably more pleasant and productive than batch processing. Most of the time, it really did feel like there were no other users.

> 这倍于通常的 32K 字节的内存。操作系统将注意力分配给已登录的用户，迅速地从一个活动用户切换到另一个活动用户，给每个用户一种错觉，他们拥有整个计算机。这被称为“分时”，(从个人经验来讲)它比批处理更加令人愉悦和富有成效。大多数时候，它确实感觉不像有其他用户。

CTSS was such a productive programming environment that researchers at MIT decided to create an even better version, one that could serve as an

> MIT 的研究人員發現 CTSS 是一個非常高效的程式開發環境，因此決定創造一個更好的版本，以便作為一個更好的環境。

"information utility" to provide computing services to a large and dispersed user population. In 1965, they beg an to design a system called "Multics," the Multiplexed Information and Computing Service.

> 1965 年，他们开始设计一个名为“Multics”的系统，即多路信息和计算服务，以提供计算服务给一个庞大而分散的用户群体。

Multics was going to be a big job, since it involved ambitious new software, and new hardware with more capabilities than the IBM 7094, so MIT

> 多路系统将会是一项重大工作，因为它涉及雄心勃勃的新软件，以及比 IBM 7094 更具能力的新硬件，因此 MIT 也加入其中。

enlisted two other organizations to help. General Electric, which at the time made computers, was to design and build a new computer with new hardware features to better support time-sharing and multiple users. Bell Labs, which had a great deal of experience from creating its own systems since the early 1950s, was to collaborate on the operating system.

> 为了帮助，另外聘请了两个组织。当时生产计算机的通用电气公司被要求设计和制造一台新的计算机，具有新的硬件功能，以更好地支持分时和多用户。自 1950 年代早期以来一直在创建自己的系统的贝尔实验室被要求参与操作系统的合作。

Multics was intrinsically a challenging prospect, and it soon ran into problems. In retrospect, it was partly a victim of the _second system effect_: after a success (like CTSS), it's tempting to try to create a new system that fixes all the remaining problems with the original while adding everybody's favorite new features too. The result is often a system that's too complicated, a consequence of taking on too many different things at the same time, and that

> 多西斯本质上是一个具有挑战性的前景，很快就遇到了问题。回想起来，它在某种程度上是第二系统效应的受害者：在取得成功(如 CTSS)之后，试图创建一个新系统来解决原始系统中所有剩余的问题，同时添加每个人最喜欢的新功能，结果往往是一个太复杂的系统，这是一次太多的事情同时发生的后果。

[]{#index_split_000.html#p46}32 CHAPTER 2: PROTO-UNIX

was the case with Multics. The phrase "over-engineered" appears in several descriptions, and Sam Morgan described it as "an attempt to climb too many trees at once." Furthermore, one does not need to be much of a student of organizations to anticipate that there might also be problems with a project involving two very different companies and a university, in three locations spread across the country.

> 对于 Multics 来说也是如此。"过度设计"这个词出现在许多描述中，Sam Morgan 将其描述为"试图一次爬上太多树"。此外，不需要成为组织学的学者，就可以预见，一个涉及两家非常不同的公司和一所位于全国三个不同地点的大学的项目可能会存在一些问题。

Half a dozen or more Bell Labs researchers worked on Multics from 1966

through 1969, including Doug McIlroy, Dennis Ritchie, Ken Thompson, and Peter Neumann, who had taken over Vic Vyssotsky's role when Vic moved to another Bell Labs location. Doug was deeply involved with PL/I, the programming language that was to be used for writing Multics software. Dennis had worked on Multics documentation while a student at Harvard and worked on the device input and output subsystem at the Labs. Ken focused on the input/output subsystem, experience that proved valuable when he began work on Unix, though in a 2019 interview, he described his Multics work as being "a notch in a big wheel and it was producing something that I didn't want to use myself."

> 1969 年至今，包括 Doug McIlroy、Dennis Ritchie、Ken Thompson 和接替 Vic Vyssotsky 的 Peter Neumann，他们都参与了 Multics 软件的开发。Doug 对 PL/I 编程语言有深入的了解，而 Dennis 在哈佛大学期间就参与了 Multics 的文档编写，并在实验室负责设备输入和输出子系统的工作。Ken 专注于输入/输出子系统，这种经验在他开始 Unix 的工作时变得非常宝贵，尽管在 2019 年的一次采访中，他把自己的 Multics 工作描述为“一个大轮子上的一个齿，而且它生产的是我自己不想使用的东西”。

From the Bell Labs perspective, by 1968 it was clear that although Multics was a good computing environment for the handful of people that it supported, it was not going to achieve its goal of being an information utility that would provide computing services for the Labs at any reasonable cost; it was just too expensive. Accordingly Bell Labs dropped out of the project in April 1969, leaving MIT and GE to soldier on.

> 从贝尔实验室的角度来看，到 1968 年，虽然 Multics 是一个很好的计算环境，可以支持少数人，但它还没有实现它的目标，即以合理的成本为实验室提供计算服务的信息公用事业，它太昂贵了。因此，贝尔实验室于 1969 年 4 月退出了该项目，剩下麻省理工学院和通用电气继续奋战。

Multics was eventually completed, or at least declared a success. It was supported and used until 2000, though not widely. Multics was the source of many really good ideas, but its most lasting contribution was entirely unan-ticipated: its influence on a tiny operating system called Unix that was created in part as a reaction to the complexity of Multics.

> 多西斯最终被完成，或者至少被宣布为一个成功。它被支持和使用到 2000 年，虽然没有得到广泛使用。多西斯是许多非常好的想法的来源，但它最持久的贡献完全是出乎意料的：它对一个叫做 Unix 的微小操作系统的影响，该操作系统部分是作为对多西斯复杂性的反应而创建的。

**2.3 The origin of Unix**

When Bell Labs pulled out of Multics, the people who had been working on it had to find something else to do. Ken Thompson (Figure 2.2) still wanted to work on operating systems, but upper management at the Labs had been burned by the Multics experience and had no interest in buying hardware for another operating system project. So Ken and others spent time exploring ideas and doing paper designs for various operating system components, though with no concrete implementations.

> 当贝尔实验室从 Multics 退出时，那些一直在其上工作的人们不得不寻找其他事情做。肯·汤普森(图 2.2)仍然想继续研究操作系统，但实验室的上层管理人员已经因 Multics 的经历感到烧伤，对购买另一个操作系统项目的硬件没有兴趣。因此，肯和其他人花时间探索各种操作系统组件的想法和纸质设计，但没有具体的实现。

Around this time, Ken found a little-used DEC PDP-7, a computer whose main purpose was as an input device for creating electronic circuit designs.

> 大約在這個時候，Ken 發現了一台很少使用的 DEC PDP-7，這台電腦的主要用途是作為用於創建電子電路設計的輸入設備。

[]{#index_split_000.html#p47}![](./index-47_1.jpg){.calibre4}

CHAPTER 2: PROTO-UNIX 33

**Figure 2.2:**

Ken Thompson, ∼1981 (Courtesy of Gerard Holzmann) The PDP-7 was first shipped in 1964 and computers were evolving quickly, so by 1969 it was dated. The machine itself wasn't very powerful, with only 8K 18-bit words of memory (16K bytes), but it had a nice graphics display, so Ken wrote a version of a space-travel game to run on it. A player could wander through the solar system and land on different planets. It was mildly addictive and I spent hours playing with it.

> 肯·汤普森(Ken Thompson)于 1981 年(由杰拉德·霍尔茨曼(Gerard Holzmann)提供)，PDP-7 最早于 1964 年发货，计算机正在迅速发展，因此到 1969 年它已经过时了。机器本身不是很强大，只有 8K 18 位字的内存(16K 字节)，但它有一个很好的图形显示器，因此肯在上面编写了一个太空旅行游戏的版本。玩家可以穿梭于太阳系，登陆不同的行星。它有点让人上瘾，我花了几个小时玩它。

The PDP-7 had another interesting peripheral, a very tall disk drive with a single vertical platter. Credible folklore held that it was potentially danger-ous to stand in front of it in case something broke. The disk was too fast for the computer. This presented an interesting problem, and Ken wrote a disk scheduling algorithm that would try to maximize throughput on any disk, but particularly this one.

> PDP-7 有另一個有趣的外圍設備，一個非常高的磁碟機，只有一個垂直的碟片。可信的民間傳說說站在它前面可能會有危險。磁碟機的速度太快了，這帶來了一個有趣的問題，肯尼寫了一個磁碟調度演算法，試圖在任何磁碟機上最大限度地提高吞吐量，特別是這個磁碟機。

Now the question was how to test the algorithm. That required loading the disk with data, and Ken decided that he needed a program to put data on it in quantity.

> 现在的问题是如何测试算法。这需要将磁盘加载数据，肯决定他需要一个程序来大量地将数据放在上面。

"At some point I realized that I was three weeks from an operating system." He needed to write three programs, one per week: an editor, so he could create code; an assembler, to turn the code into machine language that could run on the PDP-7; and a "kernel overlay---call it an operating system."

> 在某个时刻，我意识到距离操作系统只有三周的时间。他需要编写三个程序，每周一个：一个编辑器，以便他可以创建代码；一个汇编器，将代码转换为可在 PDP-7 上运行的机器语言；以及一个“内核叠加层——称之为操作系统”。

Right at that time, Ken's wife went on a three-week vacation to take their one-year-old son to visit Ken's parents in California, and Ken had three weeks to work undisturbed. As he said during a 2019 interview, "One week,

> 正在那时，肯的妻子出去度三个星期的假，带着他们一岁的儿子去加利福尼亚拜访肯的父母，肯有三个星期可以安静地工作。正如他在 2019 年的一次采访中所说：“一个星期，

[]{#index_split_000.html#p48}34 CHAPTER 2: PROTO-UNIX

one week, one week, and we had Unix." By any measure, this is real software productivity.

> 一周，一周，我们有了 Unix。以任何衡量标准，这都是真正的软件生产力。

A couple of years after Ken and I had both retired from Bell Labs, I asked him about the story that he had written the first version of Unix in three weeks. Here, verbatim, is his email response, which is completely consistent with the much more recent interview:

> 几年后，肯和我都从贝尔实验室退休后，我问他有关他用三周写出第一个 Unix 版本的故事。以下是他的电子邮件回复，完全符合最近的采访：

Date: Thu, 9 Jan 2003 13:51:56 -0800

unix was a file system implementation to test thruput and the like.

once implemented, it was hard to get data to it to load it up.

i could put read/write calls in loops, but anything more sophisticated was near impossible.

> 我可以在循环中放置读/写调用，但任何更复杂的操作几乎是不可能的。

that was

the state when bonnie went to visit my parents in san diego.

i decided that it was close to a time sharing system, just lacking an exec call, a shell, an editor, and an assembler.

> 我决定它接近一个时间共享系统，只是缺少了一个 exec 调用，一个 shell，一个编辑器和一个汇编器。

(no compilers) the exec call was trivial and the other 3

were done in 1-week each - exactly bonnie's stay.

the machine was 8k x 18 bits.

4k was kernel and 4k was

swapped user.

ken

This first version of a recognizable Unix system was running in mid to late 1969, so it seems reasonable to say that's when Unix was born.

> 这个可认出的 Unix 系统的第一个版本是在 1969 年中期至下期运行的，因此可以合理地说 Unix 诞生了。

The early system had a small group of users: Ken and Dennis, of course, plus Doug McIlroy, Bob Morris, Joe Ossanna, and through a bit of blind luck, me. Each user had a numeric user id. Some of these ids corresponded to system functions, not to human users---the root or super-user was id 0, and there were a couple of other special cases. Ids for real users started around 4.

> 早期的系统有一小群用户：当然是肯和丹尼斯，还有道格·麦克伊尔罗伊、鲍勃·莫里斯、乔·奥桑纳，还有我，这是一种运气的结晶。每个用户都有一个数字用户 ID。其中一些 ID 对应的是系统功能，而不是人类用户——超级用户的 ID 是 0，还有其他一些特殊情况。真正用户的 ID 从 4 开始。

I think that Dennis was 5, Ken was 6, and mine was 9. There must be some cachet in having a single-digit user id on the original Unix system.

> 我认为丹尼斯是 5，肯是 6，我是 9。在原始 Unix 系统上有单位数字的用户 ID 一定有一些特权。

**2.4 What's in a name?**

Sometime during these early days the new PDP-7 operating system acquired a name, though the details are murky.

> 在早期的某个时候，新的 PDP-7 操作系统获得了一个名字，但细节不清楚。

I hav e a memory of standing in my office doorway, talking with a group that probably included at least Ken, Dennis and Peter Neumann. The system had no name at that point, and (if memory serves) I suggested, based on Latin roots, that since Multics provided "many of everything" and the new system had at most one of anything, it should be called "UNICS," a play on

> 我记得站在办公室门口，和一群人聊天，其中肯定包括肯、丹尼斯和彼得·纽曼。当时系统还没有名字，如果我没记错的话，我建议根据拉丁根源，由于 Multics 提供“许多一切”，而新系统至多只有一样，它应该被称为“UNICS”，一种对 Multics 的取笑。

"uni" in place of "multi."

[]{#index_split_000.html#p49}CHAPTER 2: PROTO-UNIX 35

An alternative memory is that Peter Neumann came up with the name UNICS, for "UNiplexed Information and Computing Service." As Peter recalls,

> 另一种记忆是彼得·纽曼想出了 UNICS 的名字，代表"UNiplexed 信息和计算服务"。正如彼得回忆的那样：

"I remember vividly that Ken came in one morning for lunch and said that overnight he had written a thousand-line one-user OS kernel for the PDP-7 that Max Matthews had lent him. I suggested that he should make it a multi-user system, and sure enough the next day he came in for lunch having written another thousand lines with a multi-user kernel. It was the one-user kernel that prompted the 'castrated Multics' concept of UNICS."

> 我清楚地记得肯在一个早晨来吃午饭时说，他在一夜之间为马克斯·马修斯借给他的 PDP-7 编写了一个一个用户的操作系统内核，一千行代码。我建议他应该把它变成一个多用户系统，果然第二天他来吃午饭时，又写了另外一千行代码，搞出了一个多用户内核。正是这个一个用户的内核促成了"被割除的 Multics"概念，也就是 UNICS。

Peter has graciously said that he doesn't recall further specifics, and so, deservedly or not, I have gotten credit for coining the name.

> 彼得大方地表示他不记得更多的细节，因此，无论是否应得，我都得到了创造这个名字的荣誉。

Either way, UNICS somehow mutated into Unix, which was clearly a much better idea. (It was rumored that AT&T lawyers did not like "Unics"

> 不管怎样，UNICS 不知怎的变成了 Unix，显然是一个更好的想法。(有传言说，AT&T 的律师不喜欢"Unics")

because of its similarity to "eunuchs.") Dennis Ritchie subsequently characterized the name as "a somewhat treacherous pun on Multics," which indeed it is.

> 由于它与“太监”的相似性，丹尼斯·里奇随后将其称为“多拉诺斯的一个有些危险的双关语”，的确如此。

**2.5 Biography: Ken Thompson**

In May 2019, Ken and I had an informal "fireside chat" at the Vintage Computer Festival East in Wall, New Jersey. My role was to ask a few leading questions, then sit back and listen. Some of the material here is paraphrased from that event, which can be found on YouTube.

> 五月 2019 年，肯和我在新泽西州沃尔的复古电脑节上进行了一次非正式的“炉边聊天”。我的角色是提几个引导性问题，然后坐下来倾听。这里的一些材料是从那次活动中概括出来的，可以在 YouTube 上找到。

Ken was born in 1943. His father was in the US Navy, so Ken spent significant parts of his childhood living in different parts of the world, including California, Louisiana, and a few years in Naples.

> 肯出生于 1943 年。他的父亲在美国海军服役，所以肯在不同的地方度过了他童年的大部分时间，包括加利福尼亚州、路易斯安那州，以及在那不勒斯度过的几年。

He grew up interested in electronics, and went to the University of California at Berkeley to study electrical engineering. He said that he found the electronics part really easy because it had been his hobby for 10 years before college. At Berkeley, he discovered the field of computing.

> 他从小就对电子学感兴趣，因此去加州大学伯克利分校学习电子工程。他说，他发现电子学部分很容易，因为在上大学之前他已经玩这个爱好 10 年了。在伯克利，他发现了计算机领域。

"I consumed computers, I loved them. At that time, there was no computer science curriculum at Berkeley; it was being invented.

> 我消耗了电脑，我喜欢它们。当时，伯克利没有计算机科学课程，它正在被发明。

I was drifting along the summer after I graduated. \[Graduation\] was a surprise because I didn't know that I had gotten all the requirements.

> 我毕业后的夏天漂浮着，[毕业]出乎我的意料，因为我不知道自己已经满足了所有的要求。

I was just going to stay in the university because \... I owned it. My fin-gers were in absolutely everything. The main monster computer at the

> 我本来只是打算留在大学，因为我拥有它。我的手指参与到了所有的事情中。主要的怪物电脑就在那里。

[]{#index_split_000.html#p50}36 CHAPTER 2: PROTO-UNIX

university shut down at midnight and I'd come in with my key and I'd open it up and it would be my personal computer until 8 AM.

> 大学在午夜关闭，我用钥匙进来，打开它，它将是我的个人电脑直到上午 8 点。

I was happy. No ambition. I was a workaholic, but for no goal."

In his final year, Ken audited a course taught by Elwyn Berlekamp, a Berkeley professor who soon afterwards went to Bell Labs. In the summer after graduating, Ken didn't apply for grad school because he didn't think he was good enough.

> 在他最后一年，肯参加了伯克利教授埃尔温·伯勒坎普(Elwyn Berlekamp)教授的课程。在毕业后的夏天，肯没有申请研究生，因为他认为自己不够好。

"Tow ards the end of the summer, \[Berlekamp\] said 'Here's your classes for grad school.' He had applied for me and I got accepted!"

> 夏末的时候，伯勒坎普说：“你的研究生课程开始了。”他为我申请了，我被接受了！

When Ken finished his MS at Berkeley in 1966, Bell Labs was among several companies that tried to recruit him, but he explicitly said that he didn't want to work for a company.

> 当肯在 1966 年完成他在伯克利的硕士学位时，贝尔实验室是试图招募他的几家公司之一，但他明确表示他不想为公司工作。

The recruiter kept trying. As Ken says, "I skipped maybe 6 or 8 recruiting attempts by Bell Labs---again, no ambition. The Bell Labs recruiter came and knocked on my door at home. I invited him in; his story is that I offered him ginger snaps and beer." (This must be part of some odd California diet.)

> 招聘人员一直在努力。正如肯·说的，“我跳过了贝尔实验室大约六到八次招聘尝试——又一次没有雄心壮志。贝尔实验室的招聘人员来到我家门口敲门，我邀请他进来，他的故事是我给他提供了姜饼和啤酒。(这一定是加州奇怪的饮食习惯。)

Finally, Ken agreed to come to New Jersey at Bell Labs' expense, but only for a day, and primarily to visit friends from high school days. But when he arrived at Bell Labs, he was impressed by the names he saw:

> 最后，肯同意以贝尔实验室的费用前往新泽西，但只有一天，主要是去拜访高中时代的朋友。但当他到达贝尔实验室时，他对所看到的名字感到印象深刻。

"The very first thing I did was walk down the corridor of computer science research and every name on the doors on the way down, I knew.

> 我做的第一件事就是沿着计算机科学研究的走廊走，一路上的每一扇门上的名字我都认识。

It was just shocking. I was interviewed by two amazing people \... one was Shen Lin.

> 这真是太惊人了。我被两个了不起的人采访——其中一个是沈林。

I got in my rent-a-car after the day. Somehow they tracked me, and there was an offer waiting at like the third stop down the east coast. I picked up the offer and drove it from one stop to another, which was maybe two hours, thinking about it, and when I got to the next friend's house, I called them and said OK."

> 我租了一辆车，第二天就开上路了。不知怎么的，他们跟踪到了我，在东海岸的第三站有一个报价等着我。我接了报价，开车从一站到另一站，大概花了两个小时。当我到达朋友家时，我打电话给他们说“好”。

Ken arrived at Bell Labs in 1966 and started work on Multics, then on Unix as described earlier, so I won't repeat that here.

> 1966 年，Ken 来到贝尔实验室，开始着手开发 Multics，然后是如前所述的 Unix，所以我不在这里重复了。

Ken had a long-standing interest in games, and was a chess enthusiast as a kid. He didn't like to lose but at the same time, when he won he felt bad for his opponent, so eventually he became a spectator only. In 1971, he wrote a chess playing program for the PDP-11. This was promising enough that he began to build special-purpose hardware to speed up computation, for

> 肯在游戏上有着长久的兴趣，小时候是个象棋爱好者。他不喜欢输，但同时，当他赢了的时候，他会为对手感到难过，所以最后只能成为一个旁观者。1971 年，他为 PDP-11 编写了一个象棋游戏程序。这太有希望了，他开始建立专用硬件来加速计算。

[]{#index_split_000.html#p51}![](./index-51_1.jpg){.calibre4}

CHAPTER 2: PROTO-UNIX 37

example to generate legal moves from a given position. Eventually this culminated in Belle (Figure 2.3), the chess-playing computer that he and Joe Condon evolved from 1976 through 1980.

> 例如，从给定位置生成合法着法。最终，他和乔·孔登(Joe Condon)从 1976 年至 1980 年不断演变，最终形成了象棋计算机 Belle(图 2.3)。

**Figure 2.3:**

Ken Thompson and Joe Condon (Computer History Museum) Belle (Figure 2.4) had a successful career. It was the first computer to become a chess master, a rating of 2200 in regular tournament play against human opponents, and it won the 1980 World Computer Chess championship and several ACM computer chess tournaments before retiring to the Smithso-nian Institution.

> 肯·汤普森和乔·孔登(计算机历史博物馆)的贝尔(图 2.4)职业生涯非常成功。它是第一台成为国际象棋大师的计算机，在与人类对手的定期比赛中获得 2200 分的评分，并在 1980 年世界计算机国际象棋锦标赛和几次 ACM 计算机国际象棋比赛中获胜，之后退休到史密森尼学会。

Dennis Ritchie wrote a short article for the International Computer Chess Association on Ken Thompson's activities with various games: _[www.belllabs.com/usr/dmr/www/ken-games.html](http://www.belllabs.com/usr/dmr/www/ken-games.html)_. It shows Ken's breadth of game interests, well beyond just chess. There is also a description of Belle's win over Blitz 6.5 at the ACM computer chess championship on December 5, 1978, with comments from Monty Newborn, a computer chess pioneer, and International Master David Levy:

> Dennis Ritchie 为国际计算机国际联盟写了一篇关于 Ken Thompson 在各种游戏中的活动的短文：_[www.belllabs.com/usr/dmr/www/ken-games.html](http://www.belllabs.com/usr/dmr/www/ken-games.html)_。它显示了肯的游戏兴趣的广度，远远超出了国际象棋。还有一个关于贝尔在 1978 年 12 月 5 日 ACM 计算机国际象棋锦标赛中击败 Blitz 6.5 的描述，以及计算机国际象棋先驱蒙蒂·纽博恩和国际大师戴维·利维的评论：

1\. e4 e5 2. Nf3 Nc6 3. Nc3 Nf6 4. Bb5 Nd4 5. Bc4 Bc5 6. Nxe5 Qe7

[]{#index_split_000.html#p52}![](./index-52_1.jpg){.calibre4}

38 CHAPTER 2: PROTO-UNIX

**Figure 2.4:**

Belle chess computer (Courtesy of Computer History Museum) 7. Bxf7+ Kf8 8. Ng6+ hxg6 9. Bc4 Nxe4 10. O-O Rxh2!! 11. Kxh2

> 7. Bxf7+ Kf8 8. Ng6+ hxg6 9. Bc4 Nxe4 10. O-O Rxh2!! 11. Kxh2

1. Bxf7+ Kf8 8. Ng6+ hxg6 9. Bc4 Nxe4 10. O-O Rxh2!! 11. Kxh2
   美丽象棋电脑(敬赠计算机历史博物馆)7. Bxf7+ Kf8 8. Ng6+ hxg6 9. Bc4 Nxe4 10. O-O Rxh2!! 11. Kxh2

{hastening the loss} Qh4+ 12. Kg1 Ng3 13. Qh5 {ineffectual delay}

gxh5 14. fxg3+ Nf3# {perhaps uniquely blocking a check, giving a double check and mating simultaneously; "the most beautiful combination created by a computer program to date\... computer chess wit-nessed the start of a new era."}

> 谷克斯 5 14. 法克斯 3+ 纳夫 3#(可能是唯一阻止检查，同时双重检查和互相杀死；“迄今为止，由计算机程序创造的最美丽的组合。...计算机国际象棋见证了一个新时代的开始。”)

Chess games end with a win, loss or draw. The 50-move rule says that a player can claim a draw if there have been 50 moves without a capture or a pawn move; this prevents one player from just playing on when there is no way to force a win.

> 国际象棋游戏以胜利、失败或和棋结束。50 步规则规定，如果 50 步内没有发生吃子或者兵步，玩家可以宣布和棋；这样可以防止一方继续走棋，而另一方无法取胜。

Ken decided explore the question of whether 50 moves is the right number. He used Belle and some sophisticated database organization to evaluate all four- and five-piece endgames and discovered that some were winnable in more than 50 moves, given optimal play. By this time, Ken was well known in the chess world, and sometimes grandmasters would show up at the Labs to try their hand against Belle, particularly for endgames. I met world champions Anatoly Karpov and Vishy Anand just by being around on the right weekends.

> 肯决定探索 50 步是否是正确的数字的问题。他使用贝尔和一些复杂的数据库组织来评估所有四和五件结局，发现有些在给定最佳游戏的情况下，可以在 50 步以上获胜。到这个时候，肯在国际象棋界已经很有名气，有时大师会出现在实验室，试着对抗贝尔，尤其是结局时。我通过在正确的周末出现，认识了世界冠军阿纳托利·卡尔波夫和维希·阿南德。

Ken was also an avid pilot, and regularly flew himself and guests around New Jersey, starting from the airport in Morristown. He got other members

> 肯也是一位熱心的飛行員，經常自己駕駛飛機把客人帶到新澤西州，從莫里斯敦機場出發。他還邀請其他成員一起飛行。

[]{#index_split_000.html#p53}![](./index-53_1.jpg){.calibre4}

CHAPTER 2: PROTO-UNIX 39

of 1127 interested in flying as well, and at peak there were half a dozen private pilots in the "1127 air force." This group used to set off to view fall foliage or fly to some interesting place for lunch. Doug McIlroy recalls:

> 1127 人也对飞行感兴趣，在高峰时期，"1127 空军"中有半打私人飞行员。这个小组经常出发去观赏秋叶或者飞到一些有趣的地方吃午餐。道格·麦克尔罗伊回忆道：

"Besides fall foliage in New England, the air force attended an eclipse in the Adirondacks, thanks to Ken's piloting and Rob Pike's tele-scopes. There was also a flight to observe a transit of Mercury. The astronomical theme in the Unix crew beg an with Joe Ossanna's azel, which had controlled the Telstar ground station, and we used to tell us where to find artificial satellites. Next came Bob Morris's sky program, then Ken's celestial event predictor, Lee McMahon's star maps made with my map program, and finally Rob's scat star catalog."

> 除了新英格兰的秋叶，空军还参加了阿迪朗德克斯的日食，这要归功于肯的飞行技术和罗布·派克的望远镜。还有一次飞行观测水星的过境。Unix 小组的天文主题始于乔·奥萨纳的 azel，它曾控制过 Telstar 地面站，我们曾经用它来告诉我们去哪里寻找人造卫星。接下来是鲍勃·莫里斯的天空计划，然后是肯的天文事件预测，李·麦克马洪的星图是用我的地图程序制作的，最后是罗布的 scat 星表。

In December 1992, Ken and Fred Grampp went to Moscow to fly a MiG-29, a step up from their normal Cessnas. Figures 2.5 and 2.6 show Ken ready to go and taxiing back after a flight.

> 在 1992 年 12 月，肯和弗雷德·格兰普去莫斯科乘坐米格-29(比他们平时乘坐的切斯纳飞机更高级)。图 2.5 和 2.6 显示肯准备出发和飞行后停在停机坪上的情景。

**Figure 2.5:**

Ken Thompson preparing to take off (Courtesy of cat-v.org) Ken and I retired from Bell Labs at the end of 2000. I went to Princeton, and he joined Entrisphere, a startup founded by Bell Labs colleagues. In 2006, he moved to Google, where with Rob Pike and Robert Griesemer, he created the Go programming language. I heard about his move from

> 陈汤普森准备起飞(由 cat-v.org 提供)2000 年底，我和他都从贝尔实验室退休了。我去了普林斯顿，他加入了由贝尔实验室同事创立的 Entrisphere 初创公司。 2006 年，他搬到了谷歌，与 Rob Pike 和 Robert Griesemer 一起，他创建了 Go 编程语言。我听说他的搬迁。

[]{#index_split_000.html#p54}![](./index-54_1.jpg){.calibre4}

40 CHAPTER 2: PROTO-UNIX

**Figure 2.6:**

Ken taxiing after a flight (Courtesy of cat-v.org) Entrisphere to Google from someone else, so I asked for confirmation. His reply:

> 我从别人那里从 Entrisphere 订了一辆出租车，所以我要求确认。他的回复是：

Date: Wed, 1 Nov 2006 16:08:31 -0800

Subject: Re: voices from the past

its true. i didnt change the median age of google much, but i think i really shot the average.

> 是的，我没有改变谷歌的平均年龄太多，但我认为我真的提高了平均水平。

ken

[]{#index_split_000.html#p55}Chapter 3

**First Edition (1971)**

"This manual gives complete descriptions of all the publicly available features of Unix. It provides neither a general overview (see "The Unix Time-sharing System" for that) nor details of the implementation of the system (which remain to be disclosed)."

> 这本手册提供了 Unix 可公开使用的各项功能的完整描述。它既不提供一般概述(参见《Unix 时间共享系统》)，也不提供系统实现的细节(这些仍有待公开)。

First Edition Unix Programmer's Manual, November 3, 1971

"BUGS: rm probably should ask whether a read-only file is really to be removed."

> "BUG：rm 可能应该询问只读文件是否真的要被删除。"

Section of manual page for rm command, November 3, 1971

The PDP-7 Unix system was interesting enough that people were starting to use it, even though it ran on a tiny computer and didn't hav e a lot of software. Still, it was clearly useful and had become the preferred computing environment for a small group who found it more fun and productive than the big central computer. Thus Ken Thompson, Dennis Ritchie and others began to lobby for a larger computer that would support more users and enable more interesting research.

> PDP-7 Unix 系统很有趣，即使它在一台微型计算机上运行而且没有很多软件，人们也开始使用它。尽管如此，它显然是有用的，已经成为一小群人更喜欢和更有效率的首选计算环境。因此，Ken Thompson、Dennis Ritchie 和其他人开始游说更大的计算机，以支持更多的用户和实现更有趣的研究。

One of the early proposals was for the purchase of a DEC PDP-10, which was popular at universities and other research labs. The PDP-10 was loosely similar to the IBM 7090, with 36-bit words like the 7090 and the GE 635 and 645, and it had a great deal more horsepower than the wimpy little PDP-7.

> 一个早期的提议是购买一台 DEC PDP-10，它在大学和其他研究实验室中很受欢迎。PDP-10 与 IBM 7090 类似，有像 7090 和 GE 635 和 645 一样的 36 位字，它的性能比微弱的 PDP-7 强得多。

But it would also cost much more; the proposal was for half a million dollars.

> 但这也会花费更多；提案是五百万美元。

The Multics experience was an all-too-recent bad memory, so the PDP-10

proposal never got off the ground. As Ken said, the management position was "We don't do operating systems," though perhaps it was more like

> 提案从未落实。正如肯所说，管理层的立场是“我们不做操作系统”，尽管也许是更像是

"We're not going to give you a lot of money for a big machine."

[]{#index_split_000.html#p56}42 CHAPTER 3: FIRST EDITION

I suppose that it could be argued that one positive role of management is to be cautious most of the time, so that people who want resources are forced to hone their proposals and focus their pitches. If resources are tight, that's more likely to lead to good, well-thought-out work than if there are no constraints.

> 我认为，管理的一个积极作用就是大多数时候要谨慎，这样希望获得资源的人就被迫提炼他们的提案，集中他们的努力。如果资源有限，这比没有限制的情况下更有可能产生出良好、经过深思熟虑的工作。

In any case, the Unix group came up with another idea, to acquire a new minicomputer that DEC had just announced, the PDP-11, which would cost more like \$65,000 than \$500,000 in 1971 dollars.

> 在任何情况下，Unix 小组想出了另一个主意，购买 DEC 刚刚宣布的新迷你计算机 PDP-11，1971 年的价格接近 65000 美元，而不是 500000 美元。

This was rejected too. A remark from Sam Morgan in Mike Mahoney's 1989 oral history interview explains some of the reasoning:

> 这也被拒绝了。萨姆·摩根在迈克·马奥尼 1989 年的口述历史采访中的一句话解释了一些原因：

"The management principles here are that you hire bright people and you introduce them to the environment, and you give them general directions as to what sort of thing is wanted, and you give them lots of freedom. Doesn't mean that you always necessarily give them all the money that they want. And then you exercise selective enthusiasm over what they do. And if you mistakenly discourage or fail to respond to something that later on turns out to be good, if it is really a strong idea, it will come back."

> 这里的管理原则是，你雇佣聪明的人，让他们熟悉环境，给他们大致的指示，让他们拥有很大的自由。这并不意味着你总是给他们他们想要的所有资金。然后你会对他们的工作表现出选择性的热情。如果你错误地打击或没有回应后来被证明是好的想法，如果它真的是一个很强的想法，它会再次回来。

In hindsight, being forced to work within constraints was a good thing.

As Ken himself said in his 1983 Turing Award lecture,

"Unix swept into popularity with an industry-wide change from central mainframes to autonomous minis. I suspect that Daniel Bobrow would be here instead of me if he could not afford a PDP-10 and had had to 'settle' for a PDP-11."

> Unix 因业界从中央大型机转向独立小型机而迅速流行起来。如果丹尼尔·鲍布罗无法负担得起 PDP-10 而只能“勉强”使用 PDP-11，我想他会在这里而不是我。

(Daniel Bobrow was the primary author of the Tenex operating system, which was written for the PDP-10 in 1969.) **3.1 Unix for patent applications**

> 丹尼尔·鲍布罗(Daniel Bobrow)是 1969 年为 PDP-10 编写的 Tenex 操作系统的主要作者。3.1 Unix 用于专利申请。

Direct appeals for a machine failed, but there was an alternative. Bell Labs, as a large and productive scientific research operation, generated a lot of patent applications. At that time, it was being granted an average of almost one patent per day. Patent applications were text documents but with some rigid format requirements, like line-numbered pages. No existing computer system could handle these oddities, so the Patent department was planning to buy hardware from a company which promised software that would ev entually produce applications in the proper format, though it could not do numbered lines at the time.

> 直接要求一台机器失败了，但有一个替代方案。贝尔实验室作为一个大型和高效的科学研究机构，申请了大量专利。当时，它平均每天获得一项专利。专利申请书是文本文件，但有一些严格的格式要求，如行号页面。当时没有现有的计算机系统可以处理这些奇怪的东西，因此专利部门计划从一家公司购买硬件，该公司承诺最终能够以正确的格式生成申请，尽管当时不能处理编号行。

[]{#index_split_000.html#p57}CHAPTER 3: FIRST EDITION

43

Joe Ossanna came up with another plan. The Patent department would use a PDP-11 for preparing patent applications; the Unix group would write the necessary software for them, complete with a formatting program that would print applications in the proper format; and no, no one would be working on operating systems.

> 乔·奥桑纳提出了另一个计划。专利部门将使用 PDP-11 准备专利申请；Unix 小组将为他们编写必要的软件，包括一个格式化程序，可以以正确的格式打印申请；不，没有人会在操作系统上工作。

This combination of ideas slalomed around any residual management objections. Money for a PDP-11 came from Max Matthews, the director of the Speech and Acoustics Research Center. Max was supportive because one of his departments heads, Lee McMahon, was very interested in text processing and along with Ossanna was a promoter of the plan.

> 这种想法的组合绕开了任何残留的管理异议。PDP-11 的资金来自 Max Matthews，语音和声学研究中心的主任。Max 支持，因为他的一个部门主管 Lee McMahon 非常感兴趣文本处理，与 Ossanna 一起推动了这个计划。

The deal was approved, a PDP-11 was purchased, and Ken and Dennis quickly converted the PDP-7 version of Unix to run on it. The PDP-11 was a limited machine, with only 24K bytes of primary memory and a half-megabyte disk. The implementation used 16K bytes for the operating system and the remaining 8K for user programs.

> 交易已获批准，已购买了一台 PDP-11，肯和丹尼斯迅速将 PDP-7 版本的 Unix 转换为在其上运行。PDP-11 是一台有限的机器，只有 24K 字节的主存储器和半兆字节的磁盘。该实现使用 16K 字节用于操作系统，剩下的 8K 字节用于用户程序。

Joe Ossanna wrote a program called Nroff ("new roff"), analogous to the existing Roff text formatter, that was able to print patent applications in the required format. By the last half of 1971 typists were cranking out patent applications on Unix full time. Chapter 5 has much more to say about text formatting, since it was a major part of the Unix story in the 1970s.

> 乔·奥桑纳(Joe Ossanna)编写了一个名为 Nroff(“新的 roff”)的程序，类似于现有的 Roff 文本格式化程序，可以以所需的格式打印专利申请。到 1971 年下半年，打字员已经全职在 Unix 上打印专利申请了。第 5 章有更多关于文本格式化的内容，因为它是 20 世纪 70 年代 Unix 故事的一个重要组成部分。

That was during the day. At night, Ken, Dennis, and others were developing software on the same PDP-11. Development had to be done at night so as not to interfere with the typists, and it had to be careful. The PDP-11 had no hardware protection mechanisms to keep programs from interfering with each other or with the operating system, so a careless mistake could easily crash the system, and an error in the file system could lose everyone's work.

> 那是白天的事情。晚上，肯、丹尼斯和其他人在同一台 PDP-11 上开发软件。开发必须在晚上进行，以免干扰打字员，而且必须非常小心。PDP-11 没有硬件保护机制来防止程序相互干扰或与操作系统相互干扰，因此一个粗心的错误可能会轻易地使系统崩溃，而文件系统中的错误可能会使每个人的工作都丢失。

But the experience was so successful that the patent department bought another PDP-11 for the Unix group, and that made it possible to do development full time. This version became the first edition of Unix.

> 但是经验非常成功，专利部门为 Unix 组购买了另一台 PDP-11，这使得可以全职开发。这个版本成为了 Unix 的第一版。

Figure 3.1 is a 1972 public-relations picture of Ken Thompson and Dennis Ritchie using a PDP-11 running an early version of Unix. The computer itself is apparently a specific model called a PDP-11/20. The smallish round objects at about head level are DECtapes, which were magnetic tape devices that held 144K 18-bit words. Individual blocks could be read and written, so they could serve as temporary slow but reliable disks; the tapes themselves were removable, so they were used for backup as well.

> 图 3.1 是 1972 年 Ken Thompson 和 Dennis Ritchie 使用一台运行早期 Unix 版本的 PDP-11 的公共关系照片。计算机本身显然是一种叫做 PDP-11/20 的特定型号。头部大约水平位置的小圆物体是 DECtapes，它们是一种磁带设备，容量为 144K 18 位字。可以读取和写入单个块，因此它们可以作为慢速但可靠的磁盘使用；磁带本身是可移动的，因此可以用于备份。

Ken is typing at a Model 33 Teletype, a sturdy but slow and noisy device, basically a computer-controlled electro-mechanical typewriter that could only print in upper case, at 10 characters per second. The Model 33 dates from 1963 but earlier versions had been in widespread use since the early 1930s.

> 肯在一台 Model 33 Teletype 上打字，这是一种坚固但速度缓慢而嘈杂的设备，基本上是一种由计算机控制的机械式打字机，只能以大写字母打印，每秒 10 个字符。Model 33 号产品始于 1963 年，但早期版本自 1930 年代以来就已经广泛使用。

[]{#index_split_000.html#p58}![](./index-58_1.jpg){.calibre4}

44 CHAPTER 3: FIRST EDITION

Teletype Corporation was a part of AT&T, and Teletypes were widely used throughout the Bell System and elsewhere for sending messages, and later for connecting to computers. Whatever was typed on the Teletype keyboard was sent to the computer, and responses were printed (in upper case) on a long roll of paper; the tops of the paper rolls are just visible in the picture.

> 电传公司是 AT&T 的一部分，电传机在整个 Bell 系统以及其他地方被广泛使用，用于发送消息，后来也用于连接计算机。电传键盘上输入的任何内容都会被发送到计算机，而响应则会以大写字母的形式打印在一张长长的纸卷上；图片中可以看到纸卷的顶部。

Arguably, one reason why many command names on Unix are short is that it took considerable physical force to type on a Model 33, and printing was slow.

> 可以说，Unix 上的许多命令名称短小是因为在 Model 33 上输入需要相当大的力量，而且打印速度很慢。

**Figure 3.1:**

Ken (seated) and Dennis at the PDP-11, ∼1972 (Wikipedia) Someone even built an experimental "portable" Model 33. The keyboard and printer were shoehorned into a suitcase-like container that in theory could be carried around, though at 55 pounds (25 kg) you wouldn't carry it far. (It had no wheels either.) It was connected to a remote computer through a dial-up phone connection and a built-in acoustic coupler: plug a telephone handset into a couple of rubber sockets and the coupler converted data into sound and back again, rather like a fax machine. I managed to haul one of these terminals home a couple of times, but calling it portable was too

> 肯(坐著)和丹尼斯在 PDP-11 上，大約 1972 年(維基百科)，有人甚至建造了一個實驗性的“便攜式”型號 33。鍵盤和打印機被擠進一個像手提箱一樣的容器中，理論上可以攜帶，但重 55 磅(25 公斤)你不會攜帶太遠。(它也沒有輪子。)它通過撥號電話連接和內置的聲音耦合器與遠程計算機連接：將電話听筒插入兩個橡膠插座，耦合器將數據轉換為聲音，再轉換回去，有點像傳真機。我設法將其中一個終端機拖回家兩次，但稱它為便攜式太過於簡單了。

[]{#index_split_000.html#p59}CHAPTER 3: FIRST EDITION

45

charitable.

Things improved markedly when the Model 37 Teletype came along. It had lower case letters as well as upper case, and was somewhat faster (15

> 事情在 Model 37 Teletype 出现后明显改善了。它不仅有大写字母，而且速度也更快(15)

characters per second rather than 10), though it was still strenuous to type on it. It had an extended typebox so it could print mathematical symbols, which was useful for the patent applications as well as our own technical papers, and it could roll the paper back and forth in half-line steps, which made mathematical subscripts and superscripts possible.

> 这台打字机每秒可以打出比 10 个字符更多的字符，但打字仍然很费力。它有一个扩展的打字框，可以打印数学符号，这对专利申请和我们自己的技术论文都很有用，它还可以把纸卷回来，每次半行，这使得数学下标和上标成为可能。

Feeding paper into it was also a challenge; it took real contortions to load a new box of fan-fold paper. Bob Morris once sent Joe Ossanna a mail message that consisted of 100 reverse line-feeds; when Joe tried to read the message, the Model 37 sucked the paper back out and deposited it on the floor.

> 把纸张放进去也是一个挑战；要加载一箱扇形纸张真的需要绞尽脑汁。鲍勃·莫里斯曾给乔·奥桑纳发送了一封由 100 个反向换行符组成的邮件；当乔试图阅读这封邮件时，模型 37 吸回纸张并将其放在地上。

Bob occupied the office across from me for a number of the early years.

"Robert Morris" was a common name at Bell Labs; indeed, there was a visitor named Robert Morris in the same office a few years later. So Bob frequently got misdirected mail, which he would dutifully send back, explaining that he was the wrong Morris. One piece of mail kept on coming, an elaborate blueprint from some other part of the company that said "Please initial and return." All attempts to head it off failed, so finally one day Bob did initial it and sent it back. It never appeared again.

> "罗伯特·莫里斯"在贝尔实验室很常见；事实上，几年后还有一位叫罗伯特·莫里斯的访客在同一个办公室。所以鲍勃经常会收到错发的邮件，他会认真地将其寄回去，解释说他不是那个莫里斯。有一封邮件一直收到，来自公司的另一部分，上面写着“请签字并回复”。所有试图把它拦下来的努力都失败了，所以最后一天鲍勃签了字并寄回去了。它再也没有出现过。

**3.2 The Unix room**

Although each Research MTS had a private office, much Unix development went on in a shared space called "the Unix room." Its actual location changed a couple of times over the years, but it was always a place to hang out, learn what was going on, contribute ideas, or just socialize.

> 尽管每个研究 MTS 都有一个私人办公室，但 Unix 开发大都在一个叫做“Unix 室”的共享空间里进行。它的实际位置随着时间的推移发生了一些变化，但它始终是一个可以闲逛、了解发生的事情、提出想法或者只是社交的地方。

The original Unix room was briefly on the fourth floor of Building 2

where the PDP-7 lived, but the main location for many years was on the sixth floor of Building 2 in room 2C-644. Building 2 only had five office floors.

> 在 PDP-7 的所在地，但多年来的主要地点是 2 号楼的六楼，2C-644 室。2 号楼只有五层办公楼。

The sixth floor was basically a service corridor: dingy, dimly lit and lined with storage areas holding dusty abandoned equipment in locked wire cages.

> 第六层基本上是一条服务走廊：阴暗、灯火昏暗，沿着被锁上的金属网笼围起来的储存区域，里面放着尘封的废弃设备。

At one end there was an open area with vending machines that offered appalling coffee and almost inedible pastries that fueled late-night programming, and there were a handful of enclosed spaces, one of which was the Unix room for at least a decade. It held the PDP-11; the picture of Ken and Dennis in Figure 3.1 was taken there. A few tables and chairs and some other terminals made it a good shared working area.

> 在一端有一片开放区域，里面有臭名昭著的咖啡机和几乎无法下咽的糕点，为深夜编程提供燃料，还有几个封闭的空间，其中一个是至少有十年之久的 Unix 室。里面有 PDP-11；图 3.1 中的肯和丹尼斯的照片就是在那里拍摄的。几张桌子和几把椅子，以及其他一些终端，使它成为一个很好的共享工作区。

One of the early non-1127 Unix enthusiasts was a very distinguished theoretical physicist, now deceased, who I will call "M--- L---." M--- L--- was

> 一位早期非 1127 Unix 热衷者是一位非常杰出的理论物理学家，现已故去，我称之为“M--- L---”。M--- L---是

[]{#index_split_000.html#p60}![](./index-60_1.jpg){.calibre4}

46 CHAPTER 3: FIRST EDITION

eager to use Unix, he was forward-thinking in his use of computers in physics, and he was a kind and generous person. But he would talk your ear off. Once he got started, there was no way to stop him, and you were in for an hour of one-way conversation. So someone scratched a small hole in the frosting of the door to the Unix room so we could peer in before entering, to see if he was there. It was called the "L--- hole."

> 他对 Unix 充满渴望，在计算机物理学方面的使用上非常前瞻，而且他是一个善良而慷慨的人。但是他会把你的耳朵聊死。一旦他开始了，就没有办法阻止他，你就要承受一小时的单向谈话。所以有人在 Unix 房间的门上刮了一个小洞，我们可以在进入前透过去看他是否在里面。这就叫做“L---洞”。

**Figure 3.2:**

Unix room espresso machine and coffee grinders At some point the Unix room migrated to room 2C-501, on the fifth floor at Stair 9, just around the corner from my office. It also acquired a variety of coffee machines, originally the usual carafes with a heater that kept the coffee warm until it burned (or the carafe did, something that happened regularly), and then a sequence of ever more expensive coffee grinders and espresso machines (Figure 3.2), the last of which cost something like \$3,000.

> 在某一时刻，Unix 室迁移到了位于 9 号楼梯五楼 2C-501 室，就在我办公室的拐角处。它还收购了各种咖啡机，最初是通常的加热壶，可以一直保持咖啡热直到烧焦(或者壶子烧焦，这种情况经常发生)，然后是一系列越来越昂贵的咖啡磨机和咖啡机(图 3.2)，其中最后一个大约花费了 3000 美元。

If my sources are right, Unix room denizens paid for the machine by passing the hat and management paid for the coffee.

> 如果我的消息源是正确的，Unix 室的居民通过传帽子来支付机器费用，管理层则支付咖啡费用。

The Unix room was just plain fun; there was always something going on.

Some people worked there almost exclusively and rarely used their offices.

> 一些人几乎专门在那里工作，很少使用他们的办公室。

Others would drop in multiple times a day for coffee and conversation. It's

> 他们会一天多次来喝咖啡聊天。

[]{#index_split_000.html#p61}CHAPTER 3: FIRST EDITION

47

hard to overstate how important the Unix room was for keeping up with what colleagues were doing, and for creating and maintaining a sense of community.

> 很难夸大 Unix 室对于跟上同事们正在做什么，以及创造和维持一种社区感的重要性。

In retrospect, I think that Bell Labs did a good job with space. Private offices, though they cost more than open areas, give people peace and quiet, a place to focus without constant noise in the background, storage for books and papers, and a door to close for intense thought or private conversations.

> 回想起来，我认为贝尔实验室在空间的使用上做得很好。私人办公室虽然比开放区域贵，但可以给人们带来安静、集中精力的空间，不受背景噪音的干扰，可以存放书籍和文件，还可以关上门，进行深入思考或私下交谈。

By now, I'v e spent enough time in open-plan work areas to know that, for me at least, they are utterly destructive of concentration. The Bell Labs mixture of one's own private office and a shared space for the community worked very well.

> 截至目前，我已经在开放式工作区花费了足够的时间，知道对我来说，它们完全破坏了集中精力。贝尔实验室将自己的私人办公室和共享空间结合起来，效果非常好。

The Labs also made it easy for people to keep on working at home in the ev ening. For many years, I had a dedicated phone line (after all, AT&T was the phone company) in my home that let me connect to the Unix systems at Murray Hill so I could work evenings and weekends. As an unexpected fringe benefit, there was a special access code that allowed us to make unlimited and unbilled long distance telephone calls to anywhere in the USA, which was rather a nice perk at a time when long distance calls cost actual money. Ken Thompson told me more on how this came to be:

> 实验室也使得人们在晚上在家里继续工作变得更容易。多年来，我在家里有一条专用电话线(毕竟，AT＆T 是电话公司)，让我可以连接到 Murray Hill 的 Unix 系统，以便我可以在晚上和周末工作。作为一个意外的额外好处，有一个特殊的接入码，允许我们在美国任何地方免费无限制地打长途电话，这在当时长途电话要花费实际费用的时候是一个不错的额外福利。肯·汤普森告诉我更多关于这是如何发生的：

"Joe Ossanna decided that we deserved home phone lines and tele-types. He invented a form to order them and made copies that he put in the stationery store room. He put himself down as the approver and then submitted several for the core Unix crowd. After several questioning telephone calls, Joe started getting the forms all filled out, which he approved. It was that simple, he just invented the form and it happened."

> 乔·奥桑纳决定我们应该有家庭电话线路和电传打字机。他发明了一种订购它们的表格，并复印出来放在文具室里。他把自己列为批准者，然后提交了几份给核心 Unix 群体。经过几次质疑的电话，乔开始把表格都填好了，他批准了。就是这么简单，他只是发明了这个表格，事情就发生了。

In 1985, Peter Weinberger was promoted to department head in 1127, and a professional photograph was taken for the company newspaper, the _Bell_ _Labs News_ (familiarly known as the _Bell Labs Good News_ since it only printed positive stories). In a serious tactical error, Peter left the original print of his headshot (Figure 3.3) in the Unix room.

> 1985 年，彼得·温伯格被提升为 1127 部门负责人，为公司报纸《贝尔实验室新闻》(俗称《贝尔实验室好消息》，因为它只刊登积极的新闻)拍摄了一张专业照片。彼得在 Unix 室里犯了一个严重的战术错误，把他的头像原片(图 3.3)留在了那里。

Soon his image was all over the place, sometimes filtered through the AT&T logo (Figure 3.4), which had recently been introduced. As Gerard Holzmann says,

> 不久，他的形象到处可见，有时会经过 AT&T 标志(图 3.4)的过滤，这个标志最近才推出。正如 Gerard Holzmann 所说，

"Within a few weeks after AT&T had revealed the new corporate logo, Tom Duff had made a Peter logo (Figure 3.5) that has since become a symbol for our center. Rob Pike had T-shirts made. Ken Thompson ordered coffee mugs with the Peter logo.

> 在 AT&T 公司公布新标志几周后，汤姆·达夫(Tom Duff)创作了彼得标志(图 3.5)，自那以后，它就成为我们中心的象征。罗布·派克(Rob Pike)印制了 T 恤衫。肯·汤普森(Ken Thompson)订购了印有彼得标志的咖啡杯。

[]{#index_split_000.html#p62}![](./index-62_1.jpg){.calibre4}

![](./index-62_2.jpg){.calibre4}

48 CHAPTER 3: FIRST EDITION

**Figure 3.3:**

Original Peter face (Courtesy of Gerard Holzmann) **Figure 3.4:**

AT&T "death-star" logo

Over the years, Peter's visage showed up in dozens of places---an organization chart with Peter faces all the way to the top, a large array of circular magnets on stairway walls, impressed in newly laid concrete floors, on microprocessor chips, and, most prominently, in the night of September 16, 1985, on one of the Bell Labs water towers (Figure 3.6).

> 这些年来，彼得的面容出现在很多地方：一张组织图上，彼得的脸在最上面；楼梯墙上的大堆圆形磁铁；新铺设的混凝土地板上的印记；微处理芯片上；最显眼的是在 1985 年 9 月 16 日的夜晚，出现在贝尔实验室的一个水塔上(见图 3.6)。

Rumors have circulated about who the painters were, but lips are still sealed more than three decades later. A reimbursement request for the paint was submitted, but it was rejected. In any case, within a couple of days the water tower image was painted over by an officialdom that apparently did not share our sense of humor.

> 传言有关画家是谁，但三十多年后嘴唇仍然密不可分。涂料的报销要求已经提出，但被拒绝了。无论如何，几天内，水塔图像被官方覆盖，显然他们不能理解我们的幽默感。

The full story of Peter's many faces can be found at _spinroot.com/pjw_, a web site maintained by Gerard, who with Rob Pike did many of the original enhancements of Peter's picture.

> 可以在 spinroot.com/pjw 上找到彼得多个面孔的完整故事，这是由杰拉德维护的网站，他和罗布·派克一起对彼得的照片进行了许多原始增强。

[]{#index_split_000.html#p63}![](./index-63_1.jpg){.calibre4}

CHAPTER 3: FIRST EDITION

49

**Figure 3.5:**

Peter filtered through AT&T logo (Courtesy of Gerard Holzmann) Bell Labs was an informal place, but sometime in the early to mid 1980s, a new policy was instituted: employees had to wear their badges at all times.

> 彼得透過 AT&T 標誌(Gerard Holzmann 提供)過濾了 Bell Labs，它是一個非正式的地方，但在 1980 年代初期到中期，一項新政策被實施：員工必須隨時佩戴識別證。

This was undoubtedly a sensible precaution to discourage interlopers, but it wasn't popular. As a protest, one colleague, who will remain nameless here, stuck his badge to his forehead with super-glue; another took to wearing it clipped to the hair on his chest, revealing it only upon demand.

> 这无疑是一个明智的预防措施，以阻止闯入者，但它并不受欢迎。作为一种抗议，一位同事(在此处不予透露姓名)用超级胶把他的徽章粘在他的前额上；另一位则把它夹在胸口的头发上，只有在要求时才暴露出来。

The badges had no security features; they consisted only of a picture in a template. Accordingly, we undertook a campaign to create a fake person, Grace R Emlin, who had her own login, gre, her own badge (Figure 3.7), and from time to time an appearance on official lists and publications.

> 徽章没有安全特征；它们仅由模板中的图片组成。因此，我们启动了一项运动，创建一个假人格雷斯·R·埃姆林，她有自己的登录名 gre，自己的徽章(图 3.7)，不时出现在官方名单和出版物上。

I made my own badge with a Mickey Mouse image (Figure 3.8). I wore it regularly, including one day at Bell Labs in Holmdel, New Jersey, for a meeting with Bill Gates, who was there for some marketing of Windows 3.0. No one noticed.

> 我用米老鼠图像(图 3.8)制作了自己的徽章，我经常佩戴它，其中一天是在新泽西霍尔姆德尔的贝尔实验室，参加与比尔·盖茨的会议，他当时来宣传 Windows 3.0。没人注意到。

Figures 3.9 and 3.10 show random parts of the Unix room in 2005.

**3.3 The Unix Programmer's Manual**

One of the early contributions of Unix was its online manual, in a now-familiar format and concise style. Every command, library function, file format, and so on had a page in the manual that described briefly what it was and how to use it. For example, Figure 3.11 shows the 1st Edition manual page for the cat command, which concatenates zero or more files onto the standard output stream, by default the user's terminal.

> Unix 的早期贡献之一是它的在线手册，采用现在熟悉的格式和简洁的风格。每个命令、库函数、文件格式等都有一个手册页，简要描述它的功能及如何使用它。例如，图 3.11 显示了第一版手册中 cat 命令的页面，该命令可以将零个或多个文件连接到标准输出流(默认为用户的终端)。

Early man pages tended to be literally only a single page, a slimness that is uncommon today. Besides brevity, a couple of features of man pages were novel at the time, like the BUGS section, which acknowledged that programs

> 早期的 man 页面往往只有一页，这种简洁性在今天已经不多见了。除了简洁之外，man 页面的一些特性当时是新颖的，比如 BUGS 部分，它承认程序可能存在缺陷。

[]{#index_split_000.html#p64}![](./index-64_1.jpg){.calibre4}

50 CHAPTER 3: FIRST EDITION

**Figure 3.6:**

Peter on the water tower, 1985 (Courtesy of Gerard Holzmann)

[]{#index_split_000.html#p65}![](./index-65_1.jpg){.calibre4}

CHAPTER 3: FIRST EDITION

51

**Figure 3.7:**

Grace Emlin, MTS

do have bugs, or perhaps "features," imperfections that should at least be recorded even if not fixed right away.

> 存在缺陷，或者可称为“功能”，即使暂时不能修复，也应该记录下来。

The cat command hasn't changed in 50 years, aside from acquiring a few optional and probably unnecessary arguments that somewhat modify its behavior; it's still part of the core set of Unix commands. You can see its current status by typing the command

> 猫命令在 50 年里没有改变，除了获得一些可选的、也许是不必要的参数，它们有点改变了它的行为; 它仍然是 Unix 命令的核心集合的一部分。您可以通过输入该命令来查看它的当前状态。

\$ _man cat_

in a terminal window in Linux, macOS or Windows Subsystem for Linux (WSL). And of course you can view the manual page for the man command itself with

> 在 Linux、macOS 或 Windows Subsystem for Linux(WSL)的终端窗口中。当然，您也可以查看 man 命令本身的手册页面。

\$ _man man_

[]{#index_split_000.html#p66}![](./index-66_1.jpg){.calibre4}

52 CHAPTER 3: FIRST EDITION

**Figure 3.8:**

My high-security Bell Labs badge

**3.4 A few words about memory**

Younger readers might wonder about the accuracy of some of the memory sizes that I have been quoting along the way. For instance, an IBM 7090 or 7094 had 32K (32,768) 36-bit words; the original PDP-7 that Ken used had 8K (8,192) 18-bit words, that is, around one eighth of the 7090 memory; and the first PDP-11 had 24K bytes of primary memory and a half-megabyte disk. For comparison, my 2015 Macbook Air has 8 GB of memory (over 330,000 times as much), a 500 GB disk (half a million times as much), and cost barely a thousand dollars.

> 读者可能会对我一直引用的内存大小的准确性感到疑惑。例如，IBM 7090 或 7094 有 32K(32,768)36 位字；Ken 使用的原始 PDP-7 有 8K(8,192)18 位字，也就是说，大约是 7090 内存的八分之一；而第一台 PDP-11 有 24K 字节的主内存和半兆字节的磁盘。相比之下，我 2015 年的 Macbook Air 有 8GB 内存(超过 330,000 倍)，500GB 磁盘(500 万倍)，而且只花了不到 1000 美元。

In short, memories were tiny by today's standards, where gigabytes of primary memory and terabytes of disk storage are cheap, compact and therefore common. But memory technology in the 1960s and early 1970s was different. The primary memory of a computer was built from arrays of tiny donut-shaped ferrite cores, connected with an intricate though orderly set of wires that were threaded by hand through the cores. Each core could be magne-tized one way or the other (think clockwise or counterclockwise) and thus was capable of representing one bit of information; eight cores would be a byte.

> 简而言之，今天的标准下，内存的容量很小，而千兆字节的主存和太字节的磁盘存储器便宜又紧凑，因此普遍存在。但 1960 年代和 1970 年代初的内存技术有所不同。计算机的主存是由一系列小的甜甜圈形铁氧体构成的，它们用一组复杂而有序的电线相互连接。每个铁氧体可以以一种方式磁化(想象顺时针或逆时针)，因此能够表示一位信息；八个铁氧体就是一个字节。

Core memory was very expensive, since manufacturing it took highly skilled manual labor, it was bulky, and it weighed a lot. Figure 3.12 shows a

> 核心存储器非常昂贵，因为它的制造需要高技能的手工劳动，它很笨重，重量也很大。图 3.12 展示了一个。

[]{#index_split_000.html#p67}![](./index-67_1.jpg){.calibre4}

CHAPTER 3: FIRST EDITION

53

**Figure 3.9:**

Unix room, October 2005

core memory with 16K bits (2K bytes), which in 1971 would have cost about \$16,000, or close to a dollar a bit.

> 核心存储器有 16K 位(2K 字节)，1971 年的价格约为 16000 美元，每位接近一美元。

Memory was often the most costly component of a computer. When ev ery byte was precious, that scarcity imposed a certain discipline on programmers, who always had to be conscious of how much memory they were using, and sometimes had to resort to trickery and risky programming techniques to fit their programs into the available memory.

> 记忆常常是计算机最昂贵的组成部分。当每个字节都是宝贵的时候，这种稀缺性给程序员施加了一定的约束，他们总是要意识到自己正在使用多少内存，有时不得不诉诸技巧和冒险的编程技术来把程序安排进可用的内存中。

One thing that Unix did well was to make effective use of the limited memory of the computers that it ran on. Some of this was due to exceptionally talented programmers like Ken and Dennis, who knew how to sav e memory.

> Unix 在有限的计算机内存上做得很好，这部分得益于像 Ken 和 Dennis 这样的杰出程序员，他们知道如何节省内存。

Some was due to their genius in finding ways to achieve generality and uniformity that made it possible to accomplish more with less code. Sometimes this was achieved by clever programming, while in other cases it was a result of finding better algorithms.

> 有些是由于他们在寻找实现普遍性和统一性的方法的天才，使得用更少的代码就能完成更多的事情成为可能。有时是通过巧妙的编程实现的，而有时则是通过找到更好的算法而实现的。

Some was due to the use of assembly language, which at the time did make better use of instructions (run faster) and memory (use less space) than

> 一些是由于使用汇编语言，当时它能更好地使用指令(运行更快)和内存(使用更少的空间)。

[]{#index_split_000.html#p68}![](./index-68_1.jpg){.calibre4}

54 CHAPTER 3: FIRST EDITION

**Figure 3.10:**

Unix room, October 2005

could be achieved with compilers for high level languages. It was only in the mid 1970s that new memory technology based on semiconductors and integrated circuits became widely available at a price where one could afford the moderate but measurable overhead of high-level languages like C.

> 随着半导体和集成电路技术的广泛应用，中 1970 年代中期，像 C 语言这样的高级语言的费用变得可以承受，可以通过编译器实现。

Storage allocators like the original alloc and Doug McIlroy's later malloc library were used to allocate and reallocate memory dynamically as a program was running, another way to make the most of a scarce resource.

> 存储分配器，如原始分配器和 Doug McIlroy 后来的 malloc 库，用于在程序运行时动态分配和重新分配内存，是充分利用稀缺资源的另一种方式。

Naturally this had to be done carefully, since the slightest mistake could cause a program to work incorrectly (something that is not unheard of even today, I might add, at least as I observe students in my classes). Mismanage-ment of memory remains one of the leading causes of errors in C programs.

> 自然，这必须小心翼翼地做，因为一点点错误都可能导致程序运行不正确(我可以补充一句，即使是在今天，我在课堂上观察到的学生也不是没有听说过)。内存管理不当仍然是 C 程序中错误的主要原因之一。

When a program failed badly enough, the operating system would notice and would try to help the programmer by producing a file of the contents of main memory---what was in the magnetic cores---from which comes the phrase "core dump," still used though magnetic cores long ago left the scene.

> 当程序失败得足够严重时，操作系统会注意到并试图通过产生主存储器内容的文件来帮助程序员，也就是磁芯中的内容，这就是“核心转储”一词的由来，尽管磁芯早已不复存在，但这个词仍在使用。

The file is still called core.

[]{#index_split_000.html#p69}![](./index-69_1.jpg){.calibre4}

CHAPTER 3: FIRST EDITION

55

**Figure 3.11:**

cat(1) manual page from 1st Edition Unix **3.5 Biography: Dennis Ritchie**

> 3.5 传记：丹尼斯·里奇
> 丹尼斯·里奇是 Unix 第一版的贡献者之一，他是 C 语言的发明者，也是许多 Unix 工具的作者。他于 1941 年出生于美国纽约，获得了哈佛大学的物理学学位。他最初在贝尔实验室工作，后来加入了 AT&T 贝尔实验室，并在那里发明了 C 语言。他与贝尔实验室的另一名成员，Ken Thompson，一起设计了 Unix 系统。他于 2011 年 10 月 12 日去世，享年 70 岁。

This summary of Dennis Ritchie's life is adapted from a memorial that I wrote for the National Academy of Engineering in 2012.

> 这篇有关丹尼斯·里奇的生平简介改编自我于 2012 年为美国国家工程院撰写的纪念文章。

Dennis (Figure 3.13) was born in September 1941. His father, Alistair Ritchie, worked for many years at Bell Labs in Murray Hill. Dennis went to Harvard where he did his undergraduate work in physics and his graduate work in applied mathematics. His PhD thesis topic (1968) was subrecursive hierarchies of functions, and is tough going if one is not an expert, which I am certainly not; Figure 3.14 shows part of one random page, taken from a blurry copy of a draft. Explaining his career path, he said

> 丹尼斯(见图 3.13)于 1941 年 9 月出生，他的父亲艾利斯泰尔·里奇(Alistair Ritchie)在贝尔实验室(Bell Labs)的默里山(Murray Hill)工作多年。丹尼斯在哈佛大学(Harvard)攻读物理学本科，应用数学硕士。他的博士论文(1968 年)主题是子递归函数的层次结构，如果不是专家，那么这是一项艰巨的任务，我当然不是专家；图 3.14 显示了其中一页的一部分，这是从模糊的草稿复印件中拍摄的。谈论他的职业道路时，他说

"My undergraduate experience convinced me that I was not smart enough to be a physicist, and that computers were quite neat. My graduate school experience convinced me that I was not smart enough to be an expert in the theory of algorithms and also that I liked procedural languages better than functional ones."

> 我的本科经历让我确信自己不够聪明去做物理学家，而且计算机也很有趣。我的研究生学习经历让我确信自己不够聪明去成为算法理论专家，而且我更喜欢过程式语言而不是函数式语言。

As Bjarne Stroustrup, the creator of C++, once said, "If Dennis had decided to spend that decade on esoteric math, Unix would have been stillborn."

> 象 C++的创造者 Bjarne Stroustrup 曾经说过的：“如果 Dennis 决定把这十年花在深奥的数学上，Unix 就不会诞生。”

[]{#index_split_000.html#p70}![](./index-70_1.jpg){.calibre4}

56 CHAPTER 3: FIRST EDITION

**Figure 3.12:**

Magnetic core memory; 16K bits, 2K bytes (∼5.25 in, 13 cm) Dennis had spent several summers at Bell Labs, and joined permanently in 1967 as a member of technical staff in the Computing Science Research Center. For the first few years, he worked on Multics. As noted earlier, Multics proved too ambitious, and as it became clear that it would not live up to its goals, Bell Labs withdrew in 1969, leaving Ken, Dennis and colleagues with experience in innovative operating system design, an appreciation of implementation in high-level languages, and a chance to start over with much more modest goals. The result was the Unix operating system and the C programming language.

> 磁芯存储器；16K 位，2K 字节(约 5.25 英寸，13 厘米)丹尼斯曾在贝尔实验室度过几个夏天，并于 1967 年正式加入计算科学研究中心担任技术人员。在最初的几年里，他致力于 Multics。正如前面提到的，Multics 过于雄心勃勃，当显然它无法实现其目标时，贝尔实验室于 1969 年退出，让肯、丹尼斯和同事们拥有创新操作系统设计的经验，欣赏高级语言的实现，并有机会重新开始，目标更加实际。其结果就是 Unix 操作系统和 C 编程语言。

The C programming language dates from early in the 1970s. It was based on Dennis's experience with high-level languages for Multics implementation, but much reduced in size because most computers of the time had limited capacity; there simply wasn't enough memory or processing power to support a complicated compiler for a complicated language. This enforced minimality matched Ken and Dennis's preference for simple, uniform mechanisms. C was a good match as well for real computer hardware; it was clear how to translate it into good code that ran efficiently.

> C 编程语言可以追溯到 20 世纪 70 年代初期。它基于丹尼斯在 Multics 实现中使用的高级语言，但由于当时大多数计算机的容量有限，因此大小大大减少了；根本没有足够的内存或处理能力来支持一个复杂的编译器来编译一种复杂的语言。这种强制最小化与肯和丹尼斯对简单、统一机制的偏好相匹配。C 也很适合实际的计算机硬件；很明显如何将其转换为运行效率高的良好代码。

[]{#index_split_000.html#p71}![](./index-71_1.jpg){.calibre4}

CHAPTER 3: FIRST EDITION

57

**Figure 3.13:**

Dennis Ritchie, ∼1981 (Courtesy of Gerard Holzmann) C made it possible to write the entire operating system in a high level language. By 1973, Unix had been converted from its original assembly language form into C. This made it much easier to maintain and modify the system. It also enabled another giant step, moving the operating system from its original PDP-11 computer to other computers with different architectures.

> 丹尼斯·里奇，约 1981 年(提供赫尔茨曼)C 使得用高级语言编写整个操作系统成为可能。到 1973 年，Unix 已从最初的汇编语言形式转换为 C。这使得维护和修改系统变得容易得多。它还使操作系统从最初的 PDP-11 计算机转移到具有不同架构的其他计算机变得更加容易。

Because most of the system code was written in C, porting the system required not much more than porting the C compiler.

> 由于系统代码大部分都是用 C 编写的，移植系统所需的不多于移植 C 编译器。

Dennis was a superb technical writer, with a spare elegant style, deft turns of phrase, and often with flashes of dry wit that accurately reflected his personality. He and I wrote _The C Programming Language_ together; it was published in 1978, with a second edition in 1988, and has since been translated into more than two dozen languages. Dennis's original C reference manual formed the basis of the ANSI/ISO standard for C that was first produced in 1988, and was a major part of the book. Without doubt, some of the success of C and Unix can be attributed to Dennis's writing.

> 丹尼斯是一位出色的技术作家，文笔简洁优雅，措辞灵巧，而且经常带有一丝幽默，恰如其分地反映了他的个性。他和我一起撰写了《C 程序设计语言》；该书于 1978 年出版，1988 年出版第二版，此后已被翻译成超过二十四种语言。丹尼斯最初的 C 参考手册成为 1988 年首次出版的 ANSI/ISO C 标准的基础，也是本书的重要组成部分。毫无疑问，C 和 Unix 的成功部分归功于丹尼斯的写作。

With Ken Thompson, Dennis received many honors and awards for his work on C and Unix, including the ACM Turing Award (1983), the National Medal of Technology (1999), the Japan Prize for Information and Communications (2011), and the National Inventors Hall of Fame (posthumously in 2019).

> 与肯·汤普森(Ken Thompson)一起，丹尼斯因其在 C 和 Unix 上的工作而获得了许多荣誉和奖项，包括 1983 年的 ACM 图灵奖，1999 年的国家技术奖，2011 年的日本信息与通信奖，以及 2019 年的国家发明家名人堂(追授)。

Dennis successfully avoided any management role for many years, but finally yielded and became head of the Software Systems department, where he was responsible for the group that was building the Plan 9 operating

> 丹尼斯成功地避开了多年的管理角色，但最终还是屈服了，成为软件系统部门的负责人，他负责组建 Plan 9 操作系统的小组。

[]{#index_split_000.html#p72}![](./index-72_1.jpg){.calibre4}

58 CHAPTER 3: FIRST EDITION

**Figure 3.14:**

Excerpt from Dennis Ritchie's PhD thesis (Courtesy of Computer History Museum)

> 从丹尼斯·里奇博士论文的摘录(由计算机历史博物馆提供)

system. Dennis stepped down from management and retired officially in 2007, but continued to come to Bell Labs almost every day until his death in October 2011.

> 系统。丹尼斯于 2007 年正式辞去管理职务退休，但他几乎每天都会来贝尔实验室，直到他于 2011 年 10 月去世。

Dennis was modest and generous, always giving credit to others while downplaying his own contributions. A typical example is found in the acknowledgment section of his 1996 retrospective on the evolution of Unix:

> 丹尼斯谦虚而慷慨，总是给予他人荣誉，而谦虚自己的贡献。一个典型的例子可以在他 1996 年关于 Unix 演变的回顾中找到：

"The reader will not, on the average, go far wrong if he reads each occurrence of 'we' with unclear antecedent as 'Thompson, with some assistance from me.' "

> 读者如果把每次出现的“我们”都理解为“汤普森在我的帮助下”，一般不会出错。

Dennis died in October 2011. This note from his sister and brothers can be found on his home page, which has been preserved at Bell Labs at _[www.bell-labs.com/usr/dmr/www](http://www.bell-labs.com/usr/dmr/www)_.

> 丹尼斯于 2011 年 10 月去世。他姐姐和兄弟的这则消息可以在他的主页上找到，该主页已经保存在贝尔实验室网站[www.bell-labs.com/usr/dmr/www]。

"As Dennis's siblings, Lynn, John, and Bill Ritchie---on behalf of the entire Ritchie family---we wanted to convey to all of you how deeply moved, astonished, and appreciative we are of the loving tributes to

> 作为丹尼斯的兄弟姐妹，林恩、约翰和比尔·里奇——代表整个里奇家族——我们想向你们传达，我们对你们对他深情的悼念、惊叹和感激之情有多么深深的感动。

[]{#index_split_000.html#p73}CHAPTER 3: FIRST EDITION

59

Dennis that we have been reading. We can confirm what we keep hearing again and again:

> 我们一直在阅读丹尼斯的作品。我们可以确认，我们一次又一次地听到的：

Dennis was an unfailingly kind, sweet, unassuming, and generous brother---and of course a complete geek. He had a hilariously dry sense of humor, and a keen appreciation for life's absurdities---though his world view was entirely devoid of cynicism or mean-spiritedness.

> 丹尼斯是一个极其和蔼可亲、温柔乐观、谦逊慷慨的兄弟，当然也是一个彻头彻尾的书呆子。他有一种幽默的干笑，对生活的荒谬有独到的洞察力——尽管他的世界观完全没有玩世不恭或刻薄的成分。

We are terribly sad to have lost him, but touched beyond words to realize what a mark he made on the world, and how well his gentle personality---beyond his accomplishments---seems to be understood."

> 我们对失去他感到非常悲伤，但超乎言语的感动，意识到他在这个世界上留下了多么深刻的印记，以及他温柔的个性——超越他的成就——似乎被人们所理解。

Lynn, John, and Bill Ritchie

[]{#index_split_000.html#p74} []{#index_split_000.html#p75}Chapter 4

**Sixth Edition (1975)**

"The number of Unix installations has grown to 10, with more expected."

_The Unix Programmer's Manual_, 2nd Edition, June 1972

"The number of Unix installations is now above 50, and many more are expected."

> 现在 Unix 安装的数量已经超过 50 个，预计还会有更多。

_The Unix Programmer's Manual_, 5th Edition, June 1974

The first edition of Unix was up and running by late 1971, if we go by the date on the manual. For the next few years, there was a new edition of the manual roughly every six months, each time with major new features, new tools, and new languages. The 6th edition, whose manual is dated May 1975, was the first that found its way outside of Bell Labs to any significant degree, and it had a major effect on the world.

> Unix 的第一个版本在 1971 年末就开始运行了，如果我们按照手册上的日期来看的话。在接下来的几年里，每过六个月就会有新版本的手册，每次都有重大的新功能、新工具和新语言。手册上标明日期为 1975 年 5 月的第六版，是第一个走出贝尔实验室，并产生重大影响的版本。

Unix was first publicly described in a paper by Dennis Ritchie and Ken Thompson, "The Unix Time-Sharing System," that appeared in the Fourth ACM Symposium on Operating Systems Principles in October 1973; it was republished with minor changes in the journal _Communications of the Association for Computing Machinery_ (CACM) in July 1974. The abstract begins with a concise summary of a remarkable number of good ideas: Unix is a general-purpose, multi-user, interactive operating system for the Digital Equipment Corporation PDP-11/40 and 11/45 computers.

> Unix 首次在丹尼斯·里奇和肯·汤普森的论文"Unix 时间共享系统"中公开描述，该论文于 1973 年 10 月发表在第四届 ACM 操作系统原理研讨会上；它在 1974 年 7 月的《计算机协会通讯》(CACM)杂志上以微小的改变重新发表。摘要以简短的总结开始，涵盖了一系列优秀的想法：Unix 是为数字设备公司 PDP-11/40 和 11/45 计算机设计的通用、多用户、交互式操作系统。

It offers a number of features seldom found even in larger operating systems, including:

> 它提供了一些甚至在更大型操作系统中也很少见的功能，包括：

\(1\) a hierarchical file system incorporating demountable volumes; (2) compatible file, device, and inter-process I/O; (3) the ability to initiate asynchronous processes; (4) system command language selectable on a per-user basis; and

> (1) 包含可卸载卷的分层文件系统；(2) 兼容文件、设备和进程间的 I/O；(3) 能够启动异步进程的能力；(4) 每个用户可选择的系统命令语言；

[]{#index_split_000.html#p76}62 CHAPTER 4: SIXTH EDITION

\(5\) over 100 subsystems including a dozen languages.

What were these features "seldom found even in larger operating systems," and what was their significance? The next few sections talk about some of them in more detail. If you're not technically inclined, you can safely skim the chapter; I've tried to summarize the important parts of each section near the beginning so you can skip the details.

> 这些特性“甚至在更大的操作系统中也很少见”是什么，它们有何重要意义？接下来的几个部分将更详细地讨论其中一些内容。如果你不是技术型的，你可以安全地浏览本章；我尽量在每个部分的开头总结重要的内容，这样你就可以跳过细节。

**4.1 File system**

The _file system_ is the part of an operating system that manages information on secondary storage like disks, which for many years were sophisticated mechanical devices based on rotating magnetic media, and which today are most often solid state disks and USB flash drives, integrated circuits that have no moving parts.

> 文件系统是操作系统的一部分，它管理二级存储(如磁盘)上的信息，多年以来，这些磁盘是基于旋转磁性介质的复杂机械设备，而今日最常见的是固态磁盘和 USB 闪存驱动器，这些集成电路没有移动部件。

We are familiar with the abstract view of this information storage through programs like Explorer on Windows and Finder on macOS. Underneath those is a significant amount of software to manage the information on physical hardware, keep track of where each part is, control access, make it efficiently accessible for reading and writing, and ensure that it's always in a consistent state.

> 我们熟悉这种信息存储的抽象视图，通过像 Windows 上的 Explorer 和 MacOS 上的 Finder 这样的程序。在这些之下，有大量的软件来管理物理硬件上的信息，跟踪每个部分的位置，控制访问权限，使其高效地可读写，并确保其始终处于一致的状态。

Before Multics, most operating systems provided at best complicated and irregular file systems for storing information. The Multics file system was much more general, regular and powerful than other file systems of the time, but it was correspondingly complex. The Unix file system that Ken developed profited from Multics, but was significantly simpler. Its clean, elegant design has over the years become widely used and emulated.

> 在 Multics 出现之前，大多数操作系统提供的文件系统最多只能提供复杂而不规则的存储信息的方式。Multics 文件系统比当时的其他文件系统更加普遍、规则和强大，但也更加复杂。Ken 开发的 Unix 文件系统从 Multics 中获益，但要简单得多。它简洁优雅的设计近年来已经被广泛使用和模仿。

A Unix file is simply a sequence of bytes. Any structure or organization of the contents of a file is determined only by the programs that process it; the file system itself doesn't care what's in a file. That means that any program can read or write any file. This idea seems obvious in retrospect, but it was not always appreciated in earlier systems, which sometimes imposed arbitrary restrictions on the format of information in files and how it could be processed by programs. Doug McIlroy describes one example:

> Unix 文件只是一个字节序列。文件内容的任何结构或组织只由处理它的程序来决定；文件系统本身并不关心文件中有什么。这意味着任何程序都可以读取或写入任何文件。这个想法在回顾时似乎是显而易见的，但在早期的系统中却并不总是如此，它们有时会对文件中的信息格式以及程序如何处理它们施加任意限制。Doug McIlroy 描述了一个例子：

"Typically source code was a distinguished type, different from data.

Compilers could read source, compiled programs could read and write

'data.' Thus the creation and inspection of Fortran programs was often walled off from the creation and inspection of other files, with completely different ways to edit and print them. This ruled out the use of programs to generate (or even simply copy) Fortran programs."

> 数据。因此，Fortran 程序的创建和检查通常与其他文件的创建和检查隔离开来，用完全不同的方式来编辑和打印它们。这排除了使用程序来生成(甚至只是复制)Fortran 程序的可能性。

[]{#index_split_000.html#p77}CHAPTER 4: SIXTH EDITION

63

Unix made no such distinctions: any program could process any file. If applying a program to a file doesn't make sense---for example, trying to compile a Fortran source file as if it were C---that doesn't hav e anything to do with the operating system.

> Unix 没有这样的区分：任何程序都可以处理任何文件。如果将程序应用于文件不合逻辑，例如试图将 Fortran 源文件编译为 C，这与操作系统无关。

Unix files are organized in directories. (Other operating systems often call these folders.) A Unix directory is also a file in the file system, but one whose contents are maintained by the system itself, not by user programs. A directory contains information about files, which may in turn be directories.

> Unix 文件存放在目录中(其他操作系统经常把这些文件夹称为文件夹)。Unix 目录也是文件系统中的一个文件，但其内容由系统本身维护，而不是由用户程序维护。目录包含有关文件的信息，而这些文件可能又是目录。

A Unix directory entry includes the file name within the directory, access permissions, file size, date and time of creation and modification, and information about where to find the contents of the file. Each directory has two special entries named "." (the directory itself) and "..", the parent directory; these are pronounced "dot" and "dotdot." The root directory is the top of this hierarchy; its name is /. Any file can be reached by following the path down from the root, and the root can be found from any file by going up the sequence of .. parent directories. Thus the text for this book might be found in _/usr/bwk/book/book.txt_. The system also supports the notion of a current directory, so that filenames can be relative to the current location in the file system, rather than having to specify a full path from the root.

> 目录条目中包括目录中的文件名、访问权限、文件大小、创建和修改的日期和时间，以及有关如何找到文件内容的信息。每个目录都有两个特殊条目，名为“。”(目录本身)和“..”，父目录；这些被称为“点”和“点点”。根目录是这种层次结构的顶部；它的名字是/。可以通过从根目录开始沿着路径访问任何文件，而且可以从任何文件通过访问序列..父目录找到根目录。因此，本书的文本可能位于*/usr/bwk/book/book.txt*。系统还支持当前目录的概念，因此文件名可以相对于文件系统中的当前位置，而不必指定从根目录开始的完整路径。

Because any directory can contain subdirectories, the file system can be arbitrarily deep. This organization of nested directories and files is called a

> 因为任何目录都可以包含子目录，所以文件系统可以是任意深度的。这种嵌套目录和文件的组织称为

"hierarchical" file system. Again, though the advantages are obvious in hindsight, hierarchical file systems were not widely available before Multics and then Unix. For example, some file systems limited the depth of nesting; CTSS limited it to two lev els.

> 分层文件系统。虽然这种优势在事后看来是显而易见的，但在 Multics 和 Unix 之前，分层文件系统并不普遍。例如，一些文件系统将嵌套深度限制在两级，CTSS 就将其限制在两级。

**4.2 System calls**

An operating system provides a set of services to programs that run on it, services like starting and stopping programs, reading or writing information in files, accessing devices and network connections, reporting information like date and time, and many others. These services are implemented within the operating system, and are accessible from running programs through a mechanism called _system calls._

> 操作系统为运行在其上的程序提供一组服务，如启动和停止程序、读取或写入文件中的信息、访问设备和网络连接、报告日期和时间等信息，以及其他许多服务。这些服务在操作系统内实现，并通过一种称为系统调用的机制从运行程序访问。

In a very real sense, the system calls _are_ the operating system, since they define what services the system provides. There may be multiple independent implementations of a set of system calls, as is the case with different versions of Unix and Unix-like systems. A completely different operating system, say Windows, could provide software to convert Unix system calls into its own system calls. And there are sure to be system calls that are

> 在一个非常真实的意义上，系统调用就是操作系统，因为它们定义了系统提供的服务。一组系统调用可以有多个独立的实现，就像 Unix 和类 Unix 系统的不同版本一样。完全不同的操作系统，比如 Windows，可以提供软件来将 Unix 系统调用转换为自己的系统调用。当然还有一些系统调用是特定于某个操作系统的。

[]{#index_split_000.html#p78}64 CHAPTER 4: SIXTH EDITION

unique to a particular operating system even if it is Unix-like.

The first edition of Unix had just over 30 system calls, about half of which were related to the file system. Because files contained only uninterpreted bytes, the basic file system interface was dead simple, only five system calls to open or create a file, read or write its bytes, and close it. These were accessed from a C program by calling functions using statements like these: fd = creat(filename, perms)

> 第一版的 Unix 只有 30 多个系统调用，其中大约一半与文件系统有关。由于文件只包含未解释的字节，基本文件系统接口非常简单，只有五个系统调用来打开或创建文件，读取或写入其字节，并关闭它。从 C 程序访问这些调用的语句如下：fd = creat(filename，perms)。

fd = open(filename, mode)

nread = read(fd, buf, n)

nwrite = write(fd, buf, n)

status = close(fd)

The creat system call creates a new file and sets its access permissions, which normally would include or exclude the ability to read, write and execute for the user, for the user's group, and for everyone else. These nine bits give considerable control with comparatively little mechanism. The open system call opens an existing file; mode specifies whether the file is to be read from or written to, and filename is an arbitrary path in the hierarchical file system.

> 系统调用 creat 创建一个新文件，并设置其访问权限，通常包括或排除用户、用户组和其他人的读、写和执行权限。这九位二进制数提供了相当大的控制，同时机制也相对较少。系统调用 open 打开一个已存在的文件；模式指定文件是用于读取还是写入，文件名是分层文件系统中的任意路径。

The fd value that results from calling open and creat is called a _file_ _descriptor_, a small non-negative integer that is used in subsequent reads and writes of the file. The read and write system calls attempt to transfer a specified number n of bytes either from the file or to the file; each function returns the number of bytes that were actually transferred. For all of these system calls, if a negative value (usually −1) is returned, that indicates some kind of error.

> 调用 open 和 creat 得到的 fd 值被称为文件描述符，这是一个非负的小整数，用于对文件的后续读写。读写系统调用尝试传输指定数量 n 的字节，要么从文件，要么向文件；每个函数返回实际传输的字节数。对于所有这些系统调用，如果返回负值(通常为-1)，则表示某种错误。

By the way, the creat system call really is spelled that way, for no good reason other than Ken Thompson's personal taste. Rob Pike once asked Ken what he would change if he were to do Unix over again. His answer? "I'd spell creat with an e."

> 顺便说一句，creat 系统调用的拼写没有任何好的理由，只是凯恩·汤普森的个人口味。罗布·派克曾经问凯恩，如果他要重新做 Unix，他会改变什么？他的回答是：“我会用 e 拼写 creat”。

Another Unix innovation was to have peripheral devices like disks, terminals, and others appear as files in the file system; disks are the "demountable volumes" mentioned in the list of features. The same system calls are used to access devices as are used to access files, so the same code can manipulate files and devices. Of course it isn't that simple, since real devices have weird properties that must be handled, so there are other system calls for dealing with the idiosyncrasies, especially of terminals. This part of the system was not pretty.

> 另一项 Unix 创新是将外围设备，如磁盘、终端和其他设备，作为文件系统中的文件出现；磁盘是列出的功能中所提到的“可拆卸卷”。使用相同的系统调用来访问设备，因此可以使用相同的代码来操作文件和设备。当然，情况并不那么简单，因为真实的设备具有必须处理的奇怪属性，因此还有其他系统调用来处理特殊情况，特别是终端。该系统的这一部分并不漂亮。

There are also system calls for setting a position within a file, determining its status, and the like. These have all been embellished and occasionally improved over 50 years, but the basic model is simple and easy to use.

> 也有系统调用可用于设置文件中的位置，确定其状态等。这些系统调用已经在 50 年间被装饰和改进，但基本模型仍然简单易用。

[]{#index_split_000.html#p79}CHAPTER 4: SIXTH EDITION

65

It may be hard for today's readers to appreciate just how much of a simplification all of this was. In early operating systems, all of the myriad complexities of real devices were reflected through to users. One had to know all about disk names, their physical structure like how many tracks and cylinders they had, and how data was organized on them. Steve Johnson reminded me of how awkward it was with the time-sharing subsystem on the main Honeywell computer at this time:

> 今天的读者很难意识到这一切有多么简化。在早期的操作系统中，所有真实设备的无数复杂性都反映到用户身上。一个人必须知道磁盘的名称，它们的物理结构，比如有多少个轨道和汽缸，以及数据是如何在上面组织的。史蒂夫·约翰逊提醒我，当时这台主要的霍尼韦尔计算机上的时间共享子系统是多么尴尬：

"The Honeywell TSS system required you to enter a subsystem to create a disk file. You were asked about 8 questions: initial size of file, maximum size, name, device, who could read it, who could write it, etc. Each of these had to be answered interactively. When all the questions had been answered, the operating system was given the information, and, likely as not, something was mistyped and the file creation failed. That meant you got to enter the subsystem again and answer all the questions again. It's no wonder that when a file finally got created, the system said 'SUCCESSFUL!' "

> 霍尼韦尔 TSS 系统要求您输入一个子系统来创建磁盘文件。您被问了 8 个问题：文件的初始大小、最大大小、名称、设备、谁可以读取它、谁可以写入它等等。这些都必须交互式地回答。当所有的问题都被回答了，操作系统就会得到这些信息，很可能有些东西被打错了，导致文件创建失败。这意味着你必须再次输入子系统并再次回答所有的问题。难怪当文件终于被创建时，系统会说“成功！”

Unix followed the example of Multics in hiding all of this irrelevant non-sense: files were just bytes. The user determined what the bytes were, while the operating system looked after storing and retrieving them, without expos-ing device properties to users.

> Unix 跟随 Multics 的例子，隐藏所有无关的废话：文件只是字节。用户确定字节是什么，而操作系统负责存储和检索它们，而不向用户公开设备属性。

**4.3 Shell**

The shell is a program that runs other programs. It's the program that lets users run commands, and is the primary interface between users and the operating system. When I log in to a Unix system, my keyboard is connected to a running instance of the shell. I can type commands, usually one at a time, and the shell runs each in turn, and after each one completes, it's ready for the next. So a session might look like this, where \$ is a prompt that the shell prints so I know it's waiting for me to do something. What I type is in _this slanted font_.

> shell 是一个可以运行其他程序的程序。它是用户运行命令的主要界面，也是用户和操作系统之间的主要接口。当我登录到 Unix 系统时，我的键盘连接到一个正在运行的 shell 实例。我可以输入命令，通常一次一个，shell 会依次运行每个命令，每个命令完成后，它就准备好接受下一个命令了。因此，一个会话可能是这样的，其中\$是 shell 打印出来的提示，让我知道它正在等待我做一些事情。我输入的内容用 _这种斜体字_ 来表示。

\$ _date_

_tell me the date and time_

Fri Oct 18 13:09:00 EDT 2019

\$ _ls_

_list the contents of the directory_

book.pdf

book.txt

\$ _wc book.txt_

_count the lines, words and characters in book.txt_ 9918 59395

362773 book.txt

\$ _cp book.txt backup.txt_

_copy book.txt to a backup file_

[]{#index_split_000.html#p80}66 CHAPTER 4: SIXTH EDITION

One very important note: the shell is an ordinary user program, not some integral part of the operating system, another idea taken from Multics.

> 一个非常重要的注意：shell 是一个普通的用户程序，而不是操作系统的一部分，这是从 Multics 中借鉴的另一个想法。

(That's the "system command language selectable on a per-user basis" mentioned in the feature list.) Because the shell is a user program, it's easily replaced by a different one, which is why there are so many Unix shells. If you don't like the way one shell works, you can pick another or even write your own and use it instead. Speaking of "the shell" is not specific.

> 这就是功能列表中提到的“可以按照每个用户设置的系统命令语言”。因为 shell 是一个用户程序，所以很容易用不同的程序替换掉它，这就是为什么有这么多的 Unix shell。如果你不喜欢某个 shell 的工作方式，你可以选择另一个，甚至可以自己编写一个并使用它。说到“shell”，这是不具体的。

That said, all Unix shells provide the same basic features, usually with the same syntax. The most important feature is to run programs. They all also provide filename _wildcards_, where pattern metacharacters like "\*" are expanded into a list of filenames that match the pattern. For instance, to run the program wc (word count) to count the lines, words and characters in all the files in the current directory whose names begin with book, one gives the command

> 话虽如此，所有 Unix shell 都提供相同的基本功能，通常使用相同的语法。最重要的功能是运行程序。它们都还提供文件名*通配符*，其中模式元字符(如"\*")会被扩展为与模式匹配的文件名列表。例如，要运行 wc(word count)程序来计算当前目录中以 book 开头的文件的行数、字数和字符数，可以给出命令。

\$ \*wc book\*\*

The shell expands the pattern book\* into all the filenames in the current directory that match any name beginning with book, and runs wc with those names as arguments. The wc command itself doesn't know that the list of filenames was specified by a pattern. It's important that expansion is done by the shell, not by individual programs. For many years, Microsoft's MS-DOS

> shell 会把模式 book\*扩展为当前目录中以 book 开头的所有文件名，并使用这些文件名作为参数运行 wc 命令。wc 命令本身不知道文件名列表是由模式指定的。重要的是，扩展是由 shell 而不是由单独的程序完成的。多年来，微软的 MS-DOS 都是如此。

operating system didn't work that way, so some programs did their own expansions and others didn't; users couldn't count on consistent behavior.

> 操作系统不是那种方式工作，因此有些程序进行了自己的扩展，而其他的没有；用户不能指望行为的一致性。

Another major service of the shell is input/output redirection. If a program reads from the standard input (by default the terminal), it can be made to read from an input file instead by

> shell 的另一项主要服务是输入/输出重定向。如果一个程序从标准输入(默认情况下是终端)读取，可以通过将其改为从输入文件读取来实现。

\$ _program \<infile_

and if it writes to the standard output (again by default the terminal), its output can be directed into an output file with \$ _program \>outfile_

> 如果它向标准输出(默认情况下是终端)写入，它的输出可以通过$ *program \>outfile*被重定向到输出文件中。

The output file is created if it doesn't already exist. As with filename expansion, the program doesn't know that its input or output is being redirected.

> 如果输出文件不存在，则会创建输出文件。与文件名扩展一样，程序不知道它的输入或输出正在重定向。

This is a uniform mechanism, applied by the shell, not by individual programs, and easier to use than approaches like specifying file input and output by parameters for filenames, as in

> 这是一种统一的机制，由 shell 而非单独的程序来实现，比通过参数指定文件输入和输出的方式更容易使用。

\$ _program in=infile out=outfile_

A _shell script_ is a sequence of commands that have been stored in a file.

> 一个*shell 脚本*是存储在文件中的一系列命令。

Running an instance of the shell with this file as input runs the commands of

> 运行一个 shell 实例，以此文件作为输入，运行命令。

[]{#index_split_000.html#p81}CHAPTER 4: SIXTH EDITION

67

the script as if they had been typed directly: \$ _sh \<scriptfile_

A script encapsulates a command sequence. For example, for this book, I run a sequence of simple checks that look for spelling and punctuation errors, improper formatting commands, and other potential gaffes. Each of these checks runs a program. I could type the commands over and over again, exactly the same each time. But instead, I can put the sequence of commands in a single script file called check and thus can check the book by running a single command. Other scripts print the book and make a backup copy.

> 脚本封装了命令序列。例如，对于本书，我运行一系列简单的检查，查找拼写和标点错误、不正确的格式命令以及其他潜在的失误。每个检查都运行一个程序。我可以一次又一次地输入完全相同的命令。但是，我可以将命令序列放在一个名为 check 的脚本文件中，因此可以通过运行一个命令来检查书籍。其他脚本可以打印书籍并创建备份副本。

These scripts are in effect new Unix commands, though highly specialized to me and this particular book. Such personal commands are a common use of shell scripts, a way to create shorthands for one's own frequent computations. I still use some scripts that I wrote 30 or 40 years ago, and this is not at all unusual among long-time Unix users.

> 这些脚本实际上是新的 Unix 命令，尽管对我和这本特定的书来说非常专业。这种个人命令是使用 shell 脚本的一种常见用法，是为自己的常用计算创建简写的一种方式。我仍然使用我 30 或 40 年前编写的一些脚本，这在长期使用 Unix 的用户中并不罕见。

The final step in making shell programs fully equivalent to compiled programs was to make it so that if a file was marked executable, it would be passed to a shell for execution. In this way, shell scripts became first-class citizens, indistinguishable from compiled programs when they were executed:

> 最后一步是使脚本程序完全等同于编译程序，即如果一个文件标记为可执行，它将被传递给 shell 执行。通过这种方式，脚本成为第一类公民，在执行时与编译程序无异。

\$ _check book.txt_

Shell scripts do not replace compiled programs, but they are an important part of a programmer's toolkit, both for personal use and for larger tasks. If you find yourself doing the same sequence of commands over and over again, then you put them into a shell script and thus automate away some drudgery.

> 脚本不能取代编译程序，但它们是程序员的工具箱中的重要组成部分，无论是个人使用还是更大的任务。如果你发现自己一遍又一遍地执行相同的命令序列，那么你可以将它们放入 shell 脚本中，从而自动完成一些单调的工作。

If a shell script proves to be too slow, it can be rewritten in another language.

> 如果 shell 脚本运行太慢，可以用另一种语言重写它。

We'll see more of the power of shell scripts as we examine pipes in the next section.

> 我们在下一节中检查管道时，将会看到更多的 Shell 脚本的功能。

**4.4 Pipes**

Pipes are perhaps the single most striking invention in Unix. A pipe is a mechanism, provided by the operating system and made easily accessible through the shell, that connects the output of one program to the input of another. The operating system makes it work; the shell notation to use it is simple and natural; the effect is a new way of thinking about how to design and use programs.

> 管道可能是 Unix 中最引人注目的发明。管道是操作系统提供的一种机制，通过 shell 很容易访问，它将一个程序的输出连接到另一个程序的输入。操作系统使其工作；使用它的 shell 表示法简单自然；其效果是一种关于如何设计和使用程序的新思维方式。

The idea of connecting programs has been around for a long while. One of the clearest statements in the Unix context appeared in an internal

> 连接程序的想法已经存在了很长一段时间。在 Unix 环境中，最清晰的陈述之一出现在一份内部文件中。

[]{#index_split_000.html#p82}![](./index-82_1.jpg){.calibre4}

68 CHAPTER 4: SIXTH EDITION

document that Doug McIlroy wrote in 1964, advocating, among other things, the idea of screwing programs together "like garden hose." Figure 4.1 is from a well-worn page that hung on the wall in my office at Bell Labs for 30

> 1964 年，Doug McIlroy 撰寫的文件主張，除其他事項外，還倡導將程序拧在一起“像花園轉接管一樣”的想法。 圖 4.1 來自我在貝爾實驗室的辦公室內貼了 30 年的磨損頁面。

years. By the way, notice the typing errors and the generally terrible quality.

> 这些年来，顺便提醒一下，注意打字错误和整体质量很糟糕。

This illustrates what typewritten documents often looked like. The bottom part of the figure is a corrected transcription: Summary\--what's most important

> 这个图示出了打字文件常常是什么样子的。图片下面的部分是修正后的转录：摘要--最重要的是什么？

To put my strongest concerns in a nutshell: 1. We should have some ways of coupling programs like garden hose\--screw in another segment when it becomes necessary to massage data in another way.

> 把我最强烈的担忧简述一下：1. 我们应该有一些方法来连接程序，就像花园水管一样——当有必要以另一种方式处理数据时，可以拧上另一段。

**Figure 4.1:**

Doug McIlroy's pipe idea (1964)

Doug wanted to allow arbitrary connections in a sort of mesh of programs, but it was not obvious how to describe an unconstrained graph in a natural way, and there were semantic problems as well: data that flowed between programs would have to be queued properly, and queues could explode in an anarchic connection of programs. And Ken couldn't think of any real applications anyway.

> 道格想要允许任意连接在一个程序网络中，但是如何自然地描述一个无限制的图表却不是很明显，而且还有语义上的问题：程序之间传输的数据必须要排队处理，而且在混乱的程序连接中，队列可能会爆炸。而肯也想不出任何实际的应用。

But Doug continued to nag and Ken continued to think. As Ken says,

"One day I got this idea: pipes, essentially as they are today." He added a pipe system call to the operating system in an hour; he describes it as "super trivial" given that the mechanisms for I/O redirection were already there.

> 一天我有了这个想法：管道，基本上就像它们今天的样子。他在一个小时内给操作系统添加了一个管道系统调用；他把它描述为“超级简单”，因为 I/O 重定向的机制已经存在了。

Ken then added the pipe mechanism to the shell, tried it out, and called the result "mind-blowing."

> 然后肯将管道机制加入到壳中，尝试了一下，并称之为“令人惊叹的”。

The pipe notation was simple and elegant, a single character (the vertical bar \| ) between a pair of commands. So, for example, to count the number of files in a directory, pipe the output of ls (one line per file) into the input of wc (counts the lines):

> 管道符号很简单而优雅，一个字符(竖线\|)在一对命令之间。所以，例如，要计算一个目录中的文件数，将 ls 的输出(每个文件一行)管道输入 wc(计数行)：

\$ _ls \| wc_

[]{#index_split_000.html#p83}CHAPTER 4: SIXTH EDITION

69

It is often appropriate to think of a program as a _filter_ that will read data in, process it in some way, and write the output. Sometimes this is perfectly natural, as in programs that select or mutate or count things on the fly, but sometimes the filter does not operate on the fly. For example, the sort command necessarily has to read all its input before it can produce any output, but that's irrelevant---it still makes sense to package it as a filter that can fit into a pipeline.

> 经常可以把一个程序当作一个过滤器，它会读取数据，对其进行某种处理，然后输出结果。有时这是非常自然的，比如程序可以实时选择、突变或计数，但有时过滤器并不是实时运行的。例如，排序命令必须先读取所有的输入才能产生输出，但这无关紧要---仍然可以把它封装为一个可以放入管道的过滤器。

Ken and Dennis upgraded every command on the system in a single night.

The major change was to read data from the standard input stream when there were no input filename arguments. It was also necessary to invent stderr, the standard error stream. The standard error was a separate output stream: error messages sent to it were separated from the standard output and thus would not be sent down a pipeline. Overall, the job was not hard---most programs required nothing more than eliminating extraneous messages that would have cluttered a pipeline, and sending error reports to stderr.

> 主要的变化是在没有输入文件名参数时，从标准输入流读取数据。还有必要发明标准错误流 stderr。标准错误是一个单独的输出流：发送到它的错误消息与标准输出分开，因此不会通过管道发送。总的来说，这项工作并不困难-大多数程序只需要消除会淹没管道的多余消息，并将错误报告发送到 stderr。

The addition of pipes led to a frenzy of invention that I remember vividly.

> 加入管道引發了一陣創新狂熱，我清楚地記得。

I don't hav e an exact date but it would have been in the second half of 1972, since pipes were not in the second edition of the manual (June 1972) but were present in the third edition (February 1973).

> 我没有准确的日期，但应该是在 1972 年下半年，因为管道没有在 1972 年 6 月的第二版手册中出现，但在 1973 年 2 月的第三版手册中出现了。

Everyone in the Unix room had a bright idea for combining programs to do some task with existing programs rather than by writing a new program.

> 所有在 Unix 房间里的人都有一个明智的想法，即通过结合现有程序而不是编写新程序来完成某项任务。

One of mine was based on the who command, which lists the currently logged-in users. A command like who isn't terribly relevant today when most people work on their own computer, but since the essence of time-sharing was _sharing_ the same computer, it was helpful to know who else was using the system at the same time. Indeed, who added to the sense of community: you could see who was also working, and perhaps get help if you had a problem, even if both parties were at their homes late at night.

> 一个我们使用的命令是 who，它可以列出当前登录的用户。当大多数人都在自己的电脑上工作时，这样的命令不再那么重要了，但是由于时间共享的本质就是共享同一台电脑，所以知道其他人也在使用系统是很有帮助的。实际上，who 命令增加了社区感：你可以看到谁也在工作，即使大家都是在深夜在家里，你也可以寻求帮助。

The who command prints one line for each logged-in user, grep finds all occurrences of a specific pattern, and wc counts the number of lines, so these pipelines report the state of logged-in users.

> 命令 who 会为每个已登录的用户打印一行，grep 会查找特定模式的所有出现，而 wc 会计算行数，因此这些管道可以报告已登录用户的状态。

who \# who is logged in?

who \| wc

\# how many are logged in?

who \| grep joe

\# is joe logged in?

who \| grep joe \| wc \# how many times is joe logged in?

To see what an improvement pipes were, consider how the last task would be performed without pipes, using input and output redirection to files:

> 要看看管道有多大的改善，考慮一下如果沒有管道，使用輸入和輸出重定向到文件來執行最後的任務會是什麼樣子：

[]{#index_split_000.html#p84}70 CHAPTER 4: SIXTH EDITION

who \>temp1

grep joe \<temp1 \>temp2

wc \<temp2

followed by removing the temporary files. Pipes make this into a single command without temporary files.

> 用管道合并成一个命令，而无需临时文件。

Ken's favorite pipe example was a speaking desk calculator that used Bob Morris's dc calculator program. Ken's program number printed numbers as words ("127" became "one hundred and twenty seven"), and speak synthesized speech from its input. As Ken said in an interview in 2019,

> 肯的最喜歡的管道示例是一個會說話的計算器，它使用了鮑勃·莫里斯的 dc 計算器程序。肯的程序號碼將數字以文字(“127”變成“一百二十七”)打印出來，並從其輸入中發出合成語音。正如肯在 2019 年的一次採訪中所說，

"You typed _1 2 +_ into dc, which was piped to number, which was piped to speak, and it said 'four.' "

> 你在 dc 中输入了 _1 2 +_，然后管道传递给 number，再管道传递给 speak，它说出了“四”。

\[Laughter\]

"I was never good at math."

Pipes are one of the foremost of Unix contributions, and obvious only in retrospect. As Dennis said in "The Evolution of the Unix Time-sharing System" in 1984,

> 管道是 Unix 贡献的首要之一，只有回顾过去才能明显看出。正如丹尼斯在 1984 年的《Unix 时间共享系统的演化》中所说，

"The genius of the Unix pipeline is precisely that it is constructed from the very same commands used constantly in simplex fashion. The mental leap needed to see this possibility and to invent the notation is large indeed."

> "Unix 管道的天才之处在于它是由用于单简模式的相同命令构建而成的。要看到这种可能性并发明这种表示法，需要做出巨大的思维飞跃。"

**4.5 Grep**

Unix began life as a commandline system, that is, one where users type commands to run programs, rather than pointing at and clicking icons with a mouse, as is normal when using Windows or macOS. A commandline interface is not as easy as point and click for novices, but in the hands of someone with even moderate experience, it can be far more effective. It allows for automation that's not possible with a graphical interface: sequences of commands can be run from scripts and applied to large numbers of files with a single command.

> Unix 最初是一个命令行系统，也就是说，用户输入命令来运行程序，而不像使用 Windows 或 macOS 那样用鼠标指向和点击图标。命令行界面对新手来说不像点击那么容易，但对于有一定经验的人来说，它可以更有效。它允许图形界面不可能实现的自动化：可以从脚本中运行一系列命令，并用一条命令应用于大量文件。

Unix has always had a rich collection of small commandline tools, that is, programs that handle simple frequently occurring tasks. Half a dozen commands manipulate the file system, like ls for listing the files in a directory, rather like Finder on a Mac or Explorer on Windows; cat and cp for copying files in various ways; mv ("move") for renaming; and rm for removing files. There are commands for processing file contents, like wc for counting

> Unix 一直拥有丰富的小型命令行工具，也就是处理简单常见任务的程序。有半打命令可以操作文件系统，比如 ls 用来列出目录中的文件，就像 Mac 上的 Finder 或 Windows 上的 Explorer 一样；cat 和 cp 可以以各种方式复制文件；mv(“移动”)用于重命名；rm 用于删除文件。还有一些命令用于处理文件内容，比如 wc 用于计数。

[]{#index_split_000.html#p85}CHAPTER 4: SIXTH EDITION

71

things, sort for sorting files, plus a handful for comparing files, another few for transformations like case conversion, and some for selecting parts of files.

> 事物，排序用于排序文件，加上一把用于比较文件的工具，另一些用于像大小写转换之类的转换，还有一些用于选择文件的部分。

(Unix users will recognize uniq, cmp, diff, od, dd, tail, tr, and comm.) Add another dozen tools that don't fit into those categories, and you have a repertoire of 20 or 30 commands that let you do all kinds of basic tasks easily.

> Unix 用户会识别 uniq、cmp、diff、od、dd、tail、tr 和 comm 这些命令。再加上十几个不属于这些类别的工具，你就拥有了 20 到 30 个命令，可以轻松地完成各种基本任务。

In effect, the tools are verbs in a language, and files are the nouns that the verbs apply to. The language is often irregular, and each command has optional arguments that modify its behavior; for example, sort normally sorts by line in alphabetic order, but arguments can change that so it sorts in reverse order, numerically, on specific fields, and so on.

> 实际上，工具就是语言中的动词，而文件则是这些动词应用的名词。语言通常是不规则的，每个命令都有可选的参数来修改其行为；例如，排序通常按字母顺序排序，但参数可以改变它，使其按倒序、数值或特定字段排序等等。

To use Unix well, one must learn what amounts to a family of irregular verbs, just as for natural languages. Naturally there are frequent complaints about the historical irregularities, but occasional attempts to rationalize them have for the most part not been very successful.

> 要熟练使用 Unix，就必须学习一系列不规则动词，就像学习自然语言一样。当然，人们经常抱怨这些历史上的不规则性，但是偶尔试图将它们理解化的努力大多没有成功。

The prototypical tool, the command that started us thinking about "tools"

more than just "programs," was grep, the pattern-searching program originally written by Ken Thompson. As Ken said about grep in 2019,

> 除了"程序"外，grep 还是由肯·汤普森(Ken Thompson)最初编写的模式搜索程序。肯在 2019 年关于 grep 的话是：

"I had it written but I didn't put it in the central repository of programs because I didn't want people to think that I dictated what was there.

> 我曾经写过，但是我没有把它放到程序的中央仓库里，因为我不想让人们认为我决定了那里的内容。

Doug McIlroy said 'Wouldn't it be great if we could look for things in files?' I said 'Let me think about it overnight' and the next morning I showed him the program that I had written earlier. He said 'That's exactly what I wanted.'

> 道格·麦克伊尔罗伊说：“如果我们能在文件中搜索东西，那会太棒了！”我说：“让我考虑一下，等到第二天早上，我会给他看我之前写的程序。”他说：“这正是我想要的！”

Since then grep has become a noun and a verb; it's even in the OED.

The hardest part was naming it; it was originally 's', for search."

The name grep comes from a command in the ed text editor, g/re/p, that prints all lines that match the regular expression pattern re; the Oxford English Dictionary entry for grep (Figure 4.2) has it right. (Since the OED

> 名称 grep 来自于文本编辑器 ed 中的一个命令 g/re/p，它会打印所有匹配正则表达式模式 re 的行；欧路词典条目 grep(图 4.2)正确地描述了它。(由于欧路词典的历史)

has blessed grep as a legitimate English word, I'm going to use it without special fonts or capitalization.)

> 神赐予了 grep 作为一个合法的英语单词，我将不使用特殊字体或大小写来使用它。

My personal favorite grep story comes from a day in 1972 when I was called by someone at the Labs who said

> 我最喜欢的 grep 故事发生在 1972 年的一天，当时我接到实验室里的某人的电话，他说

"I noticed that when I hold my new pocket calculator upside down, some of the numbers make letters; for example, 3 becomes E and 7

> 我注意到，当我倒置我的新口袋计算器时，一些数字会变成字母；例如，3 变成 E，7 变成 7。

becomes L. I know you guys have a dictionary on your computer. Is there any way you can tell me what words I can make on my calculator

> 变成 L. 我知道你们的电脑上有字典。有没有办法可以告诉我我可以在计算器上做什么单词？

[]{#index_split_000.html#p86}![](./index-86_1.jpg){.calibre4}

72 CHAPTER 4: SIXTH EDITION

**Figure 4.2:**

OED entry for grep

when I hold it upside down?"

Figure 4.3 shows what he had in mind.

Being in a research group, it felt good to be able to help someone who had a really practical problem. So I asked him what letters he could make when he held his calculator upside down, and he said "BEHILOS". I turned to my keyboard and typed this command:

> 在一个研究小组中，能够帮助一个有实际问题的人感觉很好。所以我问他，当他倒着拿着计算器时，他能做出什么字母，他说“BEHILOS”。我转向我的键盘，输入了这个命令：

grep 'ˆ\[behilos\]\*\$' /usr/dict/web2

The file /usr/dict/web2 is the word list from Webster's Second International dictionary---234,936 words, one per line---and the cryptic string of characters between quotes is a _regular expression_ or pattern that in this case specifies lines that contain only arbitrary combinations of any of these seven letters and nothing else.

> 文件/usr/dict/web2 是来自 Webster's Second International 字典的单词列表---234,936 个单词，每行一个---而引号中的晦涩的字符串是一个*正则表达式*或模式，在这种情况下，它指定的行只包含这七个字母中的任意组合，而不包含其他内容。

Out came the most amazing list, the 263 words in Figure 4.4. I'm a native speaker of English, but that list has a fair number of words I've nev er seen

> 出现了最令人惊叹的列表，即图 4.4 中的 263 个单词。我是英语的母语人士，但是这个列表中有相当多的我从未见过的词。

[]{#index_split_000.html#p87}![](./index-87_1.jpg){.calibre4}

CHAPTER 4: SIXTH EDITION

73

**Figure 4.3:**

BEHILOS on a calculator

before. In any case, I printed them out and sent them to the guy. I think he must have been satisfied; I never heard from him again. But he left me with a great story and a wonderful demonstration of the value of tools like grep and notations like regular expressions.

> 之前，无论如何，我把它们打印出来，然后寄给了那个人。我想他一定很满意，我从未再听到他的消息。但是他给了我一个很棒的故事，以及一个关于像 grep 这样的工具和像正则表达式这样的符号的价值的精彩示范。

Over time, the word grep became a noun, a verb, a gerund (grepping), and part of everyday speech in the Unix community. Hav e you ever grepped your apartment for your car keys? Bumper stickers and t-shirts riffed on the AT&T commercial that invited people to "reach out and touch someone":

> 随着时间的推移，grep 这个词变成了名词、动词、动名词(grepping)，也成为了 Unix 社区日常语言的一部分。你曾经在你的公寓里用 grep 搜索过你的车钥匙吗？保险杠贴纸和 T 恤上印的也受到了 AT&T 的商业广告的启发，那个广告邀请人们“伸手去触摸某人”：

"Reach out and grep someone."

Arno Penzias, Nobel Prize winner and, as vice president of Research, my boss three levels up, called me one day to ask whether it was safe for him to use this phrase in a public talk.

> 諾貝爾獎得主阿諾·彭齊亞斯，他是研究部門的副總裁，有一天他打電話給我，問我他可以在公開演講中使用這個短語是否安全。

**4.6 Regular expressions**

I've used the phrase "regular expression" without really explaining it. A regular expression is a notation for specifying a pattern of text. It could be as simple as a word like _expression_ or a phrase like _regular expression_ or something significantly more complicated. In effect, a regular expression is a small language for describing text patterns. In the usual notations, a word or phrase is a regular expression that stands for itself in text, and a regular

> 我使用了“正则表达式”这个短语，但没有真正解释它。正则表达式是一种用于指定文本模式的符号。它可以像*expression*这样简单，也可以像*regular expression*这样的短语，或者更复杂的东西。实际上，正则表达式是一种用于描述文本模式的小型语言。在通常的符号中，一个单词或短语是一个正则表达式，它在文本中代表自己，而一个正则表达式则代表一种更复杂的文本模式。

[]{#index_split_000.html#p88}74 CHAPTER 4: SIXTH EDITION

b

be

bebless beboss

bee beeish

beelol

bees bel

belee belibel

belie bell

belle

bes besee

beshell besoil

bib bibb

bibble

bibi bibless

bilbie bilbo

bile bilio

bill

bilo bilobe

bilsh bios

biose biosis

bis

bleb blee bleo bless

blibe bliss blissless

blo blob

bo bob

bobbish bobble

bobo

boho boil bole bolis

boll bolo boo

boob boohoo

bool boose

bose bosh boss

e

ebb eboe

eel eelbob

eh el

elb ell elle

els else

es ess

h

he

heel heelless

hei heii

helbeh

hele helio

heliosis hell

hellhole hellish

hello

heloe helosis

hi hie

hill his

hish

hiss ho

hob hobbil

hobble hobo

hoe

hoi hoise

hole holeless

holl hollo

hoose

hoosh hose

hosel hoseless

i

ibis ibisbill

ie ihi

ill illess

illish io

is

isle isleless

iso isohel

issei l

lee

lees lei

less lessee

li libel

libelee

lie liesh

lile lill lis

lish lisle

liss lo

lob lobbish

lobe lobeless

lobo

lobose loess

loll loo

loose loosish

lose

losel losh

loss lossless

o

obe obese

obi oboe

obol obole

obsess oe

oes

oh ohelo

oho oii oil oilhole

oilless

oleo oleose

olio os

ose osse

s

se see

seel seesee

seise sele

sell

sellie sess

sessile sh

she shee

shell

shi shiel

shies shih

shill shilloo

shish

sho shoe

shoebill shoeless shole

shoo shooi

shool si

sib sie sil sile

sill

silo siol sis

sise sisel

sish sisi

siss sissoo

slee slish

slob sloe sloo

sloosh slosh

so sob

soboles soe

soh

soho soil soilless

sol sole

soleil soleless

soles soli

solio solo

sool sooloos

sosh

soso sosoish

soss sossle

[]{#index_split_001.html}

**Figure 4.4:**

Make these on your calculator upside-down expression recognizer will find that word wherever it occurs.

> 在计算器上做这些倒置表达式识别器将会在任何地方发现该词。

Regular expressions also make it possible to specify more complicated patterns by giving special meanings to some characters, called metacharacters. For example, in grep, the metacharacter "." will match any single character, and the metacharacter "\*" will match any number of repetitions of the

> 正则表达式还可以通过给一些字符赋予特殊含义，即所谓的元字符，来指定更复杂的模式。例如，在 grep 中，元字符“。”将匹配任何单个字符，元字符“\*”将匹配任意数量的重复。

[]{#index_split_001.html#p89}CHAPTER 4: SIXTH EDITION

75

preceding character, so the pattern (.\*) will match any sequence of characters enclosed in parentheses.

> (.\*)匹配任何用括号括起来的字符序列，前面的字符不受限制。

Unix has had a long love aff air with regular expressions, which are pervasive in text editors, in grep and its derivatives, and in many other languages and tools. Regular expressions of a slightly different flavor are also used in filename patterns as seen in shell "wildcards" that match groups of filenames.

> Unix 和正则表达式有着悠久的爱情缘分，它们遍布文本编辑器、grep 及其衍生物以及许多其他语言和工具中。稍有不同的正则表达式也用于文件名模式，如 shell 中的"通配符"可以匹配一组文件名。

Ken Thompson's QED editor on Multics and later the GE 635 (where I first encountered it) used regular expressions, and Ken invented a very fast algorithm that allowed it to process arbitrarily complicated expressions quickly. The algorithm was even patented. QED was sufficiently powerful that in principle it was possible to write any program just using editor commands (though no one in their right mind would do so). I even wrote a tutorial on QED programming; that was largely wasted effort, but it started me writing such documents.

> 肯·汤普森(Ken Thompson)在 Multics 上开发的 QED 编辑器以及我最初遇到的 GE 635 上也使用了正则表达式，肯发明了一种非常快速的算法，可以快速处理任意复杂的表达式。该算法甚至被专利了。QED 的功能非常强大，原则上可以只使用编辑器命令来编写任何程序(尽管没有人会这么做)。我甚至写了一个关于 QED 编程的教程；这大部分是徒劳的努力，但它让我开始写这样的文档。

QED was overkill for most purposes. The Unix ed text editor that Ken and Dennis wrote originally and several other people subsequently modified (even me) was much simpler than QED, but it too had regular expressions.

> QED 对大多数用途来说都是过度设计。肯和丹尼斯最初写的 Unix ed 文本编辑器，以及其他几个人后来修改的(甚至我也修改过)比 QED 要简单得多，但它也有正则表达式。

Since grep was derived from ed, its regular expressions were the same as those in ed.

> 由于 grep 源自 ed，因此它的正则表达式与 ed 中的相同。

A variant style of regular expressions is used for filename wildcards.

Although wildcards are interpreted by the shell, because primary memory on the PDP-7 was so limited, the first implementation was a separate program called glob (for "global") called by the shell, and the act of generating an expanded list of filenames from a pattern was called "globbing." The name glob lives on in libraries in several programming languages today, including Python.

> 尽管通配符是由 shell 解释的，但由于 PDP-7 的主存储器容量有限，第一个实现是一个名为 glob(即"全局")的独立程序，由 shell 调用，而从模式生成扩展的文件名列表的动作被称为"globbing"。今天，名为 glob 的库仍存在于包括 Python 在内的几种编程语言中。

One of Al Aho's early contributions to Unix was an extension of grep that allowed a richer class of regular expressions, for example making it possible to search for alternatives like this\|that. Al called the program _egrep_, for

> 一个阿尔·阿霍对 Unix 的早期贡献是一个扩展的 grep，可以使用更丰富的正则表达式，例如可以搜索这样的替代品\|那个。阿尔将这个程序称为*egrep*，

"extended grep."

It's worth saying a bit more about egrep, since the story behind it is an excellent example of the kind of interplay between theory and practice, and of typical interactions among members of 1127, that led to so much good software. This story comes from Doug McIlroy:

> egrep 的背后故事是理论与实践之间以及 1127 成员之间典型交互的绝佳例子，值得多说一些。这个故事来自 Doug McIlroy：

"Al Aho's first egrep was a routine implementation of an algorithm from _The Design and Analysis of Computer Algorithms_ by Aho, Hopcroft and Ullman. I promptly used it for a calendar program that used a huge automatically generated regular expression to recognize date patterns like 'today,' 'tomorrow,' 'until the next business day,' and

> 阿霍的第一个 egrep 是根据 Aho、Hopcroft 和 Ullman 的《计算机算法的设计与分析》中的算法进行的常规实现。我立即用它来编写一个日历程序，该程序使用一个巨大的自动生成的正则表达式来识别像“今天”、“明天”、“直到下一个工作日”等日期模式。

[]{#index_split_001.html#p90}76 CHAPTER 4: SIXTH EDITION

so on, represented in a large range of date styles.

To Al's chagrin, it took something like 30 seconds to compile into a recognizer that would then run in no time at all.

> 让艾尔感到惊讶的是，编译成识别器只需要 30 秒，然后就能立刻运行。

He then came up with the brilliant strategy of generating the recognizer lazily as parts of it were needed, rather than all in advance, so only a tiny fraction of the exponentially vast number of states were ev er constructed. That made a tremendous difference: in practice, egrep always ran fast no matter how complex the pattern it was dealing with. So egrep is distinguished by technical brilliance, invisible unless you know how badly standard methods can perform."

> 他随后想出了一个聪明的策略，即只有当需要时才会懒惰地生成识别器，而不是提前生成所有的，因此只有极少量的指数级的状态被构建出来。这带来了巨大的不同：实践中，egrep 无论处理的模式有多复杂，都能运行得很快。因此，egrep 的特点是技术上的聪明，除非你知道标准方法的表现有多糟糕，否则是看不到的。

This is a common Unix story: a real problem from a real user, deep knowledge of relevant theory, effective engineering to make the theory work well in practice, and continuous improvement. It all came together because of broad expertise in the group, an open environment, and a culture of experimenting with new ideas.

> 这是一个典型的 Unix 故事：来自真实用户的真实问题、相关理论的深入知识、有效的工程技术，使理论能够在实践中得到很好的应用，以及持续改进。这一切都是由于团队广泛的专业知识、一个开放的环境和尝试新想法的文化而实现的。

**4.7 The C programming language**

New programming languages have been a big part of Unix since the very beginning.

> 自从一开始，新的编程语言就一直是 Unix 的重要组成部分。

One of the most important contributions of Multics was its attempt to write the operating system in a high-level language, PL/I. PL/I was created in 1964 by IBM to try to combine all the good ideas from Fortran, Cobol and Algol into a single language. It turned out to be a grand example of the second system effect. The language was too big and complicated for most programmers, it was hard to compile, and a working compiler for Multics was not delivered on time. As an interim measure, Doug McIlroy and Doug East-wood created a simplified subset called EPL ("Early PL/I") for use with Multics, but it was still a complicated language.

> 一项最重要的多特斯贡献是，它试图用高级语言 PL / I 编写操作系统。 PL / I 由 IBM 于 1964 年创建，旨在将所有 Fortran，Cobol 和 Algol 的好主意结合成一种语言。结果发现，这是第二系统效应的宏伟例子。该语言对大多数程序员来说太大复杂，很难编译，而且多特斯的工作编译器没有按时交付。作为一种临时措施，道格·麦克罗伊(Doug McIlroy)和道格·伊斯特伍德(Doug East-wood)为多特斯创建了一个简化的子集，称为 EPL(“早期 PL / I”)，但它仍然是一种复杂的语言。

BCPL ("Basic Combined Programming Language") was another language intended for system programming. It had been designed by Martin Richards, a professor at the University of Cambridge, and he wrote a compiler for it while visiting MIT in 1967. BCPL was much simpler than any dialect of PL/I, and was well suited for writing operating system code. Members of the Bell Labs Multics effort were very familiar with BCPL.

> BCPL(“基本组合编程语言”)是另一种用于系统编程的语言。它由剑桥大学教授 Martin Richards 设计，他于 1967 年访问 MIT 时编写了一个编译器。BCPL 比 PL / I 的任何方言都要简单得多，非常适合编写操作系统代码。贝尔实验室 Multics 工作组对 BCPL 非常熟悉。

When the Labs pulled out of Multics, Ken Thompson decided that "no computer is complete without Fortran," so he started to write a Fortran compiler for the PDP-7. This proved too tough, since PDP-7 Unix had only 4K

> 当实验室从 Multics 撤出时，肯·汤普森决定“没有 Fortran，没有完整的电脑”，因此他开始为 PDP-7 编写一个 Fortran 编译器。由于 PDP-7 Unix 只有 4K，这太难了。

18-bit words (8 KB) of primary memory for user programs like a compiler.

[]{#index_split_001.html#p91}CHAPTER 4: SIXTH EDITION

77

Ken kept redesigning, eventually coming up with a language that did fit the PDP-7 and was much closer to BCPL than to Fortran. He called it B. As Dennis Ritchie explained in "The Development of the C Language" in 1993,

> 肯一直在重新设计，最终找到一种符合 PDP-7 的语言，更接近 BCPL 而不是 Fortran。他称之为 B。正如丹尼斯·里奇在 1993 年的《C 语言的发展》中所解释的那样。

"B can be thought of as C without types; more accurately, it is BCPL

squeezed into 8K bytes of memory and filtered through Thompson's brain. Its name most probably represents a contraction of BCPL, though an alternate theory holds that it derives from Bon, an unrelated language created by Thompson during the Multics days. Bon in turn was named either after his wife Bonnie, or (according to an encyclope-dia quotation in its manual), after a religion whose rituals involve the murmuring of magic formulas."

> 被压缩到 8K 字节的内存中，并通过汤普森的大脑过滤，它的名字很可能代表着 BCPL 的缩写，不过另一种理论认为它源自 Thompson 在 Multics 时期创造的一种不相关的语言 Bon，Bon 又可能是以他的妻子 Bonnie 的名字命名，或者(根据手册中的一段百科全书引用)以一种宗教的名字命名，这种宗教的仪式涉及到咕哝魔法公式。

Up to this point, the computers in our story have been "word-oriented,"

not "byte-oriented." That is, they manipulate information in chunks that are significantly larger than a single byte. The IBM 7090 and similar computers like the GE series manipulated information naturally only in chunks that were 36 bits (roughly four bytes); PDP-7 chunks were 18 bits (two bytes).

> 他们不是“基于字节的”。也就是说，它们操作的信息块比单个字节大得多。IBM 7090 和类似的计算机，如 GE 系列，自然只能以 36 位(大约 4 个字节)的块来操作信息；PDP-7 的块是 18 位(2 个字节)。

Word-oriented computers were clumsy for processing bytes individually or in sequences: programmers had to use library functions or go through programming contortions to access the individual bytes that were packed into the larger chunks.

> 言语导向的计算机对于单独处理字节或序列是笨拙的：程序员必须使用库函数或者通过编程技巧来访问打包在更大块中的单个字节。

By contrast, the PDP-11 was byte-oriented: its fundamental unit of primary memory was the 8-bit byte, not the 18- or 36-bit words of earlier computers, though it could also manipulate information in larger chunks like 16-and 32-bit integers and 16-bit addresses.

> 相比之下，PDP-11 是基于字节的：它的主存储器的基本单位是 8 位字节，而不是早期计算机的 18 位或 36 位字，尽管它也可以处理更大的块，如 16 位和 32 位整数和 16 位地址。

B was a good fit for word-oriented computers like the PDP-7 but not for byte-oriented ones like the PDP-11, so when the PDP-11 arrived, Dennis started to enhance B for the new architecture and to write a compiler for it.

> B 适合诸如 PDP-7 这样以字为主的计算机，但不适合诸如 PDP-11 这样以字节为主的计算机，因此当 PDP-11 到来时，丹尼斯开始为新的架构增强 B，并为其编写编译器。

The new language was called "NB," for "New B," and eventually it became C.

> 新语言被称为“NB”，代表“新 B”，最终它变成了 C。

One of the main differences was that where B was typeless, C supported data types that matched the data types that the PDP-11 provided: single bytes, two-byte integers, and eventually floating-point numbers with four or eight bytes. And where languages like BCPL and B treated pointers (memory addresses) and integers as the same, C formally separated them, though for many years programmers unwisely treated them as if they were the same size.

> 一个主要的不同是，B 是无类型的，而 C 支持与 PDP-11 提供的数据类型相匹配的数据类型：单字节、两字节整数，最终还有四字节或八字节的浮点数。而像 BCPL 和 B 这样的语言将指针(内存地址)和整数视为相同的，C 正式将它们分开，尽管多年来程序员不明智地将它们视为相同的大小。

One of C's novel contributions to programming languages was the way that it supported arithmetic operations on typed pointers. A pointer is a value corresponding to an address, that is, a location in primary memory, and it has

> C 语言在编程语言中的一项新颖贡献是它支持指针类型的算术运算。指针是一个对应于地址(即主存中的位置)的值，它具有

[]{#index_split_001.html#p92}78 CHAPTER 4: SIXTH EDITION

a type, the type of the objects that it will point to. If that location corresponds to an element of an array of that particular type of object, then in C, adding 1 to the pointer yields the address of the next element of the array.

> 一种类型，指向的对象的类型。如果该位置对应于该类型对象的数组的一个元素，那么在 C 中，将指针加 1 就可以得到数组的下一个元素的地址。

Although careless use of pointers is a recipe for broken code, pointer arithmetic is natural and works well when used correctly.

> 尽管不小心使用指针会导致代码出错，但是如果正确使用，指针运算是很自然的，并且能够很好地工作。

It had been clear for some time that Unix should be converted from assembly language to a higher level language, and C was the obvious choice.

> 很明显，Unix 应该从汇编语言转换为更高级的语言，而 C 是显而易见的选择。

Ken tried three times in 1973 to write the kernel in C but it proved too difficult until Dennis added a mechanism for defining and processing nested data structures (struct) to the language. At that point, C was sufficiently expressive for writing operating system code, and Unix became mostly a C

> 陈在 1973 年尝试了三次用 C 编写内核，但是发现太难，直到丹尼斯增加了一种定义和处理嵌套数据结构(struct)的机制，C 的表达能力就足够写操作系统代码，Unix 也基本上变成了 C 编写的。

program. The 6th edition kernel has about 9,000 lines of C and about 700

lines of assembly language for machine-specific operations like setting up registers, devices and memory mapping.

> 组装语言的行，用于像设置寄存器、设备和内存映射等特定机器操作。

The first widely distributed description of C was _The C Programming_ _Language_ (Figure 4.5), a book that Dennis and I published in 1978; a second edition was published in 1988.

> 首个广泛发行的 C 语言描述是《C 程序设计语言》(图 4.5)，这本书由丹尼斯和我在 1978 年出版；第二版于 1988 年出版。

I had learned B rather superficially, and for my own amusement wrote a tutorial to help others to learn it too. When Dennis created C, it was easy to modify the B tutorial to make one for C. The C tutorial proved to be popular, and as Unix and C spread, I thought that it would be worth trying to write a book about C. Naturally I asked Dennis if he would write it with me. He might have initially been reluctant, but I twisted his arm harder and eventually he agreed. Getting Dennis to work on the book was the smartest or maybe just the luckiest thing I ever did in my technical career---it made the book authoritative because Dennis was a co-author, and it allowed me to include his reference manual.

> 我只是草率地学习了 B，为了自娱自乐，我写了一本教程来帮助别人也学习它。当丹尼斯创造了 C 时，很容易修改 B 教程，制作一本 C 教程。这本 C 教程很受欢迎，随着 Unix 和 C 的传播，我认为写一本关于 C 的书是值得一试的。我自然而然地问了丹尼斯是否愿意和我一起写这本书。他最初可能不太愿意，但是我更加坚持，最终他同意了。让丹尼斯参与这本书的写作是我在技术生涯中最聪明也许是最幸运的事情---因为丹尼斯是联合作者，这让这本书具有权威性，也让我可以把他的参考手册收入其中。

I wrote the first drafts of most of the tutorial material originally, but Dennis wrote the chapter on system calls, and of course provided the reference manual. We made many alternating passes over the main text, so that's a blend of our styles, but the reference manual stayed almost exactly as it had been, a pure example of Dennis's writing. It describes the language with what Bill Plauger once called "spine-tingling precision." The reference manual is like C itself: precise, elegant, and compact.

> 我最初写了大部分教程材料的初稿，但是丹尼斯写了系统调用的章节，当然还提供了参考手册。我们对主文本做了多次交替修改，所以这是我们两种风格的结合，但是参考手册几乎完全保留了原样，是丹尼斯纯粹的写作风格的一个纯粹的例子。它以比尔·普劳格曾经称之为“令人骨髓发凉的精确度”描述语言。参考手册就像 C 语言本身一样：精确、优雅而简洁。

The first official C standard, from ANSI, the American National Standards Institute (and also from ISO, the International Standards Organization) was completed in 1989. Its description of the language was directly based on Dennis's reference manual. Dennis was involved in the early stages of the first C standard, where his standing as the creator of the language gav e his opinions weight, and he was able to head off one or two really bad proposals.

> 美国国家标准学会(ANSI)和国际标准组织(ISO)于 1989 年完成了第一个正式的 C 标准。该标准对语言的描述直接基于丹尼斯的参考手册。丹尼斯参与了第一个 C 标准的早期阶段，他作为语言的创造者的地位赋予了他的意见权重，他能够阻止一两个真正糟糕的提案。

[]{#index_split_001.html#p93}![](./index-93_1.jpg){.calibre4}

CHAPTER 4: SIXTH EDITION

79

**Figure 4.5:**

Cover of K&R first edition, 1978

The C language is important, but so also is its use of a standard library that provides the basic facilities that programmers need for operations like formatted input and output, string processing, and mathematical functions. C

> C 语言很重要，但标准库也同样重要，它提供程序员所需的基本功能，如格式化输入和输出、字符串处理和数学函数。C

came with a modest-sized library of such functions, so that programmers did not need to reinvent each routine when they wrote a new program.

> 他们带来了一个规模适中的这样的函数库，这样程序员们在编写新程序时就不需要重新发明每个例程了。

The largest library component provided formatted output, familiar today to all programmers through C's printf function, which has been adopted into many other languages. Mike Lesk's portable I/O package, written in 1972 so that programs could be easily moved to and from Unix, contained the first version of printf and also included scanf for parsing formatted input. These were reworked and included with the C compiler.

> 最大的图书馆组件提供格式化的输出，现今所有程序员都熟悉的 C 的 printf 函数，它已被采用到许多其他语言中。 1972 年 Mike Lesk 编写的可移植 I/O 包，使程序可以轻松地在 Unix 之间移动，包含了第一个版本的 printf，还包括用于解析格式化输入的 scanf。这些被重新设计，并包含在 C 编译器中。

Although printf and scanf have had extensions since, the core set of conversions work as they did in the early 1970s, as do most of the other functions in the library. Today, the standard library is just as much a part of the C

> 虽然 printf 和 scanf 自从以前就有了扩展，但核心转换集仍像 1970 年代初那样工作，大多数标准库中的其他函数也是如此。今天，标准库与 C 语言一样重要。

standard as is the language specification itself.

It's interesting to contrast the C approach to other languages. In Fortran and Pascal, for example, input and output are part of the language, with special syntax for reading and writing data. Some other languages don't include

> 有趣的是比较 C 语言与其他语言的不同。例如，在 Fortran 和 Pascal 中，输入输出是语言的一部分，有特殊的语法来读取和写入数据。而一些其他的语言则没有包含这些功能。

[]{#index_split_001.html#p94}80 CHAPTER 4: SIXTH EDITION

input and output and at the same time don't provide a standard library, which is probably the least satisfactory choice.

> 输入和输出同时又不提供标准库，这可能是最不令人满意的选择。

C has been very successful, one of the mostly widely used languages of all time. Although it began life on PDP-11 Unix, it has spread to essentially ev ery kind of computer that exists. As Dennis said in a paper for the second _History of Programming Languages_ conference in 1993,

> C 已经取得了非常成功的成果，是有史以来使用最广泛的语言之一。虽然它最初是在 PDP-11 Unix 上诞生的，但它已经扩展到几乎所有存在的计算机上。正如丹尼斯在 1993 年第二届编程语言历史会议上的论文中所说：

"C is quirky, flawed, and an enormous success. While accidents of history surely helped, it evidently satisfied a need for a system implementation language efficient enough to displace assembly language, yet sufficiently abstract and fluent to describe algorithms and interactions in a wide variety of environments."

> C 是有怪癖、有缺陷，但却取得了巨大的成功。虽然历史的巧合也起到了帮助，但它显然满足了一种需求，即一种系统实现语言既足够有效以取代汇编语言，又足够抽象和流畅以描述各种环境中的算法和交互。

Of course there are many programming languages, often with noisy adherents and detractors, and C comes in for its share of criticism. It remains the core language of computing, however, and is almost always in the top two or three in lists of language popularity, influence and importance. To my mind, no other language has ever achieved the same balance of elegance, expressiveness, efficiency and simplicity. C has also inspired the basic syntax of many other languages, including C++, Java, JavaScript, Awk and Go.

> 当然有很多编程语言，经常有支持者和反对者，C 也不例外受到批评。但它仍然是计算机的核心语言，而且几乎总是在语言流行度、影响力和重要性的排行榜上排在前两三位。在我看来，没有其他语言能够像 C 语言一样做到优雅、表达力、效率和简洁的完美平衡。C 语言还启发了许多其他语言的基本语法，包括 C++、Java、JavaScript、Awk 和 Go。

It has been an exceptionally influential contribution.

**4.8 Software Tools and Ratfor**

By mid to late 1975, Unix had been publicly described at conferences and in journal papers and the 6th edition was in use at perhaps a hundred universities and a limited number of commercial operations. But most of the technical world still used Fortran and ran on operating systems from hardware vendors, like IBM's System/360. Locally, most programmers at Murray Hill used the GE 635 with GE's batch operating system GECOS (renamed GCOS

> 1975 年中末，Unix 已经在会议上和期刊文献中公开描述，第六版在大约一百所大学和一些商业运营中使用。但大多数技术世界仍然使用 Fortran，运行硬件供应商的操作系统，如 IBM 的 System / 360。当地，Murray Hill 的大多数程序员使用 GE 635，并使用 GE 的批处理操作系统 GECOS(更名为 GCOS)。

when GE sold its computer business to Honeywell in 1970).

By 1973, I had started to program in C regularly, but I was still writing Fortran as well. Although Fortran was fine for numerical computation, its control-flow statements were almost non-existent and it was constrained by its origin as a punchcard-based language from the 1950s. By contrast, C control flowed naturally, so to speak.

> 1973 年，我开始经常使用 C 编程，但我仍然也在写 Fortran。尽管 Fortran 对于数值计算很好，但它的控制流语句几乎不存在，并且它受到 1950 年代基于穿孔卡的语言的限制。相比之下，C 的控制流很自然，可以这么说。

Accordingly, I wrote a simple compiler that would translate a dialect of Fortran that looked like C into valid Fortran. I called it _Ratfor_, for "rational Fortran." Ratfor converted C control flow, with _if-else_, _for_, _while_, and braces for grouping, into Fortran's IF and GOTO statements and its one looping

> 因此，我编写了一个简单的编译器，可以将类似 C 的 Fortran 方言翻译成有效的 Fortran。我称之为*Ratfor*，意为“合理的 Fortran”。 Ratfor 将 C 的控制流，包括*if-else*，_for_，*while*和大括号用于分组，转换为 Fortran 的 IF 和 GOTO 语句及其一个循环。

[]{#index_split_001.html#p95}CHAPTER 4: SIXTH EDITION

81

construct, the DO loop. The preprocessor also provided notational con-veniences like free-form input (not the rigidly formatted 80-column card images that Fortran still required), a convenient comment convention, and natural logical and relational operators like \< and \>= instead of Fortran's klunky .LT. and .GE. forms.

> 构建 DO 循环。预处理器还提供了诸如自由格式输入(不是 Fortran 仍然需要的严格格式化的 80 列卡图像)、便捷的注释约定以及自然的逻辑和关系运算符(如<和>=)而不是 Fortran 笨拙的.LT.和.GE.形式。

As a short example, here's the Fortran program of Chapter 1 in one of several ways that it might be written in Ratfor:

> 以下是第一章的 Fortran 程序的简短示例，用 Ratfor 编写的几种方式之一：

\# make v an identity matrix

do i = 1, n

do j = 1, n

if (i == j)

v(i,j) = 1.0

else

v(i,j) = 0.0

Ratfor was the first example of a language that based its syntax on C.

Writing Fortran in Ratfor was, if I do say so myself, infinitely more pleasant than writing standard Fortran. Ratfor didn't change Fortran semantics or data types---it had no features for processing characters, for instance---but for anything where Fortran would be a good choice, Ratfor made it better. Free-form input and C-like control flow made it feel almost like writing in C.

> 写 Ratfor 的 Fortran 比写标准 Fortran，如果我这么说，要舒服得多。Ratfor 没有改变 Fortran 的语义或数据类型——例如它没有处理字符的功能——但是对于任何 Fortran 都是一个很好的选择，Ratfor 让它变得更好。自由形式的输入和类似 C 的控制流使它感觉几乎像在写 C 一样。

In a tour de force of both theory and practice, Brenda Baker created a program called struct that translated arbitrary Fortran programs into Ratfor.

> 布伦达·贝克尔(Brenda Baker)以其理论和实践的双重杰作，创建了一个名为 Struct 的程序，可以将任意的 Fortran 程序转换为 Ratfor。

Brenda showed that almost any Fortran program has a well-structured form; there is essentially a unique best way to render it in Ratfor. People who used struct found that the Ratfor version was almost always clearer than the Fortran they had originally written.

> 布伦达表明，几乎任何 Fortran 程序都具有良好的结构形式；用 Ratfor 渲染它几乎只有一种最佳方式。使用结构的人发现，Ratfor 版本通常比他们最初编写的 Fortran 更清晰。

Bill Plauger and I decided to write a book to evangelize the Unix tools philosophy for a wider audience: programmers who were writing Fortran on non-Unix systems. _Software Tools_, which was published in 1976, presented Ratfor versions of standard Unix tools: file comparison, word counting, grep, an editor like ed, a roff-like text formatter, and a Ratfor preprocessor itself, all written in Ratfor.

> 比尔·普劳格和我决定为更广泛的受众书写一本书来传播 Unix 工具哲学：那些在非 Unix 系统上编写 Fortran 的程序员。1976 年出版的《软件工具》提供了标准 Unix 工具的 Ratfor 版本：文件比较、字数统计、grep、类似 ed 的编辑器、类似 roff 的文本格式化器以及 Ratfor 预处理器，全部用 Ratfor 编写。

Our timing was about right; the book sold moderately well and a Software Tools User Group sprung up, spearheaded by Debbie Scherrer, Dennis Hall and Joe Sventek at Lawrence Livermore Labs. They polished and refined the programs, added new tools of their own, made distributions of the code, organized conferences, and kept everything running smoothly for years.

> 我们的时机恰到好处；这本书销售量适中，劳伦斯·利弗莫尔实验室的黛比·舍尔尔、丹尼斯·霍尔和乔·斯文特克牵头成立了一个软件工具用户组。他们改进和完善了程序，添加了自己的新工具，发布了代码，组织了会议，并且多年来保持着一切运行正常。

Their code was ported to more than 50 operating systems and the user group remained active and influential until it disbanded in the late 1980s.

> 他们的代码被移植到 50 多个操作系统，用户组一直保持活跃和有影响力，直到 1980 年代末解散。

[]{#index_split_001.html#p96}82 CHAPTER 4: SIXTH EDITION

In 1981 Bill and I published a version of the _Tools_ book based on Pascal, which at the time was popular as a teaching language in universities. Pascal had good properties, including sensible control flow and recursion, both of which were missing from Fortran.

> 1981 年，比尔和我出版了一本基于 Pascal 的《工具》书，当时 Pascal 作为大学教学语言很受欢迎。Pascal 具有良好的特性，包括明智的控制流和递归，而这两者在 Fortran 中都缺失。

Unfortunately, it also had some not so good properties, like awkward input and output and almost unusable character strings, which I described in a paper titled "Why Pascal is Not My Favorite Programming Language." I submitted the paper to a journal, but it was rejected as too controversial, or perhaps not substantial enough. It never was published, but in spite of that, it's cited surprisingly often.

> 遗憾的是，它也有一些不太好的特性，比如笨拙的输入输出和几乎无法使用的字符串，我在一篇名为“为什么帕斯卡不是我最喜欢的编程语言”的论文中描述了这些特性。我把论文提交给了一份期刊，但是因为太有争议或者不够实质性而被拒绝了。它从未被发表，但是尽管如此，它仍然被人们经常引用。

In any case, as C and Unix became more widely available, Pascal's serious limitations made it less and less popular, so _Software Tools in Pascal_ was not widely read. In hindsight, a C version would have had far more impact, both in the short term and in the long run.

> 无论如何，随着 C 和 Unix 的普及，Pascal 的严重局限性使它变得越来越不受欢迎，因此《Pascal 软件工具》并没有得到广泛阅读。事后看来，C 语言的版本无论是短期还是长期，都会产生更大的影响。

**4.9 Biography: Doug McIlroy**

Rob Pike has called Doug McIlroy "the unsung hero of Unix," and I agree. Ken Thompson says that Doug is smarter than everyone else, which also seems accurate, though Doug himself says "I'll leave to others to assess how smart I may be, but I know that many of BTL's practicing mathematicians were much smarter." Suffice it to say that there were many outstanding people at the Labs, the imposter syndrome was not unknown, and one was continuously stretched trying to keep up.

> 鲁柏·派克称道格·麦克爱尔鲁为“Unix 的无名英雄”，我也同意。肯·汤普森表示道格比其他人都聪明，这似乎也是准确的，不过道格本人却说：“我将把评估我有多聪明的事留给别人，但我知道贝尔实验室(BTL)里有许多优秀的数学家，他们都比我聪明得多。”可以说，实验室里有许多杰出的人，也不乏冒充者，每个人都在不断努力跟上进度。

No matter who is right here, Unix might not have existed, and certainly would not have been as successful, without Doug's good taste and sound judgment of both technical matters and people.

> 无论谁在这里是对的，没有道格的良好品味和对技术和人的正确判断，Unix 可能不会存在，肯定不会取得如此成功。

Doug received his undergraduate degree in physics from Cornell in 1954

and his PhD in applied mathematics from MIT in 1959. He too worked for a summer at Bell Labs, joined permanently in 1958, and became head of the Computing Techniques Research department in 1965, two years before I first met him. As described earlier, I spent the summer of 1967 as an intern in Doug's department, nominally working on a storage allocator problem that he suggested but in fact doing my own thing. One of his many good qualities as a manager was that he wasn't bothered by that at all.

> 他在 1959 年从麻省理工学院获得应用数学博士学位。他也曾在贝尔实验室工作了一个夏天，1958 年正式加入，1965 年成为计算技术研究部门的负责人，我第一次见他的两年前。正如前面描述的，我在 1967 年夏天作为一名实习生在道格的部门工作，从名义上说是在解决他提出的一个存储分配问题，但实际上我在做自己的事情。他作为一个经理的众多优秀品质之一就是，他对此并不在意。

I've already mentioned Doug's early language work on PL/I and EPL.

Once Unix was underway, he wrote a wide variety of fundamental software.

His storage allocator malloc was used for many years, and his research on allocators affected subsequent work. He also wrote a bunch of commands; the list on his web page at Dartmouth includes spell, diff, sort, join,

> 他的存储分配程序 malloc 被使用了多年，他对分配程序的研究也影响了后续的工作。他还编写了一堆命令；他在达特茅斯大学的网页上的列表包括 spell、diff、sort、join。

[]{#index_split_001.html#p97}CHAPTER 4: SIXTH EDITION

83

graph, speak, tr, tsort, calendar, echo, and tee.

Some of these are small, like echo, while some are large, like sort and diff, but most are central to Unix computing and many are used to this day.

> 有些很小，比如 echo，有些很大，比如 sort 和 diff，但大多数都是 Unix 计算的核心，而且至今仍在使用。

Of course pipes were his idea too, though the final version used Ken's syntax, and their existence was due to Doug's ongoing lobbying for such a mechanism.

> 当然管道也是他的主意，尽管最终版本使用了肯的语法，而且它们的存在是由道格不断游说这种机制而实现的。

His version of spell made effective use of a dictionary and heuristics for identifying parts of speech to find potential spelling mistakes, using only meager resources.

> 他的拼写版本利用字典和词性识别启发式算法，仅用有限的资源就可以发现潜在的拼写错误。

Doug's version of diff implements an efficient algorithm (invented independently by Harold Stone and Tom Szymanski) for comparing two text files, finding a minimal sequence of changes that will convert one into the other. This code is at the heart of source code control systems that manage multiple versions of files. Such systems most often work by storing one version and a set of diffs, generating other versions by running the diff algorithm. This is also used in the patch mechanism that's used for updating programs---rather than sending a new version of a program to someone, send a sequence of ed editing commands, computed by diff, that will convert the old version into the new.

> 道格的 diff 版本实现了由 Harold Stone 和 Tom Szymanski 独立发明的一种高效算法，用于比较两个文本文件，找出将一个文件转换成另一个文件的最小序列变更。该代码是管理多个文件版本的源代码控制系统的核心。这些系统通常是通过存储一个版本和一组 diff，通过运行 diff 算法生成其他版本来工作的。它也用于更新程序的补丁机制---而不是将新版本的程序发送给某人，发送由 diff 计算出的一系列 ed 编辑命令，用于将旧版本转换为新版本。

The diff program is another nice example of how good theory can combine with good practical engineering to make a fundamental tool. The output that diff produces is readable by both people and programs; output written for either one or the other would be far less useful. It is also a simple example of a program that writes a program, and its output is a fine little language.

> diff 程序是另一个很好的例子，说明良好的理论如何与良好的实际工程结合，以制作一个基本工具。diff 产生的输出既可以被人类阅读，也可以被程序读取；如果只为其中一种写输出，那么效果就会大打折扣。这也是一个简单的程序，它可以编写另一个程序，而它的输出是一种很好的小型语言。

Quite early in Unix days, 1127 bought a novel device, a Votrax voice synthesizer that converted phonemes into sound. Doug created a set of rules for converting arbitrary English text into phonemes, and wrote a program called speak that used the rules to generate Votrax input. English spelling is of course notoriously irregular, so no set of rules can do a perfect job. The output of speak was often imperfect, sometimes funny (my name rhymed: "Br-I-an Kern-I-an"), but almost always accurate enough to be genuinely useful.

> 在 Unix 早期，1127 购买了一种新型设备，一台 Votrax 语音合成器，它可以将音素转换成声音。Doug 制定了一套规则，用于将任意英文文本转换成音素，并编写了一个叫做 speak 的程序，用这些规则来生成 Votrax 输入。当然，英语拼写是出了名的不规则，所以没有一套规则可以完美地完成工作。speak 的输出通常是不完美的，有时会很有趣(我的名字押韵：“Br-I-an Kern-I-an”)，但几乎总是足够准确，真正有用。

The program was just another command, so it could be used by anyone without prearrangement; text sent to speak was played through a loud-speaker in the Unix room. This led to any number of odd services. For instance, every day at 1PM, the Votrax would say

> 这个程序只是另一个命令，所以任何人都可以在不事先安排的情况下使用它；发送到说话的文本会通过 Unix 室里的扬声器播放。这就导致了各种奇怪的服务。例如，每天下午 1 点，Votrax 就会说

"Lunchtime, lunchtime, lunchtime. Yummy, yummy, yummy."

as a reminder to the inhabitants that it was time to head off to the cafeteria before it closed at 1:15.

> 作为提醒居民 1:15 前去自助餐厅的提醒。

[]{#index_split_001.html#p98}![](./index-98_1.jpg){.calibre4}

84 CHAPTER 4: SIXTH EDITION

There was also a service that monitored incoming telephone lines and when one rang (silently) would announce

> 也有一项服务监控来电线路，当有来电(无声)时会进行提示。

"Phone call for Doug"

or whoever; in a shared space it was much less distracting than frequently ringing phones.

Doug's interests were broad and deep. Among other things, he was an expert in map projections, which are a specialized form of mathematics. His map program provided several dozen projections, and to this day, he's still producing new ones that show up in Christmas cards sent to friends and on his Dartmouth web page (Figure 4.6).

> Doug 的兴趣广泛而深刻。除其他事情外，他是地图投影的专家，这是一种专业的数学形式。他的地图程序提供了几十种投影，直到今天，他仍在制作新的投影，这些投影出现在送给朋友的圣诞贺卡上，以及他在达特茅斯大学网页上(图 4.6)。

**Figure 4.6:**

One of Doug McIlroy's many maps

Doug was a superb technical critic, often the first person to try out some new program or idea. He would experiment at the earliest possible time and, since he had excellent taste, his opinions on what was good and what needed to be fixed was invaluable. There was a steady flow of people to his office to get advice and critical comments on ideas, algorithms, programs, documents---pretty much anything. Bjarne Stroustrup used to drop in on me to discuss C++ and explain some new idea, then move a few doors along the corridor to Doug's office to get serious feedback on the language design.

> 道格是一位出色的技术评论家，经常是第一个尝试一些新程序或想法的人。他会尽早尝试，因为他有很好的品味，他对什么是好的，什么需要修正的意见是非常宝贵的。有一大批人来他的办公室寻求建议和对想法、算法、程序、文件的严苛批评——几乎什么都可以。巴尔内·斯特劳斯特鲁普(Bjarne Stroustrup)经常来找我讨论 C++，解释一些新的想法，然后沿着走廊走几步到道格的办公室，获得关于语言设计的严苛反馈。

[]{#index_split_001.html#p99}![](./index-99_1.jpg){.calibre4}

CHAPTER 4: SIXTH EDITION

85

**Figure 4.7:**

Doug McIlroy and Dennis Ritchie, May 2011 (Wikipedia) Doug was usually the first person to read drafts of papers or manuals, where he would deftly puncture rhetorical balloons, cut flabby prose, weed out unnecessary adverbs, and generally clean up the mess. In Mike Mahoney's oral history of Unix (1989), Al Aho says of Doug,

> 道格·麦克伊尔罗伊和丹尼斯·里奇，2011 年 5 月(维基百科)道格通常是第一个读草稿论文或手册的人，在那里他会灵巧地消灭修辞气球，削减拖沓的散文，清除不必要的副词，并且总体上收拾混乱。在迈克·马奥尼的 Unix 口述历史(1989 年)中，阿尔·阿霍对道格说：

"He understood everything that I was working on, with just the most fragmentary descriptions. And he essentially taught me to write, too.

> 他只听了我工作的片段描述就明白了一切。而且他也基本上教会了我如何写作。

I think he's one of the finest technical writers that I know of. He has a flair for language, and a flair for economy of expression that is remarkable."

> 我认为他是我所知道的最优秀的技术作家之一。他有语言的灵感，而且令人惊叹的是他的表达简洁明了。

Doug was the outside reader on my thesis, where he greatly improved the organization and exposition. He also read multiple drafts of all the books that I co-authored with others at the Labs, always making them better. He refined and polished the manual pages for commands, and he pulled together

> Doug 是我论文的外部读者，他大大改善了组织和阐述。他还读了我在实验室与他人合作撰写的多篇书籍的多个草稿，总是使它们变得更好。他精炼和改进了命令的手册页面，并将它们汇集在一起。

[]{#index_split_001.html#p100}86 CHAPTER 4: SIXTH EDITION

and organized the contents of the manuals for the 8th through 10th editions of Unix. He did all of this with enthusiasm and care, at some cost to his own research.

> 他充满热情和关心地组织了第八版到第十版 Unix 手册的内容，这花费了他自己的研究时间。

Doug stepped down from his management role in 1986 and retired from the Labs in 1997, heading off to teach at Dartmouth. Figure 4.7 is a picture taken at Bell Labs in Murray Hill during a 2011 celebration of the Japan Prize awarded to Ken and Dennis.

> Doug 在 1986 年辞去了管理职位，并于 1997 年从实验室退休，前往达特茅斯教书。图 4.7 是在 Murray Hill 的贝尔实验室举行的 2011 年庆祝 Ken 和 Dennis 获得日本奖的照片。

[]{#index_split_001.html#p101}Chapter 5

**Seventh Edition (1976-1979)**

"It was really with v7 that the system fledged and left the research nest.

> 这是真正的 V7 系统，它离开了研究巢穴，开始翱翔。

V7 was the first portable edition, the last common ancestor of a radiative explosion to countless varieties of hardware. Thus the history of v7 is part of the common heritage of all Unix systems."

> V7 是第一个便携式版本，是辐射性爆发的最后共同祖先，演变出无数种硬件。因此，V7 的历史是所有 Unix 系统的共同遗产。

Doug McIlroy, _A Research Unix Reader_, 1986.

The 6th edition of Unix was a great base for software development, and the tools that came with it made programming fun and productive. Some pieces were in place well before the 6th edition, while others came along afterwards. In this chapter, we'll see several threads of software development in 1127 that culminated in the 7th edition, which was released in January, 1979, nearly four years after the 6th edition.

> 第六版的 Unix 是软件开发的良好基础，随附的工具使编程变得有趣和高效。有些部分在第六版发布前就已经放置好了，而其他的则是在之后出现的。在本章中，我们将看到 1127 年发展的几条软件开发线索，并最终在 1979 年 1 月发布了第七版，距离第六版发布已近四年。

Logically and chronologically, some of this material should come after the next chapter, which describes the spread of Unix outside of Center 1127, but the story seems more cohesive if I talk about the 7th edition first. And as Doug McIlroy noted in the epigraph above, the 7th edition was the source of much of the heritage shared by all Unix systems.

> 逻辑上和按时间顺序，有些材料应该放在下一章，描述 Unix 如何蔓延到中心 1127 之外的地方，但是这个故事似乎更加紧密，如果我先谈论第七版本。正如道格·麦克伊尔罗伊(Doug McIlroy)在上面的标语中指出的，第七版本是所有 Unix 系统共享的传统的重要来源。

One of the major themes of Unix and of this chapter is the flowering of influential languages, some aimed at conventional programming, some special-purpose or domain-specific, and some declarative specification languages. I'll probably spend more time on this topic than many readers may care about, but it's been my area of interest for many years. I'll try to describe the important bits early in each section so that you can safely skip to the end.

> Unix 和本章的一个主要主题是影响力语言的开花，有些针对常规编程，有些针对特定目的或特定领域，有些是声明式规范语言。我可能会花更多的时间在这个主题上，比起许多读者可能关心的东西，但它已经是我多年的兴趣所在了。我会尽量在每个部分的开头描述重要的内容，这样你就可以安全地跳到最后去了。

It's also worth noting that 6th edition Unix was strictly a PDP-11 operating system at the beginning of this period; by 1979, the 7th edition was a portable operating system that ran on at least four different kinds of processors,

> 需要特别指出的是，在这一时期开始时，第六版 Unix 严格上是一个 PDP-11 操作系统；到 1979 年，第七版已经成为一个可在至少四种不同处理器上运行的便携式操作系统。

[]{#index_split_001.html#p102}88 CHAPTER 5: SEVENTH EDITION

of which the DEC VAX-11/780 was the most popular. I'll hav e more to say about portability in the next chapter, but for now it's important to notice that Unix had quietly evolved from being a PDP-11 system to one that was comparatively independent of specific hardware.

> DEC VAX-11/780 是最受欢迎的，在下一章中，我会更多地谈论可移植性，但现在重要的是要注意，Unix 已经从一个 PDP-11 系统悄悄地演变成一个与特定硬件相对独立的系统。

**5.1 Bourne shell**

I/O redirection and pipes in the 6th edition shell made it easy to combine programs to do some task, originally by typing a sequence of commands and then collecting them in a file---a shell script---so they could be run as a single command.

> 在第六版的 shell 中，I/O 重定向和管道使得将程序组合在一起来完成某项任务变得更加容易，原本需要输入一系列的命令，然后将它们收集到一个文件中——一个 shell 脚本——这样就可以作为一个单独的命令运行。

The 6th edition shell had an _if_ statement for conditionally executing a command, a _goto_ statement for branching to another line of a script file, and a way to label a line in a script (the \":\" command, which did nothing) so it could be branched to. Taken together, these could be used to make loops so in principle the 6th edition shell could be used to write complicated scripts.

> 第六版的 shell 有一个 if 语句用于有条件地执行命令，一个 goto 语句用于跳转到脚本文件的另一行，以及一种给脚本中的行标记(“：”命令，不做任何事)，以便可以跳转。把这些放在一起，可以用来制作循环，因此原则上第六版的 shell 可以用来编写复杂的脚本。

In practice, however, the mechanisms were awkward and fragile.

As I'll describe in the next chapter, John Mashey, a member of the Programmer's Workbench (PWB) group, had added a number of features to his version of the 6th edition shell that made it much better for programming: a general _if-then-else_ statement for testing conditions, a _while_ statement for looping, and variables for storing information within a shell file.

> 在下一章中，我将描述程序员工作台(PWB)小组成员约翰·马希(John Mashey)为第六版壳层增加的一些功能，使其更适合编程：用于测试条件的通用 if-then-else 语句、用于循环的 while 语句以及用于在壳文件中存储信息的变量。

In 1976, Steve Bourne, who had recently joined 1127, wrote a new shell that incorporated the PWB shell features, along with major enhancements of his own. The goal was to retain the easy interactive nature of the existing shell, but also make it a fully programmable scripting language. Steve's shell provided several control-flow constructs, including _if-then-else_, _while_, _for_ and _case_. It also included variables, some of which were defined by the shell itself and others that could be defined by users. Quoting mechanisms were enhanced. Finally it was modified so it could be a filter in a pipeline just like any other program. The result, which was simply called sh, quickly replaced the 6th edition shell.

> 1976 年，刚加入 1127 的史蒂夫·伯恩(Steve Bourne)编写了一个新的 shell，它结合了 PWB shell 的特性，还增加了他自己的重大改进。其目标是保留现有 shell 的容易交互性，同时也使其成为一种完全可编程的脚本语言。史蒂夫的 shell 提供了几种控制流构造，包括 if-then-else，while，for 和 case。它还包括变量，其中一些是由 shell 本身定义的，另一些则可以由用户定义。引用机制得到了增强。最后，它被修改，使其可以像其他程序一样成为管道中的过滤器。结果，这个简称为 sh 的 shell 很快取代了第六版 shell。

The control-flow syntax of the new shell was unusual, since it was based on Algol 68, a language favored by Steve though not many others in 1127.

> 新壳的控制流语法很不寻常，因为它是基于 Steve 喜欢的 Algol 68 语言，而 1127 年的其他人却不太喜欢它。

For example, Algol 68 used reversed words as terminators, like fi to terminate if and esac to terminate case. But since od was already taken (for the octal dump command), do was terminated by done.

> 例如，Algol 68 使用反转的单词作为终止符，比如 fi 用于终止 if，esac 用于终止 case。但由于 od 已被占用(用于八进制转储命令)，因此 do 由 done 终止。

[]{#index_split_001.html#p103}CHAPTER 5: SEVENTH EDITION

89

for i in \$\*

_loop over all arguments_

do

if grep something \$i

then

echo found something in \$i

else

echo something not found in \$i

fi

done

The conditions tested by the if and while statements were the status returns from programs, that is, numeric values that a program could use to report results like whether it had worked properly. Most programs at the time were cavalier about returning sensible status, since it had rarely mattered before. So Steve set his shell to print an irritating message each time a program didn't produce a sensible status. After a week of this automated nag-ging, most programs had been upgraded to return meaningful status values.

> 如果和 while 语句测试的条件是程序返回的状态，也就是说，程序可以使用的数字值来报告结果，例如它是否正常工作。当时大多数程序都不太在乎返回明确的状态，因为以前很少有关系。因此，史蒂夫设置了他的 shell，每次程序不产生明确的状态时都会打印一条令人讨厌的消息。经过一周的自动责备，大多数程序都已经升级为返回有意义的状态值。

Steve's shell also significantly enriched I/O redirection. The BUGS section of the 6th edition shell had said "There is no way to redirect the diagnos-tic output." One especially useful new shell feature was a way to separate the standard error stream (by default file descriptor 2) from the standard output (file descriptor 1), so that the output of a script could be directed to a file while error messages went somewhere else, usually the terminal: prog \>file

> 史蒂夫的壳也大大丰富了 I/O 重定向。第六版壳的 BUGS 部分曾经说过“没有办法重定向诊断输出”。一个特别有用的新壳特性是一种将标准错误流(默认文件描述符 2)与标准输出(文件描述符 1)分开的方法，因此脚本的输出可以被重定向到文件，而错误消息可以发送到其他地方，通常是终端：prog \>file

\# stdout to file, stderr to terminal

prog 2\>err

\# stdout to terminal, stderr to err

prog 1\>file 2\>err \# stdout to file, stderr to err prog \>file 2\>&1

\# merge stderr with stdout

By this point, the shell had become a real programming language, suitable for writing pretty much anything that could reasonably be formulated as a sequence of commands. It could often do this well enough that there was no need to write a C program.

> 到这一步，外壳已经变成了一种真正的编程语言，适合编写几乎任何可以合理表述为一系列命令的东西。它通常可以做得很好，以至于没有必要编写 C 程序。

Over the years, more features have been added, particularly in Bash, the

"Bourne Again Shell" that is now the de facto standard shell for most Linux and macOS users. Although personal shell scripts tend to be small and simple, the source code for major tools like compilers is often distributed with configuration scripts of 20,000 or more lines. These scripts run programs that test properties of the environment, like the existence of libraries and sizes of data types, so they can compile a version that has been tuned to the specific system.

> "Bourne Again Shell" 现在是大多数 Linux 和 macOS 用户的默认 Shell。尽管个人 Shell 脚本往往很小很简单，但像编译器这样的主要工具的源代码通常会附带 2 万行或更多行的配置脚本。这些脚本运行程序来测试环境的属性，比如库的存在和数据类型的大小，因此它们可以编译一个针对特定系统调优的版本。

[]{#index_split_001.html#p104}90 CHAPTER 5: SEVENTH EDITION

**5.2 Yacc, Lex, Make**

We use language to communicate, and better languages help us to communicate more effectively. This is especially true of the artificial languages that we use to communicate with computers. A good language lowers the barrier between what we want to say ("just do it") and what we have to say to get some job done. A great deal of research in computing is concerned with how to create expressive languages.

> 我们使用语言进行交流，更好的语言可以帮助我们更有效地进行交流。这对于我们用来与计算机进行交流的人工语言尤其如此。一种好的语言可以降低我们想要表达的内容(“只要做就行了”)和我们必须表达的内容之间的障碍。计算机领域的大量研究都是关于如何创建表达能力强的语言的。

Seventh edition Unix offered a diversity of language-based tools, some rather unconventional. I think it's fair to say that the majority of those languages would not exist had it not been for tools, especially Yacc, that made it easy for non-experts to create new languages. This section describes the language-building tools. The overall message is that Unix tools facilitated the creation of new languages and thus led to better ways to communicate with computers. You can safely skip the details, but the message is important.

> 第七版 Unix 提供了多种基于语言的工具，有些相当不寻常。我认为可以公平地说，如果没有特别是 Yacc 这样的工具，使非专家很容易创建新语言，那么大多数语言都不会存在。本节介绍了语言构建工具。总的来说，Unix 工具促进了新语言的创造，从而更好地与计算机进行交流。您可以安全地跳过细节，但信息很重要。

Computer languages are characterized by two main aspects, syntax and semantics. Syntax describes the grammar: what the language looks like, what's grammatically legal and what's not. The syntax defines the rules for how statements and functions are written, what the arithmetic and logical operators are, how they are combined into expressions, what names are legal, what words are reserved, how literal strings and numbers are expressed, how programs are formatted, and so on.

> 计算机语言的特点有两个主要方面，语法和语义。语法描述了语言的样子：什么是合法的语法，什么不是。语法定义了如何编写语句和函数，算术和逻辑运算符是什么，它们如何组合成表达式，什么名字是合法的，什么单词是保留的，如何表达字面字符串和数字，程序如何格式化等等。

Semantics is the meaning that is ascribed to legal syntax: what does a legal construction mean or do. For the area computation program in Chapter 2, which is repeated here:

> 语义是赋予法律语法的意义：法律构造的意思是什么或者做什么。对于第 2 章中重复出现的面积计算程序，可以简化为：

void main() {

float length, width, area;

scanf(\"%f %f\", &length, &width); area = length \* width;

printf(\"area = %f\\n\", area);

}

the semantics say that when the function main is called, it will call the function scanf to read two data values from the standard input, compute the area, and call printf to print area =, the area and a newline character (\\n).

> 函数 main 被调用时，语义表明它将调用函数 scanf 从标准输入读取两个数据值，计算面积，并调用 printf 打印出“面积=”，面积和换行字符(\n)。

A compiler is a program that translates something written in one language into something semantically equivalent in another language. For example, compilers for high-level languages like C and Fortran might translate into assembly language for a particular kind of computer; some compilers translate from other languages, such as Ratfor into Fortran.

> 编译器是一种程序，它将用一种语言编写的内容翻译成另一种语言中的语义等价物。例如，C 和 Fortran 等高级语言的编译器可能会将其翻译成特定计算机的汇编语言；有些编译器可以将其他语言，如 Ratfor 翻译成 Fortran。

[]{#index_split_001.html#p105}![](./index-105_1.jpg){.calibre4}

CHAPTER 5: SEVENTH EDITION

91

The first part of the compilation process is to _parse_ the program, that is, to determine its syntactic structure by recognizing names, constants, function definitions, control flow, expressions, and the like, so that subsequent processing can attach suitable semantics.

> 编译过程的第一部分是对程序进行*解析*，也就是通过识别名称、常量、函数定义、控制流、表达式等来确定其句法结构，以便后续处理可以附加适当的语义。

Today, writing a parser for a programming language is well-understood technology, but in the early 1970s it was an active research area, focused on creating programs that would convert the grammar rules of a language into an efficient parser for programs written in that language. Such parser-generator programs were also known as "compiler-compilers," since they made it possible to generate the parser for a compiler mechanically. Typically they created a parser and also provided a way to execute code when particular grammar constructs were encountered during parsing.

> 今天，编写一个编程语言的解析器已经是一项很好理解的技术，但是在 20 世纪 70 年代早期，它是一个活跃的研究领域，致力于创建程序，将语言的语法规则转换为用该语言编写的程序的有效解析器。这样的解析器生成器程序也被称为“编译器编译器”，因为它们可以机械地生成编译器的解析器。通常它们创建一个解析器，并且在解析期间遇到特定语法结构时提供一种执行代码的方式。

**Yacc**

In 1973, Steve Johnson (Figure 5.1), with language-theory help from Al Aho, created a compiler-compiler that he called YACC (henceforth Yacc). A comment from Jeff Ullman inspired the name, which stands for "yet another compiler-compiler," suggesting that it was not the first such program.

> 1973 年，史蒂夫·约翰逊(图 5.1)在 Al Aho 的语言理论支持下创建了一个编译器编译器，他称之为 YACC(以下简称 Yacc)。杰夫·厄尔曼的一句话给它起了名字，它的意思是“又一个编译器编译器”，表明它不是第一个这样的程序。

**Figure 5.1:**

Steve Johnson, ∼1981 (Courtesy of Gerard Holzmann)

[]{#index_split_001.html#p106}92 CHAPTER 5: SEVENTH EDITION

A Yacc program consists of grammar rules for the syntax of a language, and semantic actions attached to the rules so that when a particular grammatical construction is detected during parsing, the corresponding semantic action can be performed. For example, in pseudo-Yacc, part of the syntax of arithmetic expressions might be:

> Yacc 程序包括语言的语法规则和附加到规则上的语义动作，以便在解析过程中检测到特定的语法结构时，可以执行相应的语义动作。例如，在伪 Yacc 中，算术表达式的语法可能是：

_expression_ := _expression_ + _expression_ _expression_ := _expression_ \* _expression_ and the corresponding semantic actions might be to generate code that would add or multiply the results of the two expressions together and make that the result. Yacc converts this specification into a C program that parses input and performs the semantic actions as the input is being parsed.

> _表达式_ := _表达式_ + _表达式_ _表达式_ := _表达式_ \* _表达式_，相应的语义动作可能是生成代码，将两个表达式的结果相加或相乘，并将其作为结果。Yacc 将此规范转换为 C 程序，该程序解析输入并在解析输入时执行语义动作。

Normally a compiler writer would have to write more complicated rules to handle the fact that multiplication has higher precedence than addition (that is, multiplications are done before additions), but in Yacc, operator precedence and associativity can be specified by separate declarations rather than additional grammar rules, which is a huge simplification for non-expert users.

> 一般来说，编译器的编写者必须编写更复杂的规则来处理乘法比加法具有更高的优先级(也就是说，先执行乘法)，但是在 Yacc 中，运算符优先级和结合性可以通过单独的声明而不是额外的语法规则来指定，这对非专家用户来说是一个巨大的简化。

Steve himself used Yacc to create a new "portable C compiler" (PCC) that had a common front end for parsing the language and separate back ends for generating code for different computer architectures. Steve and Dennis also used PCC in their implementation of Unix for the Interdata 8/32, as described in Section 6.5.

> 史蒂夫自己使用 Yacc 创建了一个新的“可移植 C 编译器”(PCC)，它具有用于解析语言的通用前端和用于为不同计算机体系结构生成代码的单独后端。史蒂夫和丹尼斯还在他们为 Interdata 8/32 实现的 Unix 中使用 PCC，如第 6.5 节所述。

PCC had other uses as well. As Steve recalls,

"An unexpected spin-off from PCC was a program called Lint. It would read your program and comment on things that were not portable, or just plain wrong, like calling a function with the wrong number of arguments, inconsistent sizes between definition and use, and so on.

> PCC 的一个意外产物是一个叫做 Lint 的程序。它会读取你的程序，并对不可移植的事情或者错误的事情发表评论，比如用错误的参数调用一个函数，定义和使用之间的尺寸不一致等等。

Since the C compiler only looked at one file at a time, Lint quickly became a useful tool when writing multi-file programs. It was also useful in enforcing standards when we made V7 portable, things like looking for system calls whose error return was −1 (Version 6) instead of null (V7). Many of the checks, even the portability checks, were ev entually moved into the C language itself; Lint was a useful test-bench for new features."

> 由于 C 编译器一次只能查看一个文件，当编写多文件程序时，Lint 很快就成为一个有用的工具。当我们使 V7 可移植时，它也很有用，比如查找系统调用的错误返回值是-1(版本 6)而不是 null(V7)。许多检查，甚至可移植性检查，最终被移动到 C 语言本身； Lint 是新功能的有用的测试台。

The name _Lint_ comes from the image of picking lint off clothing. Although its functionality is now often subsumed into C compilers, the idea is common in analogous tools for a number of other languages.

> 名字“Lint”来源于从衣服上拾取绒絮的图像。尽管现在它的功能通常被合并到 C 编译器中，但这个想法在其他一些语言的类似工具中也很常见。

[]{#index_split_001.html#p107}![](./index-107_1.jpg){.calibre4}

CHAPTER 5: SEVENTH EDITION

93

Yacc was instrumental in several of the languages that were developed in 1127 over the years, some of which are described in the next few sections.

> Yacc 在 1127 年開發的幾種語言中起到了重要作用，其中一些在接下來的幾個部分有所描述。

Lorinda Cherry and I used it for the mathematical typesetting language Eqn.

> 罗琳达·樱桃和我用它来为数学排版语言 Eqn。

I also used Yacc for the document preparation preprocessors Pic and Grap (the latter with Jon Bentley, Figure 5.2), for the AMPL modeling language, for at least one version of Ratfor, and for other one-off languages over the years. Yacc was also used for the first Fortran 77 compiler f77, Bjarne Stroustrup's C++ preprocessor cfront, the Awk scripting language (to be described shortly), and a variety of others.

> 我还使用 Yacc 为文档准备预处理器 Pic 和 Grap(后者与 Jon Bentley，图 5.2)，AMPL 建模语言，至少一个版本的 Ratfor，以及这些年来的其他一次性语言提供服务。Yacc 也用于第一个 Fortran 77 编译器 f77，Bjarne Stroustrup 的 C ++预处理器 cfront，Awk 脚本语言(稍后将进行描述)以及各种其他语言。

**Figure 5.2:**

Jon Bentley, ∼1981 (Courtesy of Gerard Holzmann) Yacc's combination of advanced parsing technology, high efficiency and convenient user interface helped it to become the sole survivor among the early parser generators. Today it lives on under its own name, in independent implementations like Bison that are derived from it, and in reimplementations in half a dozen other languages.

> Jon Bentley 在 1981 年(由 Gerard Holzmann 提供)发明了 Yacc，它具有先进的解析技术、高效率和方便的用户界面，这使它成为早期解析器生成器中唯一的幸存者。如今，它以自己的名字存在，在像 Bison 这样的独立实现中，它们都源自它，并在其他半打语言中重新实现。

**Lex**

In 1975, Michael Lesk (Figure 5.3) created a lexical analyzer generator called Lex, which is a direct parallel to Yacc. A Lex program consists of a sequence of patterns (regular expressions) that define the "lexical tokens"

> 1975 年，Michael Lesk(见图 5.3)创建了一个名为 Lex 的词法分析器生成器，它与 Yacc 直接平行。Lex 程序由一系列模式(正则表达式)组成，它们定义了“词法标记”。

that are to be identified; for a programming language, these would be components like reserved words, variable names, operators, punctuation, and so on.

> 那些需要被识别的；对于编程语言，这些将是像保留字、变量名、操作符、标点符号等组件。

As with Yacc, a semantic action written in C can be attached to each

[]{#index_split_001.html#p108}![](./index-108_1.jpg){.calibre4}

94 CHAPTER 5: SEVENTH EDITION

**Figure 5.3:**

Michael Lesk, ∼1981 (Courtesy of Gerard Holzmann) specified token. From these, Lex generates a C program that will read a stream of characters, identify the tokens it finds, and perform the associated semantic actions.

> 麦克尔·莱斯克，约 1981 年(提供者：杰拉德·霍尔茨曼)指定了一系列令牌。基于这些令牌，Lex 生成一个 C 程序，它可以读取一个字符流，识别它找到的令牌，并执行相关的语义动作。

Mike wrote the first version of Lex but it was quickly revised in the summer of 1976 by an intern who had just graduated from Princeton. Mike recalls:

> 麦克写了 Lex 的第一个版本，但 1976 年夏天很快就被一个刚从普林斯顿毕业的实习生修改了。麦克回忆起来：

"Lex was rewritten almost immediately by Eric Schmidt as a summer student. I had written it with a non-deterministic analyzer that couldn't handle rules with more than 16 states. Al Aho was frustrated and got me a summer student to fix it. He just happened to be unusual."

> 艾力克·施密特作为一名暑期學生，立刻就對雷克斯進行了重寫。我用一個不確定的分析器來寫它，然而它無法處理超過 16 個狀態的規則。阿霍感到沮喪，所以他給我找了一個暑期學生來修復它，而他恰好是個不尋常的人。

Eric went on to a PhD at Berkeley, and was the CEO of Google from 2001 to 2011.

> Eric 继续在伯克利攻读博士学位，并于 2001 年至 2011 年担任谷歌公司的首席执行官。

Yacc and Lex work well together. Each time Yacc needs the next token while parsing, it calls on Lex, which reads enough input to identify a complete token and passes that back to Yacc. The Yacc/Lex combination mechanizes the front-end components of a compiler while taking care of complicated grammatical and lexical constructs. For example, some programming languages have operators that are two or three characters long, like the ++

> Yacc 和 Lex 协同工作效果很好。每次 Yacc 在解析时需要下一个标记时，它就会调用 Lex，Lex 会读取足够的输入以识别出完整的标记，然后将其返回给 Yacc。Yacc/Lex 组合机械化了编译器的前端组件，同时处理复杂的语法和词汇结构。例如，某些编程语言的操作符可以是两个或三个字符长，比如++。

operator in C. When the lexical analyzer sees a +, it has to look ahead to know whether the operator is ++ or an ordinary + followed by something else. It's not too hard to write this kind of code by hand, but it's a lot easier

> 当词法分析器看到一个加号时，它必须提前查看这个运算符是 ++ 还是普通的加号，后边跟着其他东西。手动编写这种代码并不难，但是更容易一些。

[]{#index_split_001.html#p109}CHAPTER 5: SEVENTH EDITION

95

to have it written for you. In Lex, one would only have to say

\"++\" { return PLUSPLUS; }

\"+\" { return PLUS; }

to distinguish the two cases. (PLUS and PLUSPLUS are names for numeric codes that are easy for the C code to deal with.) Figure 5.4 shows how Yacc and Lex are used in the creation of a C program that is a compiler for some language. Yacc generates a C file for the parser and Lex generates a C file for the lexical analyzer. These two C files are combined with other C files that contain semantics, and compiled by a C

> 图 5.4 展示了如何在创建一个 C 程序的编译器(用于某种语言)时使用 Yacc 和 Lex。Yacc 生成一个 C 文件用于解析器，Lex 生成一个 C 文件用于词法分析器。这两个 C 文件与其他包含语义的 C 文件结合起来，然后由 C 编译器编译，以区分 PLUS 和 PLUSPLUS 这两种数字编码(这些编码对 C 代码很容易处理)。

compiler to make an executable program. This figure was created with Pic, which has exactly this structure.

> 编译器用于创建可执行程序。此图是使用 Pic 创建的，具有完全相同的结构。

grammar rules

lexical rules

other

Yacc

Lex

C code

generated

generated parser

lexer

C compiler

executable program

(a compiler)

**Figure 5.4:**

Using Yacc and Lex to create a compiler In spite of how easy and powerful Lex is, over the long haul, it has not been as extensively used as Yacc has. Perhaps this is because writing a parser for a complex language can be daunting for a comparatively inexperienced programmer, while writing a lexical analyzer is not. But writing a lexical analyzer by hand, however easy and straightforward it might seem, is not necessarily a good idea.

> 使用 Yacc 和 Lex 来创建一个编译器，尽管 Lex 非常容易和强大，但长期以来，它的使用并不像 Yacc 那样广泛。也许这是因为对于一个相对不熟练的程序员来说，编写一个复杂语言的解析器可能是一项艰巨的任务，而编写词法分析器则不然。但是，手工编写词法分析器虽然容易直观，但不一定是一个好主意。

My experience with the Awk scripting language (discussed later in this chapter) may be instructive. The first implementation of Awk used Yacc for the grammar and Lex to tokenize the input program. When we tried to port Awk to non-Unix environments, however, Lex was not available or it worked

> 我在本章后面讨论的关于 Awk 脚本语言的经验可能有所启发。第一个 Awk 的实现使用 Yacc 作为语法分析器，Lex 用于解析输入程序。但是，当我们尝试将 Awk 移植到非 Unix 环境时，Lex 不可用，或者它不起作用。

[]{#index_split_001.html#p110}96 CHAPTER 5: SEVENTH EDITION

differently. After a few years, I reluctantly rewrote the lexical part of Awk in C, so it would be portable to all environments. But for years afterwards, that hand-crafted lexical code was a fruitful source of bugs and subtle problems that were not present in the Lex-generated version.

> 几年后，我不情愿地用 C 重写了 Awk 的词法部分，以便在所有环境中可移植。但是多年以来，这个手工制作的词法代码一直是错误和微妙问题的源泉，而这些问题在 Lex 生成的版本中并不存在。

This is a good example of a general rule: if a program writes your code for you, the code will be more correct and reliable than if you write it yourself by hand. If the generator is improved, for example to produce better code, everyone benefits; by contrast, improvements to one hand-written program do not improve others. Tools like Yacc and Lex are excellent examples of this rule, and Unix provides many others as well. It's always worth trying to write programs that write programs. As Doug McIlroy says, "Anything you have to do repeatedly may be ripe for automation."

> 这是一个很好的一般规则的例子：如果一个程序为你编写代码，那么这个代码会比你自己手动编写的更加正确可靠。如果生成器得到改进，比如产生更好的代码，每个人都受益；相比之下，对一个手写程序的改进不会改善其他程序。像 Yacc 和 Lex 这样的工具是这条规则的绝佳例子，Unix 也提供了许多其他的例子。总是值得尝试编写程序来编写程序。正如 Doug McIlroy 所说，“任何你必须反复做的事情都可能适合自动化。”

**Make**

Most large programs consist of multiple source files, which have to be compiled and linked together to create an executable program. This can often be done with a single command such as cc \*.c to compile all the source files for a C program, but in the 1970s computers were so slow that recompiling a multi-file program after making a change in a single file could take significant time, minutes instead of seconds. It was more efficient to recompile only the changed file and link the result with the other previously compiled files.

> 大多数大型程序由多个源文件组成，这些文件必须编译并链接在一起才能创建可执行程序。这通常可以用单个命令，例如 cc \*.c 来编译 C 程序的所有源文件，但是在 1970 年代，计算机太慢了，在更改单个文件后重新编译多文件程序可能需要很长时间，分钟而不是秒。更有效的是只重新编译更改的文件，并将结果与其他先前编译的文件链接在一起。

Remembering which files had been compiled recently enough and which needed to be recompiled was a nuisance, however, and it was easy to make mistakes. Steve Johnson complained about this to Stu Feldman (Figure 5.5) one day, after spending hours of fruitless debugging, only to realize that he had simply failed to recompile one of the files he had changed.

> 记住哪些文件最近已经编译过，哪些需要重新编译是令人讨厌的，而且容易出错。史蒂夫·福尔曼(见图 5.5)有一天，史蒂夫·约翰逊抱怨了这一点，花了几个小时无用的调试，最后才意识到他只是忘记重新编译了其中一个他更改过的文件。

Coincidentally, Stu had done exactly the same thing and had also struggled to debug a program that was really correct, just not recompiled. He came up with a elegant idea, a specification language that describes how the pieces of a program depend on each other. A program that he called Make analyzed the specification and used the times that files had been changed to do the minimum amount of recompilation necessary to bring everything up to date. The first implementation was in 1976:

> 巧合的是，斯图也做了同样的事情，也苦苦调试一个实际上正确但没有重新编译的程序。他想出了一个优雅的想法，一种描述程序各部分如何相互依赖的规范语言。他称之为 Make 的程序分析了规范，并利用文件被更改的时间来做最少的重新编译，以使一切更新。这种第一次实施是在 1976 年。

"I wrote Make over the weekend, and then rewrote it the next weekend with macros (the list of built-in code was getting too long). I didn't fix the tab-in-column-1 because I quickly had a devoted user base of more than a dozen people and didn't want to upset them."

> 我上周末写了 Make，然后下周末用宏重写了它(内置代码列表太长了)。我没有修复第一列中的标签，因为我很快就有了十几个忠实用户，我不想让他们不高兴。

[]{#index_split_001.html#p111}![](./index-111_1.jpg){.calibre4}

CHAPTER 5: SEVENTH EDITION

97

**Figure 5.5:**

Stu Feldman, ∼1981 (Courtesy of Gerard Holzmann) Make was an instant success, since it obviated a whole class of silly errors while making compilation as efficient as possible. It was also a boon for programs that involved more complicated processing than just C compilation, for example programs that used Yacc and Lex, each of which had to be run first to create C files that were then compiled, as in Figure 5.4 above. One makefile could capture all the processing steps necessary to compile a new version of a program, and could also describe how to do related tasks like running Lint, making a backup and printing documentation. A makefile had some of the same properties as a shell script, but the language was declarative: a specification of dependencies and how to update components but without explicit tests of file creation times.

> Stu Feldman 在 1981 年左右发明的 Make 工具一经问世就大获成功，因为它可以避免编译过程中出现的一类愚蠢的错误，同时又使编译效率达到最高。它对于复杂处理程序(比如使用 Yacc 和 Lex 的程序)的编译也有巨大帮助，这类程序必须先运行 Yacc 和 Lex 来生成 C 文件，然后再编译，如上图 5.4 所示。一个 makefile 可以捕捉编译一个新版本程序所需的所有处理步骤，还可以描述如何执行其他任务，如运行 Lint、备份和打印文档。makefile 具有和 shell 脚本类似的一些特性，但它的语言是声明式的：指定依赖关系和如何更新组件，但没有明确的文件创建时间测试。

The "tab-in-column-1" problem that Stu refers to is an unconventional and somewhat awkward restriction on the format of makefiles. It's arguably a design flaw. It's also a nice example of a general problem that any successful program faces: if the program is good, it attracts users, and then it becomes hard to change the program in any incompatible way. Unix and most other systems are replete with examples of initial blemishes that are now too entrenched to fix.

> "Stu 提到的“tab-in-column-1”问题是对 Makefile 格式的一种不寻常且有点尴尬的限制。可以说，这是一个设计缺陷。它也是任何成功程序都会面临的一个很好的例子：如果程序很好，它会吸引用户，然后就很难以任何不兼容的方式改变程序。Unix 和大多数其他系统都充斥着最初的瑕疵，现在太顽固了，无法修复。

Make is also a good example of a theme in this section: rather than writing code or doing sequences of operations by hand, create a notation or

> 在本节中，Make 也是一个很好的主题例子：不是手动编写代码或执行操作序列，而是创建一种简化的符号

[]{#index_split_001.html#p112}98 CHAPTER 5: SEVENTH EDITION

specification that declares what has to be done, and write a program to interpret the specification. This approach replaces code with data, and that's almost always a win.

> 定义必须做什么的规范，并编写一个程序来解释规范。这种方法用数据取代了代码，几乎总是有好处的。

Yacc, Lex and Make are very much with us today, because they address important problems that programmers still face, and they solve those problems well enough that the designs and sometimes even the original implementations are still in use.

> Yacc、Lex 和 Make 今天仍然非常重要，因为它们解决了程序员们仍然面临的重要问题，而且它们解决这些问题的效果很好，以至于它们的设计甚至有时原始实现仍然在使用。

As a digression, I first met Stu in about 1967 when I was a grad student at Princeton and he was an undergrad; he was working part-time on Multics for Bell Labs during the school year. He joined 1127 after getting his PhD in astrophysics at MIT. He went to Bellcore in 1984, then to IBM, then to Google, where in a bit of good fortune for me, he was my manager several levels up when I visited there for summers.

> 作为一个偏离，我大约在 1967 年遇见了斯图，当时我是普林斯顿大学的研究生，他是本科生；学校期间他在贝尔实验室兼职 Multics。他在麻省理工获得天体物理学博士学位后加入 1127。他 1984 年去了贝尔核心，然后去了 IBM，然后去了谷歌，在那里，幸运的是，当我夏天去那里时，他是我几级以上的经理。

**5.3 Document preparation**

Unix had good tools for document production from very early on, and this helped to make its documentation good. This section tells an extended story about the history of document preparation tools on early Unix systems. Like so much of Unix, it's a story of how the interactions among programs, programmers and users formed a virtuous cycle of innovations and improvements.

> Unix 從很早就有很好的文檔製作工具，這有助於使其文檔質量更好。本章將詳細講述早期 Unix 系統文檔製作工具的歷史。就像 Unix 的許多方面一樣，它是一個關於程序、程序員和用戶之間的互動如何形成一個持續創新和改進的良性循環的故事。

When I was an intern at MIT in 1966, I encountered Jerry Saltzer's Runoff program. (The name comes from expressions like "I'll run off a copy for you.") Runoff was a simple text formatter: its input consisted of ordinary text interspersed with lines beginning with a period that specified formatting.

> 当我 1966 年在麻省理工学院实习时，我遇到了 Jerry Saltzer 的 Runoff 程序(这个名字来源于像“我会给你跑出一份副本”这样的表达)。Runoff 是一个简单的文本格式化程序：它的输入包括普通文本和以句点开头的行，指定格式。

For example, a document might say

.ll 60

.ce

Document preparation

.sp 2

.ti 5

Unix had good tools for document production \...

.sp

.ti 5

When I was an intern at MIT in 1966 \...

This "markup" told Runoff how to format the text: set the line length to 60 characters, center the next line, space down two lines, temporarily indent 5 spaces, print the paragraph in lines of at most 60 characters, then space down one line and temporarily indent again for the next paragraph.

> 这个"标记"告诉 Runoff 如何格式化文本：将行长度设置为 60 个字符，居中下一行，向下空两行，暂时缩进 5 个空格，以最多 60 个字符的行打印段落，然后向下空一行，暂时缩进下一段落。

[]{#index_split_001.html#p113}CHAPTER 5: SEVENTH EDITION

99

Runoff had a dozen or two commands like this that made it easy to format simple documents---manual pages, program descriptions, letters to friends---

> Runoff 有十几到二十多个这样的命令，可以轻松格式化简单的文档---手册页面、程序描述、给朋友的信件---

any text formatting that one might do today with a tool like Markdown.

**Early formatters**

Runoff was a revelation to me, a way to use computers that had nothing to do with mathematical computations or compiling. It became easy to refine one's writing over and over again at little cost. It may be hard for readers today to appreciate just how labor-intensive it was to prepare documents before the creation of word processing programs, when there were only mechanical typewriters---better than clay tablets or quill pens, to be sure, but any change of more than a few words in a document would require a complete retype. Thus most documents went through only one or two revisions, with handwritten changes on a manuscript that had to be laboriously retyped to make a clean copy.

> 运行给我的是一个启示，一种使用计算机而与数学计算或编译无关的方法。经过反复修改，耗费很少的成本，写作变得轻松起来。今天的读者可能很难体会在没有文字处理程序之前，准备文件有多么耗费力气，只有机械打字机---虽然比泥瓦片或鹅毛笔要好得多，但是任何文档的改动都需要重新打印一遍。因此，大多数文件只经历一到两次修改，手写的改动要费力地重新打印出一份干净的副本。

简体中文：运行对我来说是一个启示，一种使用计算机而与数学计算或编译无关的方法，可以轻松地反复修改文字，而成本很低。今天的读者可能很难想象，在没有文字处理软件之前，准备文件是多么耗费力气，只有机械打字机，虽然比泥瓦片或鹅毛笔要好，但任何文档的改动都需要重新打印。因此，大多数文件只经历一到两次修改，手写的改动要费力地重新打印出一份干净的副本。

When I started to write my thesis in the fall of 1968, I really wanted Runoff, since the alternative would have been to type the thesis myself on a manual typewriter (and retype it for each set of changes), or pay someone to do it for me. I'm a fast but inaccurate typist, so the former was not practical, and since I was both cheap and poor, the latter wasn't either.

> 当我在 1968 年秋天开始写论文时，我真的很想用 Runoff，因为另一种选择就是自己用手动打字机打论文(每次修改都要重新打)，或者让别人帮我打。我打字速度快，但不准确，所以前者不可行，而且由于我既又穷又小气，后者也不行。

Thus I wrote a simple version of Runoff that I called "Roff," for "an abbreviated form of Runoff." The problem was that there was no interactive computer system like CTSS at Princeton; there weren't any computer terminals either. All that was available was punch cards, which only supported upper case letters. I wrote Roff in Fortran (far from ideal, since Fortran was meant for scientific computation, not pushing characters around, but there were no other options) and I added a feature to convert everything to lower case while automatically capitalizing the first letter of each sentence. The resulting text, now upper and lower case, was printed on an IBM 1403 printer that could print both cases. Talk about bleeding edge! My thesis was three boxes of cards. Each box held 2,000 cards, was about 14 inches (35 cm) long and weighed 10 pounds (4.5 kg). The first 1,000 cards were the program and the other 5,000 were the thesis itself in Roff.

> 因此，我写了一个简化版的 Runoff，我称之为“Roff”，意思是“Runoff 的缩写形式”。问题是普林斯顿没有像 CTSS 这样的交互式计算机系统；也没有计算机终端。可用的只有打孔卡，只支持大写字母。我用 Fortran 编写了 Roff(远非理想，因为 Fortran 是为科学计算而设计的，而不是推动字符，但没有其他选择)，我还添加了一个功能，可以将所有内容转换为小写，同时自动将每个句子的首字母大写。结果文本现在是大小写混合的，可以在可以打印大小写的 IBM 1403 打印机上打印出来。让我们一起来探索最前沿的技术！我的论文是三盒卡片。每盒有 2000 张卡片，长约 14 英寸(35 厘米)，重 10 磅(4.5 千克)。前 1000 张卡片是程序，另外 5000 张是用 Roff 编写的论文本身。

Readers who have nev er worked with cards may find this confusing. Each card contained at most 80 characters, either one line of Fortran code or one line of thesis text. If some part of the text needed to be changed, the replace-ment text was punched onto a few new cards that replaced the old cards, which were discarded. Fixing a spelling mistake would generally require replacing only one card, though if the new text were much longer, more cards might be needed.

> 读者们如果从未使用过卡片，可能会感到困惑。每张卡片最多包含 80 个字符，可以是一行 Fortran 代码或一行论文文本。如果需要更改某一部分文本，则需要在几张新卡片上打出替换文本，以取代旧卡片，旧卡片将被丢弃。修正拼写错误通常只需要替换一张卡片，但如果新文本更长，则可能需要更多卡片。

[]{#index_split_001.html#p114}![](./index-114_1.jpg){.calibre4}

100 CHAPTER 5: SEVENTH EDITION

**Figure 5.6:**

A page of my thesis, formatted with Roff I had to manually insert a few special characters like summation signs (Σ) into the printed pages but this kludgy mechanism worked surprisingly well, certainly enough for me to print my thesis, which I believe was the first computer-printed thesis at Princeton. (Figure 5.6 shows a random page.) For some years afterwards, there was a student agency that would "roff" documents for students for a modest fee. Roff was thus the first program I ever

> 我的论文有一页是用 Roff 格式化的，我不得不手动插入一些特殊字符，比如求和符号(Σ)，但这种笨拙的机制却出乎意料地有效，足以让我打印出论文，我相信这是普林斯顿大学第一份电脑打印的论文(图 5.6 显示了一页随机页面)。在此之后的几年里，有一家学生服务机构以适度的费用为学生们“roff”文档。因此，Roff 是我接触的第一个程序。

[]{#index_split_001.html#p115}CHAPTER 5: SEVENTH EDITION

101

wrote that was used by other people in any significant way.

When I got to Bell Labs, I found that there were a couple of other roff-like programs also underway, including one by Doug McIlroy that was based on Saltzer's original. And Joe Ossanna shortly thereafter wrote a much more powerful version that he called Nroff, for "new Roff," which made it possible for the patent department to format patent applications. As I described earlier, Nroff was the critical tool that enabled the purchase of the first PDP-11

> 当我来到贝尔实验室时，我发现还有其他几个类似 roff 的程序正在进行，其中一个是由道格·麦克罗伊(Doug McIlroy)基于 Saltzer 的原始程序开发的。然后不久，乔·奥萨纳(Joe Ossanna)编写了一个更强大的版本，他称之为 Nroff，意为“新 Roff”，这使得专利部门能够格式化专利申请。正如我之前所描述的，Nroff 是购买第一台 PDP-11 的关键工具。

computers for Unix.

This little pocket of document preparation enthusiasts, and a community of active users of such programs, fit my interests perfectly, and I spent a significant part of the next ten years happily working on tools for text formatting.

> 这个小群文档准备爱好者以及这些软件的活跃用户社区完全符合我的兴趣，在接下来的十年里，我很高兴地专注于文本格式化工具的开发。

**Tr off and typesetters**

Roff and Nroff only handled fixed-width ("monospace") character sets, not much more than the standard alphabetic characters found on the Model 37 Teletype, so the output quality wasn't very high. In 1973, however, Joe Ossanna arranged to buy a phototypesetter, a Graphic Systems CAT, which was popular in the newspaper industry. Joe's intent was to produce better-looking internal technical documents and also to help the patent department to prepare better patent applications.

> 罗夫和 Nroff 只处理固定宽度(“等宽”)字符集，而不是模型 37 电传打字机上找到的标准字母字符，因此输出质量不是很高。然而，1973 年，乔·奥萨纳安(Joe Ossanna)安排购买了一台广泛应用于报业的 Graphic Systems CAT 活字印刷机。乔的意图是制作更好看的内部技术文件，也帮助专利部门准备更好的专利申请。

The CAT could print conventional proportionally spaced fonts in roman, italic and bold, along with a set of Greek letters and special characters for mathematics. It printed on long rolls of photographic paper that had to be developed in a couple of baths of noxious and messy chemicals. This technology predates laser printers, which did not become widely available for at least another 10 years. Furthermore, the output was black and white; inex-pensive color printing did not arrive until several decades later.

> CAT 可以打印出传统的比例分布的罗马字体、斜体和粗体，以及一组希腊字母和数学特殊字符。它打印在长长的照相纸卷上，需要在有毒和凌乱的化学液中进行发展。这项技术早于激光打印机，而激光打印机至少要再过 10 年才能广泛普及。此外，输出是黑白的；直到几十年后，便宜的彩色打印才到来。

Each font was a piece of 35mm film with character images, mounted on a rapidly spinning wheel. The wheel held four fonts of 102 characters each, so the total repertoire for a single job was 408 characters. The typesetter flashed an intense light through the film strip image onto photographic paper when the paper and the desired character were in the right positions. It was capable of 16 distinct sizes.

> 每个字体都是一张 35 毫米胶片，上面有字符图像，它们被安装在快速旋转的轮子上。轮子上有四个 102 个字符的字体，所以单个工作的总表演范围是 408 个字符。当纸张和所需字符处于正确位置时，排字机会通过胶片图像向照相纸投射强烈的光。它能够实现 16 种不同的尺寸。

The typesetter was slow---changing sizes required it to rotate a mechanical lens turret---and the photographic chemicals were most unpleasant, but the output quality was high enough that we could produce professional-looking documents. Indeed, there were occasions when a paper submitted to a journal by a Bell Labs author was questioned: it looked so polished that it

> 排字工作缓慢——需要旋转机械镜头来改变尺寸——而且摄影化学品也很不舒服，但输出质量足够高，可以制作出看起来很专业的文件。实际上，有时候贝尔实验室的作者提交给期刊的论文会受到质疑：看起来太过精美了。

[]{#index_split_001.html#p116}102 CHAPTER 5: SEVENTH EDITION

must have already been published.

To drive the typesetter, Joe created a significant extension of Nroff that he called Troff. "T" is for typesetter; it's pronounced tee-roff. The Troff language was arcane and tricky, but with sufficient skill and patience, it could be made to do any formatting task, though few people ever mastered it. In effect, Troff was an assembly language for a truly weird computer, so most people used it through packages of macros that encapsulated common formatting operations like titles, headings, paragraphs, numbered lists, and so on. The macros provided a higher-level language above the low-level Troff commands. Mike Lesk, who created the widely used ms package, was the master of creating macro packages; no one else in my orbit came close to his skill in using the programming capabilities of Troff.

> 为了操控排字机，乔创建了一个重要的 Nroff 扩展，他称之为 Troff。“T”代表排字机，发音为“ti-roff”。Troff 语言很晦涩难懂，但只要有足够的技能和耐心，就可以完成任何格式化任务，尽管很少有人掌握它。实际上，Troff 是一种真正奇怪的计算机的汇编语言，所以大多数人都通过封装常见格式化操作的宏(如标题、标题、段落、编号列表等)来使用它。宏提供了低级 Troff 命令之上的高级语言。Mike Lesk 创建了广泛使用的 ms 包，他是创建宏包的大师；在我的范围内，没有人能像他在使用 Troff 的编程能力方面接近他的技能。

Once we had a typesetter that could produce output in a variety of fonts with proportional spacing and enough special characters, it became possible to think about typesetting books as well as internal technical documents. The first book produced in that way was _The Elements of Programming Style_, which Bill Plauger and I wrote in 1974. It was typographically rough in many places because we did not have a monospace font for displaying programs, but it was otherwise satisfactory.

> 一旦我们有了一台可以以各种字体、比例间距以及足够特殊字符输出的排版机，就有可能考虑排版书籍以及内部技术文件了。第一本用这种方式排版的书是 1974 年由比尔·普劳格和我共同撰写的《编程风格要素》。由于我们没有用等宽字体来显示程序，所以在许多地方排版上都比较粗糙，但其他方面都还可以接受。

One of the main motivations that Bill and I had for doing our own typesetting was to avoid the errors that the conventional publishing process frequently introduced into printed computer programs. Because we had total control over our content, from input to final pages ready to be printed, we could test the programs directly from the text, which would never be touched by copy-editor or compositor hands. The result was an essentially error-free programming book, which was most unusual at the time. I've used that same process ever since; the books listed at the front of this one have all been produced with Troff or its modern incarnation, Groff. Fortunately, one no longer needs typesetters and their expensive and unpleasant media. Today it's sufficient to get everything right in a PDF file and send that to a publisher or printer.

> 我和比尔的主要动机之一是为了避免传统出版过程经常引入到印刷的计算机程序中的错误。由于我们完全控制我们的内容，从输入到最终准备好打印的页面，我们可以直接从文本中测试程序，而不会被校对或排版工人触及。结果是一本基本上没有错误的编程书，这在当时是非常不寻常的。我从那时起一直使用同样的过程；本书前面列出的书籍都是用 Troff 或其现代版本 Groff 制作的。幸运的是，人们不再需要排版工和他们昂贵而讨厌的媒体。今天，只需要在 PDF 文件中正确获得所有内容，然后将其发送给出版商或印刷商就可以了。

**Eqn and other preprocessors**

Bell Labs authors wanted to create documents that contained more than just text, most obviously mathematics, but also tables, figures, bibliographic citations, and so on. Troff itself was capable in principle of handling such things, but not in any remotely convenient way. Thus we began to create special-purpose languages that made it easier to handle specific types of technical material. In effect, we were repeating for document preparation the kind of evolution that had already happened for conventional programming

> 贝尔实验室的作者想要创建的文档不仅仅是文本，最明显的是数学，还有表格、图表、参考文献等等。 Troff 本身原则上可以处理这些东西，但不是任何方便的方式。因此，我们开始创建特殊目的语言，使其更容易处理特定类型的技术材料。实际上，我们正在为文档准备重复传统编程已经发生的进化。

[]{#index_split_001.html#p117}![](./index-117_1.jpg){.calibre4}

CHAPTER 5: SEVENTH EDITION

103

languages.

The first of these special-purpose languages was Eqn, a language and program for typesetting mathematical expressions that Lorinda Cherry (Figure 5.7) and I wrote in 1974. As might be expected of a scientific research lab, Bell Labs produced a great number of technical documents, mostly for internal consumption, and many of those were full of mathematics. The Labs had a cadre of talented typists who could read hand-written mathematics and type it into recognizable form using manual typewriters, but this process was time-consuming and edits were painful.

> 1974 年，我和洛琳达·雪莉(见图 5.7)编写了一种特殊用途语言 Eqn，它是一种用于排版数学表达式的语言和程序。正如人们所料，贝尔实验室生产了大量的技术文档，大多是供内部使用，其中许多充满了数学内容。实验室有一群有才华的打字员，他们可以读懂手写的数学，并使用手动打字机将其转换成可识别的形式，但这个过程很耗时，编辑也很艰难。

**Figure 5.7:**

Lorinda Cherry, ∼1981 (Courtesy of Gerard Holzmann) Lorinda had been exploring the idea of a tool for printing mathematics, and I wanted a language that would match the way that mathematics is spo-ken aloud by mathematicians. I think that this language idea was in my sub-conscious, because while I was a graduate student, I had volunteered for several years to read technical books aloud so they could be recorded onto audio tapes at Recording for the Blind, and so I had spent many hours speaking mathematics.

> 劳林达·樱桃，约 1981 年(由杰拉德·霍尔茨曼提供)劳林达一直在探索一种打印数学的工具的想法，我想要一种能够与数学家口头表达方式相匹配的语言。我认为这种语言想法深藏在我的潜意识中，因为当我是一名研究生的时候，我曾自愿几年来朗读技术书籍，以便它们可以被录制到盲人录音带上，所以我花了很多时间说数学。

Eqn did a decent job on simple mathematical expressions. For example, the summation

> Eqn 在简单的数学表达式上做得不错。例如，求和

∞ 1

Σ

= 2

_i_=0 2 _i_

[]{#index_split_001.html#p118}104 CHAPTER 5: SEVENTH EDITION

is written as

sum from i=0 to inf 1 over 2 sup i = 2

Eqn proved to be easy to teach to the mathematical typists and then to others, and experiments verified that it was much faster than manual typewriters. The language was simple enough that PhD physicists could also learn it, and after a while, people started doing their own typing rather than relying on expert typists. Eqn was one of the inspirations for math mode in Don Knuth's TeX (1978), which is now the standard for mathematical typog-raphy.

> Eqn 被证明很容易教给数学打字员，然后再教给其他人，实验证明它比手动打字机快得多。语言足够简单，以至于博士物理学家也可以学习它，过了一段时间，人们开始自己打字而不依赖专家打字员。Eqn 是 Don Knuth 的 TeX(1978)数学模式的灵感之一，现在它已成为数学排版的标准。

Eqn was implemented as a preprocessor for Troff; the normal usage was to pipe the output of Eqn into Troff like this: eqn file \| troff \>typeset.output

> Eqn 被用作 Troff 的预处理器；正常使用方式是将 Eqn 的输出管道传给 Troff，如下所示：eqn file \| troff \>typeset.output。

Eqn recognized mathematical constructs and translated those into Troff commands, while passing everything else through untouched. The preprocessor approach provided a clean separation into two languages and two programs with different concerns. Lorinda and I had been forced into a good idea by the physical limitations of the PDP-11. There simply wasn't enough memory to include mathematical processing in Troff, which was already about as big as a program could be, and in any case, Joe Ossanna would not have encouraged us to modify Troff even if we had wanted to.

> Eqn 识别数学结构，并将其转换为 Troff 命令，而将其余内容原封不动地传递。预处理器方法提供了两种语言和两个具有不同关注点的程序之间的清晰分离。由于 PDP-11 的物理限制，Lorinda 和我被迫接受了一个好主意。简单地说，内存不足以在 Troff 中包含数学处理，而且无论如何，Joe Ossanna 也不会鼓励我们修改 Troff，即使我们想要这样做。

The Eqn language is based on a box model: an expression is built up as a sequence of boxes positioned and sized relative to each other. For example, a fraction is a numerator box centered over a denominator box, with a long-enough line between them. A subscripted expression like _xi_ is a pair of boxes where the contents of the second box are in a smaller size and positioned somewhat down from the first box.

> 语言 Eqn 基于一个盒子模型：表达式是由相对于彼此的位置和大小的一系列盒子构建而成的。例如，分数是一个居中于分母盒子上方的分子盒子，中间有一条足够长的线。像*xi*这样的下标表达式是一对盒子，其中第二个盒子的内容以更小的大小显示，并且相对于第一个盒子稍微偏下。

We used Steve Johnson's newly invented Yacc compiler-compiler to define the grammar and hang semantics on it. Eqn was the first Yacc-based language that wasn't a traditional compiler for a traditional language. Speaking for myself, Eqn would not have happened without Yacc, since I was not up to writing a parser by hand for a new language. The grammar was too complicated to write an _ad hoc_ parser for, and it changed frequently while Lorinda and I were experimenting with syntax. Our experience with Yacc is a compelling example of how having good tools makes it possible to do things that would otherwise be too hard or not even conceivable.

> 我们使用史蒂夫·约翰逊最新发明的 Yacc 编译器编译器来定义语法和悬挂语义。Eqn 是第一个基于 Yacc 的语言，它不是传统语言的传统编译器。就我个人而言，如果没有 Yacc，Eqn 是不可能发生的，因为我无法手动为新语言编写解析器。语法太复杂，无法为其编写*ad hoc*解析器，而在 Lorinda 和我尝试语法时，它经常发生变化。我们使用 Yacc 的经验是一个有力的例子，证明拥有良好的工具可以实现本来太难或甚至不可想象的事情。

Preprocessors for different kinds of typographically difficult material turned out to be a good idea. Soon after Eqn, Mike Lesk created Tbl, which provided a very different language for specifying complex tables, and Refer

> 处理不同类型排版困难材料的预处理器被证明是一个好主意。在 Eqn 之后不久，Mike Lesk 创建了 Tbl，它提供了一种非常不同的语言来指定复杂的表格，以及 Refer。

[]{#index_split_001.html#p119}CHAPTER 5: SEVENTH EDITION

105

for managing bibliographic citations, which were important for technical papers.

> 用于管理技术论文中重要的参考文献。

Many of the programs described in this chapter are preprocessors, that is, programs that convert some language into a suitable form for a subsequent process. Cfront, the original version of C++, would be more accurately described as an object-oriented preprocessor for C that evolved into C++.

> 许多在本章中描述的程序是预处理器，也就是将某种语言转换成适合后续处理的形式的程序。Cfront，C++的最初版本，更准确地说是一个针对 C 的面向对象预处理器，它演变成了 C++。

Sometimes, as with C++, the preprocessor eventually went away as functionality was absorbed into the downstream process. Most other times, however, the programs stayed separate, as with the document preparation tools like Eqn and Tbl. Another example is bc, a preprocessor for dc, Bob Morris's original unlimited-precision calculator. Lorinda Cherry wrote bc to provide conventional infix arithmetic notation for dc, whose postfix notation was hard for novices to use casually.

> 有时，就像 C++一样，预处理器最终会随着功能被吸收到下游流程中而消失。然而，大多数情况下，程序仍保持分离，就像文档准备工具 Eqn 和 Tbl 一样。另一个例子是 bc，这是 Bob Morris 的原始无限精度计算器 dc 的预处理器。Lorinda Cherry 编写了 bc，为 dc 提供了传统的中缀算术符号，而新手很难随意使用 dc 的后缀符号。

Preprocessors have many advantages. First, if one implements a language, it is not limited by existing syntax but can use a completely different style, as with the various Troff preprocessors. Second, when memories were small, it was simply not possible to include more functionality in already-large programs; this was especially the case with Troff. Finally, because the output of a preprocessor is available, it can be manipulated before being passed on, to handle other kinds of processing. In the document preparation suite, I've often used Sed scripts and the like to fix character sets and spacing.

> 预处理器有很多优势。首先，如果实现一种语言，它不受现有语法的限制，而可以使用完全不同的风格，就像各种 Troff 预处理器一样。其次，当内存很小时，根本不可能在已经很大的程序中包含更多的功能；这在 Troff 中尤其如此。最后，由于预处理器的输出可用，可以在传递之前对其进行操作，以处理其他类型的处理。在文档准备套件中，我经常使用 Sed 脚本等来修复字符集和间距。

Chris Van Wyk and I wrote programs to do vertical justification of pages, by modifying the output of Troff before it went to a device driver. These would not have been possible if the functionality were embedded in a single program, but when the process is a pipeline, it's easy to add new stages at the front or back or middle.

> 我和 Chris Van Wyk 编写了程序来实现页面的垂直对齐，通过修改 Troff 输出在发送到设备驱动程序之前。如果这些功能被嵌入到一个单独的程序中，就不可能实现这些功能，但是当这个过程是一个管道时，很容易在前面、后面或中间添加新的阶段。

**Device-independent Troff**

Joe Ossanna died in 1977 at the age of 48. Part of his legacy was the source code for Troff, which at the time was nearly 10,000 lines of inscrutable C that Joe had hand-transliterated from its original assembly language form---no comments, dozens of global variables with 2-letter names, and (see the discussion of memory above) a variety of subtle tricks for cram-ming as much information as possible into not enough memory. In Joe's defense, this was absolutely necessary to pack all of Troff's functionality into 65K bytes, the maximum memory that was available to user programs on the PDP-11/45 that we were using at the time.

> 乔·奥桑纳于 1977 年去世，享年 48 岁。他的遗产之一就是 Troff 的源代码，当时几乎有 1 万行乔手工从其原始的汇编语言形式翻译而来的难以理解的 C 语言——没有注释，许多以两个字母命名的全局变量，以及(参见上文关于内存的讨论)各种巧妙的技巧来把尽可能多的信息塞进不够的内存中。为了给 Troff 放进 65K 字节的最大内存(当时我们在 PDP-11/45 上使用)，这种做法是绝对必要的，以此为乔辩护。

I did nothing with the code for at least a year, but finally got up enough courage to start fiddling with it. Slowly and cautiously, I beg an an upgrade.

> 我至少有一年没有对代码做任何事情了，但最终还是鼓起勇气开始摆弄它。我小心翼翼地开始升级。

The biggest single problem, aside from the fact that there were no comments

> 最大的問題，除了沒有評論的事實之外。

[]{#index_split_001.html#p120}106 CHAPTER 5: SEVENTH EDITION

or documentation beyond the user manual, was that it was strongly dependent on the original Graphic Systems CAT typesetter, which by this time was obsolete.

Eventually I managed to find all the places where the code relied on pecu-liarities of the CAT and replaced them with generic code driven by tables of typesetter characteristics like character sets, sizes, fonts, and resolutions. I invented a typesetter description language so that Troff could produce output that was tuned to the capabilities of a specific typesetter. Straightforward drivers converted that output into whatever input was needed for specific devices. This resulted in the so-called device-independent version called Ditroff. It also enabled other document preparation preprocessors, especially Pic, which was able to take advantage of the higher resolution of new typesetting devices to draw lines and figures.

> 最终，我设法找到了所有代码依赖 CAT 特性的地方，并用基于字符集、大小、字体和分辨率等排版机特性表的通用代码替换了它们。我发明了一种排版机描述语言，这样 Troff 就可以生成针对特定排版机能力的输出。简单的驱动程序将这些输出转换为特定设备所需的输入。这就产生了所谓的设备无关版本，称为 Ditroff。它还使其他文档准备预处理器，特别是 Pic，能够利用新的排版机的更高分辨率来绘制线条和图形。

One of those devices was a new typesetter from Mergenthaler called the Linotron 202. On paper, this device seemed like just what we needed to replace the CAT. It was fast, it had high resolution, it drew characters by painting them on a screen, its processor was a standard minicomputer (a Computer Automation Naked Mini), and it was controlled by a simple program similar to the ones that I had written for other typesetters. The main drawback was the cost, \$50,000 in 1979, but we had done enough good work with the previous typesetter that management approved the purchase with hardly any discussion.

> 一种是来自 Mergenthaler 的新型排字机 Linotron 202。从纸张上看，这台设备似乎正是我们需要用来取代 CAT 的设备。它速度快，分辨率高，通过在屏幕上绘制字符，其处理器是标准小型计算机(Computer Automation Naked Mini)，由一个类似我为其他排字机编写的简单程序控制。主要缺点是 1979 年的价格 5 万美元，但我们用前一台排字机做了足够好的工作，管理层几乎没有任何讨论就批准了购买。

Once the 202 arrived, we discovered that its hardware was impossibly flaky; the only thing worse was its software. This started several months of almost daily visits from Mergenthaler's repair service, and a remarkable feat of reverse engineering of the hardware by Ken Thompson and Joe Condon (Figure 5.8).

> 一旦 202 到达，我们发现它的硬件出现了不可思议的故障；更糟糕的是它的软件。这开始了几个月几乎每天来自 Mergenthaler 维修服务的访问，以及 Ken Thompson 和 Joe Condon 的硬件反向工程的了不起的壮举(图 5.8)。

Joe was a physicist by training, but as his interests shifted, he became an exceptional designer of electronic circuits. He wrote many of the circuit design tools that the Center used for its hardware experiments, and with Ken was the designer of the Belle chess machine. His hardware expertise was crucial to figuring out the 202.

> 乔本来是一名物理学家，但随着他的兴趣转变，他成为一位杰出的电子电路设计师。他写了许多中心用于硬件实验的电路设计工具，并与肯一起设计了贝尔象棋机器。他的硬件专业知识对于弄清 202 号机器至关重要。

Ken beg an by writing a disassembler for the binary programs that ran on the machine. (For the record, he did this in a couple of hours one evening, while I went home for dinner and then came back for an evening of work.) Disassembling Mergenthaler's programs gav e Ken and Joe a toehold into how the typesetter itself worked, and after several weeks of intense reverse engineering they figured out Mergenthaler's proprietary encoding of characters and wrote code so we could create our own characters, like the then-current Bell System symbol at the top of Figure 5.9, a chess font for printing

> 肯开始通过编写一个反汇编器来处理在机器上运行的二进制程序。(顺便说一句，他在一个晚上几个小时内就完成了这项工作，而我则回家吃晚饭，然后回来继续工作。)反汇编梅尔根塔勒的程序给肯和乔提供了一个了解排字机本身如何工作的踏脚石，在几周的强烈反向工程之后，他们弄清楚了梅尔根塔勒的专有字符编码，并编写了代码，以便我们可以创建自己的字符，如图 5.9 顶部的当前 Bell 系统符号，一种用于打印的国际象棋字体。

[]{#index_split_001.html#p121}![](./index-121_1.jpg){.calibre4}

CHAPTER 5: SEVENTH EDITION

107

**Figure 5.8:**

Joe Condon, ∼1981 (Courtesy of Gerard Holzmann) games and board diagrams, and a Peter face that had a variety of uses (for example, Figure 5.10).

> 乔·孔登，约 1981 年(提供赫尔茨曼)游戏和棋盘图，以及一个彼得的脸有各种用途(例如，图 5.10)。

Ken wrote a B interpreter for the Mergenthaler controller, and we wrote B

programs to drive it. This story is told in detail in a technical memo that Bell Labs management suppressed at the time, probably to avoid revealing any of Mergenthaler's intellectual property, but which was finally published in 2013

> 程序驱动它。贝尔实验室管理层当时封存了这个故事的详细内容，可能是为了避免披露任何梅尔根塔勒的知识产权，但最终在 2013 年发表了。

(see _[www.cs.princeton.edu/](http://www.cs.princeton.edu/)˜bwk/202_). Figure 5.9 shows part of the first page; the incomplete internal memorandum numbers like 80-1271-x indicate that an official number was never assigned.

> 请参见[www.cs.princeton.edu/](http://www.cs.princeton.edu/)˜bwk/202\_)。图 5.9 显示了第一页的部分内容；不完整的内部备忘录号码，如 80-1271-x，表明没有指定官方号码。

When it eventually began to work, the high resolution of the 202 made it possible to achieve interesting graphical effects, including half-tone images and line drawings like the diagram of a digital typesetter in Figure 5.9. For the latter, I created a language called Pic in which figures like org anization charts or network packet diagrams could be described textually. Naturally it used Yacc for the grammar and Lex for the lexical part. Figure 5.11 shows a simple example of Pic input and output.

> 当它最终开始工作时，202 的高分辨率使得它可以实现有趣的图形效果，包括半色调图像和线绘图，如图 5.9 中的数字排版机图表。对于后者，我创建了一种名为 Pic 的语言，可以用文字描述组织图表或网络数据包图表等图形。它自然使用 Yacc 作为语法部分，Lex 作为词法部分。图 5.11 显示了一个简单的 Pic 输入和输出示例。

**Book publication**

One reason why the document preparation tools worked well is that they were used for everything---manuals, technical papers, books. If a program had bugs or didn't work well, the authors of the code were in the same

> 一个文档准备工具之所以表现良好的原因是它们被用来处理所有事情——手册、技术文件、书籍。如果一个程序有 bug 或者不能很好地工作，代码的作者就在同一个地方。

[]{#index_split_001.html#p122}![](./index-122_1.jpg){.calibre4}

108 CHAPTER 5: SEVENTH EDITION

**Figure 5.9:**

Unpublished Bell Labs memo on doing battle with the Linotron 202

hallway, and there was strong pressure to fix things and to add features when necessary. This applied more broadly than just document preparation software, of course---we were all users of our own software, and that gav e us a real incentive to improve it.

> 走廊里有强烈的压力来修复事情并在必要时添加功能。当然，这种压力不仅仅限于文档准备软件，我们都是自己软件的用户，这给了我们真正的动力来改进它。

[]{#index_split_001.html#p123}![](./index-123_1.jpg){.calibre4}

CHAPTER 5: SEVENTH EDITION

109

**Figure 5.10:**

Peter face eye-chart (Courtesy of Gerard Holzmann)

[]{#index_split_001.html#p124}110 CHAPTER 5: SEVENTH EDITION

arrow \"stdin\" above

box \"command\"

arrow \"stdout\" above

arrow down from last box.s \"

stderr\" ljust

stdin

stdout

command

stderr

**Figure 5.11:**

The Pic drawing language (input and output) Members of the Computing Science Research Center wrote an unusually large number of influential books during the 1970s and 1980s, well beyond what one might expect from an industrial research lab. As a result, after a while, Bell Labs became known as a source of authoritative books about computing and computer science.

> 在 1970 年代和 1980 年代，计算科学研究中心的成员写了异常多的有影响力的书籍，远远超出了一个工业研究实验室的预期。因此，过了一段时间，贝尔实验室就被认为是有关计算和计算机科学的权威书籍的来源。

Al Aho wrote several widely used textbooks, including the famous 1977

"Dragon book" ( _Principles of Compiler Design_, Figure 5.12) with Jeff Ullman, and _Design and Analysis of Computer Algorithms_ with Jeff and John Hopcroft. Bjarne Stroustrup (Figure 5.13) created C++ in the early 1980s and wrote several C++ books a few years later. Jon Bentley's _Programming_ _Pearls_ books grew out of his columns for _Communications of the ACM_.

> 《龙书》(《编译器原理》，图 5.12)由 Jeff Ullman 编写，以及 Jeff 和 John Hopcroft 合著的《计算机算法设计与分析》。Bjarne Stroustrup(图 5.13)于 1980 年代初创立了 C++，并在几年后写了几本 C++书籍。Jon Bentley 的《编程珠玑》书籍源于他为《ACM 通讯》撰写的专栏。

Mike Garey and David Johnson of the math center used Troff and Eqn for their core book _Computers and Intractability: A Guide to the Theory of NP-Completeness_. We also published book-form manuals for Unix, Plan 9, and so on. These publications became standard texts and references for a generation of programmers and computer science students.

> 麦克·加里和大卫·约翰逊来自数学中心，他们用 Troff 和 Eqn 为他们的核心书籍《计算机与难以处理：NP 完备性理论指南》做出了贡献。我们还出版了 Unix、Plan 9 等的书籍形式的手册，这些出版物成为一代程序员和计算机科学学生的标准文本和参考资料。

How did this relatively small group of researchers from industry manage to produce so many influential books?

> 这个来自行业的相对较小的研究小组是如何做到出版如此多有影响力的书籍的？

I can see several reasons. First and foremost, people took writing seriously, they took pains with their own writing, and they were great critical readers of what other people wrote. Doug McIlroy was first among this group; no one else matched Doug's ability to spot errors (from tiny to crucial) no matter what the topic, nor had his eye for murky prose. I don't think that I ever wrote anything at Bell Labs that I did not ask Doug to comment on, and he always did. It was humbling when he shredded my words but it made me into a much better writer, and that happened to others as well.

> 我能看到几个原因。首先，人们认真对待写作，他们努力处理自己的写作，并且他们是别人写作的优秀批评读者。道格·麦克伊尔罗伊(Doug McIlroy)是这群人中的第一个; 没有人能像道格一样无论讨论什么话题都能发现错误(从微小到至关重要)，也没有他对模糊文字的眼力。我不认为我在贝尔实验室写过的任何东西，我都没有让道格评论，他总是这样做。当他撕裂我的文字时，我感到很沮丧，但这也使我成为一个更好的作家，其他人也是如此。

[]{#index_split_001.html#p125}![](./index-125_1.jpg){.calibre4}

CHAPTER 5: SEVENTH EDITION

111

**Figure 5.12:**

Aho and Ullman Dragon book, first edition, 1977

Of course Doug wasn't the only critical reader. Everyone gav e generously of their time; it was simply part of the culture that you provided detailed comments on what your colleagues wrote. This was unusual, and was one of the things that made the Labs a great place to be.

> 当然，Doug 不是唯一的批评性读者。每个人都慷慨地投入了时间;这只是你提供对同事写作的详细评论的文化的一部分。这很不寻常，也是实验室成为一个伟大之地的原因之一。

Second, local management was supportive of book writing. Publication was important for maintaining Bell Labs' reputation in the scientific and academic communities, and that included books. With managerial support, it was possible to devote full time to a book for six months, and that concentrated effort was enough to basically finish a job that might take sev eral years if it were done as a part-time or evening activity. And it gets better: although Bell Labs retained the copyrights on books, the authors got to keep the royal-ties. I doubt that any of us ever wrote a book explicitly to make money---no one at the Labs would be dumb enough to think that writing a technical book was lucrative---but if a book had some success, the authors kept the money.

> 第二，当地管理层支持写书。出版对于维持贝尔实验室在科学和学术界的声誉非常重要，其中包括书籍。在管理层的支持下，可以全职投入到一本书上六个月，这种集中的努力足以基本完成一个可能需要几年时间完成的兼职或晚上活动的工作。而且情况更好：尽管贝尔实验室保留书籍的版权，但作者可以保留版税。我怀疑我们中没有人会明确写书是为了赚钱---贝尔实验室的人不会傻到认为写技术书是有利可图的---但如果一本书成功了，作者可以赚到钱。

That enlightened management and company policy encouraged people to write, and in the long run it paid off for the company as well as for the authors. Publications by Bell Labs authors were important for recruiting.

> 那种开明的管理和公司政策鼓励人们写作，从长远来看，这对公司和作者都有好处。贝尔实验室作者的出版物对招聘也很重要。

[]{#index_split_001.html#p126}![](./index-126_1.jpg){.calibre4}

112 CHAPTER 5: SEVENTH EDITION

**Figure 5.13:**

Bjarne Stroustrup, ∼1984 (Courtesy of Bjarne Stroustrup) Bell Labs wasn't some mysterious secret operation; students knew it as the place where their software was created and their textbooks were written.

> Bjarne Stroustrup 于 1984 年(由 Bjarne Stroustrup 提供)，贝尔实验室并不是一个神秘的秘密行动；学生们把它当作软件创造和教科书写作的地方。

Potential new hires could see that good work was being done and it was published; they didn't hav e to worry about disappearing into an "industrial"

> 潜在的新雇员可以看到良好的工作正在进行，而且已经发布；他们不必担心会消失在一个“工业”中。

research lab. That put Bell Labs recruiting on an equal footing with universities, with the added advantage that people could do research full time at the Labs, without the distractions of teaching, administration and raising money.

> 研究实验室。这使贝尔实验室招聘与大学平等，额外的优势是人们可以在实验室全职进行研究，而无需分心于教学、行政和筹集资金。

This combination of great software and influential books was a big part of what made the Labs so successful at the time.

> 这种优秀的软件和有影响力的书籍的结合，是当时实验室取得成功的重要因素之一。

A third factor is more technical: the symbiosis among C and Unix as a programming environment, document preparation as a research area, and writing about technical computer topics as a major activity. This began with text formatting programs like Doug McIlroy's Roff, Joe Ossanna's Nroff and Troff, and then the preprocessors like Eqn, Tbl, and so on. Those tools made it easier to produce documents that included ever more typographically challenging content, like mathematics, tables, figures, diagrams, and graphs.

> 第三个因素更具技术性：C 语言和 Unix 作为编程环境的共生，文档准备作为一个研究领域，以及关于技术计算机主题的写作是一项主要活动。这始于像 Doug McIlroy 的 Roff，Joe Ossanna 的 Nroff 和 Troff 这样的文本格式化程序，然后是像 Eqn，Tbl 等预处理程序。这些工具使得生成包含更多排版挑战性内容(如数学，表格，图形，图表和图形)的文档变得更加容易。

That in turn led to better writing, because all of these document preparation programs shared a vital characteristic: they made it easy to make multiple revisions of documents and always have a clean copy to work from, as opposed to the slow and painful alternative of giving material to a typist and waiting days for it to come back.

> 这反过来促使更好的写作，因为所有这些文档准备程序都具有一个重要特征：它们使得对文档进行多次修订变得容易，并且总是有一个干净的副本可以工作，而不是将材料交给打字员并等待几天才能收到的缓慢而痛苦的替代方案。

[]{#index_split_001.html#p127}CHAPTER 5: SEVENTH EDITION

113

It may sound trivial, but I'm sure that the ability to make revisions so easily led to better writing, because it pretty much eliminated the overhead of making an up to date copy, and it completely eliminated middlemen like typists, editors and printers. Accuracy mattered for technical papers and for the Unix Programmer's Manual, but control of the whole process especially mattered for books. For programming books, it was vital that the programs were typeset directly from the source code, so we could be sure that what was printed was correct, that it hadn't been inadvertently changed by human intervention.

> 这听起来可能微不足道，但我相信，这种能够轻松修改的能力导致了更好的写作，因为它几乎消除了制作最新副本的开销，完全消除了打字员、编辑和印刷工等中间人。准确性对技术论文和 Unix 程序员手册都很重要，但对于书籍来说，控制整个过程尤为重要。对于编程书籍来说，直接从源代码排版是至关重要的，这样我们才能确保印刷的内容是正确的，没有被人为干预改变。

These tools were all written in C, of course, since it was expressive and efficient. It's hard to remember today, perhaps, that efficiency in both time and space were crucial when machine capacities were expressed in kilobytes, not gigabytes. Every byte counted, and so at some level did every instruction, so a language that economized on both was not just nice, but a practical necessity.

> 这些工具当然都是用 C 编写的，因为它具有表达力和效率。今天很难回想起，当机器容量以千字节而不是千兆字节表示时，时间和空间的效率是多么重要。每个字节都很重要，每条指令也是如此，因此一种节省时间和空间的语言不仅很好，而且是一种实际的必要性。

All of this has come full circle---this book was produced by the descen-dants of these document preparation programs, though with the excellent fresh implementations and enhancements in Groff, Geqn, and so on, written by James Clark.

> 这一切都已经圆满结束：这本书是由这些文档准备程序的后代制作的，不过有了 James Clark 出色的新实现和增强，如 Groff、Geqn 等，就更加完美了。

**5.4 Sed and Awk**

One of the major simplifications of the Unix file system was its uniform treatment of files as sequences of uninterpreted bytes. There were no records, no required or prohibited characters, and no internal structure imposed by the file system---just bytes.

> Unix 文件系统的一个主要简化是将文件作为未经解释的字节序列进行统一处理。没有记录，没有必需或禁止的字符，也没有文件系统内部结构强加的字节。

There was a similar simplification in the way that most Unix programs handled textual data. Te xt files were just sequences of bytes that happened to be characters in ASCII, the American Standard Code for Information Inter-change. This uniform view of plain text was a natural fit for pipelines, and the Unix toolkit was full of programs that read text input, did something with or to it, and wrote text output. I've already mentioned examples like word counting, comparison, sorting, transliteration, finding duplicates and of course the quintessential example, grep for searching.

> 在大多数 Unix 程序处理文本数据的方式中也存在着类似的简化。文本文件只是一系列字节，这些字节恰好是美国信息交换标准 ASCII 码中的字符。这种对纯文本的统一视图很适合管道，Unix 工具箱中充满了读取文本输入、对其进行某些操作或处理，然后输出文本的程序。我已经提到了一些例子，如计数、比较、排序、转换、找重复以及最典型的例子——grep 搜索。

**Sed**

The success of grep inspired Lee McMahon to write an analog called gres that did simple substitutions on text as it flowed through; "s" was the substitute command in ed. Lee soon replaced it by a generalization, a stream

> grep 的成功鼓舞了 Lee McMahon 编写一个类似的程序 gres，它可以在文本流中进行简单的替换；在 ed 中，"s"是替换命令。Lee 很快就将其替换为了更一般化的流。

[]{#index_split_001.html#p128}114 CHAPTER 5: SEVENTH EDITION

editor called Sed that applied a sequence of editing commands to text on its way from input to output; grep and gres were both special cases of Sed. The commands that Sed uses are the same as the editing commands in the standard ed text editor. Sed is frequently used today in shell scripts, for transforming a stream of data in some way: replacing characters, or adding or removing unwanted spaces, or discarding something unwanted.

> 编辑器称为 Sed，它将一系列编辑命令应用于从输入到输出的文本上；grep 和 gres 都是 Sed 的特殊情况。Sed 使用的命令与标准 ed 文本编辑器中的编辑命令相同。Sed 今天经常在 shell 脚本中使用，用于以某种方式转换数据流：替换字符，添加或删除不需要的空格，或丢弃不需要的东西。

Lee had an unusual background---a PhD in psychology from Harvard, and time in a Jesuit seminary preparing for the priesthood before switching to a more conventional path as a computer scientist. He was one of the first in the Unix group to think about processing text at scale, at a time when primary memories were too small to store large amounts of text. I might add that

> 李有一个不寻常的背景：哈佛大学的心理学士学位，以及在耶稣会修道院准备担任神职之前转向更传统的计算机科学道路的时间。他是 Unix 组中第一个考虑以大规模处理文本的人，当时主存储器太小，无法存储大量文本。我可以补充说

"large" is relative. Lee's particular interest in the early 1970s was the Feder-alist Papers, which altogether are only a little over a meg abyte.

> "大" 是相对的。李在 1970 年代初期的特别兴趣是联邦党文件，总共只有一点点超过一兆字节。

**Awk**

I was interested in tools that could process both numbers and text equally well. Neither grep or Sed could handle numeric data or do arithmetic, and grep couldn't deal with multiple text lines; such computations still required a C program. So I was looking for some kind of generalization. At the same time, Al Aho (Figure 5.14) had been experimenting with a richer class of regular expressions than grep supported, and had written egrep ("extended grep"). Finally, Peter Weinberger, who not long afterwards transferred into 1127 and moved into the office between Al and me, was interested in databases.

> 我对可以同时处理数字和文本的工具感兴趣。Grep 和 Sed 都不能处理数值数据或做算术运算，而且 grep 也不能处理多行文本；这样的计算仍然需要一个 C 程序。因此，我正在寻找一种概括的方法。与此同时，阿尔·阿霍(见图 5.14)一直在尝试比 grep 支持的更丰富的正则表达式，并编写了 egrep(“扩展 grep”)。最后，彼得·温伯格不久之后转入 1127，搬进了阿尔和我之间的办公室，他对数据库感兴趣。

In the fall of 1977, the three of us talked about how to combine these ideas, taking some inspiration from RPG, IBM's powerful but inscrutable report program generator, along with a neat idea from Marc Rochkind that's described in the next chapter. Ultimately we designed a language that we called AWK (Awk from now on). As we said in the original description, naming a language after its authors shows a certain paucity of imagination. I don't recall now whether we thought about cognates related to "awkward," or perhaps we found the name apt in a sardonic way, but in any case it stuck.

> 1977 年秋天，我们三个人谈论如何结合这些想法，从 RPG(IBM 强大而又难以理解的报告程序生成器)中获得一些灵感，再加上 Marc Rochkind 在下一章中描述的一个不错的想法。最终我们设计了一种我们称之为 AWK(从现在开始简称为 Awk)的语言。正如我们在最初的描述中所说，以作者的名字命名一种语言显示出一定程度的想象力的缺乏。我现在不记得我们是否考虑过与“笨拙”有关的同源词，或者我们可能发现这个名字在讽刺的方式中是很合适的，但无论如何它都坚持下来了。

Peter wrote the first version very quickly, in just a few days, using Yacc, Lex and Al's egrep regular expression code.

> 彼得很快就写出了第一版，只用了几天，使用了 Yacc、Lex 和 Al 的 egrep 正则表达式代码。

An Awk program is a sequence of patterns and actions. Each line of input is tested against each pattern, and if the pattern matches, the corresponding action is performed. Patterns can be regular expressions or numeric or string relations. Actions are written in a dialect of C. An omitted pattern matches all lines; an omitted action prints the matching line.

> 一个 Awk 程序是一系列模式和动作的序列。每一行输入都会被测试与每一个模式，如果模式匹配，相应的动作就会被执行。模式可以是正则表达式或者数字或字符串关系。动作是用 C 语言的一种方言编写的。省略的模式会匹配所有行；省略的动作会打印出匹配的行。

[]{#index_split_001.html#p129}![](./index-129_1.jpg){.calibre4}

CHAPTER 5: SEVENTH EDITION

115

**Figure 5.14:**

Al Aho, ∼1981 (Courtesy of Gerard Holzmann) This example prints all input lines that are longer than 80 characters; it's a pattern with no action.

> 这个例子打印出所有长度超过 80 个字符的输入行；它是一个没有动作的模式。(出处：Gerard Holzmann，1981 年左右)

awk 'length \> 80'

Awk supports variables that hold numbers or strings, and associative arrays whose subscripts can be numbers or arbitrary strings of characters.

> Awk 支持保存数字或字符串的变量，以及其下标可以是数字或任意字符串的关联数组。

Variables are initialized to zero and an empty string, so there is usually no need to set initial values.

> 变量默认初始化为零和空字符串，因此通常无需设置初始值。

Awk automatically reads each line of each input file and splits each input line into fields, so one rarely needs code to explicitly read input or parse individual lines. There are also built-in variables that contain the number of the current input line and the number of fields on it, so those values do not have to be computed either. Such defaults eliminate boilerplate code and mean that many Awk programs are only a line or two long.

> Awk 自动读取每个输入文件的每一行，并将每一行输入拆分为字段，因此很少需要代码显式读取输入或解析单个行。还有内置的变量，其中包含当前输入行的编号和其上的字段数，因此无需计算这些值。这种默认设置消除了样板代码，这意味着许多 Awk 程序只有一行或两行长。

To illustrate, this program prefixes each line by its line number: awk '{print NR, \$0}'

> 举例来说，这个程序会为每一行添加行号前缀：awk '{print NR, \$0}'

NR is the number of the current input line, and \$0 is the input line itself.

> NR 是当前输入行的行号，$0 是输入行本身。

The following canonical example counts the number of occurrences of each word in its input, and prints the words and their counts at the end:

> 以下的规范示例计算输入中每个单词的出现次数，并在最后打印出单词及其计数：

[]{#index_split_001.html#p130}116 CHAPTER 5: SEVENTH EDITION

{ for (i = 1; i \<= NF; i++) wd\[\$i\]++ }

END { for (w in wd) print w, wd\[w\] }

The first line is an action with no pattern, so it is evaluated for each input line. The built-in variable NF is the number of fields on the current input line; this is computed automatically. The variable \$i is the i-th field, again computed automatically. The statement wd\[\$i\]++ uses that value, which is a word of the input, as a subscript in the array wd and increments that element of the array. The special pattern END matches after the last input line has been read. Note the two different kinds of for loop. The first is borrowed straight from C. The second loops over the elements of an array, so in this example, it prints a line for each distinct word of the original input, along with the count of how many times that word occurred.

> 第一行没有模式，因此它会为每一行输入进行评估。内置变量 NF 是当前输入行的字段数，它会自动计算。变量$i是第i个字段，也会自动计算。语句wd[$i]++使用该值(即输入的一个单词)作为数组 wd 的下标，并将该数组元素加一。特殊模式 END 会在读取最后一行输入之后匹配。注意两种不同的 for 循环。第一种是直接从 C 中借用的。第二种是遍历数组的元素，因此在本例中，它会为原始输入中的每个不同的单词打印一行，同时还会显示该单词出现的次数。

Although Perl and later Python took over many potential applications, Awk is still widely used today; it's a core tool and there are at least four or five independent implementations, including Arnold Robbins's Gawk and Michael Brennan's Mawk. Awk certainly has some questionable design decisions and dark corners, but I think it gives the most bang for the programming buck of any language---one can learn much of it in 5 or 10 minutes, and typical programs are only a few lines long. It doesn't scale well to big programs, though that hasn't stopped people from writing Awk programs that are thousands of lines long.

> 尽管 Perl 和后来的 Python 取代了许多潜在的应用，但 Awk 今天仍然被广泛使用；它是一个核心工具，至少有四五个独立的实现，包括 Arnold Robbins 的 Gawk 和 Michael Brennan 的 Mawk。 Awk 当然有一些值得怀疑的设计决策和黑暗角落，但我认为它为编程提供了最大的回报，任何语言都可以在 5 到 10 分钟内学习，典型的程序只有几行。它不能很好地扩展到大型程序，尽管这并没有阻止人们编写数千行的 Awk 程序。

Sed is popular as well, a frequent component of shell pipelines. I even have a bumper sticker that says

> Sed 也很受欢迎，经常用于 shell 管道中。我甚至有一个挡泥板贴纸上写着

"Sed and Awk: together we can change everything."

It's worth noting that Sed, Awk, Make, Yacc and Lex all implement some flavor of the _pattern-action paradigm_. Programs in these languages consist of a sequence of patterns and actions; the basic operation is to check the input against each pattern and when a pattern is matched, perform the corresponding action. Patterns and actions may sometimes be omitted, in which case a default behavior takes place.

> 值得注意的是，Sed、Awk、Make、Yacc 和 Lex 都实现了某种模式动作范式。这些语言的程序由一系列模式和动作组成；基本操作是检查输入是否与每个模式匹配，如果模式匹配，则执行相应的操作。有时模式和动作可能被省略，在这种情况下，将采取默认行为。

For example, grep, Sed and Awk can all be used to match a single regular expression. The following three commands are equivalent if the specific regular expression is valid for each:

> 例如，Grep、Sed 和 Awk 都可以用来匹配单个正则表达式。如果每个正则表达式有效，以下三条命令是等价的：

grep re

sed -n /re/p

awk /re/

The pattern-action paradigm is a natural way to think about computations that are primarily a sequence of tests and actions.

> 模式行动范式是一种思考主要由测试和行动序列组成的计算的自然方式。

[]{#index_split_001.html#p131}![](./index-131_1.jpg){.calibre4}

CHAPTER 5: SEVENTH EDITION

117

**Figure 5.15:**

Awk in popular culture

**5.5 Other languages**

The Unix programming environment, its language-development tools, a rich set of potential application domains, and of course local experts in everything from compilers to language theory and algorithms, led to the design and implementation of other languages as well. I'm not going to dive deeply into any of these, but it's worth a quick look at a partial list.

> Unix 编程环境、语言开发工具、丰富的应用领域以及当地的编译器、语言理论和算法专家，都促使了其他语言的设计和实现。我不会深入研究其中任何一个，但是值得快速看一下部分列表。

There's no need to understand any of the details in these examples. The real lesson is that wide-ranging interests, language expertise, and tools like

> 不需要了解这些例子中的任何细节。真正的教训是，广泛的兴趣、语言专业知识以及像这样的工具。

[]{#index_split_001.html#p132}118 CHAPTER 5: SEVENTH EDITION

Yacc and Lex made it possible for members of the Center to create new languages for new application areas relatively easily. This would have been much harder without that combination of factors, and I think that many of these interesting languages would not have existed otherwise.

> 使用 Yacc 和 Lex 使中心的成员们能够相对容易地为新的应用领域创建新的语言。如果没有这种组合因素，这将会变得更加困难，而我认为，许多有趣的语言也不会存在。

The most significant example is C++, which started in 1979 when Bjarne Stroustrup joined 1127, fresh from his PhD at Cambridge. Bjarne was interested in simulation and operating systems, but existing languages didn't really satisfy his needs. Accordingly, he took some of the good ideas from the closest match, Simula, and merged them with C. The result, which combined the ideas of object-oriented programming with the efficiency and expressiveness of C, was called "C with classes," and dates from 1980.

> 最重要的例子是 C++，它始于 1979 年，当时 Bjarne Stroustrup 从剑桥大学获得博士学位后加入了 1127。Bjarne 对仿真和操作系统感兴趣，但现有的语言并不能真正满足他的需求。因此，他从最接近的匹配 Simula 中提取了一些好的想法，并将它们与 C 融合在一起。这个结果将面向对象编程的思想与 C 的效率和表达力相结合，被称为“C with classes”，起源于 1980 年。

This proved to be a good combination, and the language prospered. In 1983, it acquired the name C++, Rick Mascitti's pun on the C ++ increment operator. Today C++ is one of the most widely used programming languages, at the heart of the implementation of Microsoft's Office suite, big parts of Google's infrastructure, your favorite browser (whatever it is), many video games, and much other behind-the-scenes software.

> 这证明是一个很好的组合，语言发展迅速。1983 年，它获得了 C++的名字，Rick Mascitti 对 C ++增量运算符的双关语。今天，C++是最广泛使用的编程语言之一，是 Microsoft Office 套件实现的核心，Google 基础设施的重要组成部分，您喜欢的浏览器(无论是什么)，许多视频游戏以及其他许多幕后软件的核心。

Bjarne was a member of my department for about 15 years, and as described earlier, he used to drop in frequently to talk out design decisions, so I got to see the evolution of C++ from the beginning. At least in the early days I understood it, but it's now a much bigger language and I'm barely literate in it.

> 贝尔尼曾经在我们部门工作了大约 15 年，正如之前所描述的，他经常来讨论设计决定，所以我有机会从一开始就看到 C++的演变。至少在早期，我能理解它，但现在它变得更大了，我几乎不懂它了。

C++ is often criticized for its size, and sometimes for some of the syntax that it inherited from C. I know from years of conversations that there isn't anything in the language for which Bjarne didn't hav e a good reason. It also was a sound engineering and marketing decision to make C++ a superset of C, even though that required including many of C's syntactic and semantic rough spots. If Bjarne had not aimed at C compatibility, C++ would have had much less chance of success. It's hard to establish a new language; making it compatible at both source level (for cultural familiarity) and object level (use of existing C libraries) was crucial, and at the time so was making it as efficient as C.

> C++常常因它的大小而受到批评，有时也因为它从 C 语言中继承的一些语法而受到批评。我凭借多年的对话知道，语言中没有任何一点是 Bjarne 没有好的理由的。让 C++成为 C 的超集也是一个可靠的工程和营销决策，即使这意味着必须包括许多 C 语言的语法和语义上的粗糙点。如果 Bjarne 没有以兼容 C 为目标，C++将没有太大的成功机会。建立一种新语言是很难的；在源级别(文化熟悉度)和对象级别(使用现有的 C 语言库)上实现兼容性是至关重要的，而且当时还要像 C 语言一样高效。

A handful of significant other languages, not yet mentioned, also came out of 1127.

> 1127 至今也出现了一些重要的其他语言。

Stu Feldman and Peter Weinberger wrote the first Fortran 77 compiler, called f77. As a language, Fortran 77 was somewhat better than the Fortran 66 that I had papered over with Ratfor, though it still didn't hav e a sensible set of control-flow statements. In any case, f77 was challenging to build but worthwhile, since it was heavily used by numerical analysts in 1127 on both

> Stu Feldman 和 Peter Weinberger 编写了第一个 Fortran 77 编译器，称为 f77。作为一种语言，Fortran 77 比我用 Ratfor 覆盖的 Fortran 66 要好一些，但它仍然没有一套合理的控制流语句。无论如何，f77 构建起来是具有挑战性的，但是值得的，因为它在 1127 年被数值分析师广泛使用。

[]{#index_split_001.html#p133}![](./index-133_1.jpg){.calibre4}

CHAPTER 5: SEVENTH EDITION

119

the PDP-11 and the VAX.

In a related effort, Stu and Dave Gay wrote f2c, which translated Fortran into C; f2c made it possible to use Fortran on systems where no compiler was available, or where a Fortran compiler was an expensive commercial product.

> 在一项相关的工作中，Stu 和 Dave Gay 写了 f2c，将 Fortran 翻译成 C；f2c 使得在没有编译器或 Fortran 编译器是昂贵商业产品的系统上使用 Fortran 成为可能。

Gerard Holzmann (Figure 5.16), who joined 1127 from the University of Technology in Delft, had always been interested in photography. In the early 1980s he conceived the idea of a programming language for making algorithmic transformations of digital image files. He called it Pico:

> Gerard Holzmann(见图 5.16)，他从荷兰代尔夫特理工大学加入 1127，一直对摄影感兴趣。早在 1980 年代，他构想出了一种用于对数字图像文件进行算法变换的编程语言。他称之为 Pico。

"Originally the name indicated its size, later it was more easily understood as an abbreviation of 'picture composition.' "

> 最初，这个名字表示它的大小，后来它更容易被理解为“图片组成”的缩写。

Pico is another example of a pattern-action language. It defines new images by evaluating a user-defined expression once for every pixel in the original image; expressions can refer to values, coordinates, various functions, and parts of other images. Such expressions can lead to entertaining transformations, many of which appeared in _Beyond Photography_, a book that Gerard published in 1988 to describe and illustrate Pico. (Figure 5.17 is an example.) Not surprisingly, Pico was implemented in C with a Yacc parser.

> Pico 是另一种模式动作语言的例子。它通过一次为原始图像中的每个像素评估用户定义的表达式来定义新图像；表达式可以引用值、坐标、各种函数和其他图像的部分。这些表达式可以产生有趣的变换，其中许多出现在 Gerard 于 1988 年出版的《超越摄影》一书中，用来描述和说明 Pico。(图 5.17 是一个例子)不出所料，Pico 是用 C 和 Yacc 解析器实现的。

**Figure 5.16:**

Gerard Holzmann, ∼1981 (Courtesy of Gerard Holzmann) Gerard also created another specialized language-based tool, Spin, for analyzing and checking the correctness of software systems that involve

> Gerard Holzmann，1981 年(Gerard Holzmann 提供)Gerard 还创建了另一种专门的基于语言的工具 Spin，用于分析和检查涉及软件系统的正确性。

[]{#index_split_001.html#p134}![](./index-134_1.jpg){.calibre4}

120 CHAPTER 5: SEVENTH EDITION

**Figure 5.17:**

Gerard Holzmann, transformed by Pico

separate communicating processes. Spin can be used to verify that a particular system is logically correct, free of defects like deadlock where no progress can be made. ("After you." "No, after you.") Spin is an excellent example of research in 1127 into how to represent the interactions between separate processes over time, along with some first-rate software engineering to make a system that's easy to use and that runs fast enough to be useful.

> 可以使用 Spin 来验证某个系统是否逻辑正确，没有像死锁这样的缺陷，无法取得进展。(“您先请。”“不，您先请。”)Spin 是 1127 年研究如何表示不同进程之间的交互以及一流的软件工程，以制作一个易于使用、速度足够快的系统的出色示例。

Spin models are written in another special-purpose language called Promela (protocol metalanguage), also implemented with Yacc.

> 模型旋转是用另一种特殊目的语言 Promela(协议金言)书写的，也用 Yacc 实现。

Spin is thriving, with many thousands of installations and an annual conference. It has been used to verify a large number of systems, ranging from hardware designs to railway signaling protocols.

> 自旋正在蓬勃发展，有数以千计的安装和一年一度的会议。它已经被用来验证大量的系统，从硬件设计到铁路信号协议。

Bob Fourer, Dav e Gay and I designed and implemented AMPL, a language for specifying optimization problems like linear programming. Bob was a professor of management science and operations research at North-western University, and had long been interested in helping people create mathematical optimization models. Our work on AMPL began when he spent a sabbatical at the Labs in 1984.

> 鲍勃·福勒、戴夫·盖伊和我设计并实施了 AMPL，一种用于指定线性规划等优化问题的语言。鲍勃是西北大学管理科学与运筹学教授，一直致力于帮助人们创建数学优化模型。我们在 AMPL 的工作始于 1984 年，他在实验室度过了一个沙巴克假期。

The AMPL language makes it easy to define models that describe particular optimization problems, like finding the best way to ship goods from factories to stores, given data for shipping costs, expected sales at each store, the manufacturing capacity of each factory, and so on. Optimization problems are written in an algebraic notation for systems of constraints that have to be satisfied, and an objective function to be maximized or minimized.

> AMPL 语言可以轻松地定义模型，描述特定的优化问题，比如根据运费数据、每个商店的预期销售量、每个工厂的生产能力等，找到最佳的将货物从工厂运往商店的方式。优化问题用代数表示法写成，包含必须满足的约束系统，以及要最大化或最小化的目标函数。

[]{#index_split_001.html#p135}CHAPTER 5: SEVENTH EDITION

121

Optimization problems like these are at the heart of many industries: airline crew scheduling, manufacturing, shipping and distribution, inventory control, advertising campaigns, and an enormous variety of other applications.

> 优化问题像这些是许多行业的核心：航空公司的机组排班、制造业、运输和分销、库存控制、广告活动，以及许多其他应用。

I wrote the initial AMPL implementation in C++, along with a Yacc grammar and (I think) Lex for lexical analysis. It was my first serious C++

> 我用 C++编写了最初的 AMPL 实现，还有一个 Yacc 语法和(我想)Lex 用于词法分析。这是我第一次严肃的 C++编程。

program, but I soon relinquished the code to Dave Gay.

AMPL is perhaps the only widely used language originating in 1127 that is proprietary. (The language itself can't be copyrighted, but there are at this point no open-source implementations that I am aware of.) AT&T started licensing AMPL to companies a few years after it was first created. When Dave and I retired from Bell Labs, the three of us formed a small company, AMPL Optimization, to continue AMPL development and marketing. Eventually we bought the rights from Bell Labs so we could go our own way. The company remains small but is a significant player in its niche market.

> AMPL 可能是唯一一种起源于 1127 年的广泛使用的专有语言。(语言本身不能受版权保护，但是据我所知，目前没有开源实现。)AT&T 在 AMPL 最初创建几年后开始向公司授权使用 AMPL。当戴夫和我从贝尔实验室退休时，我们三人成立了一家小公司 AMPL Optimization，继续开发和营销 AMPL。最终，我们从贝尔实验室购买了权利，以便走出自己的道路。公司虽然规模较小，但在其细分市场中仍然是重要参与者。

In the early 1980s, Rob Pike (Figure 5.18) and Luca Cardelli experimented with languages for concurrency, especially for interactions with input devices like mice and keyboards; that led to the names Squeak and Newsqueak. The ideas from Newsqueak eventually found their way into the concurrent languages Limbo and Alef that were used in Plan 9, and a decade later into the Go programming language, which was created at Google in 2008 by Rob Pike, Ken Thompson and Robert Griesemer.

> 在 1980 年代早期，Rob Pike(见图 5.18)和 Luca Cardelli 尝试使用语言来实现并发，尤其是与鼠标和键盘等输入设备的交互；这就导致了 Squeak 和 Newsqueak 的名字。 Newsqueak 的想法最终进入了用于 Plan 9 的并发语言 Limbo 和 Alef，十年后，这些想法又进入了 2008 年由 Rob Pike、Ken Thompson 和 Robert Griesemer 在 Google 创建的 Go 编程语言中。

**5.6 Other contributions**

Most of the emphasis so far has been on system software, especially languages, since that's what I know best, but I should mention some significant activities in scientific computing, communications, security and hardware, since they were often influential, and of course they all had substantial software components. These don't all fall neatly into the 7th edition time frame.

> 大部分重点都放在系统软件上，尤其是语言，因为那是我最擅长的，但是我应该提到一些重要的科学计算、通信、安全和硬件的活动，因为它们经常有影响力，当然它们都有大量的软件组件。这些都不能完全符合第七版的时间表。

简体中文：
迄今为止，大部分重点都放在系统软件上，尤其是语言，因为这是我最擅长的，但是我也应该提到科学计算、通信、安全和硬件方面的重要活动，因为它们也经常产生重大影响，而且这些活动当然也都有大量的软件组件。这些活动并不完全符合第七版的时间表。

**Scientific computing**

As might be expected for a scientific research operation, Bell Labs was involved very early in the use of computers for modeling and simulation of physical systems and processing, a natural extension of mathematical research. It was also a validation of Dick Hamming's prediction that computing would displace laboratories. The focus was on numerical linear algebra, differential and integral equations, function approximation, and mathematical libraries that could make the best known methods widely available.

> 作为一个科學研究運營，貝爾實驗室很早就參與了對物理系統的建模和模擬以及處理的計算機使用，這是對 Dick Hamming 預測計算會取代實驗室的數學研究的一個自然延伸。重點是數值線性代數、微分和積分方程、函數逼近以及可以使最佳已知方法廣泛應用的數學庫。

[]{#index_split_001.html#p136}![](./index-136_1.jpg){.calibre4}

122 CHAPTER 5: SEVENTH EDITION

**Figure 5.18:**

Rob Pike, ∼1981 (Courtesy of Gerard Holzmann) Phyllis Fox was a pioneer in this kind of numerical computation, and was a major contributor to the PORT library for Fortran programmers. PORT

> 罗布·派克，1981 年(提供赫尔德·霍尔茨曼)菲利斯·福克斯是这种数值计算的先驱，并且是 Fortran 程序员的 PORT 库的主要贡献者。PORT。

defined machine-specific constants for values like the ranges of numbers that would be different for different computers; its libraries assured portability of Fortran code across different computers.

> 定义了机器特定的常量，用于不同计算机上的数值范围等值；它的库确保了 Fortran 代码在不同计算机之间的可移植性。

The PORT library was a large body of work, ultimately with 130,000

lines of Fortran in 1,500 programs and a lot of documentation. Barbara Ryder and Stu Feldman developed a Fortran compiler called PFORT, which checked that Fortran code was written in a portable subset of standard Fortran. Norm Schryer wrote a program to check the arithmetic operations of computers, which often differed greatly in how they did floating-point arithmetic. This was especially important since it predated the development of standards for floating-point behavior.

> 芭芭拉·莱德和斯图·费尔德曼开发了一种叫做 PFORT 的 Fortran 编译器，用于检查 Fortran 代码是否编写在标准 Fortran 的可移植子集中。诺姆·施莱尔编写了一个检查计算机算术运算的程序，这在浮点算术方面经常有很大的差异，这在浮点行为标准发展之前尤其重要。这在 1500 个程序和大量文档中都有 Fortran 行。

Eric Grosse and Bill Coughran developed algorithms for semiconductor modeling and simulation, circuit analysis, and visualization, especially for semiconductor design and fabrication. Much of the numerical software developed at Bell Labs was distributed worldwide through the Netlib repository of mathematical software, which is still widely used by the scientific computing community. Other numerical analysts who made significant contributions to Netlib and the larger community included Dave Gay, Linda Kaufman, and Margaret Wright.

> 艾瑞克·格罗斯和比尔·科夫兰开发了用于半导体建模和仿真、电路分析和可视化的算法，特别是用于半导体设计和制造。贝尔实验室开发的大部分数值软件通过数学软件的 Netlib 存储库在全世界发布，该存储库仍被计算机科学界广泛使用。其他对 Netlib 和更大社区做出重大贡献的数值分析师还包括戴夫·盖伊、琳达·考夫曼和玛格丽特·赖特。

[]{#index_split_001.html#p137}CHAPTER 5: SEVENTH EDITION

123

**AT&T's 800-number directory**

Eric Grosse's experience with software distribution was a big help in a fun unrelated project: in 1994, Eric, Lorinda Cherry and I put AT&T's 800-number directory on the then brand new Internet. The intent was for AT&T to gain some experience with providing a real Internet service (and with the Internet itself), perhaps to generate extra calls to 800 numbers, and even ultimately to provide revenue through enhanced services like display advertisements. In addition, we hoped for some modest public relations benefit from providing something of real value, not merely a teaser like so many Internet offerings at the time.

> 艾瑞克·格罗斯在软件分发方面的经验，在一个有趣的非相关项目中发挥了重要作用：1994 年，艾瑞克、洛琳达·雪莉和我将 AT&T 的 800 号码目录放在当时全新的互联网上。其目的是让 AT&T 获得一些提供真正的互联网服务的经验(以及互联网本身的经验)，也许可以增加 800 号码的呼叫量，甚至最终通过增强服务(如显示广告)获得收入。此外，我们希望通过提供真正有价值的东西，而不仅仅是当时很多互联网产品的诱饵，获得一些适度的公关效益。

We obtained a database snapshot of 157,000 records, about 22 MB, in August 1994 and in a few hours had it running on a local computer as a searchable and browsable web site. Convincing AT&T management to make it public was a much slower process. After much internal deliberation, howev er, managerial reluctance and inertia eventually succumbed to a rumor that AT&T's competitor MCI was about to offer some Internet service, and the directory went public on October 19, 1994. It was AT&T's first web service.

> 我们在 1994 年 8 月获得了一个 157000 条记录的数据库快照，大约 22MB，几个小时之内就将它部署在本地计算机上，可以搜索和浏览。说服 AT&T 管理层将其公开更是一个漫长的过程。然而，经过多次内部讨论，管理层的抗拒和惰性最终屈服于一个谣言，即 AT&T 的竞争对手 MCI 即将提供某种互联网服务，这个目录于 1994 年 10 月 19 日正式公开。这是 AT&T 的第一个网络服务。

The political delay was mildly frustrating, but the data story was instructive. The database was replete with errors, a host of listings that clearly no one had ever looked at with a critical eye, such as 9 different spellings of Cincinnati. (They would make a good example of a regular expression.) In spite of its imperfections, the directory service garnered some public relations benefit: it was listed for a while as the first of the "Cool Links" on the Yahoo WWW Guide. (Yahoo itself was founded early in 1994, and its indexing was entirely manual.) AT&T scored a minor victory over MCI by being first with a useful service, though it was a near thing. The directory did make AT&T appear to be involved in the Internet and it stimulated a significant amount of internal discussion and plans to make plans for planning further services. If nothing else, the experience brought home the remarkable rate at which the Internet was growing and changing; as my unofficial report said at the time, "We hav e to learn to act quickly in this area if we are to be in it at all."

> 政治延迟虽然令人有些沮丧，但数据故事却很有启发性。数据库里充满了错误，很多明显没有经过严格审查的资料，比如说有 9 种不同的辛辛那提拼写方式(这可以作为一个正则表达式的很好的例子)。尽管有这些缺陷，这个电话簿服务还是获得了一些公关上的好处：它曾经被列为雅虎 WWW 指南里的“酷链接”第一位。(雅虎本身是在 1994 年初创立的，当时的索引是完全手动的。)虽然只是小小的胜利，AT&T 还是比 MCI 更早推出了一项有用的服务。这个电话簿让 AT&T 看起来似乎参与了互联网，也引发了大量的内部讨论和计划，以便计划进一步的服务。即使没有别的，这次经历也让我们意识到了互联网以惊人的速度在增长和变化；正如我当时的非官方报告所说，“我们必须学会在这个领域快速行动，才能够参与其中。”

**UUCP**

In the mid 1970s, Mike Lesk wrote UUCP, the Unix to Unix copy program. It was used to send files from one Unix system to another, generally using ordinary phone lines. Those were slow and sometimes expensive, but they were ubiquitous and most Unix systems of the time had some kind of dial-up access, though fewer had dial-out capabilities, since that would

> 1970 年代中期，Mike Lesk 编写了 UUCP，这是一个 Unix 到 Unix 的复制程序。它用来在两个 Unix 系统之间发送文件，通常使用普通的电话线路。这些线路很慢，有时也很贵，但它们无处不在，当时的大多数 Unix 系统都有某种形式的拨号接入，但拨号出去的功能较少，因为这样做会花费更多的成本。

[]{#index_split_001.html#p138}124 CHAPTER 5: SEVENTH EDITION

involve paying for phone calls.

Although UUCP was primarily used for software distribution, it was also the basis of remote command execution, mail transfer and news groups long before the Internet was widely available. Usenet, which was one of the first worldwide information distribution systems, was based on UUCP.

> 尽管 UUCP 主要用于软件分发，但在互联网普及之前，它也是远程命令执行、邮件传输和新闻组的基础。 Usenet，这是最早的全球信息分发系统之一，是基于 UUCP 的。

The first UUCP distribution was included in the 7th edition; it was refined, ported to other operating systems, and made open source over the next few years. UUCP usage finally died out as the Internet became the standard communications network and its protocols took over.

> 第七版中包含了第一个 UUCP 发行版；在接下来的几年里，它得到了完善、移植到其他操作系统，并开源。随着互联网成为标准通信网络并取代 UUCP，UUCP 的使用最终消失了。

**Security**

People in the Unix community had been concerned with security from the earliest days, an interest that came in part from Multics, and in part from experience in cryptography.

> 在 Unix 社区的人们从最早的日子就一直关注安全问题，这种兴趣部分来自 Multics，部分来自对密码学的经验。

One security concern was to allow file system users to control access to their files. The Unix file system used 9 bits for each file to control what kinds of access could be made to the file. The file's owner had three bits, independently controlling read access, write access, and execute access. For a regular text file, read and write would normally be allowed for the owner, and execute would not, unless the file was an executable program or a shell script. There were three more bits for the owner's group, which might be something like a department or a project or a faculty/student distinction. The final three bits applied to all other users.

> 一个安全问题是允许文件系统用户控制对其文件的访问权限。Unix 文件系统使用 9 位来控制对文件的什么样的访问权限。文件的所有者有三位，独立控制读取访问权限、写入访问权限和执行访问权限。对于一个普通文本文件，所有者通常允许读写，除非文件是可执行程序或 shell 脚本，否则不允许执行。还有三位用于所有者的组，可能是部门、项目或教职工/学生的区分。最后三位适用于所有其他用户。

This mechanism was substantially simpler than what Multics had provided, but it has served well for a long time. For example, standard commands like editors, compilers, shells, and so on, are owned by a privileged account, typically the root user, which can read, write and execute them at will, but ordinary users can only execute (and perhaps read) but not write them. Note that it is possible to execute a program without being able to read its contents; in that way, the program can safely contain protected information.

> 这种机制比 Multics 提供的要简单得多，但它已经很长时间服务得很好了。例如，标准命令，如编辑器、编译器、shell 等，都由特权账户拥有，通常是 root 用户，它可以随意读取、写入和执行它们，但普通用户只能执行(也许还可以读取)，而不能写入它们。请注意，可以在不能读取其内容的情况下执行程序；以这种方式，程序可以安全地包含受保护的信息。

One early refinement was a 10th permission bit, called the _setuid_ (set user id) bit, for each file. When this bit is set, and the file is executed as a program, the user id for checking permissions is not the person running the program but the owner of the file. If the bit is set, an ordinary user can run a program with the privileges of the program's owner. This is used for programs that manipulate the file system to create directories, rename files, and so on: programs that execute privileged system calls are owned by a super-user that has unrestricted access. Naturally, setuid programs have to be

> 一个早期的改进是为每个文件设置了第 10 个权限位，称为*setuid*(设置用户 ID)位。当此位被设置时，并且文件作为程序执行时，用于检查权限的用户 ID 不是运行程序的人，而是文件的所有者。如果该位被设置，普通用户可以以程序所有者的权限运行程序。这用于操作文件系统以创建目录、重命名文件等程序：执行特权系统调用的程序由具有无限访问权限的超级用户拥有。当然，setuid 程序必须被严格控制。

[]{#index_split_001.html#p139}CHAPTER 5: SEVENTH EDITION

125

carefully written and managed; if not, they can open large holes in system security. Setuid was invented by Dennis Ritchie, who received a patent for it in 1979.

> 经过仔细编写和管理；如果没有，它们可能会在系统安全中开辟出大洞。Setuid 由丹尼斯·里奇发明，他在 1979 年获得了专利。

As mentioned earlier, the idea of passwords originated with CTSS and was followed through in Multics and then into Unix. A text file called

> 按照之前提到的，密码的想法起源于 CTSS，并在 Multics 中得到延续，然后又进入了 Unix。一个叫做

_/etc/passwd_ contains one line for each user, with login name, user id number, password, and a few other fields. From earliest times, the password was stored in a hashed form, not in the clear. Hashing is a form of scrambling for which the only practical way to recreate the original is to try all possible passwords. This meant that anyone can read the password file but can't use the hashed passwords to login as someone else.

> `/etc/passwd` 包含每个用户的一行，包括登录名、用户 ID 号、密码和其他一些字段。从最早的时候，密码就以哈希形式存储，而不是明文形式。哈希是一种扰乱形式，重建原始形式的唯一实用方法是尝试所有可能的密码。这意味着任何人都可以读取密码文件，但不能使用哈希密码以其他人的身份登录。

That's the theory. If the hashing isn't good or if people choose passwords poorly, howev er, decryption may be possible. Ken and Bob Morris collected password files from a variety of Unix systems and experimented with dictionary attacks, trying plausible passwords to see if they hashed to what was stored in the password file. Their studies in the mid 1970s showed that 10 to 30 percent of passwords could be obtained this way.

> 那就是理论。但是，如果散列不好或者人们选择密码不当，解密就有可能成功。肯和鲍勃·莫里斯从各种 Unix 系统收集了密码文件，并尝试用字典攻击，试图猜测合理的密码，看它们是否与存储在密码文件中的内容相匹配。他们在 20 世纪 70 年代中期的研究表明，有 10%到 30%的密码可以通过这种方式获得。

Dictionary attacks are still effective, though the technology on all sides is more sophisticated. One would hope that today's users are more aware of the perils of weak passwords, but recent lists of frequently used passwords suggest that they are not. (As an aside, this attack was also used in the Morris Worm of 1998, when Robert T. Morris, son of Bob, inadvertently released a program that tried to log in to Unix systems on the Internet and propagate itself. One of its mechanisms was to use a dictionary of likely passwords, like "password" and "12345.")

> 字典攻击仍然有效，尽管双方的技术都更加复杂。人们希望今天的用户更加意识到弱口令的危险，但最近流行的密码清单表明他们并没有。(顺便说一句，1998 年的莫里斯蠕虫也使用了这种攻击，当时罗伯特·T·莫里斯(Bob 的儿子)无意中发布了一个程序，试图登录互联网上的 Unix 系统并传播自身。其中一种机制是使用可能的密码字典，比如“password”和“12345”。)

Bob wrote the original Unix crypt command. He retired from Bell Labs in 1986, to become the chief scientist at the National Security Agency (NSA), which suggests that he did know a fair amount about computer security and cryptography. He died in 2011 at the age of 78.

> 鲍勃在 1986 年退休，成为国家安全局(NSA)的首席科学家，他为 Unix crypt 命令编写了原始程序，这表明他对计算机安全和密码学有相当多的了解。他于 2011 年去世，享年 78 岁。

Cryptography was an on-going interest of several 1127 members, including Bob, Ken, Dennis, Peter Weinberger and Fred Grampp (Figure 5.19).

> 加密学是 1127 成员中一个持续发展的兴趣，其中包括 Bob、Ken、Dennis、Peter Weinberger 和 Fred Grampp(见图 5.19)。

(Dennis's web page tells some interesting behind-the-scenes stories.) Although encryption today is all done with software, it was done by mechanical devices during the Second World War. The German military used the Enigma machine, and somehow Fred obtained one. One story has it that he bought it on the open market; another says that his father, an American GI, brought it back from Germany after the end of the war. Fred kept it at Bell Labs and when he died left it to Ken Thompson, where it sat in the bottom drawer of Ken's file cabinet, across the hall from me.

> 登尼斯的网页讲述了一些有趣的幕后故事。尽管如今的加密都是通过软件完成的，但在二战期间是由机械设备完成的。德国军队使用了“英格玛”机器，而弗雷德竟然获得了一台。有一个故事说他是在公开市场上买的，另一个故事说他的父亲是美国的 GI，在战争结束后从德国带回来的。弗雷德把它放在贝尔实验室，他去世后把它留给肯·汤普森，它就放在肯的文件柜底层，就在我隔壁。

[]{#index_split_001.html#p140}![](./index-140_1.jpg){.calibre4}

126 CHAPTER 5: SEVENTH EDITION

**Figure 5.19:**

Fred Grampp, ∼1981 (Courtesy of Gerard Holzmann) One day I borrowed it for a class I was teaching at Princeton that included a lecture on cryptography. I asked if anyone had ever seen an Enigma. No, no one had, so I pulled it out from under the table. I hav e never before or since seen such interest from my students, some of whom were literally standing on the table to get a proper look. Ken subsequently donated the Enigma to a museum.

> 弗雷德·格兰普，约 1981 年(由杰拉德·霍尔茨曼提供)有一天，我借来一台用于普林斯顿大学教学的课程，其中包括密码学讲座。我问有没有人见过 Enigma。没有，没有人见过，所以我从桌子底下拿出来。我以前也没有见过我的学生如此感兴趣，其中一些人甚至站在桌子上才能看到。肯后来将 Enigma 捐赠给了一家博物馆。

When Ken and Dennis won the Turing Award in 1983, Ken's prescient talk, "Reflections on Trusting Trust," explained a series of modifications that he could make to a compiler that would eventually install a Trojan horse in the login program for a system.

> 当肯和丹尼斯在 1983 年获得图灵奖时，肯的先见之明的演讲“对信任的反思”解释了一系列他可以对编译器进行的修改，最终会在系统的登录程序中安装一个木马。

"You can't trust code that you did not totally create yourself. (Especially code from companies that employ people like me.) No amount of source-level verification or scrutiny will protect you from using untrusted code."

> 你不能相信你没有完全自己创造的代码。(特别是来自雇用像我这样的人的公司的代码)没有任何源代码验证或审查可以保护你不使用不可信任的代码。

As he noted, the same kinds of tricks can be applied to hardware, where they will be even harder to discover. Things have not gotten better in the interim, and the paper is still highly relevant today.

> 他指出，同样的把戏可以应用于硬件，这些把戏将更加难以发现。情况并没有得到改善，这篇论文今天仍然非常相关。

**Hardware**

Software was the primary activity in 1127, but hardware interests were well represented too. In the early days, it often required hardware expertise

> 软件是 1127 年的主要活动，但硬件也得到了充分体现。早期，它往往需要硬件专业知识。

[]{#index_split_001.html#p141}CHAPTER 5: SEVENTH EDITION

127

to connect odd devices to the PDP-11; examples included the Votrax voice synthesizer, telephone equipment, typesetters, and a variety of network devices. This led over the years to the development of a suite of computer-aided design (CAD) tools, and involved a number of people, like Joe Condon, Lee McMahon, Bart Locanthi, Sandy Fraser, Andrew Hume, and others that I am surely forgetting.

> 为 PDP-11 连接奇特的设备；例如 Votrax 语音合成器、电话设备、排版机和各种网络设备。这随着时间的推移，导致了一套计算机辅助设计(CAD)工具的发展，涉及到许多人，比如乔·孔登(Joe Condon)、李·麦克马洪(Lee McMahon)、巴特·洛坎蒂(Bart Locanthi)、桑迪·弗雷泽(Sandy Fraser)、安德鲁·休姆(Andrew Hume)等，还有我肯定忘记的其他人。

Bart used the CAD tools to design and build a bitmap terminal in the early 1980s. At the time most terminals could only display 24 rows of 80 fixed width and fixed height ASCII characters. By contrast, a bitmap terminal displayed a large array of pixels, each of which could be independently set to a value, like the screens of all laptops and cell phones today, though the first bitmap displays were monochrome. Bart originally called his bitmap terminal the Jerq, an oblique reference to a somewhat analogous device called Perq offered by a Pittsburgh company named Three Rivers.

> 巴特在 80 年代初期使用 CAD 工具设计和制造了一个位图终端。当时，大多数终端只能显示 24 行 80 个固定宽度和高度的 ASCII 字符。相比之下，位图终端显示了一个大的像素数组，每个像素都可以被单独设置一个值，就像今天所有笔记本电脑和手机屏幕一样，尽管第一个位图显示器是单色的。巴特最初称他的位图终端为 Jerq，这是一个含糊的参照，它类似于由匹兹堡的 Three Rivers 公司提供的一种叫做 Perq 的设备。

The Jerq started life with a Motorola 68000 processor, which was popular at the time (it was often used in workstations, for example), but both the name and the implementation fell victim to corporate politics. The Jerq was renamed the Blit (after the bitblit operation for rapidly updating screen contents) but was made only in small quantities. Western Electric, still the manufacturing arm of AT&T, redesigned it to use a Bellmac 32000, a processor chip designed by Bell Labs and manufactured by Western Electric. "Blit"

> Jerq 最初使用的是当时很流行的 Motorola 68000 处理器(它经常用于工作站)，但这个名字和实现都成为了公司政治的牺牲品。Jerq 被改名为 Blit(取自用于快速更新屏幕内容的 Bitblit 操作)，但只生产少量。AT&T 仍然是制造部门的西电，将其重新设计为使用 Bellmac 32000 处理器芯片，这是由贝尔实验室设计，由西电制造的。"Blit"

was replaced by the catchy "DMD-5620." The redesign cost a full year and AT&T lost whatever chance it might have had to compete in the growing workstation marketplace.

> 被有趣的“DMD-5620”取代了。重新设计花费了整整一年，AT&T 失去了可能参与快速增长的工作站市场的机会。

Rob Pike wrote most of the operating system for the Blit and the 5620.

Its most novel aspect was that computation could proceed in multiple over-lapping windows. Overlapping windows had been seen before, but only one of them could be active at a time. Rob got a patent on the improvement.

> 它最新颖的方面是可以在多个重叠窗口中进行计算。以前也见过重叠窗口，但一次只能激活其中一个。罗布获得了对这项改进的专利。

The 5620 was a good graphics terminal, though physically heavy and bulky. I used it to write graphical programs such as a Troff previewer. It was also the environment in which Rob Pike wrote a series of mouse-based text editors, one of which I use by preference even today: this book was written with Sam.

> 5620 是一款不错的图形终端，尽管它体积庞大而重量沉重。我用它来编写图形程序，比如 Troff 预览器。它也是 Rob Pike 编写一系列基于鼠标的文本编辑器的环境，其中我今天仍然有首选：本书是用 Sam 写的。

There was also a sustained interest in integrated circuits and VLSI (Very Large Scale Integration). In 1980, Center 1127 offered a three-week crash course in integrated circuit design taught by Carver Mead of Caltech. Lynn Conway and Carver had literally written the book ( _Introduction to VLSI Systems_, 1980) on how to design and implement integrated circuit chips, and their course had already been given at a number of universities. Carver had a gift for telling a carefully calibrated sequence of lies about how circuits

> 也有人对集成电路和 VLSI(大规模集成)保持持续的兴趣。 1980 年，中心 1127 提供了由加州理工学院的卡弗·米德(Carver Mead)教授的三周集成电路设计简短课程。 林恩·康威(Lynn Conway)和卡弗(Carver)几乎写了一本书(《VLSI 系统入门》，1980)，讲述如何设计和实现集成电路芯片，他们的课程已经在许多大学上授课。 卡弗(Carver)有一种讲述一系列精心校准的谎言的天赋，关于电路如何运作

[]{#index_split_001.html#p142}128 CHAPTER 5: SEVENTH EDITION

worked. The simplest version was that when a red line crossed over a green line, that made a transistor. Of course this gross over-simplification was unmasked, to be replaced by another more sophisticated lie, which in turn would be further refined.

> 当红线穿过绿线时，就可以制造出晶体管。当然，这种简单的概念被揭示出来，取而代之的是更加复杂的谎言，而这又将得到进一步的改进。

As a result of this excellent instruction, everyone in Carver's class was able to design and build some kind of experimental chip after a couple of weeks of training. The chips were fabricated at the Bell Labs plant in Allen-town, Pennsylvania, and returned for experimentation. At the time, Bell Labs was using state of the art 3.5 micron technology; today's circuits are usually 7 to 10 nanometers, an improvement of at least 300 in line widths, and thus about 100,000 in the number of devices in a given area.

> 结果，在几周的培训之后，卡弗班上的每个人都能够设计并建造一些实验芯片。这些芯片在宾夕法尼亚州艾伦敦的贝尔实验室工厂制造，然后返回进行实验。当时，贝尔实验室使用最先进的 3.5 微米技术；今天的电路通常为 7 到 10 纳米，线宽改善了至少 300，因此在给定区域内的器件数量约为 10 万。

My chip, a simple chess clock, never worked, thanks to a grievous logic error that was obvious in retrospect. Several people developed support tools as well as their own chips. My contribution was a program to help route on-chip wiring, so it was a productive few weeks in spite of my failure as a chip designer.

> 我的芯片，一个简单的国际象棋计时器，从来没有起作用，这要归咎于一个明显的逻辑错误，回想起来令人悲伤。几个人开发了支持工具以及他们自己的芯片。我的贡献是一个帮助路由片上布线的程序，因此尽管我作为一个芯片设计师失败了，但这几周还是很有成效的。

Over the years, at least half a dozen people in my department did VLSI in one form or another---algorithms for checking layouts, simulators, reverse-engineering, and some theoretical research. I could keep up with what they were doing, barely, thanks to Carver's course.

> 这些年来，我部门至少有半打人从事 VLSI，以某种形式或另一种形式，比如布局检查算法，模拟器，反向工程，以及一些理论研究。多亏卡弗的课程，我勉强能跟上他们的工作。

The Center's interest in VLSI persisted for a long time, ultimately leading to Dave Ditzel and Rae McLellan's CRISP (C Reduced Instruction Set Processor) microprocessor, which was one of the earliest RISC processors.

> 中心对 VLSI 的兴趣一直持续很长时间，最终导致大卫·迪泽尔和雷·麦克莱兰的 CRISP(C 减少的指令集处理器)微处理器，这是最早的 RISC 处理器之一。

"RISC" is an acronym for Reduced Instruction Set Computer, a way to design processor architectures that are simpler and more regular than ones like the VAX-11/780.

> “RISC”是“Reduced Instruction Set Computer”的缩写，这是一种设计处理器架构的方式，比像 VAX-11/780 这样的架构更简单、更规则。

CRISP aimed at an instruction set that would be well suited for the output of a C compiler. To design it, Dave worked closely with Steve Johnson.

> CRISP 旨在设计一组适合 C 编译器输出的指令集，为此 Dave 与 Steve Johnson 密切合作。

After discussing potential architecture features, Steve would modify the Portable C compiler and run benchmarks to see what effect these features would have on performance, a great example of hardware/software co-design.

> 在讨论潜在的架构特性后，史蒂夫将修改便携式 C 编译器并运行基准测试，以查看这些特性对性能的影响，这是硬件/软件协同设计的一个很好的例子。

AT&T eventually sold a version of CRISP under the name Hobbit. It was intended for the Apple Newton, one of the first personal digital assistants, but neither Newton or Hobbit was a commercial success. Dave left Bell Labs in 1995 to found Transmeta, which focused on low-power processors.

> AT&T 最终以 Hobbit 的名字出售了 CRISP 的一个版本。它旨在为 Apple Newton(最早的个人数字助理之一)使用，但 Newton 或 Hobbit 都没有取得商业上的成功。1995 年，Dave 离开了贝尔实验室，创立了专注于低功耗处理器的 Transmeta。

Even though CRISP itself did not succeed commercially, Unix and C had a large impact on computing hardware in the 1980s and 1990s. Most successful instruction set architectures were well-matched to C and Unix. Not only did Unix and C portability enable universities and especially companies

> 即使 CRISP 本身没有在商业上取得成功，Unix 和 C 在 1980 年代和 1990 年代对计算机硬件产生了重大影响。大多数成功的指令集架构都与 C 和 Unix 非常匹配。Unix 和 C 的可移植性不仅使大学，特别是公司得以实现。

[]{#index_split_001.html#p143}CHAPTER 5: SEVENTH EDITION

129

to create new architectures and rapidly port software, but it had the effect of requiring that the instruction set was good for C code, while tending to eliminate features that were hard to compile from C programs. CPU design methodology like that used by Johnson and Ditzel used statistical analysis of programs, so C code statistics tended to favor things that made C fast. Unix and C had a critical mass that caused CPU design in the 1980s and 1990s to orbit around them; nobody was successfully building CPUs tuned for other languages.

> 为了创建新的架构并快速移植软件，但它产生了一个效果，即指令集必须适合 C 代码，同时倾向于消除难以从 C 程序编译的功能。像 Johnson 和 Ditzel 所使用的 CPU 设计方法，使用程序的统计分析，因此 C 代码统计趋势偏向于使 C 代码快速运行的东西。Unix 和 C 具有关键质量，导致 1980 年代和 1990 年代的 CPU 设计围绕它们运行；没有人成功地构建针对其他语言调整的 CPU。

[]{#index_split_001.html#p144} []{#index_split_001.html#p145}Chapter 6

**Beyond Research**

"The Unix operating system presently is used at 1400 universities and colleges around the world. It is the basis for 70 computer lines covering the microcomputer to supercomputer spectrum; there are on the order of 100,000 Unix systems now in operation, and approximately 100 companies are developing applications based on it."

> Unix 操作系统目前在全世界 1400 所大学和学院使用。它是 70 种计算机线路的基础，涵盖了微机到超级计算机的范围；目前有大约 100,000 台 Unix 系统在运行，大约有 100 家公司正在开发基于它的应用程序。

R. L. Martin, _Unix System Readings and Applications_, Vol. 2, 1984

After a few years in the lab in Center 1127, Unix began to spread, both inside Bell Labs and outside, the latter primarily through universities, which were able to get the source code for the whole system for a nominal "media fee" under a trade secret agreement. This was definitely not "open source": the system could be used only for educational purposes, and licensees could talk only to other licensed users about their experience and what they were doing with Unix. Nevertheless, the community grew rapidly, user groups sprang up all over the world, and major technical innovations took place, for example ports of the system to different kinds of hardware and new mechanisms for accessing the Internet.

> 几年后，Unix 开始在 Bell Labs 内部和外部传播，后者主要是通过大学，他们可以以微不足道的“媒体费”根据保密协议获得整个系统的源代码。这绝不是“开源”：系统只能用于教育目的，许可使用者只能与其他许可使用者讨论他们的经历以及他们正在使用 Unix 做什么。尽管如此，社区迅速扩大，用户组在世界各地涌现，并发生了重大技术创新，例如将系统移植到不同类型的硬件和新的访问互联网的机制。

Bear in mind that many of the activities described in this chapter were going on in parallel with, or even years before, those of the previous chapter.

> 请记住，本章中描述的许多活动与前一章中的活动并行进行，甚至可能比前一章中的活动早几年。

This can make the chronology a bit confusing.

**6.1 Programmer's Workbench**

The patent department at Bell Labs was the first "customer" outside of the research area, but other groups found Unix useful as well, and the system started early to spread within Bell Labs development groups and other parts of AT&T.

> 美国贝尔实验室的专利部门是研究领域之外的第一个“客户”，但是其他组织也发现 Unix 很有用，系统很早就开始在贝尔实验室的开发组和 AT&T 的其他部门传播开来。

[]{#index_split_001.html#p146}132 CHAPTER 6: BEYOND RESEARCH

With over a million employees, AT&T was a very big company, with many computer systems for managing the data and operations that supported telephone services. These systems provided technician interfaces and support for AT&T, keeping track of equipment and customers, monitoring systems in the field, logging events, trouble-shooting, and the like. Collectively, these systems were called "operations support systems."

> AT&T 拥有超过一百万名员工，是一家非常大的公司，拥有许多电脑系统来管理支持电话服务的数据和操作。这些系统为 AT&T 提供技术接口和支持，跟踪设备和客户，监控现场系统，记录事件，故障排除等等。这些系统被统称为“运营支持系统”。

One of the first major Unix installations outside of Research was a group based in Piscataway, New Jersey, about 15 miles from Murray Hill, that in 1973 began to dev elop tools for programmers who did software development for large-scale production environments. The collection became known as the Programmer's Workbench or PWB.

> 一个首先在研究之外安装 Unix 的重要集群位于新泽西皮斯卡塔威，距离默里山大约 15 英里。1973 年，该集群开始为开发大型生产环境软件的程序员开发工具。这个集合被称为程序员工作台(PWB)。

Most operations support systems at AT&T ran on large mainframe computers from IBM and Univac that had their own proprietary operating systems, such as IBM's OS/360. PWB provided facilities for creating and managing the software that ran on such computers. In effect, PWB Unix served as a uniform front end for a diverse set of large non-Unix computer systems; the mainframes were treated like peripheral devices.

> 大多数 AT&T 的运营支持系统都运行在 IBM 和 Univac 的大型主机计算机上，它们拥有自己的专有操作系统，例如 IBM 的 OS/360。PWB 提供了创建和管理在这些计算机上运行的软件的设施。实际上，PWB Unix 作为一种多样的大型非 Unix 计算机系统的统一前端；主机被视为外围设备。

One major PWB service was remote job entry, a set of commands for sending jobs to target systems and returning the results, including job queue-ing, status reports, notifications, logging and error recovery. Remote job entry fit well with the Unix approach of using small tools that could be connected in a variety of ways, and then encapsulated in shell scripts for convenient use by non-experts.

> 一项主要的 PWB 服务是远程作业输入，这是一组用于将作业发送到目标系统并返回结果的命令，包括作业队列、状态报告、通知、日志记录和错误恢复。远程作业输入与 Unix 的小工具方法很好地结合在一起，可以以各种方式连接，然后用 shell 脚本封装，便于非专家使用。

To support this kind of programming, John Mashey (Figure 6.1) enhanced the 6th edition shell to create the PWB shell, which provided much better programmability, including a general _if-then-else_ for decision-making, a _while_ for looping, and shell variables for storing text. He also invented a search path mechanism, so that by setting a particular shell variable, any user could specify a sequence of directories to be searched for commands. The search path made it easy for groups of users to collect programs in project directories, rather than having to install commands in system directories for which they might not even hav e permission. As John said,

> 为了支持这种编程，约翰·马希(图 6.1)增强了第六版 shell，创建了 PWB shell，它提供了更好的可编程性，包括用于决策的通用 if-then-else、用于循环的 while，以及用于存储文本的 shell 变量。他还发明了一种搜索路径机制，因此，通过设置特定的 shell 变量，任何用户都可以指定要搜索命令的目录序列。搜索路径使得用户组可以轻松地将程序收集到项目目录中，而不必将命令安装在他们可能没有权限的系统目录中。正如约翰所说，

"We had a large (1,000+) population of users who were not usually C

programmers, who worked in groups in shared environments. They wanted to share their own sets of commands by lab, department, group. They often shared systems with others and none could be super-users."

> 程序员们在共享环境中团队合作。他们希望可以按实验室、部门和小组来共享自己的命令集。他们经常与其他人共享系统，没有人可以成为超级用户。

John also added a mechanism so that if a file was marked executable, it would either be executed as a regular command, or passed to a shell if it was

> 約翰還加入了一個機制，如果一個文件被標記為可執行，它將被作為一個普通命令執行，或者如果是一個 shell，則傳遞給該 shell。

[]{#index_split_001.html#p147}![](./index-147_1.jpg){.calibre4}

CHAPTER 6: BEYOND RESEARCH

133

a script. All of these features were in place by early 1975, and refined over the next year as more and more people began using the PWB shell. John's paper "Using a Command Language as a High-Level Programming Language" reported on experience with over 1,700 shell procedures:

> 1975 年初，这些功能就已经实现，随着越来越多的人开始使用 PWB shell，在接下来的一年里，它们也得到了完善。约翰的论文“使用命令语言作为高级编程语言”报告了超过 1700 个 shell 程序的经验。

"By utilizing the shell as a programming language, PWB users have been able to eliminate a great deal of the programming drudgery that often accompanies a large project. Many manual procedures have been quickly, cheaply, and conveniently automated. Because it is so easy to create and use shell procedures, each separate project has tended to customize the general PWB environment into one tailored to its own requirements, organizational structure, and terminology."

> 通过将 Shell 作为编程语言，PWB 用户已经能够消除大型项目中经常伴随的编程苦差事。许多手动程序已经被快速、廉价和方便地自动化。由于创建和使用 Shell 程序非常容易，因此每个单独的项目都倾向于将通用的 PWB 环境定制为适合自己要求、组织结构和术语的环境。

As noted in the previous chapter, John's improvements soon found their way back into the shell that Steve Bourne wrote.

> 正如前一章所指出的，约翰的改进很快就回到史蒂夫·伯恩编写的壳中。

**Figure 6.1:**

John Mashey, ∼2011 (Courtesy of Twitter) Another important PWB product was the Source Code Control System (SCCS), which was written in 1972 by Marc Rochkind. SCCS was the first of a sequence of programs for managing large code bases that were being worked on by several programmers at the same time.

> 约翰·马希，约 2011 年(特别感谢 Twitter)PWB 另一个重要的产品是源代码控制系统(SCCS)，这是由马克·罗希金德在 1972 年编写的。 SCCS 是管理大型代码库的程序序列的第一个，这些代码库由几个程序员同时工作。

The basic idea of SCCS was to let programmers check out part of the code base to work on; this locked that part so other programmers couldn't change it until the lock holder unlocked it. This prevented multiple programmers from making inconsistent changes to the same piece of code at the same time. Of course there were still problems; for example carelessness or crashes could leave code locked even though no one was working on it, and if the locked regions were too big, that slowed down simultaneous changes.

> 基本的 SCCS 想法是让程序员可以检出代码库的一部分来进行工作；这会锁定该部分，直到锁定者解锁，其他程序员就不能改变它。这样可以防止多个程序员在同一段代码上同时做出不一致的更改。当然，仍然存在问题；例如粗心或崩溃可能会导致代码被锁定，即使没有人在工作，而且如果锁定的区域太大，也会减慢同时的更改。

But the idea was crucial for software development that involved multiple

[]{#index_split_001.html#p148}134 CHAPTER 6: BEYOND RESEARCH

people working on the same code base, and it's even more important today with larger code bases spread across much larger developer communities that are more geographically dispersed. There's a clear evolutionary path from SCCS through RCS, CVS and Subversion, to Git, today's default standard version-control system.

> 人们在同一个代码库上工作，今天，随着更大的代码库分布在更大的地理分散的开发者社区，这一点变得更加重要。从 SCCS 到 RCS、CVS 和 Subversion，到 Git，今天的默认标准版本控制系统，有一条明确的进化路径。

Marc Rochkind also invented a tool that converted a set of regular expressions into a C program that would scan logs for occurrences of the patterns and print messages when one was found. This was such a neat idea that Al Aho, Peter Weinberger and I stole

> 马克·罗希金德(Marc Rochkind)还发明了一种工具，它可以将一组正则表达式转换成一个 C 程序，用于扫描日志以查找模式的出现，并在发现模式时打印消息。阿尔·阿霍(Al Aho)、彼得·温伯格(Peter Weinberger)和我都被这个好主意所吸引，窃取了它。

−−− adapted and generalized it for the pattern-action model used in Awk.

PWB also included a collection of tools called the Writer's Workbench (WWB) that tried to help people to write better. John Mashey and Dale Smith, with encouragement from Ted Dolotta, created a set of generic Troff commands, the Memorandum Macro or mm package, that was widely used both inside AT&T and outside for producing documentation.

> PWB 还包括一组工具，称为作家的工作台(WWB)，试图帮助人们更好地写作。约翰·马什伊和戴尔·史密斯在 Ted Dolotta 的鼓励下创建了一组通用 Troff 命令，称为备忘录宏(Memorandum Macro)或 mm 包，它在 AT＆T 内外都被广泛使用，用于生成文档。

In addition, WWB offered a spell checker and programs for finding punctuation mistakes, split infinitives, and double words (often the result of errors made while editing). There were tools for checking grammar and style, and for assessing readability. The core component was a program called _parts_, by Lorinda Cherry. It assigned parts of speech to the words of a text, and although imperfect, it yielded statistics on the frequency of adjectives, com-pound sentences, and the like. WWB was dev eloped in the late 1970s, just about the time when computers were being more frequently used by writers, and WWB got some good press, including an appearance on national TV on NBC's _Today_ show for two of its creators, Lorinda and Nina McDonald.

> 除此之外，WWB 还提供了拼写检查器和查找标点错误、分裂不定式和双词(通常是编辑时犯的错误所导致的)的程序。有检查语法和文体的工具，以及可读性评估的工具。核心组件是一个叫做*parts*的程序，由 Lorinda Cherry 开发。它为文本中的单词分配词性，尽管不完美，但可以得到有关形容词、复合句等的统计数据。WWB 是在 20 世纪 70 年代末开发的，恰好是计算机被作家更多地使用的时候，WWB 受到了一些好评，包括 NBC 的《今日》节目上 Lorinda 和 Nina McDonald 的登场。

As an example of how computing hardware has become cheaper and more powerful over the years, a 1978 PWB paper by Ted Dolotta and Mashey described the development environment, which supported over a thousand users: "By most measures, it is the largest known Unix installation in the world." It ran on a network of 7 PDP-11's with a _total_ of 3.3 megabytes of primary memory and 2 gigabytes of disk. That's about one thousandth of a typical laptop of today. Would your laptop support a population of a million users?

> 随着计算硬件越来越便宜和强大，1978 年 Ted Dolotta 和 Mashey 发表的 PWB 论文为例，描述了一个支持超过一千用户的开发环境：“按照大多数标准来衡量，这是世界上最大的 Unix 安装。”它运行在 7 台 PDP-11 上，总共有 3.3 兆主存储器和 2 千兆磁盘。这相当于今天的一台笔记本电脑的千分之一。你的笔记本电脑能支持一百万用户吗？

**6.2 University licenses**

In 1973, AT&T began licensing Unix to universities for a nominal fee, though most licenses were for the 6th edition, which became available in 1975. There were some commercial 6th edition licenses as well, but these cost \$20,000, which would be more like \$100,000 today. Licenses did

> 1973 年，AT&T 开始以微不足道的费用向大学许可 Unix，尽管大多数许可证是为 1975 年可用的第六版。也有一些商业第六版许可证，但这些费用是 2 万美元，如今相当于 10 万美元。许可证也有一些限制。

[]{#index_split_001.html#p149}CHAPTER 6: BEYOND RESEARCH

135

include all the source code, but came with no support whatsoever.

One of the most active license recipients was the University of California at Berkeley (UCB), where a number of graduate students made major contributions to the system that eventually became the Berkeley Software Distribution (BSD), one of two main branches that evolved from the original Research Unix.

> 一个最活跃的许可证接收者是加利福尼亚大学伯克利分校(UCB)，那里的许多研究生为最终成为伯克利软件分发(BSD)的系统做出了重大贡献，这是从原始研究 Unix 演变而来的两个主要分支之一。

Ken Thompson spent a sabbatical year at Berkeley in 1975 and 1976, where he taught courses on operating systems. Bill Joy (Figure 6.2), a grad student at the time, modified the local version of Unix, and added some programs of his own, including the vi text editor, which is still one of the most popular Unix editors, and the C shell csh. Bill later designed the TCP/IP

> Ken Thompson 在 1975 年和 1976 年期間在加州大學度過了一年的休假，在那裡他開設了關於操作系統的課程。當時的研究生比爾·喬伊(圖 6.2)修改了當地版本的 Unix，並添加了一些自己的程序，包括 vi 文本編輯器，它仍然是最受歡迎的 Unix 編輯器之一，以及 C shell csh。比爾後來設計了 TCP / IP。

networking interface for Unix that is still used today. His socket interface made it possible to read and write network connections with the same read and write system calls as were used for file and device I/O, so it was easy to add networking functionality.

> Unix 的网络接口今天仍在使用。他的套接字接口使得可以使用与文件和设备 I/O 相同的读写系统调用来读写网络连接，因此添加网络功能变得很容易。

Bill occasionally visited Bell Labs during the mid to late 1970s. I remember one evening when he showed me the new text editor that he was working on. By this time, video display terminals had replaced paper terminals like Teletypes, and they enabled a much more interactive style of editing.

> 比尔在 1970 年代中期至晚期偶尔会拜访贝尔实验室。我记得有一个晚上，他给我展示了他正在开发的新文本编辑器。到这个时候，视频显示终端已经取代了像电传打字机这样的纸质终端，它们可以实现更加交互式的编辑方式。

In ed and other editors of the time, one typed commands that modified the text being edited, but they did not continuously display the text; instead, if an editing command changed some text, it was necessary to explicitly print the new line. In ed, one might say

> 在当时的 ed 和其他编辑器中，人们输入命令来修改正在编辑的文本，但它们不会持续显示文本；相反，如果编辑命令改变了一些文本，就必须明确打印新行。在 ed 中，可以说

s/this/that/p

to substitute this into that in the current line and print the result. Other commands made it possible to change occurrences in multiple lines, search for lines, display ranges of lines, and so on. In the hands of experts, ed was very efficient, but not intuitive for newcomers.

> 将此替换为当前行中的那个并打印结果。其他命令使得更改多行中的出现情况成为可能，搜索行，显示行范围等等。在专家的手中，ed 非常有效，但对新手来说不直观。

Bill's editor used cursor addressing to update the screen as text was being edited. This was a major change from the line-at-a-time model: one moved the cursor to this (perhaps by using a regular expression), typed a command like cw ("change word"), and then typed that, which immediately replaced the original.

> 比尔的编辑器使用光标定位来更新屏幕，随着文本被编辑。这是一个重大的变化，从一次一行的模型：一个移动光标到这个(也许通过使用正则表达式)，输入一个命令，如 cw(“改变单词”)，然后输入，这将立即替换原来的内容。

I don't recall what I said at the time about the editor itself (though today vi is one of the two editors that I use most often), but I do remember telling Bill that he should stop fooling around with editors and finish his PhD. Fortunately for him and for many others, he ignored my advice. A few years later, he dropped out of graduate school to co-found Sun Microsystems, one of the first workstation companies, with software based on Berkeley Unix,

> 我不记得当时我关于编辑器本身说了什么(尽管今天 vi 是我最常用的两个编辑器之一)，但我记得告诉比尔他不应该再玩编辑器了，而应该完成他的士学位。幸运的是，他没有听从我的建议。几年后，他从研究生院退学，与另一位创立了 Sun Microsystems，这是第一家基于 Berkeley Unix 的工作站公司，软件也是基于 Berkeley Unix 的。

[]{#index_split_001.html#p150}![](./index-150_1.jpg){.calibre4}

136 CHAPTER 6: BEYOND RESEARCH

including his fundamental work on the system, networking and tools (and his vi editor). I often cite this story when students ask me for career advice---

> 他对系统、网络和工具(以及他的 vi 编辑器)的基础工作，我经常在学生向我寻求职业建议时引用这个故事。

older is not always wiser.

**Figure 6.2:**

Bill Joy, ∼1980 (Courtesy of Bill Joy)

**6.3 User groups and Usenix**

Since AT&T offered no support at all to Unix licensees, users were forced to band together to help each other, in what eventually became regular meet-ings with technical presentations, software exchanges, and of course social activities. This idea was certainly not original with Unix; the SHARE user

> 由于 AT&T 完全没有提供对 Unix 许可证持有者的支持，用户被迫联合起来互相帮助，最终形成了定期会议，技术展示，软件交换以及当然的社交活动。这个想法肯定不是 Unix 的原创；SHARE 用户早就这样做了。

[]{#index_split_001.html#p151}CHAPTER 6: BEYOND RESEARCH

137

group for IBM systems was established in 1955 and is still active, and there were user groups for other hardware manufacturers as well.

> 1955 年建立了 IBM 系统小组，至今仍在活跃，其他硬件制造商也有用户组。

The first Unix user group meeting was held in New York in 1974, and user groups gradually sprang up all over the world. In 1979, Ken and I attended the first meeting of the UKUUG, which was held at the University of Kent in Canterbury. It was quite an experience for me, the first time I had visited England. Ken and I flew to Gatwick Airport on Laker Airways, the first of the cheap trans-Atlantic airlines. We drove to Salisbury and visited the cathedral and Stonehenge, then went on to Canterbury for the meeting (and to visit the cathedral). Afterwards I spent a few days in London as a wide-eyed tourist.

> 1974 年，第一次 Unix 用户组会议在纽约举行，用户组逐渐在世界各地涌现出来。1979 年，肯和我参加了英国 Unix 用户组(UKUUG)在坎特伯雷大学举行的首次会议。这对我来说是一次很特别的经历，也是我第一次访问英国。肯和我乘坐莱克航空(Laker Airways)飞往盖特威克机场，这是第一家廉价的跨大西洋航空公司。我们去索尔兹伯里参观大教堂和巨石阵，然后去坎特伯雷参加会议(还参观了大教堂)。之后我在伦敦作为一个睁大眼睛的游客呆了几天。

I hav e since visited several other countries, using Unix user group meet-ings as an excuse and a great way to meet some very nice people. The most memorable was a trip to Australia in 1984, again with Ken, where the meeting was held in the Sydney Opera House. I gav e a talk on the morning of the first day, then spent the rest of the week watching the harbor from a window of the conference room; it was so fascinating that I have no memory of any of the other talks.

> 我以后又去了几个国家，以参加 Unix 用户组会议为借口，也是一个很好的机会认识一些很好的人。最令人难忘的是 1984 年和肯一起去澳大利亚的旅行，会议在悉尼歌剧院举行。第一天早上我做了一个演讲，然后整个星期都在会议室的窗户看着海港，太迷人了，以至于我对其他演讲没有任何记忆。

The user groups evolved into an umbrella organization called "Unix User Groups," which was renamed USENIX (Usenix from now on) after AT&T

> 用户组演变成一个名为“Unix 用户组”的伞形组织，在 AT&T 之后改名为 USENIX(从现在起称为 USENIX)。

complained about mis-use of the Unix trademark. Usenix now runs an extensive series of professional conferences and publishes a technical journal called ";login:". Usenix played a significant role in spreading Unix, with conference presentations and tutorials on many subjects. It also distributed UUCP and ran the Usenet news system.

> 用户组投诉 Unix 商标被滥用。Usenix 现在举办了一系列专业会议，并出版一份名为“login：”的技术期刊。Usenix 在传播 Unix 方面发挥了重要作用，举办会议和关于许多主题的教程。它还分发 UUCP，并运行 Usenet 新闻系统。

**6.4 John Lions' Commentary**

John Lions (Figure 6.3), a professor of computer science at the University of New South Wales in Sydney, was an enthusiastic early adopter of Unix, and used it extensively in courses on operating systems as well as for general educational and research support at UNSW.

> 约翰·狮子(图 6.3)，悉尼新南威尔士大学计算机科学教授，是 Unix 的热心早期采用者，并在操作系统课程以及新南大学的教育和研究支持中大量使用它。

In 1977, John wrote a line-by-line "commentary" on the 6th edition source code. Every part of the source code was explained in detail, so one could see how it worked, why it was the way it was, and how it might be done differently. John also produced a number of excellent students, several of whom wound up at Bell Labs.

> 1977 年，约翰对第六版源代码进行了逐行“评论”。源代码的每个部分都被详细解释，因此可以看到它是如何工作的，为什么是这样，以及可以如何改进。约翰还培养了许多优秀的学生，其中几个最终在贝尔实验室工作。

In the original printing, the _Commentary_ was in two separate volumes, the code in one volume and the exposition in the other, so that they could be read side by side, though the authorized version (Figure 6.4), which finally

> 在最初的印刷版本中，*Commentary*分为两个单独的卷，一卷是代码，另一卷是说明，这样它们就可以并排阅读，尽管最终授权版本(图 6.4)将两者合并在一起。

[]{#index_split_001.html#p152}![](./index-152_1.jpg){.calibre4}

138 CHAPTER 6: BEYOND RESEARCH

**Figure 6.3:**

John Lions (Courtesy of UNSW)

appeared in 1996, is a single volume.

Although it could be shared among Unix licensees, the book was technically a trade secret since it contained AT&T's proprietary source code.

> 尽管它可以在 Unix 许可用户之间共享，但由于书中包含 AT&T 的专有源代码，它技术上是一个商业机密。

Copies were carefully controlled, at least in theory; I still have my numbered copy (#135). But it was widely copied in the early days; the samizdat imagery on the cover in Figure 6.4 suggests that such copies were made clan-destinely. Years later, reality was acknowledged and John's book was published commercially.

> 复印件被仔细控制，至少在理论上是这样；我仍然有我的编号复印件(#135)。但在早期，它被广泛复制；图 6.4 中封面上的秘密出版形象表明，这些复印件是秘密制作的。多年以后，现实得到认可，约翰的书被商业出版。

John spent a sabbatical year in 1978 at Murray Hill, across the hall from me in the office that later belonged to Dennis Ritchie. John died in 1998 at the age of 62. His contributions have been remembered in a chair of computer science at UNSW. The chair was funded by donations from alumni and friends, including Ted Dolotta's 1998 auction of his California UNIX license plate, bought by John Mashey.

> 約翰在 1978 年的安息日年度在默里山，就在我的辦公室隔壁，後來變成丹尼斯·里奇的辦公室。約翰在 1998 年去世，享年 62 歲。他的貢獻被記住，聯合國大學新南威爾士大學設立了一個計算機科學講座，由校友和朋友捐贈，包括泰德·多洛塔在 1998 年拍賣他的加州 UNIX 許可證牌照，被約翰·馬謝購買。

One comment in the Unix source has become famous, thanks to the Commentary. Line 2238 says

> 一条评论在 Unix 源码中已经出名，多亏了注释。第 2238 行说

/\* You are not expected to understand this. \*/

[]{#index_split_001.html#p153}![](./index-153_1.jpg){.calibre4}

CHAPTER 6: BEYOND RESEARCH

139

**Figure 6.4:**

John Lions' Commentary on 6th Edition Unix As mentioned earlier, Dennis died in October 2011. I used this comment as the core of a tribute to Dennis during a memorial gathering at Bell Labs the following year.

> 约翰·莱恩斯对六版 Unix 的评论
> 正如前面提到的，丹尼斯在 2011 年 10 月去世。我在次年贝尔实验室举行的纪念集会上以此评论作为对丹尼斯的纪念的核心。

The Unix kernel code was jointly written by Dennis and Ken Thompson.

As far as I know, Ken always subscribed fully to the idea that good code doesn't need many comments, so by extrapolation, great code needs none at all; I think that most of the comments in the kernel come from Dennis. The specific comment, which you can find on line 2238, is famous for its dry wit, and it was widely available on t-shirts and the like for years. As Dennis himself said,

> 据我所知，肯总是完全认同好代码不需要多少注释的想法，因此推断出伟大的代码根本不需要注释；我认为内核中的大多数注释都来自丹尼斯。具体的注释可以在 2238 行找到，以其幽默的干练而闻名，多年来一直在 T 恤衫等物品上普及开来。正如丹尼斯自己所说，

"It's often quoted as a slur on the quantity or quality of the comments in the Bell Labs research releases of Unix. Not an unfair observation in general, I fear, but in this case unjustified."

> 这经常被引用来贬低 Bell Labs 研究发布的 Unix 评论的数量或质量。总的来说，我担心这并不是不公平的观察，但在这种情况下是不公正的。

If you go back and look, you can see that the comment comes just after a much longer comment that describes the context-switching mechanism that swaps control between two processes, and it really was trying to explain something difficult. Dennis went on to say,

> 如果你回顾一下，你会发现这条评论是在一条更长的评论之后，该评论描述了一种在两个进程之间切换控制的上下文切换机制，而它确实是在试图解释一些困难的东西。丹尼斯接着说：

" 'You are not expected to understand this' was intended as a remark in

[]{#index_split_001.html#p154}140 CHAPTER 6: BEYOND RESEARCH

the spirit of 'This won't be on the exam,' rather than as an impudent challenge."

> “这不会在考试中出现”这句话的精神，而不是作为一种无礼的挑战。

I mentioned earlier that Nroff and Troff were difficult tools to master. The final paragraph of the acknowledgments section of the Lions _Commentary_ suggests that John would concur:

> 我之前提到 Nroff 和 Troff 是很难掌握的工具。《狮子评论》的致谢部分的最后一段表明约翰也同意这一点：

"The cooperation of the nroff program must also be mentioned. Without it, these notes could never hav e been produced in this form. Howev er it has yielded some of its more enigmatic secrets so reluctantly, that the author's gratitude is indeed mixed. Certainly nroff itself must provide a fertile field for future practitioners of the program documenter's art."

> 需要提及 nroff 程序的合作。没有它，这些笔记不可能以这种形式产生。然而，它把一些更神秘的秘密披露得如此勉强，以至于作者的感激确实是有些混合的。当然，nroff 本身必须为程序文档艺术的未来从业者提供肥沃的领域。

**6.5 Por tability**

The 6th edition of Unix was mostly written in C, with a limited assembly language assist to access machine features that were otherwise not available, for example, setting up registers, memory mapping, and the like. At the same time, Steve Johnson had created a version of the C compiler that was

> 第六版的 Unix 主要是用 C 编写的，有有限的汇编语言协助访问机器功能，否则无法访问，例如设置寄存器、内存映射等。与此同时，Steve Johnson 创建了一个 C 编译器的版本。

"portable" in the sense that it could be straightforwardly retargeted to generate assembly language for architectures other than the PDP-11. This made it possible to move C programs to other kinds of computers merely by recompiling them. The most interesting program to port would obviously be the operating system itself. Would that be feasible?

> 可移植，意思是可以直接重定向以为其他于 PDP-11 架构生成汇编语言。这使得可以通过重新编译将 C 程序移植到其他类型的计算机上。最有趣的程序显然是操作系统本身。这可行吗？

The first port of Unix was done at the University of Wollongong in New South Wales, Australia, by Richard Miller; the target computer was an Interdata 7/32. Miller didn't use the portable C compiler. Instead he bootstrapped his way onto the Interdata by modifying the code generator of Dennis Ritchie's original C compiler. His version of Unix was working and self-sustaining by April 1977.

> 在澳大利亚新南威尔士州的伍伦贡大学，理查德·米勒完成了 Unix 的第一个版本；目标计算机是 Interdata 7/32。米勒没有使用可移植的 C 编译器，而是通过修改丹尼斯·里奇原始 C 编译器的代码生成器，在 Interdata 上引导自己的 Unix 版本。他的 Unix 版本于 1977 年 4 月就已经可以正常运行并自我维护。

Independently, and without knowing of Miller's work, Steve Johnson and Dennis Ritchie ported Unix to a similar machine, the Interdata 8/32. Their goal was somewhat different, a version of Unix that was more portable, rather than a single port of the original as it was. They got their version running late in 1977. Steve Johnson recalls some of the background:

> 独立地，而不知道米勒的工作，史蒂夫·约翰逊和丹尼斯·里奇将 Unix 移植到了类似的机器 Interdata 8/32 上。他们的目标有所不同，他们想要的是一个更具可移植性的 Unix 版本，而不是单一的原始端口。他们在 1977 年晚些时候让他们的版本运行起来。史蒂夫·约翰逊回忆起一些背景：

"There was another pressure to make Unix portable. A number of DEC's competitors were beginning to grumble that regulated AT&T

> 有另一种压力要求 Unix 可移植。许多 DEC 的竞争对手开始抱怨被调控的 AT&T。

had too cozy a relationship with DEC. We pointed out that there were no other machines like the PDP-11 on the market, but this argument

> 我們與 DEC 有太密切的關係。我們指出市場上沒有其他像 PDP-11 這樣的機器，但這個論點

[]{#index_split_001.html#p155}CHAPTER 6: BEYOND RESEARCH

141

was getting weaker. Dennis hooked me into the portability effort with one sentence: 'I think that it would be easier to move Unix to another piece of hardware than to rewrite an application to run under a different operating system.' I was all in from that point on."

> 随着时间的推移，我变得越来越虚弱。丹尼斯用一句话把我拉入可移植性的努力中：“我认为把 Unix 移植到另一块硬件比重写一个应用程序以运行在不同的操作系统下要容易得多。”从那一刻起，我就完全投入了。

Portability was a great step forward. Up to this point, operating systems had mostly been written in assembly language, and even if written in a high-level language were more or less tied to a particular architecture. But after projects like those done by Miller, and Johnson and Ritchie, porting Unix to other kinds of computers, though not trivial, was basically straightforward.

> 可移植性是一个重大的进步。到目前为止，操作系统大多是用汇编语言编写的，即使用高级语言编写，也基本上局限于特定的架构。但是经过米勒，约翰逊和里奇等人的项目，将 Unix 移植到其他类型的计算机虽然不是微不足道的，但基本上是直接的。

This had major implications for the emerging workstation marketplace, where companies both old and new were building computers that were smaller and cheaper than minicomputers like the PDP-11 and the Interdata, and used different processors.

> 这对新兴工作站市场产生了重大影响，老牌公司和新兴公司都在建造比 PDP-11 和 Interdata 等小型计算机更小、更便宜、使用不同处理器的计算机。

Workstations were meant to be personal machines for scientists and engineers, giving them a powerful and normally unshared computing environment. There were many examples of workstations, of which the ones from Sun Microsystems were the most commercially successful. Other manufacturers included Silicon Graphics, DEC, Hewlett-Packard, NeXT and even IBM. The first workstations, in the early 1980s, aimed for a megabyte of primary memory, a meg apixel display, and a speed of one megaflop (a million floating-point operations per second), a so-called "3M" machine. For comparison, my elderly Macbook has 8 gigabytes of memory and a speed of at least a gigaflop; its display is little more than a megapixel, but the pixels are 24-bit color, not monochrome.

> 工作站本来是为科学家和工程师设计的个人机器，为他们提供强大而通常不会共享的计算环境。有许多工作站的例子，其中 Sun Microsystems 的工作站是最成功的商业化产品。其他制造商包括 Silicon Graphics、DEC、Hewlett-Packard、NeXT 甚至 IBM。20 世纪 80 年代初期的第一台工作站，旨在拥有一兆字节的主内存、一百万像素的显示器以及一兆次操作(每秒一百万个浮点运算)的速度，称为“3M”机器。相比之下，我的老式 MacBook 有 8GB 内存，速度至少为千兆次操作；它的显示器不到一百万像素，但是像素是 24 位彩色的，而不是单色的。

The workstation marketplace arose because technological improvements made it possible to pack serious computing horsepower into a small physical package and sell it for a modest price. The complete system price could be reasonable in part because software, including the operating system, was already available. There was no need for new manufacturers to create a new operating system---it was enough to port Unix and its accompanying programs to whatever processor the computer used. The workstation market was thus helped significantly by the availability of Unix.

> 随着技术的进步，将大量计算能力打包成小体积的产品，以适中的价格出售，工作站市场应运而生。系统的总价格也可以合理，因为软件(包括操作系统)已经可用。新制造商不需要创建新的操作系统，只需将 Unix 及其附带程序移植到计算机使用的处理器上即可。因此，Unix 的可用性对工作站市场有很大帮助。

The IBM Personal Computer (PC) first appeared in 1981. The PC and its many clones were typically 5 to 10 times cheaper than a workstation.

> IBM 的个人电脑(PC)首次于 1981 年出现。 PC 及其许多克隆通常比工作站便宜 5 到 10 倍。

Though they were originally not at all competitive in performance, they gradually improved, and by the end of the 1990s were at least as good. Any distinction between workstation and PC eventually blurred. Today, depending on application areas, such machines most often run Microsoft Windows, macOS, or a Unix or Unix-like system.

> 他们最初在性能上根本没有竞争力，但逐渐改善，到 1990 年代末至少和现在一样好。工作站和个人计算机之间的区别最终模糊了。今天，根据应用领域，这些机器通常运行 Microsoft Windows，macOS 或 Unix 或类 Unix 系统。

[]{#index_split_001.html#p156} []{#index_split_001.html#p157}Chapter 7

**Commercialization**

"As Unix spread throughout the academic world, businesses eventually became aware of Unix from their newly hired programmers who had used it in college."

> 随着 Unix 在学术界的传播，企业最终通过他们新雇佣的在大学使用过它的程序员了解到 Unix。

Lucent web site, 2002

"Unix and C are the ultimate computer viruses."

Richard Gabriel, "Worse is Better," 1991

It had been argued that AT&T was prohibited from selling Unix commercially because as a regulated public monopoly, if it did so, it would be competing with other operating system vendors, using revenues from telephone services to cross-subsidize Unix development. The closest that AT&T came to making a real business was to license Unix to corporate customers for \$20,000 (in contrast with the nominal media fee for educational institutions) but in limited quantities and without support. That was enough to head off regulatory scrutiny.

> 据论证，由于 AT&T 作为一个受监管的公共垄断企业，如果它出售 Unix，就会与其他操作系统供应商竞争，利用电话服务的收入来跨补 Unix 开发费用。AT&T 最接近实际商业行为的是向企业客户授权 Unix，价格为 20,000 美元(与教育机构的名义媒体费相比)，但数量有限，没有支持。这足以避免监管审查。

**7.1 Divestiture**

By 1980, AT&T's position as a monopoly, regulated or not, was coming under attack. The US Department of Justice had begun an antitrust lawsuit against AT&T in 1974, on the grounds that AT&T controlled not only telephone service for most of the country but also the equipment used by its telephone companies, and thus that AT&T controlled communications for the whole country. The DoJ proposal was that AT&T should be forced to divest its manufacturing arm, Western Electric, which made the equipment.

> 1980 年，无论受到监管与否，AT&T 作为一家垄断者的地位受到攻击。美国司法部于 1974 年就以 AT&T 控制着大部分国家的电话服务以及其电话公司所使用的设备，因此控制着整个国家的通讯，发起了反垄断诉讼。司法部的提案是强迫 AT&T 剥离其制造部门西方电气(Western Electric)，该部门制造设备。

[]{#index_split_001.html#p158}144 CHAPTER 7: COMMERCIALIZATION

AT&T proposed instead to address the situation by splitting the company into one part (called AT&T) that would provide long distance telephony, and seven regional operating companies ("Baby Bells") that would provide local phone service in their respective geographic areas. AT&T would retain Western Electric but the operating companies would no longer be required to buy equipment from it. AT&T would also keep Bell Labs.

> AT&T 提出了一种解决方案，将公司分成两部分(称为 AT&T)，一部分提供长途电话服务，另一部分由七家地方运营公司(“婴儿贝尔”)提供本地电话服务。AT&T 将保留西屋电气，但运营公司不再需要从其购买设备。AT&T 还将保留贝尔实验室。

The consent decree with the Department of Justice, by which AT&T

divested itself of the operating companies, was finalized early in 1982, and took effect January 1, 1984.

> 1982 年初，脱离运营公司的计划最终敲定，并于 1984 年 1 月 1 日生效。

Divestiture was an enormous upheaval, which in the long run led to mis-fortune for AT&T, and 20 years of subsequent misjudgments and poor business choices made Bell Labs into a shadow of what it had been when its mission was clear and its funding was adequate and stable.

> 放弃是一场巨大的动荡，从长远来看，它给 AT&T 带来了不幸，而 20 年来的错误判断和糟糕的商业选择使贝尔实验室沦为它任务明确、资金充足稳定时的影子。

In 1984, part of Bell Labs was spun off into a research organization originally called Bellcore ("Bell Communications Research") that was to provide research services for the Baby Bells. The Bellcore split took a fair number of people from Bell Labs research, primarily in communications areas, but also some colleagues from 1127, including Mike Lesk and Stu Feldman. At some point, the Baby Bells decided that they didn't need the kind of research that Bellcore provided, and Bellcore was purchased by another company, SAIC, renamed Telcordia, and eventually wound up owned by the Swedish telecom company Ericsson.

> 1984 年，贝尔实验室的一部分被分拆成一个名为贝尔核心(“贝尔通信研究”)的研究机构，为婴儿贝尔提供研究服务。贝尔核心的分裂从贝尔实验室研究中获得了很多人，主要是在通信领域，还有一些来自 1127 的同事，包括迈克·莱斯克和斯图·费尔德曼。某个时候，婴儿贝尔决定他们不需要贝尔核心提供的研究，贝尔核心被另一家公司 SAIC 收购，改名为 Telcordia，最终被瑞典电信公司爱立信拥有。

1984 was also the year that "Bell Labs" became "AT&T Bell Laboratories," since as part of the consent decree, AT&T was not permitted to use the name "Bell" except in this special case and only if preceded by "AT&T." We were strongly encouraged to use the full name at all times.

> 1984 年，由于根据同意协议，AT&T 不得使用“Bell”这个名字，除非在这种特殊情况下，并且必须在前面加上“AT&T”，“Bell Labs”成为“AT&T Bell Laboratories”。我们强烈建议在任何时候都使用完整的名字。

**7.2 USL and SVR4**

After divestiture, AT&T's inability or at least reluctance to sell Unix gav e way to a substantial commercial effort by a part of the company that was organizationally far removed from Research. It was also somewhat removed physically, located in a building near Summit, New Jersey; surrounded by busy highways, it was informally known as "Freeway Island." The organization was originally called the Unix Support Group (USG) and eventually became Unix System Laboratories, or USL. The first USG was created by Berk Tague in 1973, to focus on operations support systems. Over time, USG broadened its activities to include external sales and marketing.

> 在剥离之后，AT&T 无法或不愿出售 Unix 的行为使得一部分远离研究部门的公司进行大规模商业活动。它也在空间上有所偏离，位于新泽西州萨姆伊特附近的一栋建筑内；被繁忙的高速公路包围，它被非正式地称为“高速公路岛”。该组织最初被称为 Unix 支持组(USG)，最终成为 Unix 系统实验室(USL)。第一个 USG 是由 Berk Tague 在 1973 年创建的，专注于运营支持系统。随着时间的推移，USG 扩大了其活动范围，包括外部销售和营销。

There was definitely a market for Unix; one might even say that AT&T

had inadvertently created the market by giving Unix away to university

[]{#index_split_001.html#p159}CHAPTER 7: COMMERCIALIZATION 145

students, who then wanted it when they entered the real world and worked for companies that could afford to pay real money for it. Beginning in 1984

> 学生们在 1984 年进入现实世界，为能付出真金白银的公司工作时，他们就想要它了。

USL marketed Unix aggressively, and worked hard to make it a professional commercial product. The culmination was a version called System V

> 美国联合软件公司积极地推广 Unix，努力将其打造成一款专业的商业产品。最终成果是一个名为 System V 的版本。

Release 4, or SVR4. AT&T invested substantial resources to making this version a standard, with reference implementations and careful definitions for both source and object compatibility. I think that this attention to standards and interoperability was important.

> 释放 4，或 SVR4。AT&T 投入了大量资源使这个版本成为标准，提供参考实现，并对源代码和对象兼容性进行精确定义。我认为这种对标准和互操作性的关注是很重要的。

The ins and outs of how SVR4 evolved and AT&T's interactions with cooperators and competitors over a decade are intricate and uninteresting.

> 记录 SVR4 演变的细节和 AT&T 在十年间与合作者和竞争者的相互作用复杂而乏味。

I'm not going to say anything more about them, since in a way it's all moot: the industry focus has shifted almost entirely to Linux. The Wikipedia article on System V summarizes the situation, probably accurately, like this:

> 我不再多说它们了，因为某种程度上这都毫无意义：行业的重点已经几乎完全转向 Linux 了。维基百科上关于 System V 的文章总结了这种情况，可能是准确的，就像这样：

"Industry analysts generally characterize proprietary Unix as having entered a period of slow but permanent decline."

> 行业分析师普遍认为，专有 Unix 已进入一个缓慢但永久性衰退的时期。

Of course the operative word is "proprietary"; open-source versions like the BSD family described in the next chapter are alive and well.

> 当然，关键词是“专有”；下一章中描述的 BSD 系列开源版本也很活跃。

AT&T's product line included the operating system and a variety of supporting software, including compilers for C, C++, Fortran, Ada and even Pascal, mostly based on Steve Johnson's portable C compiler. There was also a major standardization effort to ensure compatibility for source code and for binary formats in libraries.

> AT&T 的产品线包括操作系统和各种支持软件，包括 C、C++、Fortran、Ada 甚至 Pascal 的编译器，主要基于史蒂夫·约翰逊的可移植 C 编译器。还有一项重大的标准化努力，以确保源代码和库中的二进制格式的兼容性。

At this point I was Bjarne Stroustrup's department head, which meant frequent interactions with USL about the evolution of C++. For the most part, these were amicable, but there were occasions when the different priorities of research and product management were visible. One heated discussion with a USL manager in 1988 went something like this: Manager: "You have to fix all the bugs in the C++ compiler, but you can't change the behavior in any way."

> 在这一点上，我是 Bjarne Stroustrup 的部门主管，这意味着经常与 USL 就 C++的演变进行交流。大多数情况下，这些都是友好的，但有时研究和产品管理的不同优先级是可见的。1988 年与 USL 经理的一次激烈的讨论大致如下：经理：“你必须修复 C++编译器中的所有错误，但你不能以任何方式改变行为。”

Me: "That's not possible. By definition, if you fix a bug, the behavior is necessarily different."

> 我：“那是不可能的。按照定义，如果你修复了一个错误，行为必然是不同的。”

Manager: "Brian, you don't understand. You have to fix the bugs but the compiler's behavior can't change."

> 经理：“布莱恩，你不明白。你必须修复错误，但是编译器的行为是无法改变的。”

Pedantically I was right, but practically I can see what the manager was getting at---too much or too rapid change is a serious problem for those who are doing software development with new languages and tools.

> 仔细地说，我是正确的，但实际上我可以看到经理的意思---对于那些使用新语言和工具进行软件开发的人来说，太多或太快的变化是一个严重的问题。

[]{#index_split_001.html#p160}146 CHAPTER 7: COMMERCIALIZATION

USL set up a subsidiary in Japan called Unix Pacific, where the manager was Larry Crume, a Bell Labs colleague from years earlier and well known to many in the research group. This led to technical collaborations, and I got to visit Japan twice on the company's money. On one of these trips, some kind of feel-good exchange with NTT, Japan's major telephone company, there was a strikingly clear view of the pecking order. The executive director got to play golf with his NTT counterpart. The center director played tennis with his counterpart. Lowly department heads like me were offered a shop-ping trip in Tokyo, which I declined with thanks.

> 美国联合系统公司在日本设立了子公司 Unix Pacific，经理是 Larry Crume，他是贝尔实验室多年前的同事，也是研究小组中众所周知的人物。这导致了技术合作，我有机会用公司的钱去日本旅行两次。在其中一次旅行中，与日本主要电话公司 NTT 进行了一次令人感到满意的交流，当时明显可以看到等级制度。执行董事可以和他的 NTT 对等人员打高尔夫球。中心主任和他的对等人员打网球。像我这样的低级部门负责人被提供了在东京购物的机会，但我表示感谢，拒绝了这个机会。

Although AT&T's efforts to commercialize Unix were not always successful, Unix standardization was invaluable for the whole community.

> 尽管 AT&T 的统一 Unix 标准化努力并不总是成功，但它对整个社区来说价值连城。

There were occasional tensions between Research and the USL effort, but for the most part, USL had a large group of talented colleagues who made significant contributions to Unix and related software systems.

> 在研究和 USL 努力之间偶尔会出现紧张局势，但大多数情况下，USL 拥有一大批才华横溢的同事，为 Unix 和相关软件系统做出了重大贡献。

**7.3 UNIX™**

Sometime early in the life of Unix, Bell Labs' legal guardians decided that the name Unix was a valuable trademark that had to be protected, which was certainly a correct business decision. They were trying to avoid having the name become a generic term that could be used by anyone, as had happened to words like aspirin (in the US, though not everywhere), escalator, zipper and (much more recently) App Store.

> 早在 Unix 的早期，贝尔实验室的法律监护人就认为 Unix 这个名字是一个有价值的商标，必须加以保护，这当然是一个正确的商业决定。他们试图避免这个名字变成一个可以被任何人使用的通用术语，就像阿司匹林(在美国，但不是全世界)、自动扶梯、拉链和(更近期的)应用商店所发生的那样。

As a consequence, however, people inside Bell Labs were required to use the name correctly. In particular, it could not be used as a standalone noun ("Unix is an operating system"). It had to be identified as a trademark and also had to appear as an upper-case adjective in the phrase "the UNIX™

> 因此，Bell Labs 内部的人必须正确使用这个名字。特别是，它不能被用作单独的名词(“Unix 是一个操作系统”)。它必须被识别为商标，并且也必须以大写形式出现在“the UNIX™”短语中。

operating system," which led to awkward sentences like "The UNIX™ operating system is an operating system." Rob Pike and I had to fight this battle over the title of our 1984 book _The Unix Programming Environment_, which would otherwise have been something like _The UNIX™ Operating System_ _Programming Environment_. The eventual compromise: there is no footnote or trademark indicator on the cover, but on the title page there is an almost invisible asterisk and a footnote.

> UNIX™ 操作系统是一个操作系统。1984 年，罗伯·派克和我不得不为我们的书《UNIX™ 编程环境》(本来应该叫《UNIX™ 操作系统编程环境》)的书名而斗争。最终的妥协方案是：封面上没有脚注或商标指示，但是标题页上有一个几乎看不见的星号和脚注。

The klunky phrasing was a pain, especially for people who took their writing seriously, so there were workarounds and occasional attempts to evade the issue. For instance, in the standard Troff macro package ms, Mike Lesk added a formatting command that expanded into "UNIX" wherever it was used, and automatically generated a footnote on the first page where it appeared (with the name in upper case, of course). Normally the footnote

> 那些笨拙的措辞真是个痛苦，尤其是对那些认真对待写作的人来说，因此出现了一些变通方法和偶尔的尝试来回避这个问题。例如，在标准的 Troff 宏包 ms 中，Mike Lesk 增加了一个格式化命令，这个命令在使用时会展开为“UNIX”，并且会自动在第一页生成一个脚注(当然，名字是大写的)。通常脚注会

[]{#index_split_001.html#p161}![](./index-161_1.jpg){.calibre4}

CHAPTER 7: COMMERCIALIZATION 147

said

† UNIX is a trademark of Bell Laboratories.

but if the command was used with an additional undocumented parameter, it would instead print

> 但如果使用附加的未文档化参数使用该命令，它将会打印出不同的结果。

† UNIX is a footnote of Bell Laboratories.

I don't think that anyone ever noticed when we occasionally used this Easter egg, but the code is still there in the standard macro package.

> 我不认为有人注意到我们偶尔使用这个复活节彩蛋，但是这个代码仍然存在于标准宏包中。

Other uses of the word Unix for goods and services had nothing to do with operating systems, like the pens in Figure 7.1, the bookcases in Figure 7.2, and the fire extinguisher in Figure 7.3. They all seemed to be from outside the United States and thus beyond US trademark laws; the bookcases date from 1941, before Ken and Dennis were born. One other charming example is Unix baby diapers from a company called Drypers, which came up with "Unix" as a contraction of "unisex."

> 其他使用 Unix 这个词的商品和服务与操作系统无关，比如图 7.1 中的钢笔，图 7.2 中的书架，以及图 7.3 中的灭火器，它们似乎都来自美国以外的地方，因此超出了美国商标法的管辖范围；书架可以追溯到 1941 年，那时肯和丹尼斯还没有出生。另一个有趣的例子是一家名为 Drypers 的公司生产的 Unix 婴儿尿布，它们的名字源于"unisex"的缩写。

**Figure 7.1:**

Unix pens (Courtesy of Arnold Robbins)

**7.4 Public relations**

There was always a steady flow of visitors to Bell Labs, and from the mid 1970s until well into the 1980s, a Unix presentation was a frequent stop for tourists. A small group of visitors would sit in a conference room while some member of the Center gav e them a quick overview of what Unix was all about and why it was important to AT&T and the world. Mike Lesk and I probably did more of these demos than everyone else put together, which may have reflected defects in our personalities, since we both complained but in fact enjoyed them.

> 总有一群游客经常来贝尔实验室参观，从 70 年代中期一直持续到 80 年代晚期，参观者们经常会去 Unix 展示会。一小群游客会坐在会议室里，中心的某位成员会给他们快速介绍 Unix 是什么和为什么对 AT&T 和世界都很重要。Mike Lesk 和我可能比其他人一起做的演示多了，这可能反映了我们个性上的缺陷，因为我们都抱怨，但实际上喜欢这样做。

The visitors themselves ranged from ordinary mortals to "distinguished,"

a synonym for "influential" or "important for AT&T to impress" or merely

[]{#index_split_001.html#p162}![](./index-162_1.jpg){.calibre4}

148 CHAPTER 7: COMMERCIALIZATION

**Figure 7.2:**

Unix sectional bookcases, 1941 (Courtesy of Ian Utting)

[]{#index_split_001.html#p163}![](./index-163_1.jpg){.calibre4}

CHAPTER 7: COMMERCIALIZATION 149

**Figure 7.3:**

A Unix fire extinguisher

"big name." For example, in 1980 I did a demo for Walter Annenberg, founder of _TV Guide_ (which is where he made the money that perhaps helped him to become Ambassador to the Court of St James, though that role was over by the time I showed him the wonders of Unix). As a measure of his importance, he was accompanied by Bill Baker, the president of Bell Labs.

> 在 1980 年，我为沃尔特·安恩伯格(Walter Annenberg)做了一个演示，他是《电视指南》(TV Guide)的创始人(也是他赚取了大笔钱，可能帮助他成为圣詹姆斯法院的大使，尽管我向他展示了 Unix 的奇迹时，他的职位已经结束)。他的重要性可以从他身边的比尔·贝克(Bill Baker)来衡量，他是贝尔实验室(Bell Labs)的总裁。

My personal shtick often involved a demo of pipes, showing how programs could be fluidly combined to do quicky _ad hoc_ tasks. I used a shell script for finding potential spelling errors in a document, since it was a neat example of a long pipeline and helped to make the point about how existing programs could be combined in novel ways.

> 我的个人特色通常包括管道的演示，展示如何快速组合程序来完成临时任务。我使用一个 shell 脚本来查找文档中的潜在拼写错误，因为这是一个很好的长管道的例子，有助于表明如何以新颖的方式组合现有程序。

The spell script originated with Steve Johnson. The basic idea was to compare the words of a document to the words in a dictionary. Any word that occurred in the document but not in the dictionary was potentially a spelling mistake. The script looked approximately like this:

> 史蒂夫·约翰逊发明了这个拼写脚本。基本思想是将文档中的单词与字典中的单词进行比较。文档中出现但不在字典中的单词可能是拼写错误。该脚本大致如下：

[]{#index_split_001.html#p164}![](./index-164_1.jpg){.calibre4}

150 CHAPTER 7: COMMERCIALIZATION

cat document \|

tr A-Z a-z \|

\# convert to lower case

tr -d ',.:;()?!' \| \# remove punctuation, \...

tr ' ' '\\n'

\# split words into lines

sort \|

\# sort words of document

uniq \|

\# eliminate duplicates

comm -1 - dict

\# print lines found in input but

\#

not in dictionary

All these programs already existed; comm, the most unusual, was used for tasks like finding lines that were common to two sorted input files, or lines that were in one input or the other but not both. The "dictionary" was

> 所有这些程序都已经存在了；comm，最不寻常的，用于执行像找出两个排序输入文件共同的行，或者在其中一个输入文件中存在，但另一个输入文件中不存在的行的任务。“字典”是

_/usr/dict/web2_, the words in Webster's Second International dictionary, one per line, which we saw earlier.

> _/usr/dict/web2_：以前我们看到的每行一个词，出自韦氏第二国际词典。

**Figure 7.4:**

Unix building blocks, ∼1980 (Courtesy of Bell Labs) One day I was scheduled to do a demo for William Colby, who at the time was the director of the Central Intelligence Agency (CIA), and thus clearly an important person. He too would be accompanied by Bill Baker, who as head of the President's Foreign Intelligence Advisory Board had serious spook credentials of his own.

> 当时是 1980 年，我有一天要为中央情报局(CIA)局长威廉·科尔比做一个演示。他也将由比尔·贝克(Bill Baker)陪同，贝克作为总统外交情报咨询委员会主席拥有自己的专业资质。Unix 构建块(由贝尔实验室提供)。

I wanted to make the point about how Unix made some kinds of programming easy, but the spell script was not very fast and I didn't want the demo to drag on. So I ran the script ahead of time, captured the output in a file, then wrote a new script that merely went to sleep for two seconds, then

> 我想说明 Unix 使一些编程变得容易，但是 spell 脚本不是很快，我不想让演示拖慢。所以我提前运行了脚本，把输出保存到文件中，然后写了一个新脚本，只是睡眠了两秒钟，然后

[]{#index_split_001.html#p165}CHAPTER 7: COMMERCIALIZATION 151

printed the results that had been computed the day before: sleep 2

cat previously.computed.output

This bit of demo engineering worked well; if he understood it at all, Mr Colby must have thought that spell checking ran fast enough. Of course there's a lesson here for everyone who has ever sat through a demo: be wary of what you're seeing!

> 这次演示工程很成功；如果他完全理解的话，科尔比先生一定认为拼写检查的速度够快。当然，这里有一个教训，适用于所有参加过演示的人：要谨慎对待你所看到的一切！

The PR operation also made promotional movies that talked about the wonders of Bell Labs, including a number that featured Unix. Thanks to YouTube, I can see old friends (and myself) when we were all younger and in several cases had more and darker hair.

> PR 操作还制作了宣传片，讲述贝尔实验室的奇迹，其中包括一部以 Unix 为主题的片子。多亏了 YouTube，我可以看到我们年轻的时候的老朋友(还有我自己)，有的人头发更多，更黑。

There was even a brief flurry of print advertising for Unix. I think the children's blocks in the advertisement in Figure 7.4 were my idea, for better or worse. The background, too hard to see here, is a Troff document that I provided.

> 那时甚至还有一阵 Unix 的印刷广告。我想图 7.4 中的儿童积木是我的主意，不管好坏。背景，在这里很难看出，是我提供的 Troff 文档。

[]{#index_split_001.html#p166} []{#index_split_001.html#p167}Chapter 8

**Descendants**

"\... from so simple a beginning endless forms most beautiful and most wonderful have been, and are being, evolved."

> "从如此简单的起点，出现了无尽的美丽而奇妙的形式，而且正在不断演变。"

Charles Darwin, _The Origin of Species_, Chapter 14, 1859

Unix began in the Computing Science Research Center in 1969. There were internal versions like PWB that supported the Programmer's Workbench tools, of course, but starting in 1975, external versions appeared as well, originally based on the 6th edition, and then later on the 7th edition, which appeared in 1979.

> Unix 始于 1969 年的计算机科学研究中心。当然，有像 PWB 这样的内部版本，支持程序员的工作台工具，但从 1975 年开始，外部版本也开始出现，最初基于第六版，然后是 1979 年出现的第七版。

The 7th edition was the last Research version of Unix to be released and widely used. Three more editions were developed and used internally (predictably called 8th, 9th, and 10th) but by the time the 10th edition was completed in late 1989, it was clear that the center(s) of gravity of Unix development had moved elsewhere.

> 第七版是最后一个 Unix 研究版本发布并广泛使用。又开发和使用了三个版本(可想而知地被称为第八、第九和第十版)，但是到 1989 年底第十版完成时，显然 Unix 开发的重心已经转移到其他地方了。

Tw o threads evolved from the 7th edition, one from Berkeley that built on the work of Bill Joy and colleagues, and another from AT&T as it tried to build a money-making business out of its Unix expertise and ownership. The timeline in Figure 8.1 is an approximation and omits numerous systems; reality was more complicated, especially in how the versions interacted.

> 两个线程源于第七版，一个来自伯克利，建立在比尔·乔伊及其同事的工作之上，另一个来自 AT＆T，试图从其 Unix 专业知识和所有权中获取赚钱的业务。 图 8.1 中的时间线只是近似值，省略了许多系统; 现实更复杂，特别是在版本之间的交互方式上。

**8.1 Berkeley Software Distribution**

In 1978, DEC introduced a new computer, the VAX-11/780. The VAX

was a 32-bit machine with substantially more memory and computing horsepower than the PDP-11, while remaining culturally compatible with it. A 16-bit computer uses 16 bits for a memory address, while a 32-bit computer

> 它是一台 32 位机器，比 PDP-11 具有更多的内存和计算能力，同时仍然与之文化兼容。一台 16 位计算机使用 16 位来存储内存地址，而一台 32 位计算机使用 32 位来存储内存地址。

[]{#index_split_001.html#p168}![](./index-168_1.jpg){.calibre4}

154 CHAPTER 8: DESCENDANTS

**Figure 8.1:**

Unix timeline, from Wikipedia

[]{#index_split_001.html#p169}CHAPTER 8: DESCENDANTS 155

uses 32 bits and thus can address a much larger amount of primary memory.

When the VAX-11/780 first appeared, John Reiser and Tom London, who were in a research group at Bell Labs in Holmdel, New Jersey, ported the 7th edition to it, but their version, 32/V, did not use the virtual memory capabilities of the new machine and thus did not take full advantage of what the VAX

> 当 VAX-11/780 首次出现时，位于新泽西州霍尔姆德尔的贝尔实验室的研究小组 John Reiser 和 Tom London 将第 7 版移植到该机器上，但他们的版本 32/V 没有使用新机器的虚拟内存功能，因此没有充分利用 VAX 的优势。

could do.

Bill Joy and his colleagues at the Computer Systems Research Group at the University of California, Berkeley, started with Reiser and London's 32/V

> 比尔·乔伊和他在加州大学伯克利分校计算机系统研究小组的同事们从赖泽尔和伦敦的 32/V 开始。

and added code to use virtual memory. This version quickly supplanted 32/V

> 并增加了使用虚拟内存的代码。这个版本很快取代了 32/V

and the VAX itself became the primary Unix machine for most users as they outgrew the PDP-11. The Berkeley version was packaged and shipped to Unix licensees as BSD, the Berkeley Software Distribution. BSD descen-dants are still active, with variants like FreeBSD, OpenBSD and NetBSD all continuing development. NextSTEP, used for Apple's Darwin, the core of macOS, was also a BSD derivative.

> 随着用户从 PDP-11 转移到更大的机器，VAX 本身成为最主要的 Unix 机器。伯克利版本被打包并作为 BSD(伯克利软件分发)发送给 Unix 许可方。BSD 后代仍然很活跃，有 FreeBSD、OpenBSD 和 NetBSD 等变体继续开发。NextSTEP，用于 Apple 的 Darwin，也是 macOS 的核心，也是一个 BSD 衍生版本。

One of the early Berkeley distributions formed the base of SunOS, which was used on computers from Sun Microsystems, co-founded by Bill Joy.

> 一个早期的伯克利分发版本形成了 SunOS 的基础，它被用于由比尔·乔(Bill Joy)共同创立的 Sun Microsystems 的计算机上。

Others spun off a few years later into the BSD variants mentioned above. All of these eventually were reimplementations that provided the same functionality but with entirely new code. Once rewritten, they were free of AT&T

> 其他一些几年后分裂成上面提到的 BSD 变体。所有这些最终都是提供相同功能但全新代码的重新实现。一旦重写，它们就脱离了 AT&T 的控制。

code and thus did not infringe AT&T's intellectual property.

Another spinoff was created for NeXT, which was founded by Steve Jobs in 1985. The NeXT workstation had a variety of innovative features, and was an early example of the elegant and polished industrial design that Apple users are familiar with. I was in the audience at Bell Labs on December 11, 1990, when Jobs gav e a demonstration of the NeXT. It was a very nice machine, and it was the only time that I can recall thinking "I want one of those" about any technological gadget. I had obviously been seduced by the famous Jobs "reality distortion field." When he did another presentation at the Labs three years later, there was no such effect, and I don't even remember what he was showing off.

> 另一种衍生产品是为史蒂夫·乔布斯于 1985 年创立的 NeXT 公司制作的。NeXT 工作站有各种创新功能，是苹果用户熟悉的优雅和精致的工业设计的早期例子。1990 年 12 月 11 日，我在贝尔实验室的观众席上，当乔布斯展示 NeXT 时，我非常喜欢这台机器，这是我唯一一次记得对任何技术产品想要拥有它的时刻。显然，我已经被著名的乔布斯“现实扭曲场”所诱惑。三年后，当他在实验室做另一次演示时，没有这种效果，我甚至不记得他在展示什么。

Although the NeXT computer itself was not a commercial success, the company was bought by Apple in 1997, and Jobs returned to his old company, becoming CEO within a year. One can still see some of the NextSTEP

> 尽管 NeXT 电脑本身并未取得商业上的成功，但该公司于 1997 年被苹果收购，乔布斯也随即回到了他的老公司，一年内就担任了首席执行官。人们仍然可以看到一些 NextSTEP 的影子。

operating system legacy in names like NSObject and NSString in Objective-C programs.

> 在 Objective-C 程序中，像 NSObject 和 NSString 这样的操作系统遗留名称。

The timeline reveals another little known fact: in the 1980s Microsoft distributed a version of Unix called Xenix; Figure 8.2 is part of an advertisement from the time. One wonders how different the world would be today if

> 时间线揭示了另一个鲜为人知的事实：在 1980 年代，微软发布了一个名为 Xenix 的 Unix 版本；图 8.2 是当时的一则广告的一部分。不禁让人想象，如果当时发展的路线有所不同，今天的世界会是什么样子。

[]{#index_split_001.html#p170}![](./index-170_1.jpg){.calibre4}

156 CHAPTER 8: DESCENDANTS

Microsoft had pushed Xenix instead of its own MS-DOS, and if AT&T had been easier to deal with than it apparently was. According to The Unix Heritage Society, the Santa Cruz Operation (SCO) later acquired Xenix, which in the mid to late 1980s was the most common Unix variant as measured by the number of machines on which it was installed.

> 微软曾经推出 Xenix 而不是自己的 MS-DOS，如果 AT&T 的交易比它显然容易的话。根据 Unix 遗产协会，Santa Cruz Operation(SCO)后来收购了 Xenix，在 20 世纪 80 年代中期至后期，它是安装最多的 Unix 变体。

**Figure 8.2:**

Xenix: Microsoft's version of Unix

**8.2 Unix wars**

In the late 1980s there were numerous vendors of Unix systems, all using the trademarked name, and purveying software at least originally based on Version 7 from Bell Labs research. There were incompatibilities, however, particularly between AT&T's System V and the Berkeley distributions. All parties agreed that it would be highly desirable to have a common standard, but naturally disagreed on what it would be.

> 1980 年代末，有许多使用商标名称的 Unix 系统供应商，至少最初都是基于贝尔实验室研究的版本 7 提供的软件。然而，AT&T 的系统 V 和伯克利分发版之间存在不兼容性。所有各方都同意，有一个共同的标准是非常理想的，但自然也会对它的具体形式存在分歧。

X/Open, an industry consortium, was formed in 1984 to try to create a standard source-code environment so that programs could be compiled on

> X/Open，一个行业联盟，成立于 1984 年，试图创建一个标准的源代码环境，以便程序可以在上面编译。

[]{#index_split_001.html#p171}CHAPTER 8: DESCENDANTS 157

any Unix system without change.

AT&T and some allies formed their own group, Unix International, to promulgate their standard, in competition with a different standard from a group called the Open Software Foundation. The result? Two competing and different "open" standards. Eventually peace broke out, with a standard called POSIX (Portable Operating System Interface) for basic library functions, and a "Single Unix Specification" administered by X/Open that between them standardized libraries, system calls, and a large number of common commands (including the shell, Awk, ed, and vi ).

> AT&T 和一些盟友组建了他们自己的组织 Unix International，来推广他们的标准，与另一个叫做 Open Software Foundation 的组织的标准竞争。结果呢？两个不同的“开放”标准竞争。最终和平统一，推出了一个叫做 POSIX(可移植操作系统接口)的标准，用于基本库函数，以及由 X/Open 管理的“单一 Unix 规范”，它们统一了库、系统调用和许多常见命令(包括 shell、Awk、ed 和 vi)。

In 1992, USL and AT&T sued Berkeley over intellectual property rights in Unix, claiming that Berkeley was using AT&T code without permission.

> 1992 年，USL 和 AT&T 就 Unix 的知识产权权利起诉伯克利，称伯克利在未经许可的情况下使用了 AT&T 的代码。

Berkeley had made many changes in the AT&T code, and added much valuable material of their own, including the TCP/IP code that made the Internet accessible.

> 伯克利在 AT&T 的代码中做了许多改变，并添加了许多自己的宝贵材料，包括使 Internet 可访问的 TCP/IP 代码。

Berkeley continued to remove and rewrite code that had come from AT&T, and in 1991 released a version of Unix that they felt contained none of AT&T's proprietary material. AT&T and USL were not convinced, howev er, and this led to the lawsuit. After much maneuvering the case was heard in a New Jersey court, where Berkeley prevailed, in part on the grounds that AT&T had failed to put proper copyright notices on the code that it had distributed. Counter-suits ensued.

> 贝克利继续删除和重写从 AT&T 收到的代码，并在 1991 年发布了一个他们认为没有 AT&T 专有材料的 Unix 版本。然而，AT&T 和 USL 并不确定，这导致了诉讼。经过多次调整，这个案子在新泽西的一个法庭上审理，贝克利获胜，部分原因是 AT&T 在发布的代码上没有正确添加版权声明。随后反诉也随之而来。

If this all sounds terminally complicated and boring, you're right, but it was a big deal at the time, with much waste of time and money on all sides.

> 如果这一切听起来极其复杂而乏味，你是对的，但当时这是一件大事，双方都浪费了大量的时间和金钱。

In 1991, AT&T sold shares in USL to 11 companies, and in 1993 Novell bought the rights to USL and Unix. Novell's CEO, Ray Noorda, decided to settle any remaining legal cases, perhaps realizing that the parties involved were spending more money on lawyers than they could possibly ever recoup in sales.

> 1991 年，AT&T 向 11 家公司出售了 USL 的股份，1993 年 Novell 购买了 USL 和 Unix 的权利。Novell 的首席执行官 Ray Noorda 决定解决任何剩余的法律案件，也许意识到当事方花费的律师费比他们可能获得的销售额还要多。

In retrospect, I suppose one could say that all the legal wrangling was a by-product of AT&T's early and almost accidental decision to make Unix available to universities. As Unix spread from universities using it for free to companies that were willing to pay for it, it became commercially viable, at least potentially. But it was too late for effective protection. Even if AT&T's source code was restricted, the system call interface was in effect in the public domain, and there was so much expertise in the community that creating versions unencumbered by AT&T licenses was almost routine. The same was true of application software like compilers, editors, and all the tools. To mix several metaphors, AT&T was trying to lock the barn door after the crown jewels had flown the coop.

> 回想起来，我想可以说，所有的法律纠纷都是 AT&T 早期几乎是意外地决定把 Unix 提供给大学的副产品。随着 Unix 从免费使用它的大学传播到愿意为它付费的公司，它变得具有商业价值，至少在潜在上是如此。但是为了有效的保护已经太晚了。即使 AT&T 的源代码受到限制，但系统调用接口实际上已经处于公共领域，社区中有如此多的专业知识，以至于创建不受 AT&T 许可约束的版本几乎变得司空见惯。编译器、编辑器和所有工具等应用软件也是如此。把几个比喻混合起来，AT&T 正试图在宝石已经飞离马厩之后锁上马厩的大门。

[]{#index_split_001.html#p172}158 CHAPTER 8: DESCENDANTS

**8.3 Minix and Linux**

AT&T's licensing of Unix became more and more restrictive as the company tried to make money from the software. This included restrictions on how Unix could be used in universities, which gav e an advantage to BSD, which had no such constraints. At the same time, the ongoing wars between AT&T and BSD encouraged others to try rolling their own Unix-like systems. Independently created versions were free of commercial restrictions, since they used only the system call interface, but no one else's code.

> AT&T 在试图从软件中赚钱时，对 Unix 的许可越来越受限制。这包括限制在大学中如何使用 Unix，这给 BSD 带来了优势，因为它没有这种限制。与此同时，AT&T 和 BSD 之间的持续战争鼓励其他人尝试滚动自己的类 Unix 系统。独立创建的版本不受商业限制，因为它们只使用系统调用接口，而不使用其他人的代码。

At the Free University in Amsterdam in 1987, Andy Tanenbaum created Minix, a Unix lookalike that was compatible at the system call level but written entirely from scratch with a different kernel organization.

> 在 1987 年的阿姆斯特丹自由大学，Andy Tanenbaum 创造了 Minix，一个类似 Unix 的操作系统，它在系统调用层面上兼容，但是完全从头开始编写，具有不同的内核组织。

Minix was comparatively small, and to help with its spread, Andy wrote a textbook on it that metaphorically was a parallel to the Lions book of a decade earlier. Minix source code was available for free---one edition of the book came with a set of about a dozen floppy disks that could be loaded onto an IBM PC to provide a running system. I still have the first edition of Andy's book, and I might even hav e my Minix floppies as well.

> Minix 比较小，为了帮助它的传播，Andy 写了一本关于它的教科书，比喻是十年前狮子的书。Minix 源代码可以免费获得-一本书附带了十几张软盘，可以加载到 IBM PC 上，提供一个运行系统。我仍然拥有 Andy 的第一版书，甚至可能还有我的 Minix 软盘。

Minix is alive and well today, a vehicle for education and for experimenting with operating systems.

> Minix 今天仍然很活跃，是一种用于教育和实验操作系统的工具。

One other result of AT&T's restrictive licensing, combined with the availability of Minix as a guide, was the independent development of another Unix-like system, compatible at the system call level, by a 21-year-old Finnish college student. On August 25, 1991, Linus Torvalds posted an item on comp.os.minix, a Usenet news group, shown in Figure 8.3.

> AT&T 的严格许可限制，加上 Minix 的可用性，另一个类似 Unix 的系统，在系统调用级别上兼容，由一位 21 岁的芬兰大学生独立开发，是另一个结果。1991 年 8 月 25 日，Linus Torvalds 在 Usenet 新闻组 comp.os.minix 上发布了一个条目，见图 8.3。

Linus did not predict the remarkable future of his hobby system, any more than Ken and Dennis predicted the success of Unix. What started out as a few thousand lines of code now stands at well over 20 million lines, with Torvalds (Figure 8.4) as the principal developer and coordinator of a worldwide developer community maintaining and enhancing it. Torvalds is also the creator of Git, the most widely used version-control system for tracking code changes in software systems, of course including Linux.

> 林纳斯没有预测他的爱好系统的出色未来，就像肯和丹尼斯没有预测 Unix 的成功一样。最初只有几千行代码，现在已经超过 2000 万行，托瓦尔兹(图 8.4)是主要的开发者和全球开发者社区的协调者，维护和增强它。托瓦尔兹也是 Git 的创造者，Git 是用于跟踪软件系统中代码更改的最广泛使用的版本控制系统，当然包括 Linux。

At this point, Linux is a commodity operating system that can run on any kind of computer. It's on literally billions of devices (all Android phones, for example). It runs a substantial part of Internet infrastructure, including servers for major operations like Google, Facebook, Amazon, and so on. It's inside many Internet of Things (IoT) devices---my car runs Linux, as does my TV, your Alexa and Kindle, and your Nest thermostat. At the other end of the computing horsepower spectrum, it's the operating system on all of the top 500 supercomputers in the world. It's not a significant player in markets

> 在这一点上，Linux 是一个可以在任何类型的计算机上运行的商品操作系统。它出现在数以十亿计的设备上(所有安卓手机，例如)。它运行着大部分互联网基础设施，包括 Google，Facebook，Amazon 等大型运营商的服务器。它也是许多物联网(IoT)设备的内部操作系统---我的汽车和电视都是 Linux，你的 Alexa 和 Kindle，以及 Nest 恒温器也是。在计算能力谱系的另一端，它是世界上前 500 台超级计算机的操作系统。它在市场上不是一个重要的参与者。

[]{#index_split_001.html#p173}CHAPTER 8: DESCENDANTS 159

Hello everybody out there using minix -

I'm doing a (free) operating system (just a hobby, won't be big and professional like gnu) for 386(486) AT clones.

> 我正在为 386(486) AT 克隆机做一个(免费)操作系统(只是个爱好，不会像 GNU 那样大型且专业)。

This

has been brewing since april, and is starting to get ready.

I'd like any feedback on things people like/dislike in minix, as my OS resembles it somewhat (same physical layout of the file-system (due to practical reasons) among other things).

> 我想要了解人们对 MINIX 的喜欢/不喜欢的反馈，因为我的操作系统在某些方面与它有些相似(出于实际原因，文件系统的物理布局相同)。

I've currently ported bash(1.08) and gcc(1.40), and things seem to work.

This implies that I'll get something

practical within a few months, and I'd like to know what features most people would want.

> 在几个月内实施，我想知道大多数人想要什么功能。

Any suggestions are

welcome, but I won't promise I'll implement them :-) Linus (torv\...@kruuna.helsinki.fi)

> 欢迎，但我不能保证我会实施它们 :-) Linus(torv\...@kruuna.helsinki.fi)

PS. Yes - it's free of any minix code, and it has a multi-threaded fs.

It is NOT protable (uses 386 task

switching etc), and it probably never will support anything other than AT-harddisks, as that's all I have :-(.

> 切换等)，而且它可能永远不会支持除 AT 硬盘外的任何其他东西，因为我只有 AT 硬盘:-(。

**Figure 8.3:**

Linus Torvald's announcement of Linux, August 1991

like laptop and desktop computers, however; there the majority run Windows, followed by macOS.

> 就像笔记本电脑和台式电脑一样，但大多数运行 Windows 系统，其次是 macOS 系统。

As a modern aside, the issue of whether it's possible to copyright a programming interface like the C standard library or the system calls for an operating system is now the center of an apparently endless lawsuit between Oracle and Google. Oracle acquired Sun Microsystems in 2010 and thus became the owner of the Java programming language. Later that year, it sued Google, claiming that Google was using Oracle's copyrighted Java interface in Android phones without permission, along with some patent claims.

> 作为一个现代的注解，现在有一个似乎永无止境的官司，是关于是否可以对像 C 标准库或操作系统的系统调用这样的编程接口进行版权保护的问题。2010 年，甲骨文公司收购了 Sun Microsystems，因此成为 Java 编程语言的所有者。同年晚些时候，它起诉谷歌，声称谷歌在没有得到许可的情况下使用了甲骨文的 Java 接口，以及一些专利权利的索赔。

Google won this case, with the judge ruling that the patent claims were invalid and the Java API (application programming interface) could not be copyrighted.

> 谷歌赢得了这场官司，法官裁定专利请求无效，Java API(应用程序编程接口)不能被版权保护。

Oracle appealed, and eventually a new trial was held. Google won again, but Oracle filed another appeal and this time the appeals court ruled for Oracle. Google appealed to the Supreme Court for the right to present the case there, in the hope of resolving the issue of whether APIs (not implementations!) could be copyrighted and thus used to prevent other parties from using an interface specification to create lookalike systems.

> 欧拉克尔上诉，最终又举行了一次新的审判。谷歌再次获胜，但欧拉克尔又提起上诉，这次上诉法院判决支持欧拉克尔。谷歌向最高法院申请提出案件，希望解决 API(而不是实现！)是否可以被版权保护，从而阻止其他当事人使用接口规范来创建类似系统的问题。

[]{#index_split_001.html#p174}![](./index-174_1.jpg){.calibre4}

160 CHAPTER 8: DESCENDANTS

**Figure 8.4:**

Linus Torvalds in 2014 (Wikipedia)

Disclosure: I've signed on to a couple of amicus briefs on the Google side here, since I do not believe that APIs should be copyrightable. If they were, we would not have had any of the Unix lookalikes, including Linux, since they are based on independent implementation of the Unix system call interface. We would probably also not have packages like Cygwin, a Windows implementation of Unix utilities that provides a Unix-like commandline interface for Windows users. Indeed, we would not likely have many independent implementations of interfaces for anything if they could be restricted by companies that claimed ownership.

> 披露：我在这里已经签署了几份关于谷歌一方的友好简报，因为我不相信 API 应该受版权保护。如果它们受到版权保护，我们就不会有任何类似 Unix 的产品，包括 Linux，因为它们是基于独立实现 Unix 系统调用接口的。我们可能也不会有像 Cygwin 这样的软件包，它是一个为 Windows 用户提供类似 Unix 命令行界面的 Windows 实现的 Unix 实用程序。事实上，如果它们可以被声称拥有所有权的公司限制，我们可能不太可能有许多独立实现的任何接口。

At the time I'm writing this, the Supreme Court has not decided whether to hear the case. We shall see, since once the Court decides, that's it, short of Congress changing the law in a clear fashion. And of course who knows what might happen in other countries.

> 此时此刻，最高法院尚未决定是否听取这个案件。我们将拭目以待，因为一旦法院作出决定，除非国会以明确的方式改变法律，否则就没有办法改变了。当然，谁也不知道其他国家会发生什么。

**8.4 Plan 9**

By the mid to late 1980's, Unix research in 1127 was slowing. The 7th edition, which was widely distributed and formed the base for most external versions, had been released in 1979. The 8th edition appeared six years later in 1985, the 9th in 1986, and the 10th, the final research version, was completed in 1989, though it was not distributed externally.

> 到 1980 年代中期到晚期，1127 的 Unix 研究正在放缓。第七版已于 1979 年发布，并成为大多数外部版本的基础。第八版在 1985 年出现，第九版在 1986 年，最终的研究版本第十版在 1989 年完成，但未外部发布。

[]{#index_split_001.html#p175}CHAPTER 8: DESCENDANTS 161

The perception was that Unix was a mature commercial system, and no longer a suitable vehicle for research in operating systems. A small group---

> 人们认为 Unix 是一个成熟的商业系统，不再适合用于操作系统研究。一小群人......

Ken Thompson, Rob Pike, Dave Presotto and Howard Trickey---gathered together to work on a new operating system, which they called Plan 9 from Bell Labs after the 1959 science-fiction movie _Plan 9 from Outer Space_.

> Ken Thompson、Rob Pike、Dave Presotto 和 Howard Trickey 聚集在一起，开发了一个新的操作系统，他们称之为贝尔实验室的 Plan 9，这是以 1959 年科幻电影《Plan 9 from Outer Space》命名的。

( _Plan 9_ the movie had gained a reputation as the worst movie ever made---a tough competition, to be sure---though some movie fans felt that it was so bad that it was actually good in a perverse way.) Plan 9 the operating system was in part an attempt to take the good ideas in Unix and push them further. For example, in Unix, devices were files in the file system. In Plan 9, many more data sources and sinks were files as well, including processes, network connections, window-system screens and shell environments. Plan 9 also aimed for portability right from the beginning, with a single source that could be compiled for any supported architecture. Another outstanding feature of Plan 9 was its support for distributed systems. Processes and files on unrelated systems with different architectures could work together exactly as if they were in the same system.

> 《Plan 9》这部电影被誉为有史以来最糟糕的电影---这可不是一项容易的竞争---尽管一些电影迷认为它太糟糕以至于在某种反常的方式中它其实是很棒的。Plan 9 操作系统部分是为了把 Unix 中的好主意推向更远。例如，在 Unix 中，设备是文件系统中的文件。在 Plan 9 中，更多的数据源和汇也是文件，包括进程、网络连接、窗口系统屏幕和 shell 环境。Plan 9 从一开始就着眼于可移植性，可以使用单一源代码编译到任何支持的架构。Plan 9 的另一个出色的特性是它对分布式系统的支持。在不同的架构系统上的进程和文件可以像在同一个系统中一样协同工作。

Plan 9 was made available to universities in 1992, and released publicly a few years later for commercial use, but aside from a small community of afi-cionados, it is not used much today. The major reason is probably that Unix and increasingly Linux simply had too much momentum and there wasn't a compelling reason for most people to switch systems. A smaller part of the reason it didn't catch on may be that it took a rather Procrustean view. Plan 9

> Plan 9 於 1992 年提供給大學，幾年後又放行商業使用，但除了一小群熱愛者外，今天並未大量使用。主要原因可能是 Unix 和 Linux 系統擁有太大的勢頭，沒有太多理由讓大多數人切換系統。它沒有流行的另一個原因可能是它對於東西採取了一種極端的態度。

mechanisms were in many cases better than the Unix equivalents, and there wasn't much attempt to provide compatibility. For example, Plan 9 originally did not provide the C standard I/O library stdio, instead using a new library called _bio_. _Bio_ was cleaner and more regular than stdio, but without the standard library, it took real work to convert programs to run on both Unix and Plan 9. Similarly, there was a new version of Make called Mk, which was superior in many ways, but it was incompatible and so existing makefiles had to be rewritten.

> 在许多情况下，机制比 Unix 等效性更好，而且没有太多尝试提供兼容性。例如，Plan 9 最初没有提供 C 标准 I/O 库 stdio，而是使用一个名为*bio*的新库。 *Bio*比 stdio 更干净，更规则，但没有标准库，要将程序转换为在 Unix 和 Plan 9 上运行需要真正的工作。同样，有一个名为 Mk 的新版本的 Make，在许多方面都优于它，但是它是不兼容的，因此必须重写现有的 makefile。

There were mechanisms for conversion, and Howard Trickey (Figure 8.5) ported a number of key libraries like stdio, but in spite of that, at least for some potential users, including me, it was too much effort. Thus Plan 9 was unable to profit directly from a lot of good Unix software, and it was harder to export its software innovations to the mainstream Unix world.

> 当时有转换机制，而 Howard Trickey(图 8.5)移植了一些重要的库，比如 stdio，但是尽管如此，对于一些潜在的用户，包括我，它仍然是一种很大的努力。因此，Plan 9 无法直接从许多优秀的 Unix 软件中获利，而且很难将其软件创新出口到主流 Unix 世界。

Plan 9 did contribute one thing of surpassing importance to the world, however: the UTF-8 encoding of Unicode.

> Plan 9 为世界做出了一个超出重要性的贡献：Unicode 的 UTF-8 编码。

Unicode is an ongoing effort to provide a single standard encoding of all the myriad characters that mankind has ever used for writing. That includes

> Unicode 是一项持续的努力，旨在为人类用于书写的各种字符提供单一的标准编码。这包括简体中文。

[]{#index_split_001.html#p176}![](./index-176_1.jpg){.calibre4}

162 CHAPTER 8: DESCENDANTS

**Figure 8.5:**

Howard Trickey, ∼1981 (Courtesy of Gerard Holzmann) alphabetic scripts like those in most Western languages, but also ideographic scripts like Chinese, ancient scripts like Cuneiform, special characters and symbols of all types, and recent inventions like emojis. Unicode has nearly 140,000 characters at the moment, and the count increases slowly but steadily.

> 霍华德·特里基，约 1981 年(摄影：杰拉德·霍尔茨曼)Unicode 拥有近 14 万个字符，而且数量还在缓慢但稳定地增加。它不仅包括大多数西方语言中的字母文字，还包括汉字、楔形文字等古文字、各种特殊字符和符号以及表情符号等最新发明。

Unicode was originally a 16-bit character set, big enough to hold all alphabetic scripts and the roughly 30,000 characters of Chinese and Japanese. But it was not feasible to convert the world to a 16-bit character set when most computer text was in ASCII, a 7-bit set.

> Unicode 最初是一个 16 位字符集，足够容纳所有字母文字脚本和大约 30000 个中文和日文字符。但是，当大多数计算机文本都是 ASCII 7 位字符集时，将世界转换为 16 位字符集是不可行的。

Ken Thompson and Rob Pike wrestled with this issue for Plan 9, since they had decided that Plan 9 would use Unicode throughout, not ASCII. In September 1992, they came up with UTF-8, a clever variable-length encoding of Unicode. UTF-8 is efficient in both space and processing time. It represents each ASCII character as a single byte, and uses only two or three bytes for most other characters, with a maximum of four bytes. The encoding is compact, and ASCII is legal UTF-8. UTF-8 can be decoded as it is read, since no legal character is a prefix of any other character, nor is any character part of any other character or sequence of characters. Almost all text on the Internet today is encoded in UTF-8; it is used everywhere by ev eryone.

> Ken Thompson 和 Rob Pike 为 Plan 9 解决了这个问题，因为他们决定 Plan 9 将在整个系统中使用 Unicode 而不是 ASCII。 1992 年 9 月，他们提出了 UTF-8，一种巧妙的 Unicode 可变长度编码。 UTF-8 在空间和处理时间上都很有效。它将每个 ASCII 字符表示为单个字节，对于大多数其他字符只使用两到三个字节，最多使用四个字节。该编码紧凑，而 ASCII 是合法的 UTF-8。 UTF-8 可以随着阅读而被解码，因为没有合法字符是任何其他字符的前缀，也没有任何字符是任何其他字符或字符序列的一部分。今天互联网上几乎所有的文本都是用 UTF-8 编码的，它被每个人到处使用。

[]{#index_split_001.html#p177}![](./index-177_1.jpg){.calibre4}

![](./index-177_2.jpg){.calibre4}

CHAPTER 8: DESCENDANTS 163

**8.5 Diaspora**

In 1996, AT&T split itself again, this time voluntarily and into three parts, a process that called for a new word: "trivestiture." One part remained AT&T, focusing on long distance telephony and communications. A second part became Lucent Technologies, which was in effect the follow-on to Western Electric, focused on manufacturing telecom equipment. (One of the company's slogans was "We make the things that make communications work.") The third fission product came from undoing the ill-judged acquisition of NCR in 1991 when AT&T was trying to enter the computer business.

> 1996 年，AT＆T 又一次自行分裂成三部分，这个过程需要一个新词：“trivestiture”。一部分仍然是 AT＆T，专注于长途电话和通信。第二部分成为路印科技，实际上是西电的后续，专注于制造电信设备。(公司的一句口号是“我们制造使通信工作的东西”)第三个裂变产物来自于撤销 1991 年 AT＆T 试图进入计算机业务时的不当收购 NCR。

Bell Labs employees at the time were largely skeptical of trivestiture. The hype that came with the new company name and logo was met with some scorn. Figure 8.6 shows the flaming red Lucent logo that was announced with much fanfare in 1996; I can't repeat most of the names that were soon attached to it. Figure 8.7 is an on-point Dilbert cartoon that appeared soon afterwards.

> 当时的贝尔实验室员工大多对三方分立持怀疑态度。新公司名称和标志带来的炒作遭到了一些嘲笑。图 8.6 展示了 1996 年发布的火红色朗讯标志，我不能重复随后附在它身上的大多数名字。图 8.7 是随后出现的一个恰当的迪尔伯特漫画。

**Figure 8.6:**

Lucent Technologies logo

**Figure 8.7:**

Dilbert's take on the Lucent logo? DILBERT © 1996 Scott Adams. Used by permission of ANDREWS MCMEEL SYNDICATION. All rights reserved.

> 狄尔伯特对路易斯的标志有什么看法？狄尔伯特 © 1996 Scott Adams。 由安德鲁斯·麦克米尔报业联合公司许可使用。 保留所有权利。

Triv estiture split Bell Labs Research itself along functional lines, with roughly one third of the research staff going to AT&T to form AT&T Labs

> 三位士分割贝尔实验室研究机构按功能划分，大约三分之一的研究人员加入 AT&T，成立 AT&T 实验室。

[]{#index_split_001.html#p178}164 CHAPTER 8: DESCENDANTS

(now AT&T Shannon Labs), and the rest remaining "Bell Labs" as part of Lucent. For the most part, people went where they were told, but the members of 1127, with a long history of pushing back against management edicts, strongly resented the forced split-up of the Center. We took a hard line, and management reluctantly agreed to let everyone make their own choice. In a stressful real-time process, each person decided whether to go with AT&T or stay with Lucent. In the end, this achieved the same roughly one-third / two-thirds split that had been planned, but individuals had control over their own destinies, at least in the short run.

> 现在，AT&T Shannon 实验室已经成为 Lucent 的一部分，其余的 Bell 实验室也是如此。大多数人都按照指示去了他们被指派的地方，但 1127 的成员们有着反抗管理指令的悠久历史，他们强烈反对将中心强行分割。我们采取了强硬的立场，管理层不得不勉强同意让每个人做出自己的选择。在一个紧张的实时过程中，每个人都决定是去 AT&T 还是留在 Lucent。最终，这实现了原定的大约三分之一/三分之二的拆分，但个人至少在短期内可以控制自己的命运。

All parties ultimately fell on hard times. AT&T was eventually bought by Southwestern Bell (now SBC Communications), one of the original Baby Bells. SBC rebranded itself with the AT&T name, logo and even the stock ticker symbol " T " that had been used as early as 1901.

> 所有各方最终都落入困境。最终，AT&T 被最初的 Baby Bells 之一 Southwestern Bell(现在的 SBC Communications)收购。SBC 重新以 AT&T 的名称、标志和股票代码“T”(早在 1901 年就使用)重新塑造了自己。

Lucent went through a boom and then a bust, with some questionable business practices en route. As it struggled to survive, it spun off its enterprise communications services business into a company called Avaya in 2000, and its integrated-circuit business into another called Agere in 2002.

> 鲁昂特经历了一次繁荣，然后又遭遇了衰退，在此期间有一些可疑的商业行为。在挣扎求存的过程中，它于 2000 年将其企业通信服务业务分拆成一家名为 Avaya 的公司，并将集成电路业务分拆成另一家名为 Agere 的公司。

Each split removed more people from Bell Labs, narrowing the breadth of research activities and of course shrinking the financial base that could support long-term work. Agere was eventually absorbed into LSI Logic; after some significant ups and downs, including bankruptcy, Avaya is still in business as an independent company.

> 每一次分割都会让贝尔实验室的人数减少，缩小研究活动的范围，当然也减少了可以支持长期工作的财务基础。Agere 最终被吸收到 LSI Logic 中；经历了一些重大的起伏，包括破产，Avaya 仍然作为一家独立的公司在经营。

In 2006 Lucent merged with the French telecom company Alcatel to form Alcatel-Lucent, which in turn was taken over by Nokia in 2016. Bell Labs was swept up in this wav e of mergers and takeovers, but along the way, most of those who had been involved with Unix and Center 1127 dispersed to other places. The number 1127 itself disappeared in a reorganization in 2005.

> 2006 年，路印与法国电信公司阿尔卡特合并，形成阿尔卡特-路印，而阿尔卡特-路印又于 2016 年被诺基亚收购。贝尔实验室也被卷入这波并购和收购浪潮之中，但在此期间，大多数参与 Unix 和中心 1127 的人都分散到其他地方。2005 年，1127 号本身也在重组中消失了。

Gerard Holzmann maintains a list of the alumni of Center 1127 and where they are, at _[www.spinroot.com/gerard/1127_alumni.html](http://www.spinroot.com/gerard/1127_alumni.html)_. All too many hav e died, but of those still alive, the most common destination has been Google; others are at other companies, teaching, or retired. Only a tiny handful remain at Bell Labs.

> Gerard Holzmann 维护着中心 1127 的校友名单和他们现在的位置，可以在[www.spinroot.com/gerard/1127_alumni.html](http://www.spinroot.com/gerard/1127_alumni.html)上找到。可惜有太多人已经去世，但是在生者中，最常见的去处是谷歌；其他人则在其他公司工作、教书或者退休了。只有极少数人仍然留在贝尔实验室。

[]{#index_split_001.html#p179}Chapter 9

**Legacy**

"Unix was not only an improvement on its predecessors but also on most of its successors."

> Unix 不仅改进了它的前辈，而且改进了它的大多数后继者。

Doug McIlroy, _Remarks for Japan Prize award ceremony_ _for Dennis Ritchie_, May 2011, paraphrasing Tony Hoare on Algol Unix has been tremendously successful. As Unix or Linux or macOS or other variants, it runs on billions of computers, serves billions of people continuously, and has of course made billions of dollars for any number of people who have built on top of it (though not for any of its creators). Later operating system have been strongly shaped by its decisions.

> 陶夫·麦克伊尔罗伊(Doug McIlroy)在 2011 年 5 月为丹尼斯·里奇(Dennis Ritchie)颁发日本奖时的讲话(改编自托尼·霍尔(Tony Hoare)关于 Algol 的论述)：Unix 极为成功。它以 Unix、Linux、macOS 或其他变体的形式运行在数十亿台计算机上，持续服务于数十亿人，当然也为许多在其上构建的人赚取了数十亿美元(虽然其创造者没有得到任何回报)。后续操作系统都受到其决策的强烈影响。

Languages and tools originally developed at Bell Labs for Unix are everywhere. Among the programming languages are C and C++, which are still the backbone of system programming today and more specialized ones like Awk and AMPL. Core tools include the shell, diff, grep, Make and Yacc.

> 诞生于贝尔实验室的 Unix 语言和工具已经遍布世界各地。编程语言中包括 C 和 C++，它们仍是当今系统编程的支柱，还有更专业的诸如 Awk 和 AMPL。核心工具包括 Shell、Diff、Grep、Make 和 Yacc。

GNU (a recursive acronym for "GNU's not Unix") is a large collection of software, much based on Unix models, that is freely available in source-code form for anyone to use: it makes almost everything from Unix available, along with much more. Coupled with the Linux operating system, GNU

> GNU(递归缩写词“GNU 不是 Unix”)是一个大型软件集合，大部分基于 Unix 模型，可以以源代码形式免费提供给任何人使用：它几乎提供了 Unix 的所有功能，并且还有更多功能。结合 Linux 操作系统，GNU 提供了更多功能。

amounts to a free version of Unix. GNU implementations of Unix commands are open source, so they can be used and extended, subject only to the restriction that if the improvements are distributed, they hav e to be made available to everyone for free; they can't be taken private. A huge amount of today's software development is based on open source and in many cases GNU implementations.

> GNU 实现的 Unix 命令是开源的，因此可以使用和扩展，只受到一个限制：如果分发改进，就必须免费向所有人提供；它们不能被私有化。今天软件开发的大量工作都是基于开源的，在许多情况下都是 GNU 实现。这相当于一个免费的 Unix 版本。

What accounts for the success of Unix? Are there ideas or lessons that can be learned and applied in other settings? I think that the answer is yes, on at least two fronts: technical for sure, and organizational as well.

> 究竟是什么造就了 Unix 的成功？有没有可以在其他环境中学习和应用的观念或教训？我认为答案是肯定的，至少有两个方面：技术当然，还有组织方面。

[]{#index_split_001.html#p180}166 CHAPTER 9: LEGACY

**9.1 Technical**

The important technical ideas from Unix have been discussed in the first few chapters of the book; this section is a brief summary. Not everything here originated with Unix, of course; part of the genius of Ken Thompson and Dennis Ritchie was their tasteful selection of existing good ideas, and their ability to see a general concept or a unifying theme that simplified software systems. People sometimes talk of software productivity in terms of the number of lines of code written; in the Unix world, productivity was often measured by the number of special cases or lines of code that were removed.

> 里面的重要技术思想已经在本书的前几章讨论过；这一部分是一个简要的总结。当然，并不是所有这些都起源于 Unix；Ken Thompson 和 Dennis Ritchie 的天才之处在于他们精选现有的好思想，并能够看到一般概念或统一的主题，从而简化软件系统。有时人们用行数来说明软件的生产力；在 Unix 世界中，生产力通常是用特殊情况或行数的减少来衡量的。

The _hierarchical file system_ was a major simplification of existing practice, though in hindsight it seems utterly obvious---what else would you want? Rather than different types of files with properties managed by the operating system, and arbitrary limits on the depth to which files could be nested in directories, the Unix file system provides a straightforward view: starting from the root directory, each directory contains either information about files, or directories that contain information about further files and directories. Filenames are simply the path from the root, with components separated by slashes.

> 分层文件系统是对现有实践的一种重大简化，尽管回顾起来它似乎是如此明显——你还想要什么？Unix 文件系统提供了一种直观的视图，而不是由操作系统管理属性的不同类型的文件，以及对文件可以嵌套到目录中的深度的任意限制：从根目录开始，每个目录包含有关文件的信息，或者包含有关进一步文件和目录的信息的目录。文件名只是从根目录开始的路径，其组件用斜杠分隔。

Files contain uninterpreted bytes; the system itself does not care what the bytes are, or know anything about their meaning.

> 文件包含未解释的字节；系统本身不关心这些字节是什么，也不了解它们的含义。

Files are created, read, written and removed with half a dozen straightforward system calls. A handful of bits define access controls that are adequate for most purposes. Entire storage devices like removable disks can be mounted on a file system so that logically the contents become part of the file system at that point.

> 文件可以通过半打简单的系统调用来创建、读取、写入和删除。几位比特定义的访问控制足以满足大多数用途。可移动的存储设备，如磁盘，可以挂载到文件系统上，从而使其内容在逻辑上成为文件系统的一部分。

Naturally, there are some irregularities. Devices appear in the file system, which is a simplification, but operations on them, especially terminals, have special cases and an interface that remains messy even today.

> 自然，有一些不规则。设备出现在文件系统中，这是一种简化，但对它们的操作，特别是终端，有特殊情况，其接口即使到今天仍然很乱。

What I've described here is the logical structure of the file system. There are plenty of ways to implement this model, and in fact modern systems support a wide variety of implementations, all presenting the same interface but with different code and internal data structures to make it work. If you look at your computer, you will see multiple devices that use this model: the hard drive, USB thumb drives, SD cards, cameras, phones, and so on. The brilliance of Unix was in choosing an abstraction that was general enough to be remarkably useful, yet not too costly in performance.

> 这里描述的是文件系统的逻辑结构。有很多实现这种模型的方法，事实上，现代系统支持各种各样的实现，所有的实现都提供相同的接口，但是使用不同的代码和内部数据结构来实现。如果你看看你的电脑，你会看到很多使用这种模型的设备：硬盘，USB 闪存盘，SD 卡，相机，手机等等。Unix 的伟大之处在于选择了一种足够通用而又非常有用的抽象，但是性能成本不高。

A _high-level implementation language_, for user programs of course, but also for the operating system itself. The idea was not new; it had been tried

> 一种*高级实现语言*，当然是为用户程序，也为操作系统本身。这个想法并不新颖；它已经尝试过了。

[]{#index_split_001.html#p181}CHAPTER 9: LEGACY 167

in Multics and a couple of earlier systems, but the time and the languages were not quite ready. C was much more suitable than its predecessors, and it led to portability of the operating system. Where once there were only proprietary operating systems from hardware manufacturers, often with their own proprietary languages, Unix became an open and widely understood standard and then a commodity: the system could be used on all computers with only minor changes. Customers were no longer locked in to specific hardware, and manufacturers no longer had to develop their own operating systems or languages.

> 在 Multics 和一些早期的系统中，但时间和语言还不太成熟。C 比其前辈更合适，这导致了操作系统的可移植性。曾经只有硬件制造商提供的专有操作系统，通常有自己的专有语言，而 Unix 成为一个开放的、广泛理解的标准，然后成为一种商品：只需做一些小的改动，系统就可以在所有计算机上使用。客户不再被锁定在特定的硬件上，制造商也不再需要开发自己的操作系统或语言。

The _user-level programmable shell_, with control-flow statements and easy I/O redirection, made it possible to program by using programs as building blocks. As the shell's programming capabilities grew, it became another high-level language in the programmer's toolbox. And because it was a user-level program, not part of the operating system, it could be improved on and replaced by anyone with a better idea. The evolution from the original Unix shell through PWB, the Bourne shell and Bill Joy's csh to today's prolifera-tion illustrates the benefits, and of course some of the drawbacks---it's all too easy for incompatible versions to multiply.

> 用户级可编程 Shell，具有控制流语句和简单的 I/O 重定向功能，使得可以通过使用程序作为构建模块来编程。随着 Shell 编程能力的增强，它成为程序员工具箱中的另一种高级语言。而且由于它是一个用户级程序，而不是操作系统的一部分，它可以被任何有更好想法的人改进和取代。从最初的 Unix Shell 到 PWB、Bourne Shell 和 Bill Joy 的 csh 到今天的繁荣，这些进化都说明了它的好处，当然也有一些缺点——不兼容的版本太容易增多了。

_Pipes_ are the quintessential Unix invention, an elegant and efficient way to use temporary connections of programs. The notion of streaming data through a sequence of processing steps is natural and intuitive, the syntax is exceptionally simple, and the pipe mechanism fits perfectly with the collection of small tools. Pipes do not solve all connection problems, of course, but the fully general non-linear connections of Doug McIlroy's original concept do not show up often in practice; linear pipelines are almost always good enough.

> 管道是 Unix 发明的经典，是一种优雅而高效的方式来使用程序之间的临时连接。通过一系列处理步骤来流式传输数据的概念是自然而直观的，语法也非常简单，管道机制与小工具的集合完美契合。当然，管道并不能解决所有的连接问题，但是 Doug McIlroy 原始概念中完全通用的非线性连接在实践中并不常见；线性管道几乎总是足够好。

The notion of _programs as tools_ and using them in composition is characteristic of Unix. Writing small programs that each do one thing well, rather than large and monolithic programs that try to do many things, has many benefits. Certainly there are times when monoliths make sense, but there are strong advantages to a collection of small(ish) programs that ordinary users can combine in novel ways.

> 视程序为工具并将其用于作曲是 Unix 的特征。编写小程序，每个程序只做一件事，而不是大而单调的程序，试图做很多事情，具有许多好处。当然，有时大型程序是有意义的，但是普通用户可以以新颖的方式组合一系列小程序，这具有很强的优势。

In effect, this approach is modularization at the level of whole programs, parallel to modularization at the level of functions within a program. In both cases, the approach amounts to a kind of divide and conquer, since the individual components are smaller and don't interact with each other. It also permits a mix-and-match functionality that is hard to achieve with big programs that try to do too many different things in a single package.

> 实际上，这种方法是整个程序的模块化，与程序内部的函数模块化并行。在这两种情况下，该方法都相当于一种分治法，因为单个组件更小，它们之间不会相互影响。它还允许实现混合和匹配功能，这是通过尝试在单个软件包中完成太多不同任务而难以实现的。

[]{#index_split_001.html#p182}168 CHAPTER 9: LEGACY

_Ordinary text is the standard data format_. The pervasive use of text turns out to be a great simplification. Programs read bytes, and if they are intended to process text, those bytes will be in a standard representation, generally lines of varying length, each terminated with a newline character. That doesn't work for everything, but pretty much anything can use that representation with little penalty in space or time. As a result, all those small tools can work on any data, individually or in combination.

> 普通文本是标准数据格式。文本的普遍使用被证明是一个很大的简化。程序读取字节，如果它们旨在处理文本，那么这些字节将以标准表示形式表示，通常是长度不一的行，每行以换行符结束。这并不适用于所有情况，但几乎所有情况都可以在空间或时间上没有太大的惩罚。因此，所有这些小工具都可以单独或结合使用任何数据。

It's interesting to speculate about how differently things might have turned out if Unix had been developed in a world with punch cards instead of Teletypes. Punch cards practically force a world-view that everything comes in 80-character chunks, with information most often located in fixed fields within the chunks.

> 有趣的是推测，如果 Unix 是在一个用穿孔卡而不是电传打字机发展的世界中，事情会有多么不同。穿孔卡实际上迫使人们把世界视为一切都是 80 个字符的块，信息通常位于这些块中的固定字段中。

_Programs that write programs_ is a powerful idea. Much of the progress that we have made in computing has been through mechanization---getting the computer to do more of the work for us. It's hard to write programs by hand, so if you can get a program to write them for you, it's a big win. It's way easier, and the generated programs are more likely to be correct.

> 程序写程序这个想法很强大。我们在计算机领域取得的进步很大程度上都是通过机械化实现的——让计算机为我们做更多的工作。手工编写程序很难，所以如果你能让一个程序来为你写程序，这将是一个很大的胜利。这样做更容易，而且生成的程序更可能是正确的。

Compilers are of course an old example, but at a higher level, Yacc and Lex are excellent examples of generating code to create programming languages. Tools for automation and mechanization, like shell scripts and makefiles, are in effect programs that create programs. These tools are still widely used today, sometimes in the form of very large configuration scripts and makefile generators that accompany the source code distributions of languages like Python and compilers like GCC.

> 编译器当然是一个古老的例子，但在更高的层次上，Yacc 和 Lex 是生成代码以创建编程语言的优秀例子。自动化和机械化的工具，如 shell 脚本和 makefile，实际上是创建程序的程序。这些工具今天仍然被广泛使用，有时以 Python 和 GCC 等语言的源代码分发附带的非常大的配置脚本和 Makefile 生成器的形式。

_Specialized languages_, today often called little languages, domain-specific languages, or application-specific languages. We tell computers what to do by using languages. For most programmers, that means general-purpose languages like C, but there are a host of more specialized languages that focus on narrower domains.

> 特殊语言，如今通常被称为小语言、领域特定语言或应用特定语言。我们通过使用语言来告诉计算机该做什么。对于大多数程序员来说，这意味着像 C 这样的通用语言，但也有许多更专业的语言专注于更窄的领域。

The shell is a good example: it's meant for running programs, and it's very good at that, but you would not want to use it to write a browser or a video game. Specialization is an old idea, of course; the earliest high-level languages aimed at specific targets, for instance Fortran at scientific and engineering computation, and Cobol at business data processing. Languages that tried too early for too broad a range of applicability have sometimes foundered; PL/I is an instance.

> 贝壳就是一个很好的例子：它是用来运行程序的，而且非常擅长这一点，但是你不会想要用它来编写浏览器或者视频游戏。专业化是一个古老的想法，当然，最早的高级语言是针对特定目标的，例如 Fortran 针对科学和工程计算，Cobol 针对商业数据处理。尝试太早处理太广泛的应用程序的语言有时会失败；PL / I 就是一个例子。

Unix has a long tradition of special-purpose languages, well beyond the shell. The document preparation tools that are close to my heart are good examples, but so are calculators, circuit design languages, scripting

> Unix 有一个悠久的专用语言传统，远远超出了 shell。我心中最亲密的文档准备工具是一个很好的例子，但计算器、电路设计语言和脚本也是如此。

[]{#index_split_001.html#p183}CHAPTER 9: LEGACY 169

languages, and the ubiquitous regular expressions. One of the reasons there were so many languages is the development of tools that enabled non-experts to create them. Yacc and Lex are the primary examples here, and they are specialized languages in their own right.

Of course, not all languages need to be high-tech to be useful. Steve Johnson built the first version of the at command in an evening:

> 当然，并不是所有的语言都需要高科技才能有用。史蒂夫·约翰逊在一个晚上就构建了 at 命令的第一个版本。

"Unix had a way of scheduling jobs to be run 'out of hours' so that long jobs wouldn't interfere with peoples' work (remember, there were a dozen or so people sharing the Unix machine). To cause a job to run later, you needed to edit a system file and fill in a table of information in a rather obscure format. I was attempting this feat one day and heard myself muttering 'I want this job to run at 2AM.' Suddenly, I realized that the information about what to do could be captured in a simple syntax: 'at 2AM run_this_command.' I hacked together a version in a couple of hours and advertised it in the 'message of the day'

> Unix 有一種安排工作在非工作時間執行的方式，這樣長時間的工作就不會影響大家的工作(記得當時有十幾個人共用一台 Unix 機器)。要讓工作稍後執行，你需要編輯一個系統檔案，並以一種相當難懂的格式填入一個資訊表。有一天，我正在嘗試這項壯舉，聽到自己在嘟囔：「我想要這個工作在凌晨兩點執行。」突然，我意識到關於要做什麼的資訊可以用一個簡單的語法來捕捉：「凌晨兩點執行*這個*指令。」我在兩個小時內馬上把它修改出來，並在「每日訊息」中宣傳了它。

file the next morning."

The at command is still used 40-plus years later, with not many changes.

Like a number of other languages, the syntax is a sort of stylized English based on how we say things aloud.

> 像其它許多語言一樣，語法是一種基於我們口頭表達方式的簡化英語風格。

_The Unix philosophy_, a style of programming, of how to approach a computing task, was summarized by Doug McIlroy in his foreword to the special issue of the _Bell Labs Technical Journal_ on Unix, in July 1978: (i) Make each program do one thing well. To do a new job, build afresh rather than complicate old programs by adding new "features."

> Unix 哲学，一种编程风格，以及如何处理计算任务的方式，由 Doug McIlroy 在 1978 年 7 月的 Unix 特刊 Bell Labs Technical Journal 的序言中总结概括：(i)让每个程序做一件很好的事情。为了完成一项新任务，要重新构建，而不是通过添加新的“功能”来使旧程序变得复杂。

\(ii\) Expect the output of every program to become the input to another, as yet unknown, program. Don't clutter output with extraneous information. Avoid stringently columnar or binary input formats. Don't insist on interactive input.

> 请期望每个程序的输出成为另一个尚未知晓的程序的输入。不要在输出中添加多余的信息。避免严格的列式或二进制输入格式。不要坚持使用交互式输入。

\(iii\) Design and build software, even operating systems, to be tried early, ideally within weeks. Don't hesitate to throw away the clumsy parts and rebuild them.

> \(iii\) 尽早设计和构建软件，甚至操作系统，尝试一下，最好是在几周内。不要犹豫，把笨拙的部分扔掉，重新构建它们。

\(iv\) Use tools in preference to unskilled help to lighten a programming task, even if you have to detour to build the tools and expect to throw some of them out after you've finished using them.

> 使用工具而不是无经验的帮助来减轻编程任务，即使你不得不回避来构建工具，并预期在使用完后抛弃一些工具。

These are maxims to program by, though not always observed. One example: the cat command that I mentioned in Chapter 3. That command

> 这些是编程的格言，尽管并不总是遵守。一个例子：我在第 3 章中提到的 cat 命令。

[]{#index_split_001.html#p184}170 CHAPTER 9: LEGACY

did one thing, copy input files or the standard input to the standard output.

> 将一件事做好，将输入文件或标准输入复制到标准输出。

Today the GNU version of cat has (and I am not making this up) 12

options, for tasks like numbering lines, displaying non-printing characters, and removing duplicate blank lines. All of those are easily handled with existing programs; none has anything to do with the core task of copying bytes, and it seems counter-productive to complicate a fundamental tool.

> 这些任务，如编号行、显示非打印字符和删除重复的空行，都可以使用现有的程序轻松处理；这些都与复制字节的核心任务没有任何关系，而且在复杂化一个基本工具上似乎是适得其反的。

The Unix philosophy certainly doesn't solve all the problems of programming, but it does provide a useful guide for approaching system design and implementation.

> Unix 哲学肯定不能解决所有的编程问题，但它可以为接近系统设计和实施提供有用的指导。

**9.2 Organization**

I believe that another large component of the success of Unix was due to non-technical factors, like the managerial and organizational structure of Bell Labs, the social environment of 1127, and the flow of ideas across a group of talented people working on diverse problems in a collegial environment.

> 我相信 Unix 的成功另一个重要因素是由于非技术因素，比如贝尔实验室的管理和组织结构、1127 的社会环境以及一群有才华的人在一个同事的环境下解决不同问题时交流的思想流动。

These are harder to assess than technical notions, so this is necessarily a more subjective view. As with the previous section, most of these have been mentioned earlier.

> 这些比技术概念更难评估，因此这是一个更加主观的观点。与前一节一样，其中大多数已经在前面提到过。

A _stable environment_ is crucial: money, resources, mission, structure, management, culture---all should be consistent and predictable. As described in Chapter 1, Bell Labs research was a large operation inside a large development organization within a large corporation with a long history and a clear mission: universal service. The long-term Bell Labs goal of continuously improving telephone service meant that researchers could explore ideas that they thought were important, for long periods, even years, without having to justify their efforts every few months. There was oversight, of course, and anyone who worked on a project for several years without producing anything would be encouraged to change something. Occasionally, someone was eased out of research or out of the company entirely, but in my 15 years in management, I remember only a handful of cases.

> 稳定的环境至关重要：金钱、资源、使命、结构、管理、文化 - 都应该是一致而可预测的。正如第一章所描述的，贝尔实验室的研究是一个大型开发组织内部的大型运营，在一个具有悠久历史和明确使命的大公司内：普及服务。贝尔实验室持续改善电话服务的长期目标意味着研究人员可以探索他们认为重要的想法，长期甚至几年，而不必每隔几个月就要为自己的努力进行辩护。当然有监督，任何在一个项目上工作了几年却没有任何成果的人都会受到鼓励去改变一些东西。偶尔，有人会被轻松地从研究中淡出或者从公司完全淡出，但在我 15 年的管理经验中，我只记得几个案例。

Funding was assured, and working-level researchers did not have to think about money, nor did it concern me even when I was a department head.

> 资金得到保证，工作层面的研究人员不必考虑金钱问题，即使我是部门主管的时候也不会担心这个问题。

Certainly at some level someone did worry about such matters, but not the people doing the research. There were no research proposals, no quarterly progress reports, and no need to seek management approval before working on something. Somewhere into my time as department head, I did start to have to generate semi-annual reports on activities in my department, and for that I solicited a paragraph from each person. These were gathered for information only, howev er, not for evaluating performance.

> 毫无疑问，有人在某些层面上会担心这些问题，但不是做研究的人。没有研究建议，没有季度进展报告，也不需要在开展工作前征求管理层的批准。在我担任系主任的时候，我确实开始需要每半年生成一份有关我系活动的报告，为此我向每个人征求了一段话。然而，这些只是收集信息，而不是用来评估绩效。

There were

[]{#index_split_001.html#p185}CHAPTER 9: LEGACY 171

occasional periods when travel was scrutinized more carefully---we might be limited to one or two conferences a year, perhaps---but for the most part, if we needed to buy equipment or make a trip, money was available without much question.

> 偶尔会有一些时期旅行会受到更严格的审查——我们可能一年只能参加一两次会议，也许，但大多数情况下，如果我们需要购买设备或出行，资金就可以毫无疑问地拿到。

_Problem-rich environment_. As Dick Hamming said, if you don't work on important problems, it's unlikely that you'll do important work. But almost any topic had the potential to be important and relevant to AT&T's communications mission. Computer science was a new field, with plenty of ideas to explore on both theoretical and practical fronts, and of course the interplay between theory and practice was particularly fruitful. Language tools and regular expressions are good examples.

> 富有问题的环境。正如 Dick Hamming 所说，如果你不解决重要的问题，你很难做出重要的工作。但几乎任何主题都有可能与 AT&T 的通信使命相关重要而相关。计算机科学是一个新领域，有很多理论和实践方面可以探索的想法，当然理论与实践之间的交互尤其富有成果。语言工具和正则表达式就是很好的例子。

Within AT&T, the use of computers was exploding, and Unix was a big part of that, especially in systems for operations support, as seen with the Programmer's Workbench. The mainline telephone business was changing too, as electro-mechanical telephone switches gav e way to computer-controlled electronic switching. Again, this was a source of interesting data and projects to work on, and often to contribute as well. One downside: most of the switching work was done at very large development divisions in Indian Hill (Napierville, Illinois), so collaboration often required trips to Chicago.

> 在 AT&T 内部，计算机的使用正在爆炸，Unix 是其中的一个重要组成部分，尤其是在运营支持系统中，例如程序员工作台。主线电话业务也在发生变化，电力机械电话交换机让位于电脑控制的电子交换机。这也是一个有趣的数据和项目可供工作，并经常做出贡献。不利之处是，大多数交换工作都是在印度山(纳皮尔维尔，伊利诺伊州)的大型开发分部完成的，因此协作通常需要前往芝加哥。

Distance is hard to overcome, and is still an issue today. Even with excellent video conferencing, there is no substitute for having your collaborators next door and your stable of experts nearby.

> 距离很难克服，今天仍然是一个问题。即使有出色的视频会议，也无法代替有你的合作伙伴在隔壁，以及你的专家附近。

Bell Labs scientists were also expected to be part of the academic research community, another source of research problems and insights, and to keep up with what was going on in other industrial research labs like Xerox PARC and IBM Watson. We attended the same conferences, published in the same journals, and often collaborated with academic colleagues, with sabbaticals in both directions. For example, I spent the fall of 1996

> 研究人员也期望贝尔实验室的科学家成为学术研究社区的一部分，这是另一个研究问题和见解的来源，并且要跟上施乐 PARC 和 IBM Watson 等其他工业研究实验室正在进行的工作。我们参加同样的会议，发表在同一期刊上，经常与学术同事合作，双方都有调休假期。例如，我在 1996 年秋季度进行了调休。

teaching at Harvard, with the full support of Bell Labs; they even paid my salary, so Harvard got a freebie. The same was true in the academic year 1999-2000 at Princeton.

> 在哈佛教学，得到贝尔实验室的全力支持；他们甚至支付了我的薪水，所以哈佛得到了一份免费的东西。1999-2000 学年在普林斯顿也是如此。

In addition to internal courses, any number of colleagues taught at universities. It was easily arranged for nearby schools like Princeton, NYU, Columbia and West Point, and not much harder for extended visits to places further away: Ken Thompson spent a year at Berkeley, Rob Pike spent a year in Australia, Doug McIlroy spent a year at Oxford. External visibility was important for recruiting as well as for generally keeping up with the field.

> 除了内部课程，许多同事都在大学教书。在附近的学校如普林斯顿，纽约大学，哥伦比亚和西点军校都很容易安排，而到远处的地方也不难：肯·汤普森在伯克利大学待了一年，罗布·派克在澳大利亚待了一年，道格·麦克伊尔罗在牛津大学待了一年。外部知名度对招聘以及保持与领域的联系都很重要。

Secretive companies had a harder time attracting talent, something that appears to still be true today.

> 秘密性公司更难吸引人才，这一现象似乎至今仍然成立。

[]{#index_split_001.html#p186}172 CHAPTER 9: LEGACY

_Hire the best._ One resource was very carefully managed: hiring. In 1127, we typically could only hire one or two people a year, and almost always young ones, so hiring decisions were made very cautiously, perhaps too much so. This is of course a familiar problem in university departments as well. It is often unclear whether to go after a star in a particular field, or someone else who is broadly talented; as Steve Johnson once put it, should we be hiring athletes or first basemen? My preference has been for people who are really good at what they do, without worrying too much about specifically what it is.

> 请雇用最优秀的人才。一个资源非常谨慎地管理：招聘。在 1127 年，我们通常一年只能招聘一到两个人，而且几乎总是年轻人，因此招聘决定是非常谨慎的，也许太谨慎了。这当然也是大学部门经常遇到的问题。通常不清楚是去聘请某一领域的明星，还是其他有广泛才能的人；正如史蒂夫·约翰逊曾经说过的，我们是应该聘请运动员还是一垒手？我的偏好是对那些真正擅长自己所做的事情的人，而不用太担心它到底是什么。

In any case, Bell Labs worked hard to try to attract good people.

Recruiters from Research visited major computer science departments once or twice a year, looking at PhD candidates. When someone promising was identified, he or she was invited to visit for a couple of days, and would normally be interviewed by several groups, not just 1127. The programs like GRPW and CRFP, for women and minorities, that I mentioned in Chapter 1

> 研究部门的招聘人员每年会访问一两次主要的计算机科学系，观察博士生候选人。当发现有希望的人时，他们会被邀请来参观几天，通常会接受来自不止 1127 组的面试。我在第一章中提到的 GRPW 和 CRFP 等针对女性和少数族裔的项目，也会被考虑。

were a big help here as well, since they provided first-rate candidates for permanent employment who had already spent significant time with us during their graduate school years.

> 他们也在这里提供了很大的帮助，因为他们提供了优秀的永久性就业候选人，他们在毕业学年期间已经在我们这里度过了相当长的时间。

We used our own researchers as recruiters, not professional career recruiters. Someone doing active research of their own could have technical conversations with faculty and students, would always learn something useful, and could leave a positive impression of the company.

> 我们使用自己的研究人员作为招聘人员，而不是专业的职业招聘人员。有人可以进行自己的积极研究，可以与教师和学生进行技术交流，总会学到有用的东西，并且可以给公司留下积极的印象。

Relationships with universities tended to be long term. I was the recruiter for Carnegie-Mellon in Pittsburgh for at least 15 years. Twice a year I would spend several days at CMU, talking with computer science faculty about their research and with students who might be interested in working at Bell Labs.

> 与大学的关系往往是长期的。我在匹兹堡的卡内基梅隆大学担任招聘人员至少 15 年。每年两次，我会在 CMU 呆上几天，与计算机科学教师讨论他们的研究，以及与可能有兴趣在贝尔实验室工作的学生交谈。

I made good friends in this way even if they didn't join the Labs. Recruiting was very competitive, since good universities were hiring actively, as were top industrial research labs, so my personal list of the ones who got away is long. I was certainly right to want to recruit most of them; they've been a highly successful group.

> 我们通过这种方式结交了很多好朋友，即使他们没有加入实验室。招聘竞争非常激烈，因为一些优秀的大学正在积极招聘，而一些顶尖的工业研究实验室也在招聘，所以我的失去的人名单很长。我当然有理由想要招聘他们中的大多数；他们已经是一个非常成功的团队了。

_Technical management._ Managers have to understand the work they manage. Management in Bell Labs research was technical all the way to the top, so they had a solid understanding of the work both within their own organizations and across others. Department heads were expected to know what their people were doing in real detail, not for the purpose of arguing how great it was, but for being able to explain it to others and helping to make connections. At least in 1127 there were no turf wars; it was a cooperative and non-competitive environment where management supported their people, often collaborated, and never competed. I'm not sure that this was a universal

> 技术管理。管理者必须理解他们管理的工作。贝尔实验室的研究中，管理一直以技术的方式发展到最高水平，因此他们对自己组织内部和其他组织的工作都有扎实的了解。部门负责人需要弄清楚他们的人在做什么，而不是为了争论多么伟大，而是为了能够向其他人解释它，并帮助建立联系。至少在 1127 年，没有地盘之争；这是一个合作而不竞争的环境，管理层支持他们的人，经常进行合作，从不竞争。我不确定这是普遍的。

[]{#index_split_001.html#p187}CHAPTER 9: LEGACY 173

experience, but it's worth aiming for, and doing it well should be part of the reward mechanism for managers.

> 经验是值得去追求的，而且将其做好应该成为管理者的奖励机制的一部分。

Although Bell Labs management was technically knowledgeable at all levels, AT&T's upper management seemed removed from new technology and slow to adapt to change. For instance, in the early 1990s, Sandy Fraser, at that time the director of 1127, told AT&T executives that networking improvements would mean that long distance prices would come down from their then-current ten cents per minute to one cent a minute, and he was laughed at. Today's price is pretty close to zero cents per minute; Sandy was too conservative.

> 尽管贝尔实验室的管理层在各个层面都具备技术知识，但 AT&T 的高层管理人员似乎与新技术脱节，对变化改变比较慢。例如，在 1990 年代初，当时的 1127 负责人桑迪·弗雷泽(Sandy Fraser)告诉 AT&T 高管，网络改进意味着长途电话价格将从当时的每分钟十美分降低到每分钟一美分，但他遭到嘲笑。今天的价格接近于零美分每分钟；桑迪的预测太保守了。

_Cooperative environment._ The size and scale of Bell Labs meant that for almost any technical area, there were multiple experts, often world leaders in their field. Furthermore the culture was strongly cooperative and helpful. It was absolutely standard procedure to walk into someone's office and ask for help; most often the person being asked would drop everything to assist.

> 在贝尔实验室，由于规模庞大，几乎每一个技术领域都有多位专家，往往是该领域的世界领袖。此外，这里的文化也非常合作有助。走进别人的办公室寻求帮助是完全正常的程序；大多数时候，被询问的人会放下手头的事情来帮忙。

There was also a superb technical library, open 24 hours a day, with subscrip-tions to a large collection of journals, and remote access to other libraries; it was equivalent to a university library but focused on science and technology.

> 在那里还有一个极好的技术图书馆，每天 24 小时开放，订阅了大量的期刊，还可以远程访问其他图书馆；它相当于一所大学图书馆，但专注于科学技术。

For many people in 1127, the closest collection of relevant experts was the Mathematics Research Center, 1121, which had extraordinary mathematicians, including Ron Graham, Mike Garey, David Johnson, Neil Sloane, Peter Shor, Andrew Odlyzko---the list just goes on. John Tukey, arguably the world's foremost statistician at the time (and incidentally the person who coined the word "bit"), was just across the hall, and there were formidable experts on pretty much any aspect of mathematics and communications. For instance, my current Princeton colleague Bob Tarjan, who shared the Turing Aw ard in 1986, was in the math center.

> 对于 1127 年的许多人来说，最近的相关专家群体是 1121 年的数学研究中心，其中拥有杰出的数学家，包括罗恩·格雷厄姆、迈克·加里、大卫·约翰逊、尼尔·斯隆、彼得·肖尔、安德鲁·奥德利斯科——名单可以一直列下去。当时可以说是世界上最杰出的统计学家约翰·图基(顺便提一下，他还是“位”这个词的发明者)就在隔壁，而几乎任何数学和通信方面都有强大的专家。例如，我目前在普林斯顿大学的同事鲍勃·塔詹(Bob Tarjan)就在数学中心，他 1986 年与图灵一起获得了图灵奖。

They were always ready to help, and not always just on technical matters.

For example, in addition to being an outstanding mathematician, Ron Graham was an expert juggler and a former president of the International Jugglers' Association; he even had a net in his office to catch dropped juggling balls before they hit the floor. Ron used to say that he could teach anyone to juggle in 20 minutes. I fear that it wasn't true in my case, but an hour of one-on-one instruction (in his office!) did get me over the hump, and I still have the lacrosse balls that he gav e me to practice with.

> 例如，除了是一位杰出的数学家，罗恩·格雷厄姆还是一位专家杂耍者，也是国际杂耍者协会的前任主席；他甚至在他的办公室里放了一张网，以捕获掉落的杂耍球。罗恩曾经说他可以在 20 分钟内教任何人杂耍。我担心这不是真的，但是一小时的一对一指导(在他的办公室里！)确实让我跨越了这个障碍，我仍然拥有他给我的来练习的长曲棍球。

_Fun._ It's important to enjoy your work and the colleagues that you work with. 1127 was almost always a fun place to be, not just for the work, but the esprit of being part of a remarkable group. Since there were no local options other than the company cafeteria, lunchtime provided a mix of social and

> *有趣的。*重要的是享受你的工作和你一起工作的同事。1127 几乎总是一个有趣的地方，不仅仅是因为工作，还因为成为一个不同寻常的团队的一部分。由于当地除了公司自己的餐厅以外没有其他选择，午餐时间提供了社交和社交的混合。

[]{#index_split_001.html#p188}174 CHAPTER 9: LEGACY

technical discussions. While the Unix room crowd normally ate at 1PM, a larger group routinely ate at 11AM. Topics included everything from technical ideas both big and small to politics with no holds barred; these would often be continued during a walk around the Bell Labs property.

> 技术讨论。虽然 Unix 房间的人通常在下午 1 点吃饭，但一个更大的团体经常在上午 11 点吃饭。议题包括从大到小的技术想法到毫不留情的政治；这些往往会在 Bell Labs 财产周围的散步中继续下去。

Center members played pranks on each other, and took perhaps undue pleasure from pushing back against the bureaucracy that's inevitable in any big company. I'v e already mentioned disdain for badges. The various forms and procedures that we were supposed to use provided further opportunities.

> 中心成员彼此开玩笑，并从反对任何大公司必然存在的官僚主义中获得了过度的快乐。我已经提到对徽章的不屑一顾。我们应该使用的各种形式和程序提供了更多的机会。

For example, security staff would ticket cars that were violating some or other rule. One spring day, Mike Lesk found a blank ticket, which he put on the windshield of a colleague's car with the violation listed as "Failure to remove ski-rack by April 1." The colleague, not to be identified here, was actually taken in by this for a few hours.

> 例如，安全人员会开罚单给那些违反规定的汽车。一个春天，迈克·莱斯克发现一张空白的罚单，他把它放在同事汽车的挡风玻璃上，违规内容是“未在 4 月 1 日前拆除滑雪架”。这位同事，此处不便透露姓名，竟然被这件事惊呆了几个小时。

By far the most elaborate prank was played on Arno Penzias by a team of at least a dozen, led by Rob Pike and Dennis Ritchie, with the aid of professional magicians Penn and Teller. It's too long for the book, but Dennis tells the Labscam story at _[www.bell-labs.com/usr/dmr/www/labscam.html](http://www.bell-labs.com/usr/dmr/www/labscam.html)_, and the video is at _[www.youtube.com/watch?v=if9YpJZacGI](http://www.youtube.com/watch?v=if9YpJZacGI)_. I'm in the credits at the end as a gaffer, which is accurate---much duct tape was involved.

> 最复杂的恶作剧由至少十二人组成的团队，由 Rob Pike 和 Dennis Ritchie 带领，在 Penn 和 Teller 专业魔术师的帮助下玩到了 Arno Penzias 身上。由于太长，无法写入书中，但 Dennis 在[www.bell-labs.com/usr/dmr/www/labscam.html](http://www.bell-labs.com/usr/dmr/www/labscam.html)上讲述了 Labscam 的故事，视频在[www.youtube.com/watch?v=if9YpJZacGI](http://www.youtube.com/watch?v=if9YpJZacGI)上。我在片尾的字幕中被列为灯光师，这是准确的——涉及到了大量的胶带。

There was no free food at Bell Labs (that's a modern perk that I would have appreciated back in the day), but somehow we managed free coffee; management quietly paid for it.

> 当时贝尔实验室没有免费食物(那是我当时会很喜欢的一种现代优惠)，但是我们设法免费拿到咖啡；管理层悄悄地付钱买的。

People would leave offerings in the Unix room for the common good.

Someone found a supply of 10 kg (22 lb) blocks of high-quality chocolate and left them for people to chip away at it. The food wasn't always up to that standard, however:

> 有人发现了一批 10 公斤(22 磅)的高品质巧克力块，留给人们削减。然而，食物并不总是达到这样的标准：

"Somebody brought in a bag of objects labeled in Chinese. All of us bit into one of them and gav e up. We then noticed that they were disappearing: it turned out that \[redacted\] was eating them. Near the end of the bag somebody who knew Chinese told us that the instructions on the bag said to soak for an hour in boiling water before eating."

> 有人带来一袋用中文标注的物品，我们每个人都咬了一个，然后就放弃了。后来我们发现它们正在消失：原来是[被删除的内容]在吃它们。在袋子快要用完的时候，有个会说中文的人告诉我们，袋子上写着要先放入沸水里浸泡一小时才能吃。

At the same time, there was zero, or even neg ative, enthusiasm for the kinds of team-building exercises that one often sees today. Most of us saw them as artificial, pointless, and a waste of time.

> 同时，对于现今经常看到的团队建设活动，没有任何热情，甚至是负面的情绪。我们大多认为这些活动是人为的、毫无意义的，是浪费时间的。

It takes effort to build and maintain an organization whose members like and respect each other, and who enjoy each other's company. This can't be created by management fiat, nor by external consultants; it grows organically from the enjoyment of working together, sometimes playing together, and appreciating what others do well.

> 需要努力才能建立并维护一个成员彼此喜欢和尊重，并享受彼此公司的组织。这不能由管理者的命令创造，也不能由外部顾问创造；它是从一起工作的乐趣，有时一起玩耍，以及欣赏他人做得好的事情中有机地生长而来的。

[]{#index_split_001.html#p189}CHAPTER 9: LEGACY 175

**9.3 Recognition**

Unix and its primary creators, Ken Thompson and Dennis Ritchie, have been recognized for their contributions. When they won the ACM Turing Aw ard in 1983, the award selection committee said

> Unix 及其主要创造者 Ken Thompson 和 Dennis Ritchie 因其贡献而受到认可。当他们在 1983 年获得 ACM 图灵奖时，评奖委员会说

"The success of the Unix system stems from its tasteful selection of a few key ideas and their elegant implementation. The model of the Unix system has led a generation of software designers to new ways of thinking about programming. The genius of the Unix system is its framework, which enables programmers to stand on the work of others."

> Unix 系统的成功源于它精挑细选的几个关键理念及其优雅的实现。 Unix 系统的模型引领了一代软件设计师去思考编程的新方式。 Unix 系统的天才之处在于它的框架，使程序员能够依靠其他人的工作取得成功。

They also received the US National Medal of Technology in 1999. Figure 9.1 is a picture with President Bill Clinton, one of the few occasions where either Ken or Dennis wore a suit and tie. Bell Labs was for us at least a very informal environment by the standards of the time. As Dennis said in his online biography, "Ken's virtual coat-tails are long. I'm one of the few, besides Bonnie T., who has seen him wear a real coat (and even black tie) on more than one occasion." I personally have nev er seen Ken dressed up at all.

> 他们在 1999 年还获得了美国国家技术奖章。图 9.1 是一张与比尔·克林顿总统合影的照片，这是肯和丹尼斯很少穿西装领带的少数几次机会之一。在当时的标准来看，贝尔实验室对我们来说至少是一个非常非正式的环境。正如丹尼斯在他的在线传记中所说，“肯的虚拟马尾很长。除了邦妮·T.外，我是少数几个看到他穿真正的外套(甚至是黑领礼服)不止一次的人。”我个人从来没有看到肯穿着正式的衣服。

Other awards include membership in the National Academy of Engineering, and the Japan Prize in Information and Communications in 2011, for which the citation reads

> 其他奖项包括入选美国国家工程院，以及 2011 年获得日本信息与通信奖，奖项题词如下：

"Compared to other operating systems prevailing around that time, their new and advanced OS was simpler, faster and featured a user-friendly hierarchical file system. Unix was developed in conjunction with the programming language, C, which is still widely used for writing OS, and dramatically improved the readability and portability of Unix source code. As a result, Unix has come to be used by various systems such as embedded systems, personal computers, and super computers."

> 相比于当时普遍存在的其他操作系统，他们的新型先进操作系统更加简单、快速，并具有用户友好的分层文件系统。Unix 是与编程语言 C 一起开发的，C 语言仍然被广泛用于编写操作系统，它大大改善了 Unix 源代码的可读性和可移植性。因此，Unix 已经被嵌入式系统、个人计算机和超级计算机等各种系统所使用。

"Unix was also a major driving force behind the development of the Internet. University of California, Berkeley dev eloped Berkeley Software Distribution (BSD), an extended version of Unix that was implemented with the Internet protocol suite TCP/IP. The development was based on the sixth edition of Unix that Bell Labs distributed along with its source code to universities and research institutions in 1975, which led to the beginning of an 'open source' culture. BSD Unix helped the realization of the Internet."

> Unix 是互联网发展的主要驱动力之一。加利福尼亚大学伯克利分校开发了 Berkeley 软件分发(BSD)，它是一个基于 Unix 第六版的扩展版本，该版本实现了 Internet 协议套件 TCP / IP。这项开发是基于 1975 年贝尔实验室向大学和研究机构分发的 Unix 及其源代码，这标志着“开源”文化的开始。BSD Unix 帮助实现了 Internet 的发展。

[]{#index_split_001.html#p190}![](./index-190_1.jpg){.calibre4}

176 CHAPTER 9: LEGACY

**Figure 9.1:**

Ken, Dennis, Bill, National Medal of Technology, 1999

Other forms of recognition were more informal, signs that Unix and C

had entered popular culture, like the appearance of C on the popular TV program _Jeopardy_:

> 已经进入流行文化，如在热门电视节目《危险边缘》中出现 C：

From dmr@cs.bell-labs.commailto:dmr@cs.bell-labs.com Tue Jan

7 02:25:44 2003

Subject: in case you didn't see it

On Friday night on \"Jeopardy!\", in a category called

\"Letter Perfect\" (all the answers were single letters), the \$2,000 (most difficult) question was: DEVELOPED IN THE EARLY 1970S, IT'S THE MAIN PROGRAMMING

> "字母完美"(所有答案都是单个字母)，最难的 2,000 美元问题是：在 20 世纪 70 年代初开发的，它是主要的编程语言。

LANGUAGE OF THE UNIX OPERATING SYSTEM.

and in some kind of high point for geeks, a famous scene in the 1993 movie _Jurassic Park_, where the 13-year-old Lex Murphy (Ariana Richards) says

> 让极客们兴奋不已的是，1993 年电影《侏罗纪公园》中，13 岁的莱克斯·墨菲(Ariana Richards)说过一句著名的台词：

"It's a Unix system! I know this." She navigates the file system, finds the controls for the doors, locks them, and thus saves everyone from being eaten by velociraptors (Figure 9.2).

> 她操作着 Unix 系统！我知道这个。她浏览文件系统，找到了门控制，锁上了它们，从而拯救了大家免遭迅猛龙(图 9.2)的吞噬。

Other members of Center 1127, in part thanks to the rich environment enabled by Unix, have also been recognized professionally, like the 8 other 1127 alumni who are members of the National Academy of Engineering.

> 其他中心 1127 的成員，部分得益於 Unix 所提供的豐富環境，也得到了專業肯定，比如其中 8 位 1127 校友已成為美國工程院院士。

[]{#index_split_001.html#p191}![](./index-191_1.jpg){.calibre4}

CHAPTER 9: LEGACY 177

**Figure 9.2:**

Unix in _Jurassic Park_

**9.4 Could histor y repeat?**

Could there be another Unix? Could a new operating system come out of nowhere and take over the world in a few decades? I often get this question when I talk about Unix. My answer is no, at least at the moment. There will be no revolution; more likely, operating systems will continue to evolve, while carrying a great deal of Unix DNA.

> 或许会有另一个 Unix 吗？一个新的操作系统是否可以凭空出现，并在几十年内夺取世界？当我谈论 Unix 时，我经常会遇到这个问题。我的回答是，至少目前不会。不会有革命；更可能的是，操作系统将继续发展，同时带有大量的 Unix DNA。

But some analogous success could happen in other areas of computing.

There are always creative people, good management is not unheard of, hardware is very cheap, and great software is often free. On the other hand, there are few unfettered environments, industrial research is much reduced and constrained and far more short-term than it was fifty years ago, and academic research is always strapped for funds.

> 总是有富有创意的人，有好的管理是不足为奇的，硬件非常便宜，而伟大的软件往往是免费的。另一方面，几乎没有不受限制的环境，工业研究大大减少并受到限制，比五十年前短期得多，而学术研究总是资金紧张。

Nevertheless, I am optimistic, on the grounds that the great ideas come from individuals.

> 然而，我很乐观，因为伟大的想法来自个人。

For example, the number of people contributing to Unix in the early days was tiny; arguably the core was a single person, Ken Thompson, who is certainly the best programmer I have ever met, and an original thinker without peer. Dennis Ritchie, whose name is linked with Ken as the co-creator of Unix, was a vital contributor, and his C programming language, central to the

> 例如，早期参与 Unix 开发的人数非常少；可以说，核心的开发者就是一个人，他就是我见过的最优秀的程序员，也是无与伦比的原创思想家，他就是肯·汤普森。与肯共同创造了 Unix 的丹尼斯·里奇也是一个重要的贡献者，他的 C 编程语言也是 Unix 的核心。

[]{#index_split_001.html#p192}178 CHAPTER 9: LEGACY

ev olution of Unix in the early days, is still the _lingua franca_ of computing.

> Unix 在早期的演变，仍然是计算的共通语言。

It's instructive to examine the languages that programmers use every day and see how often they were originally the work of one or two people.

> 检查程序员每天使用的语言，看看它们最初是由一两个人完成的，这是一件有教育意义的事情。

Almost every major programming language is like that, including Java (James Gosling), C++ (Bjarne Stroustrup), Perl (Larry Wall), Python (Guido von Rossum), and JavaScript (Brendan Eich). It seems safe to predict that there will continue to be new languages to make programming easier and safer. It's also safe to predict that there won't be just one language, howev er---there are too many tradeoffs for a single language to serve all purposes well enough.

> 几乎每一种主要的编程语言都是这样，包括 Java(James Gosling)、C++(Bjarne Stroustrup)、Perl(Larry Wall)、Python(Guido von Rossum)和 JavaScript(Brendan Eich)。似乎可以安全地预测将会有新的语言出现来使编程更容易和更安全。也可以安全地预测不会只有一种语言——为了能够很好地满足所有用途，太多的折衷是不可能只有一种语言的。

Google, Facebook, Amazon, Twitter, Uber, and any number of other companies that went from startups to multi-billion-dollar enterprises originated with a bright idea by one or two people. There will be more of these, though it's also possible that as new ideas occur and new companies appear, they will quickly be snapped up by the existing big companies. The bright ideas may be preserved, and the inventors will be well compensated, but the big fish are likely to eat the little ones quite quickly.

> 谷歌、脸书、亚马逊、推特、优步等众多从初创公司发展成为亿万规模企业的公司，都源于一两个人的聪明想法。这类公司还会有更多，不过随着新想法的出现和新公司的诞生，它们可能很快就会被现有的大公司收购。聪明想法可能会得以保留，发明者也会得到丰厚的补偿，但大鱼很可能会很快吞掉小鱼。

Good management is another component of success. Doug McIlroy stands out here as unique, a leader of outstanding intellectual horsepower, with incomparable technical judgment, and a management style based on being one of the first users of whatever his colleagues developed. Unix itself, but also languages like C and C++, and any number of Unix tools, all profited from Doug's good taste and razor-sharp critiques. So did Unix documentation of all sorts, from the user manuals through a few dozen influential books.

> 良好的管理是成功的另一个组成部分。道格·麦克尔罗伊在这里显得独一无二，他是一位杰出的智力领袖，具有无与伦比的技术判断力，管理风格是他的同事开发的第一批用户之一。Unix 本身，还有像 C 和 C ++这样的语言，以及许多 Unix 工具，都受益于道格的精致品味和锐利的批评。从用户手册到几十本有影响力的书籍，Unix 文档也是如此。

I can attest to this personally: Doug was the outside reader on my PhD thesis in 1968, made incisive comments on all of my technical papers and books, and is still keeping me on target more than 50 years later.

> 我可以亲身证明：1968 年，道格是我的士论文的外部读者，对我所有的技术论文和书籍都做出了精辟的评论，并且 50 多年来仍然让我保持正确的方向。

Bell Labs management was technically competent, and especially so in 1127, so it could assess good work, and it was hands-off, so it didn't push particular projects or approaches. In over 30 years at the Labs I was never told what to work on. Bruce Hannay, vice president of Research after Bill Baker, said in 1981 in _Engineering and Science in the Bell System_,

> 贝尔实验室的管理技术上很有能力，尤其是在 1127 年，所以它可以评估出好的工作，而且它是自主的，所以它不会推动特定的项目或方法。在贝尔实验室的 30 多年中，我从未被告知该做什么。1981 年，在《贝尔系统的工程与科学》中，比尔·贝克尔(Bill Baker)之后的研究副总裁布鲁斯·汉纳(Bruce Hannay)说：

"Freedom of choice is of utmost importance to the research scientist, because research is an exploration of the unknown and there are no road maps to tell what course to take. Each discovery affects the future course of research and no one can predict or schedule discovery.

> 研究科学家最重要的是自由选择，因为研究是对未知的探索，没有路线图来告诉该走什么路线。每一项发现都会影响未来的研究进程，没有人能够预测或安排发现。

Thus Bell Laboratories research managers have provided the maximum possible freedom to the research staff, consistent with the institu-tional purpose. Research people have been chosen for their creative abilities and are encouraged to exercise these to the fullest."

> 因此，贝尔实验室的研究经理们为研究人员提供了最大可能的自由，与机构的目的相一致。研究人员是根据他们的创造能力进行选择的，并鼓励他们充分发挥这些能力。

[]{#index_split_001.html#p193}CHAPTER 9: LEGACY 179

One of the best examples I ever saw of this nearly absolute freedom was the work that Ken Thompson and Joe Condon did on their chess computer.

> 一个最好的例子，我曾经看到过的这种几乎绝对的自由，是肯·汤普森和乔·孔登在他们的国际象棋电脑上所做的工作。

One day Bill Baker, president of Bell Labs, brought some or other distinguished visitor to the Unix room, and Ken showed off Belle. The visitor asked why Bell Labs supported work on computer chess, since it didn't seem to have anything to do with telephones. Bill Baker answered: Belle was an experiment in special-purpose computers, it had led to the development of new circuit design and implementation tools, and it gav e Bell Labs visibility in another field. Ken didn't hav e to do any justification whatsoever.

> 一天，贝尔实验室的总裁比尔·贝克尔带着一位来宾来到 Unix 室，肯展示了 Belle。来宾问，为什么贝尔实验室要支持计算机国际象棋的研究，因为它似乎跟电话没有任何关系。比尔·贝克尔回答说：Belle 是一个专用计算机的实验，它促进了新的电路设计和实施工具的发展，而且给了贝尔实验室在另一个领域的知名度。肯根本不需要做任何辩护。

The big secret to doing good research is to hire good people, make sure there are interesting things for them to work on, take a long view, and then get out of the way. It certainly wasn't perfect, but Bell Labs research generally did this well.

> 大谜团在做好研究的关键是雇佣优秀的人才，确保有有趣的事情可供他们工作，从长远来看，然后把手边的事情交给他们去做。虽然它不是完美的，但贝尔实验室的研究通常做得很好。

Of course computing didn't exist in a technological vacuum. The invention of the transistor and then integrated circuits meant that for 50 years computing hardware kept getting smaller, faster, and cheaper at an exponential rate. As hardware got better, software became easier, and our understanding of how to create it got better as well. Unix rode the technology improvement wave, as did many other systems.

> 当然，计算机并不是技术真空中的存在。晶体管的发明，然后是集成电路的发明意味着，在 50 年里，计算机硬件以指数级的速度越来越小，越来越快，越来越便宜。随着硬件性能的提升，软件也变得更容易使用，我们对如何创建软件的理解也变得更好。Unix 乘着技术进步的浪潮，以及其他许多系统。

As I said in the Preface, Unix was probably a singularity, a unique combination of circumstances that changed the computing world. I doubt that we will see anything like it again in operating systems, but there will surely be other occasions when a handful of talented people with good ideas and a supportive environment do change the world with their inventions.

> 正如我在序言中所说，Unix 可能是一个奇迹，一个独特的环境组合，改变了计算世界。我怀疑我们在操作系统中再也不会看到类似的东西，但是当一小群有才华的人有好的想法和支持的环境时，他们的发明肯定会改变世界。

For me, Bell Labs and 1127 were a marvelous experience: a time and place with endless possibilities and a group of first-rate colleagues who made the most of them. Few are fortunate enough to have that kind of experience, the shared creation, of course, but especially the friends and colleagues with whom it was shared.

> 对我来说，贝尔实验室和 1127 是一次美妙的经历：一个充满无限可能性的时间和地点，以及一群一流的同事充分利用它们。很少有人有幸拥有这样的经历，当然是共同创造的，但尤其是和我们一起分享的朋友和同事。

"What we wanted to preserve was not just a good environment in which to do programming, but a system around which a fellowship could form. We knew from experience that the essence of communal computing \[\...\] is not just to type programs into a terminal instead of a keypunch, but to encourage close communication."

> “我们想要保留的不仅仅是一个编程的良好环境，而是一个可以形成团体的系统。我们从经验中知道，公共计算的本质不仅仅是把程序输入终端而不是打字机，而且要鼓励密切的沟通。”

Dennis Ritchie, "The Evolution of the Unix Time-sharing System,"

October 1984

[]{#index_split_001.html#p194} []{#index_split_001.html#p195}**Sources**

"The names of Ritchie and Thompson may safely be assumed to be attached to almost everything not otherwise attributed."

> 可以安全地假设里奇和汤普森的名字几乎都和除其他归属外的所有事物有关联。

"To look further afield would require a tome, not a report, and possibly a more dispassionate scholar, not an intimate participant."

> 要深入研究就需要一部巨著，而不是一份报告，可能还需要一位更加客观的学者，而不是一位亲身参与者。

Doug McIlroy, _A Research Unix Reader: Annotated Excerpts_ _from the Programmer's Manual, 1971-1986_, 1986

> Doug McIlroy，《研究 Unix 阅读：1971-1986 程序员手册的注释摘录》，1986

Much Unix history is online (though not always in a searchable form), thanks to some good luck and truly dedicated work by amateur and professional historians, such as The Unix Heritage Society and the Computer History Museum. Further material is available through interview videos and oral histories; some are contemporaneous like the various AT&T public relations efforts, and some are retrospective. This list of sources is in no way complete or comprehensive, but it will give readers who want to dig further a good start. Many of these documents can be found on the Internet.

> 许多 Unix 历史记录可以在网上找到(虽然不一定可以搜索)，这要归功于业余和专业历史学家们的好运气和不懈努力，比如 Unix 遗产协会和计算机历史博物馆。更多的材料可以通过视频采访和口述历史获得；有些是当代的，比如各种 AT&T 的公关活动，有些是回顾性的。这份资料清单不是完整或全面的，但它会给想要更深入挖掘的读者一个很好的开端。许多这些文件可以在互联网上找到。

_A History of Science and Engineering in the Bell System_ has seven volumes with nearly 5,000 pages written by members of technical staff at Bell Labs, mostly in the 1970s and 1980s. One volume deals with the relatively late advent of computing.

> 《贝尔系统科学与工程史》共有七卷，近 5000 页，由贝尔实验室的技术人员在 20 世纪 70 年代和 80 年代写成，其中一卷讲述了计算机相对较晚出现的情况。

Bell Labs maintains a sequence of short pages on the history of Unix at _s3-us-west-2.amazonaws.com/belllabs-microsite-unixhistory_.

> Bell Labs 维护了一系列关于 Unix 历史的短网页，可从*s3-us-west-2.amazonaws.com/belllabs-microsite-unixhistory*访问。

A. Michael Noll, a member of the Speech and Acoustics Research Center in the 1960s and early 1970s, has written a memoir of his time at the Labs, along with material from his role as the editor of the papers of Bill Baker; it can be found at _noll.uscannenberg.org_ along with a variety of other informative historical information. It's an excellent read for basic facts about the

> A. Michael Noll 是 1960 年代和 1970 年代语音和声学研究中心的一员，他写了一本回忆录，记录了他在实验室的时光，还有他担任比尔·贝克尔论文编辑的经历，可以在 noll.uscannenberg.org 上找到，还有各种有用的历史信息。这是一本很棒的读物，可以获取关于实验室的基本事实。

[]{#index_split_001.html#p196}182 SOURCES

Labs and what it was like in the speech and acoustics research area. Mike's memories about the collegiality and openness of Bell Labs generally accord with mine, though he feels things started to fall apart much sooner than I do, perhaps because we were in different (though organizationally adjacent) areas.

> Mike 在演讲和声学研究领域的记忆，以及他对贝尔实验室的同事情谊和开放性的看法，与我的看法基本一致，尽管他认为情况开始恶化的时间要比我早，可能是因为我们处于不同的(尽管在组织上相邻)领域。

Tom Van Vleck maintains a thorough repository of historical information about Multics at _multicians.org_.

> 汤姆·范·弗莱克在 multicians.org 上维护了一个关于 Multics 的历史信息库。

The special issue of the _Bell System Technical Journal_ on Unix in July 1978 has several fundamental papers, including an updated version of the CACM paper, Ken's "Unix Implementation," Dennis's "Retrospective," a paper by Steve Bourne on the shell, along with a paper on PWB by Ted Dolotta, Dick Haight and John Mashey.

> 《贝尔系统技术杂志》1978 年 7 月关于 Unix 的特刊包含几篇基础文章，其中包括 CACM 文章的更新版本，Ken 的《Unix 实施》，Dennis 的《回顾》，Steve Bourne 关于 Shell 的文章，以及 Ted Dolotta、Dick Haight 和 John Mashey 关于 PWB 的文章。

The special issue of the _AT&T Bell Labs Technical Journal_ on Unix in 1984 includes Dennis Ritchie's "Evolution of Unix" paper, and "Data Abstraction in C" by Bjarne Stroustrup, among other interesting articles.

> 1984 年的《AT&T 贝尔实验室技术杂志》的特刊论 Unix，包括丹尼斯·里奇的《Unix 的演变》论文和巴尔内·斯特劳斯特鲁普的《C 中的数据抽象》，以及其他有趣的文章。

Doug McIlroy's "A Research Unix Reader" is especially good for historical background; it can be found at _genius.cat-v.org/doug-mcilroy_.

> 道格·麦克尔罗伊的《研究 Unix 读者》尤其适合用于历史背景；可以在 genius.cat-v.org/doug-mcilroy 上找到。

The Unix Heritage Society, run by Warren Toomey with the help of many volunteers, has preserved versions of early Unix code and documentation; it's a great place to browse. For example, _[www.tuhs.org/Archive/Distributions/](http://www.tuhs.org/Archive/Distributions/)_

> 维克·图米(Warren Toomey)在众多志愿者的帮助下经营的 Unix 遗产协会(The Unix Heritage Society)已经保存了早期 Unix 代码和文档的版本；这是一个很棒的浏览地点。例如，[www.tuhs.org/Archive/Distributions/](http://www.tuhs.org/Archive/Distributions/)。

_Research/Dennis_v1_ has the code for the First Edition as provided by Dennis Ritchie.

> *研究/丹尼斯\_v1*拥有丹尼斯·里奇提供的第一版代码。

The late Michael Mahoney, professor of the History of Science at Princeton University, interviewed a dozen members of 1127 in the summer and fall of 1989 for an extensive oral history of Unix. Mike's raw transcripts and edited interviews are maintained by the History department at Princeton, and can be found at _[www.princeton.edu/](http://www.princeton.edu/)˜hos/Mahoney/unixhistory_. In addition to being a first-rate historian, Mike was a programmer who really understood what his subjects were talking about, so there is often significant technical depth.

> 迈克尔·马洪尼(Michael Mahoney)教授是普林斯顿大学历史科学的教授，1989 年夏秋之际，他采访了 1127 的十几名成员，进行一项关于 Unix 的广泛口述史料研究。迈克的原始记录和编辑后的采访记录由普林斯顿大学历史系维护，可在www.princeton.edu/˜hos/Mahoney/unixhistory/找到。除了是一位一流的历史学家，迈克还是一位编程能手，他真正理解他的访谈对象在谈论什么，因此经常有很深的技术内容。

Phyllis Fox, a pioneer of numerical computing and of technical women at Bell Labs, did an oral history for the Society for Industrial and Applied Mathematics (SIAM) in 2005, available at _history.siam.org/oralhisto-ries/fox.htm_; it includes a detailed description of the PORT portable Fortran libraries.

> 菲利斯·福克斯是贝尔实验室技术妇女的先驱，也是数值计算的先驱，2005 年，她为工业与应用数学协会(SIAM)做了一次口述历史，可以在*history.siam.org/oralhisto-ries/fox.htm*上找到；其中包括了一个详细的 PORT 可移植 Fortran 库的描述。

The May 2019 fireside chat with Ken Thompson at the Vintage Computer Festival East is on YouTube at _[www.youtube.com/watch?v=EY6q5dv_B-o](http://www.youtube.com/watch?v=EY6q5dv_B-o)_.

> 五月份 2019 年 Ken Thompson 在 Vintage Computer Festival East 的篝火聊天可以在 YouTube 上看到：[www.youtube.com/watch?v=EY6q5dv_B-o](http://www.youtube.com/watch?v=EY6q5dv_B-o)。

Tw o books on the early history of Unix are available for free download: _Life with Unix_ by Don Libes and Sandy Ressler (1989), and _A Quarter Cen-tury of Unix_ by Peter Salus (1994).

> 两本关于 Unix 早期历史的书籍可免费下载：Don Libes 和 Sandy Ressler(1989)的《Life with Unix》，以及 Peter Salus(1994)的《A Quarter Century of Unix》。

[]{#index_split_001.html#p197}SOURCES 183

Dennis Ritchie's home page at (Nokia) Bell Labs has been preserved. It has links to most of the papers that Dennis wrote and to other historical material. The link is _[www.bell-labs.com/usr/dmr/www](http://www.bell-labs.com/usr/dmr/www)_.

> 丹尼斯·里奇(Dennis Ritchie)在诺基亚贝尔实验室的主页已被保留下来，里面有丹尼斯写的大部分论文和其他历史资料的链接。链接为：[www.bell-labs.com/usr/dmr/www](http://www.bell-labs.com/usr/dmr/www)。

Kirk McKusick, one of the central figures in BSD, has written a careful history of BSD, available at _[www.oreilly.com/openbook/opensources/book/](http://www.oreilly.com/openbook/opensources/book/)_

> Kirk McKusick，BSD 的中心人物之一，已经写了一本关于 BSD 的细致的历史，可以在[www.oreilly.com/openbook/opensources/book/](http://www.oreilly.com/openbook/opensources/book/)上获取。

_kirkmck.html_. Ian Darwin and Geoff Collyer provide additional insights from a somewhat different perspective in _doc.cat-v.org/unix/unix-before-berkeley_.

> Ian Darwin 和 Geoff Collyer 从另一个角度提供了额外的见解，可以在*doc.cat-v.org/unix/unix-before-berkeley*中找到。

[]{#index_split_001.html#outline}

[]{#index_split_002.html}

# Document Outline {#index_split_002.html#calibre_pb_0 .calibre5}

- [Contents](#index_split_000.html#p7)
- [Preface](#index_split_000.html#p9)
- [Chapter 1: Bell Labs](#index_split_000.html#p15)
- [Chapter 2: Proto-Unix (1969)](#index_split_000.html#p41)
- [Chapter 3: First Edition (1971)](#index_split_000.html#p55)
- [Chapter 4: Sixth Edition (1975)](#index_split_000.html#p75)
- [Chapter 5: Seventh Edition (1976-1979(](#index_split_001.html#p101)
- [Chapter 6: Beyond Research](#index_split_001.html#p145)
- [Chapter 7: Commercialization](#index_split_001.html#p157)
- [Chapter 8: Descendants](#index_split_001.html#p167)
- [Chapter 9: Legacy](#index_split_001.html#p179)
- [Sources](#index_split_001.html#p195)

```{=html}
</p>
```

---
