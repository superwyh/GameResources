# 游戏开发常用资源

> 这里更新一些我遇到的可以提高游戏开发效率的资源和经验总结，不贪多，只有最实用的。

作者的书：[《中国游戏风云》](https://book.douban.com/subject/36077734/) | [《游戏为什么好玩》](https://book.douban.com/subject/36347706/) | [《游戏化思维》](https://book.douban.com/subject/36210962/) | [《电子游戏商业史》](https://book.douban.com/subject/36394867/) | [《游戏机图鉴》](https://book.douban.com/subject/35894947/)

本文档的 Github 地址：https://github.com/superwyh/GameResources

## 游戏引擎

| 引擎                                                  | 说明                                                                                                                                                                                                                                                                                                                                                                                        |
| --------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Unity](https://unity.com/)                         | 现阶段最主流的游戏引擎，在手游市场近乎垄断性优势。使用 C# 开发，有自己的可视化编程工具，并且有知名的 PlayMaker 插件。Unity 非常适合程序员直接上手使用，入门速度很快。而且C#非常好学，功能强大。但 Unity 不是开源的，所以没办法直接去动底层的代码。Unity这些年奇葩的事情比较多，比如 Unity 中国的神经刀操作，所以劝退了一些开发者。                                                                                                                                                                                                    |
| [Unreal Engine](https://www.unrealengine.com/zh-CN) | 也就是虚幻引擎，现在多数公司大项目都采用了 UE。使用 C++ 开发，有一套很强大的蓝图系统。UE 的优势非常多，比如很容易就能做到非常漂亮的渲染效果，比如开源，最重要的优点经常被人忽视，就是 UE 有一套非常强大并且有实用性的工具流，至今 Unity 还有明显差距。但 UE 也有缺陷，一是系统过于庞大，繁杂，而且底层代码有很多屎山，哪怕能改也不想改。                                                                                                                                                                                                         |
| [Godot](https://godotengine.org/)                   | 在独立游戏市场非常有影响力的开源引擎，引擎非常小巧，使用了专门的开发语言 [GDScript](https://gdscript.com/)。Godot 在独立游戏市场很有前景，但是因为使用人数还是相对较少，所以遇到问题可能也不容易找到文档，更难找到人帮你处理。                                                                                                                                                                                                                                                       |
| [RPG Maker](https://www.rpgmakerweb.com/)           | 一款非常古老的专门做 RPG 游戏的引擎，相对而言比较玩具级，适合完全没有编程基础的，但可以算是国内独立游戏的启蒙引擎，而且如果开发熟练度高的话，也能做出完成度极高的游戏。RPG Maker 的版本非常多，常用版本里 XP 因为是还在维护的最古老的，所以美术素材和相关技术文章最多，并且 XP 支持三层图层；VX 的整体表现非常差，作为后来者甚至缺少很多 XP 都有的基础功能，可以直接不考虑；VA 算是在发现 VX 的失败后的升级版，弥补了很多缺陷，并且插件系统也比较丰富，使用的人也较多；MV 支持鼠标操作，可以打包移动端，并且使用了 JavaScript 开发，而以前的版本都是 Ruby；MZ 是最新版，功能非常丰富，但是小缺陷很多。个人推荐直接在 XP 或者 MV 中选择。另外，RPG Maker 的所有版本都可以在 Steam 上直接购买。 |
| [Cocos](https://www.cocos.com/)                     | 基本算是国产的一套游戏引擎，在手游发展初期 Cocos2d-x 一度拥有垄断性优势，但很快就被 Unity 超越了。Cocos 现在最大的应用场景应该是微信小游戏，在传统游戏类型中已经毫无竞争优势了。                                                                                                                                                                                                                                                                                      |

> 从个人经验来讲，我只推荐以上五款引擎，因为使用人数多，并且在应用范围内都是最佳选择。但后面还是提供一些其他引擎的介绍，给特殊需求的人群。

| 引擎                                                    | 说明                                                                                                                                                     |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [CryEngine](https://www.cryengine.com/)               | 曾经有一大批公司都在使用 CryEngine，但是后来这批公司宁可去自研引擎也不再用 CryEngine了。倒不是技术不行，CryEngine 的技术非常强大，但太难用了，从工具流到开发逻辑都非常反人类。如果有兴趣的开发者可以适当尝试，现在已经支持C#了，对于Unity的开发者来说还算是比较好上手。 |
| [pygame](https://github.com/pygame/pygame)            | Python 的游戏开发框架。                                                                                                                                        |
| [GB Studio](https://github.com/chrismaltby/gb-studio) | 专门制作 GB 风格冒险游戏的引擎。                                                                                                                                     |

> 最后，如果是单纯的喜欢研究游戏引擎，可以看 [Gamefromscratch](https://www.youtube.com/c/gamefromscratch/videos)，他的视频里介绍了大量冷门的游戏引擎。

## 重要工具

### 开源工具

| 名称                                            | 说明                                                                                         |
| --------------------------------------------- | ------------------------------------------------------------------------------------------ |
| [ImGui](https://github.com/ocornut/imgui)     | 一个基于 C++ 开发用户界面的解决方案，能够极大程度节省开发时间。尤其是开发引擎时，使用这个会感觉事半功倍。但也不是没有缺陷，因为文档实在太差了，所以需要自己阅读代码来领会功能。 |
| [xLua](https://github.com/Tencent/xLua)       | 腾讯的开源项目，支持在 Unity 里插入 Lua，并且对原有项目的侵入性极低。是非常好的手游热更新框架。                                      |
| [xNode](https://github.com/Siccity/xNode)     | Unity 上的开源可视化脚本工具。                                                                         |
| [UniTask](https://github.com/Cysharp/UniTask) | Unity 上的一套异步操作解决方案。                                                                        |

## 推荐插件

| 名称                                                                | 引擎    | 说明                          |
| ----------------------------------------------------------------- | ----- | --------------------------- |
| [NaughtyAttributes](https://github.com/dbrizov/NaughtyAttributes) | Unity | 为 Unity Inspector 添加了很多新功能。 |
|                                                                   |       |                             |
|                                                                   |       |                             |

## 学习相关

### 视频教程

| 名称                                                                                                                                        | 分类      | 语言  | 说明                                                                                                                                                                                                                                           |
| ----------------------------------------------------------------------------------------------------------------------------------------- | ------- | --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Game Maker's Toolkit](https://www.youtube.com/c/MarkBrownGMT)                                                                            | 策划      | 英   | 整个Youtube上影响力最大的游戏区账号，视频都是分析游戏玩家相关的，内容质量极高，无论程序、美术还是策划都值得看。                                                                                                                                                                                  |
| [M_Studio](https://space.bilibili.com/370283072)                                                                                          | Unity   | 中   | B站知名的麦蔻老师，甚至是中文范围内最好的视频教程。最近刚上了一个付费教程[《麦田物语》模拟经营游戏开发教程](https://learn.u3d.cn/tutorial/MFarmCourse#)，应该是我看到过所有语言的Unity教程里都算是最好的之一。如果英语不好，我只推荐看麦蔻老师的教程。                                                                                        |
| [Complete C# Unity Game Developer 2D](https://www.udemy.com/course/unitycourse/)                                                          | Unity   | 英   | 类似的课程还有[Complete C# Unity Game Developer 3D](https://www.udemy.com/course/unitycourse2/)。Udemy上最好的Unity教程，两个教程加起来有60万学生，可以根据你是想学2D还是3D选择对应的。只要英语过关，我只推荐看他们的教程入门，讲的极为细致，并且从入门到最后有多个案例教学。而且非常值得一提的是，老师几乎24小时蹲在Udemy解答问题，并且教材内容一直在根据Unity的版本更新。 |
| [Unreal Engine 5 C++ Developer: Learn C++ & Make Video Games](https://www.udemy.com/course/unrealcourse/)                                 | Unreal  | 英   | 类似的课程还有[Unreal Engine Blueprint Game Developer](https://www.udemy.com/course/unrealblueprint/)。和前面Unity的Udemy课程一样，也是GameDev.tv团队制作的，非常适合新手入门，也是UE教程里，只要英语过关，也是我唯一推荐的教程。                                                                      |
| [Brackeys](https://www.youtube.com/c/Brackeys/featured)                                                                                   | Unity   | 英   | 个人认为是整个Youtube，甚至是全网最好的Unity视频教程，讲解非常清晰，并且有大量实用性极强的内容。可以按照自己需求查找，然后直接使用。但是已经不再更新了。                                                                                                                                                           |
|                                                                                                                                           |         |     |                                                                                                                                                                                                                                              |
| [Code Monkey](https://www.youtube.com/c/CodeMonkeyUnity)                                                                                  | Unity   | 英   | 也做了大量实用性极强的视频内容，而且更新频率现在还非常高，同时和网友互动也频繁。但是他的视频有个大缺陷，大部分都要依赖他自己开发的一些库，可能出现两个问题，一是虽然你的功能实现了，但是因为依赖他的库，所以不明白原理；二是他的那些库的代码质量也不算好，不排除有隐患。                                                                                                         |
| [SpeedTutor](https://www.youtube.com/c/SpeedTutor/featured)                                                                               | Unity   | 英   | 教学视频的整体质量非常高，但相较于他的教学视频，关于一些Unity商店的资源和Unity功能的评价更值得看一些。另外他的更新频率也极高。                                                                                                                                                                         |
| [Tarodev](https://www.youtube.com/c/Tarodev/videos)                                                                                       | Unity   | 英   | 大部分视频都是专注于单一功能，对于点经验的开发者来说，特别适合当字典来查，并且适合只是上的查漏补缺。                                                                                                                                                                                           |
| [Epitome](https://www.youtube.com/c/EpitomeGames/featured)                                                                                | Unity   | 英   | 提供了大量的案例教学，内容也非常细致，适合新手学习，但更新频率比较低。                                                                                                                                                                                                          |
| [Zigurous](https://www.youtube.com/c/Zigurous/featured)                                                                                   | Unity   | 英   | 也是案例教学类视频，大部分案例都是相对完整的游戏，非常适合初学者前期获得成就感。                                                                                                                                                                                                     |
| [UGuruz](https://www.youtube.com/c/UGuruz)                                                                                                | Unity   | 英   | 大多数Unity的教程都是以2D为主的，但这个账号下的视频基本都是3D内容，并且实用性非常强，很适合按需学习。                                                                                                                                                                                      |
| [UE4 Poseidon](https://www.youtube.com/c/UE4Poseidon)                                                                                     | Unreal  | 英   | 大量虚幻引擎的相关视频教程，其中[UE4: 3rd Person Game \| Tutorial series](https://www.youtube.com/playlist?list=PLd6LaoDjaEtOtR71sPsXhH7eNwBJOwlvx)是Youtube上质量最好的第三人称射击游戏教程。                                                                                 |
| [Unity Game Studio Studio Shimazu](https://www.youtube.com/channel/UCDunz_CPkqkQT5ljKXcYkhg/featured)                                     | Unity   | 日   | 专门制作日语的Unity教程，里面有大量实用性极强的开发技巧。并且因为过程非常细致，所以不懂日语光看代码其实也可以。                                                                                                                                                                                   |
| [Imphenzia](https://www.youtube.com/c/Imphenzia/featured)                                                                                 | Blender | 英   | 专门制作Blender相关的内容，视频质量极高，实用性也非常强。另外他也做过一些引擎相关的视频，比如[Unity的入门教学视频](https://www.youtube.com/watch?v=pwZpJzpE2lQ&t=3s&ab_channel=Imphenzia)。                                                                                                     |
| [AdamCYounis](https://www.youtube.com/c/AdamCYounis)                                                                                      | 像素画     | 英   | 专门制作像素画相关的教程，基本上是Youtube上质量最高的，内容涵盖也是最全的。                                                                                                                                                                                                    |
| [Pixel Overload](https://www.youtube.com/c/PixelOverloadChannel)                                                                          | 像素画     | 英   | 实用性很强的像素画教程。                                                                                                                                                                                                                                 |
| [Brandon James Greer](https://www.youtube.com/channel/UCC26K7LTSrJK0BPAUyyvtQg)                                                           | 像素画     | 英   | 质量极高的像素画教程，和前面的比他经常会有一些比较新鲜的教学内容。                                                                                                                                                                                                            |
| [AI and Games](https://www.youtube.com/c/AIGamesSeries)                                                                                   | AI      | 英   | 主要是游戏内AI相关的案例分析，实用性不强，但偶尔听听会有一些特殊的点子冒出来。                                                                                                                                                                                                     |
| [GAMES101](https://www.bilibili.com/video/BV1X7411F744/?from=search&seid=13728008737010812958&vd_source=b4a4768a500f18f74f6f9df1c4ce6392) | 引擎      | 中   | 现代计算机科学的入门课程，非常详细，是中国视频课程里质量最高的，很值得零基础入门的去看。                                                                                                                                                                                                 |

## 文字教程

| 名称                                                          | 分类     | 语言  | 说明                                                                           |
| ----------------------------------------------------------- | ------ | --- | ---------------------------------------------------------------------------- |
| [GDscript Tutorial](https://gdscript.com/tutorials/)        | Godot  | 英语  | GDScript的官方教程，其实只要你有开发基础的话，看这个基本就够了。GDScript有点像Python，要是学过Python的话基本是可以无痛上手。 |
| [Learn OpenGL](https://learnopengl.com/Introduction)        | OpenGL | 英语  | OpenGL 最好的免费教程。                                                              |
| [针对2D美术的Unity入门级教程](https://zhuanlan.zhihu.com/p/601149257) | Unity  | 中文  | 很简单的 Unity 入门教程。                                                             |

## 美术相关

### UI

| 名称                                                  | 说明                      |
| --------------------------------------------------- | ----------------------- |
| [Game UI Database](https://www.gameuidatabase.com/) | 大量游戏UI的参考图，并且可以按需求分类查询。 |

### 游戏素材

| 名称                                                 | 说明                                   |
| -------------------------------------------------- | ------------------------------------ |
| [itch.io/game-assets](https://itch.io/game-assets) | itch.io的资源站，游戏美术相关的素材非常全面，尤其是像素画相关的。 |

## GameJam

| 名称                                   | 说明                               |
| ------------------------------------ | -------------------------------- |
| [itch.io/jams](https://itch.io/jams) | itch.io的GameJam列表，基本上也是全网最全面的汇总。 |

## 开源项目

| 名称                                                                         | 说明                                        |
| -------------------------------------------------------------------------- | ----------------------------------------- |
| [Tiny Renderer](https://github.com/ssloy/tinyrenderer)                     | 一个使用 500 行代码实现的渲染器，是同类最好的入门开源项目。          |
| [osu!](https://github.com/ppy/osu)                                         | 最知名的节奏游戏之一，也是最知名的开源游戏项目之一。开发语言是 C#。       |
| [stendhal](https://github.com/arianne/stendhal)                            | 一款开源的 MMORPG，这款游戏已经持续了十几年的时间。开发语言是 Java。  |
| [Wave Function Collapse](https://github.com/marian42/wavefunctioncollapse) | Unity 中的一个 3D 波函数塌陷演示，玩家可以在一个无边界的城市里自由移动。 |
| [金庸群侠传3D重制版](https://github.com/jynew/jynew)                               | 金庸群侠传的 3D 重制，使用 Unity 开发，暂时还是比较初级阶段。      |

## 游戏上架

* [Steam](STEAM.md)
