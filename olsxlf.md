代发 wailian999

[U103] JS：定时器
来源：http://hz.yangfankeji.com/gtnewtjnmg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.9152youxi.cn/gtaujknlcj.html

[U104] JS：防抖
来源：http://hz.chenlongwang.top/gtsntwadtc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.fzhhl.top/gtslavahgs.html

[U105] JS：节流
来源：http://hz.gaohongyu789.top/gtuzwklpsj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.yonumen.top/gtoioblpfa.html

[U106] JS：日期格式化
来源：http://hz.hywenlv.cn/gtbiuokjdx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhongyouzk.top/gtgucxsihf.html

[U107] JS：数字千分位
来源：http://hz.ydzc1.top/gtpamlwvde.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.smart0.xyz/gthnxgggdh.html

[U108] JS：随机整数
来源：http://hz.9152youxi.cn/gtsjsxfyvw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.redwolf501.top/gtbsynjmyb.html

[U109] JS：数组分组
来源：http://hz.nanxinkj.top/gtzfbrueca.html

Object.groupBy(arr, x => x.type)
来源：http://hz.sxryk.cn/gtkeelpalf.html

[U110] JS：数组分块
来源：http://hz.gotoacloud.top/gtrsjkgbij.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hongshengwenyu.top/gtgqrzluyo.html

[U111] JS：对象转 Map
来源：http://hz.xingfuxueyuan.xyz/gtqvywwgvy.html

new Map(Object.entries(obj))
来源：http://hz.xingfuxueyuan.xyz/gtjxjjynjt.html

[U112] JS：字符串补位
来源：http://hz.jlsjyb.cn/gtrgypkauf.html

"7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtlprzhurv.html

[U113] JS：正则替换全部
来源：http://hz.hnqzz.top/gthsnghwyu.html

s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtsfyzudeo.html

[U114] JS：JSON 深比较
来源：http://hz.nanxuanxn.top/gtyiozzhtn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.daxiang520.top/gtomtlrssb.html

[U115] JS：生成 UUID
来源：http://hz.zhiwuduotai.top/gtkmeqnsku.html

crypto.randomUUID()
来源：http://hz.chenjidiqi.icu/gtyawdpgrw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xuanzx.com/gtolmhzxix.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ydzc1.top/gtwadvfwdp.html

[U117] JS：单元测试
来源：http://hz.0kj1m.cn/gtzpsfsqol.html

npm i -D vitest;  npx vitest
来源：http://hz.smart0.xyz/gtgmqfevyf.html

[U118] JS：开发服务器
来源：http://hz.shangyingyoupin.top/gtdftsjqlh.html

npm i -D vite;  npx vite
来源：http://hz.chenzaomai.com/gthmxidbym.html

[U119] JS：生产构建
来源：http://hz.xuetiantiany.cn/gtwnphwxpr.html

npx vite build
来源：http://hz.zdqjudy.top/gtmfhrvspv.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yj20258888.top/gtssllvqjr.html

import.meta.env.VITE_API_URL
来源：http://hz.cqqwz.cn/gtfubmwtrc.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqmjtereq.html

统计汇总
来源：http://hz.pycfn.com/gtiwnvwfol.html

================================================================================
来源：http://hz.zdqjudy.top/gtzepnlsgm.html

按语言统计（条）：
来源：http://hz.fengsongda.top/gtzwyeoprh.html

Python ......... 252
来源：http://hz.yvedp.cn/gtdiiravbf.html

PHP ............ 252
来源：http://hz.ybcxt.top/gtdpndufzx.html

JavaScript ..... 252
来源：http://hz.zhoulong.xyz/gtulkchaig.html

TypeScript ..... 212
来源：http://hz.tianlin.xyz/gtuwfsbdba.html

Java ........... 212
来源：http://hz.zhixingplan.top/gtkkpiqiru.html

Go ............. 212
来源：http://hz.shangyingyoupin.top/gtknztmlgb.html

Ruby ........... 212
来源：http://hz.cashguo.top/gtovrrhkpk.html

C# ............. 212
来源：http://hz.hywenlv.cn/gtqciwlonp.html

C .............. 30
来源：http://hz.dashuyun.cn/gtzpqbyfgp.html

C++ ............ 30
来源：http://hz.pycfn.com/gtchmzgdxy.html

SQL ............ 90
来源：http://hz.fengsongda.top/gtlpckfnqr.html

Bash ........... 80
来源：http://hz.guannengcc.top/gtdwllkmpk.html

Kotlin ......... 15
来源：http://hz.cdnleiting.top/gteukypluk.html

Swift .......... 15
来源：http://hz.shanyushiyangtech.top/gtmxnrgaqc.html

Lua ............ 10
来源：http://hz.ybcxt.top/gtjnkifsuw.html

Perl ........... 10
来源：http://hz.tanke756.top/gtuvuddgrv.html

Scala .......... 10
来源：http://hz.zhoulong.xyz/gtdnasakjt.html

------------------------------------
来源：http://hz.shangyingyoupin.top/gttbvpraaq.html

合计 ........... 2106 条
来源：http://hz.svipenyu.cn/gtcxvpadwv.html

按章节统计：
来源：http://hz.hnxiangtu.top/gtsdhtsqva.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.daxiang520.top/gtvhsoiwcu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cheryme.top/gthlzagfvd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yangfankeji.com/gtihmjxfse.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.ppjwa.cn/gtypftzcwf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yj20258888.top/gtocqgfahf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jinqigufen.top/gtkwajyeyq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.aizwys.cn/gtrciqgepv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.0kj1m.cn/gtyxppgysd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.cucudq.cn/gttyilkbke.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.yuanzhike.top/gtytsevney.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtficbdxbg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.bjfxy.top/gtyaswczse.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtypxbgkfj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtstoppwga.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xinyue.icu/gthgkwfsko.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtfklokboq.html

Q SQL 专题                              90
来源：http://hz.nanxinkj.top/gtboiiyodh.html

R Bash 专题                             80
来源：http://hz.hnxiangtu.top/gtkdozmned.html

S C / C++ 专题                          60
来源：http://hz.mhx1999.top/gtokogkogf.html

T 其他语言补充                          60
来源：http://hz.aibaodan.cn/gtrcqltshi.html

U 高频实用片段                         120
来源：http://hz.zhengqikj.top/gtfentfuew.html

------------------------------------
来源：http://hz.nanxuanxn.top/gtrqutshyj.html

合计                                  2106 条
来源：http://hz.jinqigfzy.top/gtfpnadgvh.html

--------------------------------------------------------------------------------
来源：http://hz.svipenyu.cn/gtaafmoevx.html

使用提醒
来源：http://hz.ybcxt.top/gtnpfxfctx.html

--------------------------------------------------------------------------------
来源：http://hz.sweek.top/gtwuegvkzd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.wangshuangyany.cn/gtgepztjfl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.guannengcc.top/gtxyqgztlr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.shzxlz.cn/gttixdsvqr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.iojbl.cn/gtnnkaehvi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.ybcxt.top/gttboxgtzv.html

—— 文件结束 ——
来源：http://hz.fzhhl.top/gtiercxhho.html

================================================================================
来源：http://hz.quarkkingdee.top/gtinoagfoi.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.sysykeji.top/gtyttvkpek.html

Common Programming Examples Cheat Book
来源：http://hz.hnqzz.top/gtmblkrlpr.html

================================================================================
来源：http://hz.tian-w.cn/gtdlijnbyk.html

【收录内容】
来源：http://hz.gzhubu.top/gtfqhnxcxr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.pycfn.com/gtlfuudcwe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.wangshuangyany.cn/gtupimtysg.html

SQL · Bash · C · C++
来源：http://hz.zhiwuduotai.top/gtlgzlbhbu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yueranfly.top/gtygjmhtzw.html

【使用说明】
来源：http://hz.jinyuanbaomall.cn/gtzuvsdbve.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ybcxt.top/gtxachsofu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.chenlongwang.top/gtkfzpfvrm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.chenjidiqi.icu/gtatpgdavb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.feifeiyinyue.top/gtbfghqerz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yangfankeji.com/gttjnequbk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.chenlongwang.top/gtcouejmqe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.316326.xyz/gtfsaqwkmc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.gogol.net.cn/gtmamylfnw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinqigufen.top/gtsdkfspko.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yuanzhike.top/gtkjldmlhh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.andypj.xyz/gtukwhamgo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.havefunace.top/gtkobeelzk.html

【文件统计】
来源：http://hz.sweek.top/gttucvtebc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jyoumei.cn/gtgnjyoauy.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gteuqkwnpp.html

目  录
来源：http://hz.cheryme.top/gtyuwlzuyb.html

--------------------------------------------------------------------------------
来源：http://hz.hysaishi.cn/gtoqmapsck.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.52xcode.cn/gtdypdmqrm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinghuilouyu.cn/gtpctnykra.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.nanxinkj.top/gtqekjlbns.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jinyuanbaomall.cn/gtqdiamlzr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hnxiangtu.top/gtajzzgkeg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yongpay.top/gttpmhgesm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gthxzttxmc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ywan-chungtsiang.top/gtzlzxrztu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xuetiantiany.cn/gtidjreqbi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yvedp.cn/gteevkkuac.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gtfweoyuji.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gtdukxgwpk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhijiandao.cn/gtfnxqhupi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.chenzaomai.com/gtinqpkpxf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.aizwys.cn/gtvufwihpz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtyhikbmlk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yonumen.top/gtuuoetnba.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yj20258888.top/gtpuwqjkge.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yvedp.cn/gttzzcvftt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.svipenyu.cn/gtnyhhmokr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.316326.xyz/gtpbcorsta.html

================================================================================
来源：http://hz.zycfv.cn/gtipctmpfa.html

A. 基础语法与类型
来源：http://hz.xinyue.icu/gtpmphjick.html

================================================================================
来源：http://hz.tian-w.cn/gtczwidkuu.html

[A01] Hello World
来源：http://hz.316326.xyz/gtnhimujql.html

Py:   print("Hello, World!")
来源：http://hz.ppjwa.cn/gtrupzdcgv.html

PHP:  echo "Hello, World!";
来源：http://hz.tianlin.xyz/gtacznjzqo.html

JS:   console.log("Hello, World!");
来源：http://hz.zycfv.cn/gtmzgjkvdg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yvedp.cn/gtguezlsao.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenzaomai.com/gthxdgwvah.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.yuxming.cn/gtjmoviidy.html

Ruby: puts "Hello, World!"
来源：http://hz.tian-w.cn/gtfvbaltst.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hammf.cn/gtlldcedum.html

[A02] 变量声明与赋值
来源：http://hz.tianlin.xyz/gtlfvqqjve.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.feifeiyinyue.top/gtofcyiaeb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.sxryk.cn/gtqmzedtbp.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yj202588.top/gtfxaynlwm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.tianlin.xyz/gtcfmvrmuw.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ywan-chungtsiang.top/gtugnzcube.html

Go:   name := "Alex"; age := 20
来源：http://hz.hysaishi.cn/gtknwiarux.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinqigfzy.top/gtswbbuglf.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.cdnleiting.top/gtxufcmbel.html

[A03] 常量定义
来源：http://hz.hfpthk.cn/gtubhfhmcy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhaomingkeji.xyz/gtnpydescj.html

PHP:  const PI = 3.14159;
来源：http://hz.c1oappe.top/gtujgoyzgi.html

JS:   const PI = 3.14159;
来源：http://hz.birdmap.top/gtrnfabzqd.html

TS:   const PI: number = 3.14159;
来源：http://hz.aibaodan.cn/gtxsnyjtso.html

Java: static final double PI = 3.14159;
来源：http://hz.snrcjt.cn/gtszkonvcw.html

Go:   const PI = 3.14159
来源：http://hz.yangfankeji.com/gtdebkhdqk.html

Ruby: PI = 3.14159
来源：http://hz.fengsongda.top/gtvfsdchnt.html

C#:   const double PI = 3.14159;
来源：http://hz.snrcjt.cn/gtqrfgoith.html

[A04] 判断变量类型
来源：http://hz.wangshuangyany.cn/gtqmprjdwr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.nanxuanxn.top/gtgtlwvkuz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yj20258.top/gtickqikmu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yj20258888.top/gtdoxcgiuy.html

TS:   typeof x; x instanceof Date
来源：http://hz.yonumen.top/gtzdaldjlz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.0kj1m.cn/gtdghtnptw.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.gzhubu.top/gtoidcjjxz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.cqqwz.cn/gtzdbwtiiz.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhengqikj.top/gtudrzosfa.html

[A05] 整数除法与取模
来源：http://hz.xingfuxueyuan.xyz/gtwzpihkvg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.shanyushiyangtech.top/gtxqcpjqts.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.tianlin.xyz/gtqmjcyrep.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.smart0.xyz/gtnjwbahbp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.birdmap.top/gtpmwrtfvf.html

Java: 7 / 2; 7 % 2
来源：http://hz.svipenyu.cn/gttxsfruna.html

Go:   7 / 2; 7 % 2
来源：http://hz.jinqigfzy.top/gtyrwpezzx.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.havefunace.top/gtfpuffiak.html

C#:   7 / 2; 7 % 2
来源：http://hz.sxryk.cn/gtfyajguat.html

[A06] 字符串转数字
来源：http://hz.hysaishi.cn/gtqkrtpzyc.html

Py:   int("42"); float("3.14")
来源：http://hz.hongshengwenyu.top/gtkoozyqmp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.kuanghao11.cn/gtjosafwjr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.pycfn.com/gtvxxtexis.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.wangshuangyany.cn/gtyrnrbvgv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yueranfly.top/gtlinmwrdm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yongpay.top/gtbnxaepbm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jianghu66.top/gtwljtwdmp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.wangshuangyany.cn/gtxjfademm.html

[A07] 数字转字符串
来源：http://hz.zhengqikj.top/gtcnwqqqcu.html

Py:   str(42)
来源：http://hz.shanyushiyangtech.top/gtxpchypln.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhiwuduotai.top/gtilafrjje.html

JS:   String(42); (42).toString()
来源：http://hz.gaohongyu789.top/gtjnswljxh.html

TS:   String(42)
来源：http://hz.aibaodan.cn/gtnuyxdxjp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.nanxuanxn.top/gtwavwinhf.html

Go:   strconv.Itoa(42)
来源：http://hz.hnqzz.top/gtisqbcssf.html

Ruby: 42.to_s
来源：http://hz.chenzaomai.com/gtwwbwmwtg.html

C#:   42.ToString()
来源：http://hz.52xcode.cn/gtzkzaipif.html

[A08] 取整与四舍五入
来源：http://hz.snrcjt.cn/gtpobdfffl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.hammf.cn/gtcxgpugrk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.pycfn.com/gtvwcgxwzj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.birdmap.top/gtwzpsdnfg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zhaomingkeji.xyz/gtgrqzphgv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.gogol.net.cn/gtwwmcabwf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.pycfn.com/gtrhmokaff.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yuxming.cn/gtsxdtyhrn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.nwbrower.top/gtemzdnbyj.html

[A09] 绝对值与最大最小值
来源：http://hz.tanke756.top/gtvrzelyrh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.dianchejie.cn/gtfiyxixlx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.aibaodan.cn/gtbgoqvdeq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yj20258888.top/gtuzxmafhf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.havefunace.top/gtzbpnnddf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hnxiangtu.top/gtathafvrg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.hammf.cn/gtbesatymm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.yj20258.top/gticmscoll.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.dashuyun.cn/gtcofhexmd.html

[A10] 生成随机数
来源：http://hz.xuanzx.com/gttzwnltgp.html

Py:   import random; random.randint(1, 100)
来源：http://hz.aizwys.cn/gtfbcmggce.html

PHP:  random_int(1, 100);
来源：http://hz.xuanzx.com/gtrepwpnvz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.smart0.xyz/gtcjxxxnua.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.quarkkingdee.top/gtajaximkq.html

Java: new Random().nextInt(100) + 1
来源：http://hz.iojbl.cn/gtdhpxkqtz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.sysykeji.top/gtiwyanbxz.html

Ruby: rand(1..100)
来源：http://hz.tianlin.xyz/gtupucqdvl.html

C#:   new Random().Next(1, 101)
来源：http://hz.chenjidiqi.icu/gtwlsihdpc.html

[A11] 条件表达式（三元）
来源：http://hz.guannengcc.top/gtbqebdfic.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jiagoushi.top/gtdklyylfl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.cheryme.top/gtbmkqsrgt.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.hysaishi.cn/gtakjjofpe.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.andypj.xyz/gtyqpvjqje.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.vqdsnc.cn/gtbwwforwy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.0kj1m.cn/gtwlqcfvir.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.jinghuilouyu.cn/gtwaivchmm.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.xinyue.icu/gtcyhhgdgl.html

[A12] 字符串插值 / 格式化
来源：http://hz.shanyushiyangtech.top/gtkchajosl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.guannengcc.top/gtdgymzedr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.redwolf501.top/gtxfwckbhv.html

JS:   `Hello, ${name}!`
来源：http://hz.zhiwuduotai.top/gthkzkejej.html

TS:   `Hello, ${name}!`
来源：http://hz.cheryme.top/gtigaexjar.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zhaomingkeji.xyz/gtajonwaaq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.hnqzz.top/gtiayohmrr.html

Ruby: "Hello, #{name}!"
来源：http://hz.daxiang520.top/gthpjwfyxl.html

C#:   $"Hello, {name}!"
来源：http://hz.nanxinkj.top/gtmmslbxpi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yuxming.cn/gtfxdubfeq.html

Py:   "第一行\n第二行"
来源：http://hz.hywenlv.cn/gtzndvznfj.html

PHP:  "第一行\n第二行"
来源：http://hz.xylfe.cn/gtsutrqkwr.html

JS:   "第一行\n第二行"
来源：http://hz.52xcode.cn/gtppfsnanr.html

TS:   "第一行\n第二行"
来源：http://hz.jiagoushi.top/gtrkevuiix.html

Java: "第一行\n第二行"
来源：http://hz.gogol.net.cn/gtzbpspnip.html

Go:   "第一行\n第二行"
来源：http://hz.jinqigufen.top/gtvbijqhvt.html

Ruby: "第一行\n第二行"
来源：http://hz.hnxiangtu.top/gtqdtdsasc.html

C#:   "第一行\n第二行"
来源：http://hz.daria6918.cn/gttcjifrtu.html

[A14] 注释写法
来源：http://hz.mhx1999.top/gtkcguwmxl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.0kj1m.cn/gthhgybpdc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.smart0.xyz/gtygsvruuq.html

JS:   // 单行；/* 多行 */
来源：http://hz.guowangkeji.top/gtrkewicxd.html

TS:   // 单行；/* 多行 */
来源：http://hz.haohaochexian.top/gttjnkptbl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.jianghu66.top/gtultofjzs.html

Go:   // 单行；/* 多行 */
来源：http://hz.jlsjyb.cn/gtbgaghtef.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.zhijiandao.cn/gtiwkonmin.html

C#:   // 单行；/* 多行 */
来源：http://hz.chenlongwang.top/gtbnrjzazm.html

[A15] 空值判断与默认值
来源：http://hz.aizwys.cn/gtujokdulw.html

Py:   value = data or "默认值"
来源：http://hz.wangdashe.top/gthlxagfpb.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.cqqwz.cn/gtaqcdgilq.html

JS:   const value = data ?? "默认值";
来源：http://hz.zdqjudy.top/gtlfysqnqq.html

TS:   const value = data ?? "默认值";
来源：http://hz.daria6918.cn/gtmyeqkpjk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.cdnleiting.top/gthkhymwrb.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.smart0.xyz/gtwpawaems.html

Ruby: value = data || "默认值"
来源：http://hz.yuxming.cn/gtpdqugstw.html

C#:   var value = data ?? "默认值";
来源：http://hz.jinyuanbaomall.cn/gtkdncrxny.html

[A16] 真假值判断规则
来源：http://hz.wangshuangyany.cn/gtdztcvdhb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.shzxlz.cn/gtknpyvbwo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.chenlongwang.top/gtcrjeyikn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.cdnleiting.top/gtzvylzmfx.html

TS:   if (!x) {}
来源：http://hz.redwolf501.top/gtvscasvfc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.zhijiandao.cn/gtzlzswozg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.shzxlz.cn/gtrxttirzh.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.52xcode.cn/gtzjugmcwk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.shanyushiyangtech.top/gtvrmhpfiw.html

[A17] 位运算
来源：http://hz.vqdsnc.cn/gtelqsgncn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangdashe.top/gtctjbxxfr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.jinqigfzy.top/gturgbzooc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.guowangkeji.top/gtzgzzlrro.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.hnxiangtu.top/gtydalmefh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gotoacloud.top/gtgticplvd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.yanxiufei.cn/gtspxmoxcm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cdnleiting.top/gtaqhodjqu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj202588.top/gtihcalxfy.html

[A18] 字符与 ASCII 码互转
来源：http://hz.ywan-chungtsiang.top/gtratzijph.html

Py:   ord("A"); chr(65)
来源：http://hz.jyoumei.cn/gtvcikhmfj.html

PHP:  ord("A"); chr(65)
来源：http://hz.zhengqikj.top/gtskbeulld.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nanxinkj.top/gtehvyffbd.html


<!-- 参考信息 -->