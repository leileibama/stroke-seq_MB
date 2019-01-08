单手笔顺输入法码表 stroke-seq_MB 1.1版
    
    版权：GPL v3+
    遵照《GB13000.1字符集汉字字序（笔画序）规范》共20902个汉字，遵照《GB13000.1字符集汉字笔顺规范》；
    并增补GB18030字符集（截止2017年）开源字体可见双字节和四字节汉字8783个（即本输入法编码目前涵盖29685个汉字）；
    随着开源字体的完善，以后可继续扩展录入GB18030字符集里的其它汉字，即可涵盖GB18030字符集全部汉字共70377个。
    由于Unicode编码包含大量日韩使用的、与汉字字型笔画完全相同的文字（即同一个字重复出现两次），极易造成混淆，故不以此为标准。
    编码原理基于专利权已终止的（CN03159505.7）“一种数字笔画汉字输入方法”，原发明人：马晓光 <232937@QQ.com>
    参考《数字五笔中文输入系统输入教程及编码查询手册》
    开源码表初始手工录入、简化规则、全新重排部件编码（边旁部首编码）、再次手工录入：一善鱼 YQ-YSY <YQ-YSY@163.com>
    拼音采用 wangyanhan（老老朽）整理制作并分享的《CJK汉字拼音表_42907字_14.8.10更新》，以及其它字典网站查询参考。
    核心词库包括有《现代汉语常用词汇表》（38285个）以及其它常用词汇和短语共计约18万个，已剔除方言、网络词汇、粗口话和淫秽词语。
    欢迎各位朋友利用此码表，或开发独立的笔顺输入法，或嵌入已开发的输入法，新输入法程序名称亦可自行设定。
    为了方便大家编辑并导出其它形式的码表，在此使用TXT文本文件，以及LibreOffice电子表格ods文件，里面有详细的分类编号及排序。
    随本文还附带有本输入法的Logo图标以及部件编码的SVG格式和PNG格式文件，以及“悬浮栏功能设计说明”图JPG格式的文件。
    
* * *
    
<big>按键说明</big>
    
    单手笔顺输入法使用键盘数字小键盘为主要输入工具，只用单手（右手或左手）即可完成简体繁体文字、词组以及标点符号的输入。
    输入速度极快，常用字词重码少，符合华人书写习惯，适合文案录入、会议速记、撰写书籍等工作，避免“提笔忘字”电脑病，亦方便残障人士。
    
    小键盘的0~9按键默认是录入汉字，若先输入“*（星号）”紧接着输入0~9则为录入数字；
    按键“/（斜杠号）”首先第一个输入时为逗号，若跟随在编码后输入则为切换悬浮栏第二行在“部首编码/后续编码”之间互相转换。
    按键“*（星号）”首先第一个输入时为切换到数字输入模式，若跟随在编码后输入则作为未知编码的模糊查询通配符；
    按键“-（减号）”为撤销上一步按键（类似BackSpace向左退格键）；
    按键“+（加号）”首先第一个输入时为+号，若跟随在编码后输入则切换到候选字（蓝色）选词模式，继续输入0~9选择列出的字词；
    按键“Enter（回车）”用于确认选中排在第一个的候选字词就是需要的字词；
    按键“.（点号）”首先第一个输入时为句号，若跟随在编码后输入则作为词组的汉字间隔符；
    按键“00”为列出标点符号候选；按键“09”为列出特殊数字序号候选。
    
    大键盘上的其它按键，与其它输入法功能相同。例如：
    -号 或者 PageUp 候选字词向上翻页；=号 或者 PageDown 候选字词向下翻页；
    Shift 4 为￥人民币符号，Shift 6 为……省略号，shift < 为书名号《，以及 Ctrl . 为全角半角切换等。
    为了方便没有数字小键盘的笔记本用户，建议输入法开发者提供自定义按键替换0~9的功能，以及繁体简体互换功能。
    建议输入法程序开发者采用混合输入模式，即：小键盘是单手笔顺输入法，大键盘默认是英文输入法，按一下shift键可切换为拼音输入法。
    使用拼音输入时，数字小键盘依然是继续用于笔顺输入法，拼音候选字的选取依然是使用+号来选取字词，大键盘数字键0～4用于输入音调。
    
<big>显示说明</big>
    
    输入法悬浮栏的显示方式，建议输入法开发者参考原“数字五笔输入法”分两行提示框的显示方式，方便用户学习记忆。
    用户输入编码时，已输入的数字、以及相同编码所代表的字词，相同编码的候选字列表显示在悬浮栏第一行（候选框）。
    建议精简码显示为100%全黑色（000000）、六全码显示为80%炭灰色（333333）、笔顺码显示为60%灰色（666666）。
    如果候选字太多放不完，最后末端有按钮可点击滚动显示。
    悬浮栏第二行（提示框）显示的是以该数字起头的两位数字所代表的部件编码表，因此不需要死记硬背，看见即可理解。
    悬浮栏第二行（提示框）最末端的按钮可切换显示“部首编码/后续编码”模式，显示当前数字后还可以继续输入什么数字即可打出什么汉字。
    
    编码输入完毕，用户按+号切换到备选字（蓝色）选词模式，
    三类编码显示为100%全蓝（0000ff）、80%明蓝（3333ff）、60%淡蓝（6666ff）三种深度的蓝色，用户选择了所需要的字之后：
    第一行（候选框）显示该用户最近输入的以这个字开头的句子或短语，以供用户再次重复输入，在写文章或网络聊天时经常会用到这个功能。
    其后还可以跟随有该字的联想词组，以供用户快速选择输入，最后末端有按钮可点击滚动显示更多的候选词。
    第二行（提示框）显示刚才这个字或词的精简码、六全码，及其汉语拼音，方便用户学习记忆。最后有附加按钮可链接字典网站获取信息。

    输入法悬浮栏第一行（候选框）可以用鼠标左键点击选取字或词。
    输入法悬浮栏第二行（提示框）不能选字词，鼠标左键点击并按住第二行任意位置可拖动悬浮栏，右键点击则可弹出菜单选项进行相关设置。
    
* * *
    
<big>一、笔顺码</big>
    
    仅仅以1、2、3、4、5五个数字分别代表“一丨丿丶𠃌”五个笔画，按汉字笔顺进行输入。例如：
    
    “开”字，按笔顺“一、一、丿、丨”，编码为1132；
    “我”字为31；“向”字为325；“力”为53；
    注意“万”为153，“方”为4153，“忄”为442。

    其中有些笔画容易被误解：
    “提”归为“一”：如“氵、扌”中的最后一笔；有些电脑字体繁体字的“雨字头”四点显示为四小横，皆按国标笔顺归为四点；
    “亅”一竖往左勾的归为“丨”：如“小”字的第一笔、“扌”提手旁等；“乚”一竖往右勾的归为“𠃌”：如“比、民、氏”的左边那一笔；
    “点、捺”都归为“丶”：如“文、入、表、厶”的最后一笔；“宀”宝盖头和“冖”秃宝盖的左边那一笔也都是点“丶”，不是竖“丨”；
    各种折笔（乛、フ、乚、𠃌、⺄、折弯钩、竖提等）都归为“𠃌”：如“乃、孔、民”中的笔画。
    
    标点符号输入：
    常用标点符号可以输入“00”,常用的数字序号可以输入“09”。
    
* * *
    
<big>二、六全码、精简码</big>
    
    使用0～9中某二个数字的组合来代表汉字中的边旁部首或部件，注意每个部件必须严格按笔画顺序排列，不得跨越笔顺拆解部件。
    每个汉字最多取六个编码，当汉字编码超过六个时，第六码取该汉字最后一笔编码，
    若该字最后一部分为常用部件，则取该常用部件的最后一笔编码。例如：
    
    尘：23419（"尘"的前三笔是竖丨、撇丿、点丶、编码234，后三笔为常用部件"土"，编码19。）
    镜：916185（"镜"的钅为91,立为61，日为81，儿为35，但已经超出六码，最后一笔或部件的最后编码为"𠃌"，因此第六码取5。）
    梦：121290（"梦"的两个木为1212,夕为90，恰好满六位。）
    再：125211（"再"最后三笔虽然像是一个“土”字，但按笔顺则应该是先一竖再二横，因此不能取“土”作为部件。）
    回：25801 （"回"字不能拆解为二个“口”（部件编码80），因为按笔顺外面大“囗”的最后一笔要等小“口”写完后才能封口。）
    
    六全码目前一共录入了29685个汉字，包括《GB13000.1字符集汉字字序（笔画序）规范》收录的繁体字、异体字、以及日韩所用的汉字。
    精简码则是六全码的简化格式，共5117个，囊括了《通用规范汉字表》大部分一级、二级汉字，1~5键即可快速打出最常用的汉字。例如：
    
    我：精简码为31，  六全码为312154；
    自：精简码为382， 六全码为382；
    无：精简码为1135，六全码为1135；
    心：精简码为65，  六全码为65；
    是：精简码为8，   六全码为811214；
    
    大多数常用的汉字，均不需取完所有六个编码便可出现在候选汉字的首位，然后按回车键直接完成输入，
    处在候选列表的汉字，只需在小数字键盘里，按下+号，黑色候选列表变为蓝色备选列表，再按数字键，即可选中备选列表里的汉字。
    
<big>三、部件编码表</big>
    
    利用"1、2、3、4、5"作为开头，配以其它数字，代表比较简单的部件笔画"横一、竖丨、撇丿、点丶、折𠃌"，
    利用"7、8、9、6、0"作为开头，配以其它数字，代表比较复杂的部件笔画"横一、竖丨、撇丿、点丶、折𠃌"，
    在键盘上输入方位类似的二个0~9按键，就能得到各种常见的的边旁部首和部件。在数字小键盘上的排列如下：
        
    7横一  8竖丨  9撇丿
    4点丶  5折𠃌  6点丶
    1横一  2竖丨  3撇丿
    0折𠃌        .
    
    不需要死记硬背，因为在输入第一个数字后，提示框中会出现这个数字开头的的偏旁部首（部件）列表，一看便知，打字多了自然就记住了。
    如果需要输入的汉字刚好就是这个部件，那么只需要输入这个部件编码即可。笔画数较少多、常用、结构简单的边旁部首和部件（共50个）：
    
    10 扌 11 二王  12 十丅丁木朩  13 厂丆𠂇歹豕  14 石  15 七丂匚匸  16雨  17 艹⺿卄  18 廿甘革堇(傼字边)19 土士壴
    20 山  21 丄止齿齒  22 刂业(亞字底) 23 非  24 卜⺌  25 冂巾  26 虫  27 且(直字底) 28 贝貝  29 足
    30 饣飠食  31 牜牛  32 亻  33 彳𠂆  34 八人入乂  35 九几儿匕勹角  36 月   37 ⺮竹   38 犭風  39 爫豸
    40 讠訁言  41 冫亠吂(京字头中) 42 门  43 丷(关养字头中) 44 氵  45 冖   46 宀   47 广鹿   48 疒   49 忄
    50 马馬   51 刁  52 了阝卩丩凵  53 刀力乃   54 又厶廴予 55 纟糹 56 幺乡  57 弓癶  58 孑子  59 女
    
    笔画数较多、不太常用、结构复杂的边旁部首和部件（共48个）：
    
    70 其  71 丰耒  72 耳臣(巸字边）73 𡗗來(邦字边）74 覀西  75 酉 76 走井(冓字头）77 车車  78 镸長髟  79 牙瓦
    80 口    81 日曰    82 目   83 田由甲申   84 罒四皿   85 骨黽    86 黑    87 虍尗鹵   88 門鬥    89 婁
    90 夕夂攵夊(祭字边头) 91 钅釒金 92 禾合 93 舟谷 94 矢缶 95 鬼身 96 夭舌 97 鼻臼鼠(段舆盥字边) 98 鱼魚 99 鸟鳥(鸟鳥字头)
    60 方 61 立(旁商字头中）62 礻 63 衤 64 與𦥯(兴興璺学字头中）65 心必 66 文六亦䜌(变字头）67 手毛气 68 米㡀 69 火灬𤇾
    00 (标点符号) 01 彐(录尹字头) 02 出爿韋 03 艮(即字旁) 04 习 05 巜巛 06 毌毋母 07 尸辟叚  08 𤴔疋 09 (数字序号)
    
    部件编码的规则是以汉字笔顺为准，优先选用汉字起头的边旁部首，原本就是二个笔画的边旁部首也尽量保持在与笔顺编码相同的原位。
    少数部件按视觉、听觉形成的思维习惯、以方便记忆为目的，进行编码排列。同一汉字有多种编码可能时，择取编码较少且易于记忆的方案。
    由于某些部件没有相对应的单个汉字，在此以“某字边、某字头”来说明，请输入法开发者在制作提示框时，改为用图片显示正确的部件形式。
    
    只需一个编码，即 0~9 所代表的最常用汉字分别是：1 一，2 国，3 的，4 为，5 能，6 这，7 要，8 是，9 和，0 即。
    其中仅一个或二个编码的汉字（编码1～99～09）选择使用频率最高的、在句子中经常以单字形式出现的汉字，优先于大多用于组词的汉字。
    重码的汉字，在码表中将按字频排列。在蓝色选字状态下，可以按键“/（斜杠号）加回车”滚动选取，或按键“+（加号）加数字”挑选。
    建议输入法开发者按以下优先顺序排列单字（包括仅编码相同时的单字排列顺序、及其有后续编码时的更多单字排列顺序）：
    精简码位数、六全码位数、精简码笔画数、精简码数字大小、六全码字频、六全码笔画数、六全码数字大小、笔顺码数字大小、笔顺码字频。
    例如：
    编码194514、341804、441354、463414、13251354，可用于编程测试，这几个编码在输入的过程中，汉字会出现上述复杂排列情况。
    在比较数字大小时，请留意“以0开头的编码”和“以0结尾的编码”，以避免在程序中把编码转换为数字时造成丢失编码的情况。

    如果记不全某个汉字的六全码或者笔顺码，可以在输入第一个编码之后，使用“*（星号）”作为该字未知编码的模糊查询通配符。
    例如：记不全“镜”这个字的六全码,只记得第一个和其它一两个编码：可以输入9*08*，或者9*5就可以在候选字列表中找到“镜”字。
    注意，如果按键“*（星号）”作为第一个输入按键，则切换到数字输入模式。
    例如：想输入数字123，就只需在数字小键盘输入*123回车即可。
    
    六全码或精简码也可以打出繁体字，某些繁体字与简体字编码相同的，目前是默认排在简体字后面。
    习惯使用繁体字输入的用户，可以在单字码表的基础上重新排列优先字序，让某些繁体字与简体字编码相同的，默认排在简体字前面。
    也希望输入法开发者能做出一个“繁体/简体“转换按钮，或者一个”汉字信息“按钮，用来显示这个汉字完整笔顺、拼音、内码等信息。
    
* * *
    
<big>四、词组输入规则</big>
    
    词组中的每个字之间用“.”（点号）隔开即可，用户可以输入自己记得的不定长的编码。词组码表只有六全码和笔顺码，不需要精简码。
    唯一要注意的是词组的每个字的编码必须统一，即：第一个字用六全码或精简码，后面的字就不能混用笔顺码，反之亦然。例如：
    中国：802.251（六全码）或 25.251 （笔顺码）
    汉武帝：44.11.61（六全码）或 441.11.414（笔顺码）
    
    虽然词组中每个字可以输入任意长度的编码，但建议每字输入2－3个编码，这样更有利于精确定位词组，减少选词的麻烦。
    多字超长词组的输入十分简单，只输入词组两头的汉字编码，中间要省略的多个字直接用一个“.”（点号）隔开即可。例：
    中华人民共和国：85.32..25（这时，候选列表会显示出“中华人民共和国”和“中华民国”两个词组,因为匹配的是“中华……国”。）
    百闻不如一见：13..1.25（注意不能输入 13..13..25 即：中间不能省几字、又加一字、又省几字。只能用两头、省中间。）
    
    如果记不全词组中某个汉字的编码，可以在输入第一个编码之后，使用“*（星号）”作为该字未知编码的模糊查询通配符。
    例如：记不全“汉武帝”这三个字的六全码,只记得第一个和其中两个编码：
    可以输入4*.*4.6*，或者4*.*.*5就可以在候选字列表中找到“汉武帝”这个词组,所记得的编码越多，查询越准确。
    
    注意：扩充词组编码时，应注意不要录入“错别词、网络篡改词”，以维护正确规范的词组用字行为（过多的不良杂词会影响正常输入效率）。
    扩充词汇时，可参考附带的“错别异词对照表”来修正所录入的词汇，注意此表仅是针对书面用语的词汇，并未包括“网络新词”的错别字。
    此外，也建议大家绝不录入“粗口话”和“淫言秽语”，让想说这些话的人只能一个字一个字地慢慢打出来，这样世界就安静多了。
    
    建议输入法开发者能参考“搜狗词库”的管理方式，利用单字码表生成多种分类词汇码表，并提供在线更新，以增强本输入法的生命力。
    也希望输入法开发者能开发出“自造词组”的功能，以及上次经常输入的句子短语的记忆功能，这能让用户感受到极其便利的输入体验。
    习惯使用繁体字的用户也许需要另外编排繁体字的编码和字频、以及生成繁体字专用的词组码表，或者开发一个“繁体/简体“转换按钮。
    
* * *
    
<big>    六、易错易混汉字</big>
    
    以下汉字是容易输入错误或混淆的：
    1、"末、未、果、業"等后四笔形成的"木"形结构，其结构清晰，易于辨认，且笔画顺序与"木"相同，故取"木"的编码12，“柬、谏”不行。
    2、"国、因"等含"囗"的汉字，因按笔顺这些字最后才封口，故不取"口"；正确取法应第一、二笔取"丨、𠃌"，取码25。
    3、"都、教、考、孝、老"等前三笔形成的"土"形结构，其结构清晰，易于辨认，且笔画顺序与"土"相同，故取"土"的编码19。
    4、"截、戴、载、裁"等前三笔虽也形成"土"形结构，但视觉思维习惯通常认为“土”字的最下一横属于“戈”字结构，故需按其笔顺取码121。
    5、"里、垂、重、黑"等三笔形成的"土"形结构，其笔顺却是先一竖再二横，不是"土"字笔顺，故需按其笔顺取编码（”里“不取”甲“部件）。
    6、"衰、蓑"等字中间的"口"形结构，按笔顺应先写"口"中间的一横，打乱了"口"字的笔顺，故不取"口"字部件编码，取其笔画编码2511。
    7、“冒、帽”上面不是“日”字，而是丨𠃌一一，这两横不连接到旁边，即2511。
    8、”有、育、膏“的下面不是”月“，而是先一竖，丨𠃌一一，即2511。
    9、“用、甩”字虽然有类似“月”字的结构，但是结构变形较大，且混杂有其它笔画在其中，不易记忆，所以不取36编码，取笔顺即可。
    10、“生”字虽然有类似“牛”字的结构，但是从记忆习惯上通常认为是一撇加“”字结构，因此不取“牛”字31编码，而取“”字71编码。
    11、“满、螨”等有类似“”编码18的部首，但应取“艹”编码17,因为艹字头与下方的一横是断开的，且从习惯上通常认为“一”属于“两”字。
    12、“垂、郵、甀、乗、剰”等字中间有类似“艹”的结构，但是因为混杂在其它笔画之中，不易辨认，故不取17编码，而取笔顺即可。
    13、“脑、恼、垴”的右边有类似“文”字的结构，但是从记忆习惯上通常认为“乂”是属于“凶”字结构，因此不取“文”字66编码，取笔顺即可。
    14、“刪、姍、柵"等字中虽然有类似“卄”字的结构，但是它的笔顺不是与“侖”字那样先一横再二竖，而是先二竖再一横，所以不取17编码。
    15、“刺、棘、枣、策”等字中虽然有类似“巾”字的结构，但是因为混杂在其它笔画之中，不易辨认，故不取25编码，而取笔顺即可。
    16、“夜、腋”等字中虽然有类似“夕”字的结构，但是因为被其它笔画混杂，不易辨认，故不取90编码，而取笔顺即可。
    17、“熏、薰、醺”等字中虽然有类似“黑”字的结构，但因为中间一竖穿透了“黑”字顶部，与上方其它笔画混杂，故不取86编码，而取笔顺。
    18、“啄、冢、诼”等字中虽然有类似“豕”字的结构，但因为中间一点打乱了“豕”字的笔顺，然后才接撇点结尾，故不取13编码，而取笔顺。
    19、“粛、簘、嘨”等字中虽然有类似“米”字的结构，但按笔顺应先写中间一竖，然后接一撇一竖，不是"米"字笔顺，故需按其笔顺取编码。
    20、有些汉字，在不同的电脑字体里显示出来的写法不一样，例如“爋”字的最后四点在有些字体中是放在中间的，这类汉字以国标笔顺为准。
    
    以下汉字和部件的笔顺容易出错（括号内为六全码）：
    七：一𠃌 15            九：丿𠃌 35               匕：丿𠃌 35                及：丿𠃌丶 354
    刀：𠃌丿 53            力：𠃌丿 53               乃：𠃌丿53                 办：𠃌丿丶丶 5344
    万：一𠃌丿 153         方：丶一𠃌丿 4153（60）     长：丿一𠃌丶 3154          豖：一丿𠃌丿丿丶丿丶 13533434
    小：丨丿丶234           忄：丶丶丨442             义：丶丿丶 434            火：丶丿人 4334（69）
    巨：一𠃌一𠃌 1515（72）  瓦：一𠃌𠃌丶 1554         比：一𠃌丿𠃌 1535          世：廿𠃌 12215（185）
    牜：丿一丨一 3121（31）  牛：丿一一丨 3112（31）    车：一𠃌一丨1512（77）      轧：15215（775）
    为：丶丿𠃌丶 4354       北：丨一一丿𠃌 21135       皮：𠃌丿丨又 53254         必：丶𠃌丶丿丶 45434（65）
    爿：𠃌丨一丿 5213（02）  出：𠃌丨丨𠃌丨 52252（02） 丑：𠃌丨一一 5211          那：𠃌一一丿阝 511352
    凹：丨𠃌丨𠃌一 25251     凸：丨一丨𠃌一 21251      尒：丿丶丨丿丶 34234       忝：一一丿丶丨丶丶丶 11342444
    毋：𠃌𠃌丿一 5531（06）  母：𠃌𠃌丶一丶 55414（06）   丹：丿𠃌丶一3541         贯：𠃌𠃌丨一贝 55212534（0628）
    卵：丿𠃌丶丿卩丶 3543524 兜：丿日丿𠃌𠃌一丿𠃌 32511355135（38135）   非：丨一一一丨一一一 21112111（23）
    兆：丿丶一𠃌丿丶 341534  脊：丶一丿丶人丨𠃌一一 4134342511（413431） 美：丶丿王一丿丶431121134（431114）
    來：12343434（73）      爽：一丿丶丿丶丿丶丿丶人 13434343434（134344） 飛：𠃌丿丶丿丿𠃌丿丶丨534335342
    曲：丨𠃌卄一 251221（25171）                       曹：一丨𠃌卄一日 12512212511（125171）
    衰：丶 一丨𠃌一一丿𠃌丿丶 4125113534（412514）       噩：一丨口口一口口一 1225125112512511（128081）
    敝：丶丿丨𠃌丨丿丶攵 43252343134（6890）            舆：丿丨一一车𠃌一一一丿丶 32111512511134（977754）
    肃：彐丨丿丨八 51123234（012324）                  重：丿一日丨一一 312511211（318121）