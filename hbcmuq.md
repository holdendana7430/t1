代发 wailian999

[U103] JS：定时器
来源：http://hz.yvedp.cn/gthvvdcvji.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.guannengcc.top/gtnnlxxrwi.html

[U104] JS：防抖
来源：http://hz.ywan-chungtsiang.top/gtwaizcmxh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.mhx1999.top/gtvwqlfwev.html

[U105] JS：节流
来源：http://hz.sweek.top/gtfpohnrat.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hysaishi.cn/gtyjqsspit.html

[U106] JS：日期格式化
来源：http://hz.dianchejie.cn/gtqsyqumfr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhixingplan.top/gtkgatcmaf.html

[U107] JS：数字千分位
来源：http://hz.yj20258.top/gtdtxtejzo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hammf.cn/gtnltvuokq.html

[U108] JS：随机整数
来源：http://hz.316326.xyz/gtssyumnaa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhengqikj.top/gtqlbkjjpn.html

[U109] JS：数组分组
来源：http://hz.feifeiyinyue.top/gtaagratln.html

Object.groupBy(arr, x => x.type)
来源：http://hz.zhoulong.xyz/gtbunlocey.html

[U110] JS：数组分块
来源：http://hz.gzhubu.top/gtzbrrbwnm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.shanyushiyangkeji.top/gtkjljnbmr.html

[U111] JS：对象转 Map
来源：http://hz.zhoulong.xyz/gtnhqshoqh.html

new Map(Object.entries(obj))
来源：http://hz.aibaodan.cn/gtympvpiwe.html

[U112] JS：字符串补位
来源：http://hz.tianlin.xyz/gtegoacbyn.html

"7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gtmndznckx.html

[U113] JS：正则替换全部
来源：http://hz.gzhubu.top/gtkxyuepxs.html

s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtqhihjqlr.html

[U114] JS：JSON 深比较
来源：http://hz.316326.xyz/gtiufzigyl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.redwolf501.top/gtlboxhzjx.html

[U115] JS：生成 UUID
来源：http://hz.shangyingyoupin.top/gtkwawcguu.html

crypto.randomUUID()
来源：http://hz.yj202588.top/gtisuufuad.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.shuidangran.top/gtbmzmgqmm.html

/** @param {string} name */ function f(name) {}
来源：http://hz.ywan-chungtsiang.top/gtaqabjtgl.html

[U117] JS：单元测试
来源：http://hz.yanxiufei.cn/gtkangamhn.html

npm i -D vitest;  npx vitest
来源：http://hz.pycfn.com/gtbaooiqmq.html

[U118] JS：开发服务器
来源：http://hz.gzhubu.top/gthwihtvjb.html

npm i -D vite;  npx vite
来源：http://hz.birdmap.top/gtlmaumiag.html

[U119] JS：生产构建
来源：http://hz.birdmap.top/gtfqxwwssf.html

npx vite build
来源：http://hz.zycfv.cn/gtqmowpafy.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yj20258888.top/gtwjhfvgmr.html

import.meta.env.VITE_API_URL
来源：http://hz.zhongyouzk.top/gturecayms.html

================================================================================
来源：http://hz.ppjwa.cn/gtvluaosvg.html

统计汇总
来源：http://hz.snrcjt.cn/gtulvisjor.html

================================================================================
来源：http://hz.bjfxy.top/gteilcrmmt.html

按语言统计（条）：
来源：http://hz.iojbl.cn/gtehwonqvk.html

Python ......... 252
来源：http://hz.hongshengwenyu.top/gtbzoxinrx.html

PHP ............ 252
来源：http://hz.zhaomingkeji.xyz/gtyleaxdyc.html

JavaScript ..... 252
来源：http://hz.fengsongda.top/gtsenhfrit.html

TypeScript ..... 212
来源：http://hz.yangfankeji.com/gtrgqnfesb.html

Java ........... 212
来源：http://hz.wangshuangyany.cn/gtbkqmjvcw.html

Go ............. 212
来源：http://hz.sysykeji.top/gtgdgwlawo.html

Ruby ........... 212
来源：http://hz.zycfv.cn/gtaoqwkjvo.html

C# ............. 212
来源：http://hz.chenjidiqi.icu/gtrezkxoju.html

C .............. 30
来源：http://hz.yvedp.cn/gtrfhkishs.html

C++ ............ 30
来源：http://hz.shuidangran.top/gtcatdoafm.html

SQL ............ 90
来源：http://hz.feifeiyinyue.top/gtqwlrsbuj.html

Bash ........... 80
来源：http://hz.xuetiantiany.cn/gtcnaopwxw.html

Kotlin ......... 15
来源：http://hz.redwolf501.top/gtlkoqasmy.html

Swift .......... 15
来源：http://hz.zycfv.cn/gtnggzafpz.html

Lua ............ 10
来源：http://hz.cheryme.top/gtbldtyzlq.html

Perl ........... 10
来源：http://hz.yongpay.top/gttzhcydsa.html

Scala .......... 10
来源：http://hz.iojbl.cn/gtppbkntny.html

------------------------------------
来源：http://hz.xuetiantiany.cn/gtqvcqbnzm.html

合计 ........... 2106 条
来源：http://hz.yueranfly.top/gtvkqrywzq.html

按章节统计：
来源：http://hz.guowangkeji.top/gtvnznxkaz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.cdnleiting.top/gtduefmutq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jqgfzy.top/gtttstamka.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtrbandowf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.fzhhl.top/gtqoylpqjj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hnqzz.top/gtcdiiujuv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhongyouzk.top/gtesmxutel.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.bjfxy.top/gtdaqenwud.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nwbrower.top/gtxmkpgakl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtqyacuobm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.c1oappe.top/gttxokeubt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtzydnspmr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ivvv.top/gtdcadtbhk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.yonumen.top/gtcnbpwovp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sweek.top/gtarpsakmm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shangyingyoupin.top/gtzwlueaxj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.cashguo.top/gtfjpzudyc.html

Q SQL 专题                              90
来源：http://hz.chenlongwang.top/gtdqshhctu.html

R Bash 专题                             80
来源：http://hz.jyoumei.cn/gtxfoyxefj.html

S C / C++ 专题                          60
来源：http://hz.sweek.top/gtoeawnnmo.html

T 其他语言补充                          60
来源：http://hz.gotoacloud.top/gtwddklyvg.html

U 高频实用片段                         120
来源：http://hz.sysykeji.top/gtkvkyqnvt.html

------------------------------------
来源：http://hz.cucudq.cn/gttuyigxtj.html

合计                                  2106 条
来源：http://hz.yj20258888.top/gtnnfxgidm.html

--------------------------------------------------------------------------------
来源：http://hz.havefunace.top/gtmqolvapp.html

使用提醒
来源：http://hz.chenlongwang.top/gtapqcvfls.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtkpkkreni.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.ydjk.org.cn/gtllvutheu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.iojbl.cn/gtmbpkkdkt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.tianlin.xyz/gtjtsjkvfj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sxryk.cn/gtbgcplbaq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cqqwz.cn/gtkhctavuy.html

—— 文件结束 ——
来源：http://hz.nwbrower.top/gtnebfphjh.html

================================================================================
来源：http://hz.gzhubu.top/gtgeautcpw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.guowangkeji.top/gtfjrvkndu.html

Common Programming Examples Cheat Book
来源：http://hz.quarkkingdee.top/gtzihxxrjs.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlbphifgs.html

【收录内容】
来源：http://hz.nwbrower.top/gtcfvqtsvh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.tanke756.top/gtagwuodvj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yj202588.top/gtlfdcrvmq.html

SQL · Bash · C · C++
来源：http://hz.meibo888.top/gtedrvhgma.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.tianlin.xyz/gtpckpljve.html

【使用说明】
来源：http://hz.chenlongwang.top/gtncxmjous.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xinyue.icu/gtlpugtdji.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.dashuyun.cn/gtafrqcvtq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ybcxt.top/gtammettgb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sysykeji.top/gtyunkmaas.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.pycfn.com/gtqmxzckpn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.hywenlv.cn/gtesmpgwvr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.redwolf501.top/gtehfxivdd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yonumen.top/gtnvuxrsif.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yj20258888.top/gtoobwyjti.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xziqi.cn/gtevtvihzy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hnxiangtu.top/gtabiyqjry.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xinyue.icu/gtupqipgcy.html

【文件统计】
来源：http://hz.daria6918.cn/gtkmmfxpnl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.nanxinkj.top/gtdwncpkdp.html

--------------------------------------------------------------------------------
来源：http://hz.cashguo.top/gtxdukajde.html

目  录
来源：http://hz.gogol.net.cn/gtfvfkmsgw.html

--------------------------------------------------------------------------------
来源：http://hz.chenlongwang.top/gtxbndjkcp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.wangdashe.top/gtugqlldwp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinqigfzy.top/gtoanbqyyc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hywenlv.cn/gtqsyrxcoz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.mhx1999.top/gtcskkfxku.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jqgufenzy.top/gtqlqqpqdq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.kuanghao11.cn/gtopldaagj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.redwolf501.top/gtagapaqma.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.cdnleiting.top/gtvnymbfea.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtijjdagjr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.dashuyun.cn/gtvecoprjj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.vqdsnc.cn/gtsnnshoca.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.52xcode.cn/gtxvilacgq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtvsvfrasj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.chenjidiqi.icu/gtqvhjexaj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.kuanghao11.cn/gtzbppdqvs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yj202588.top/gtqnmvreco.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.sufxvd.cn/gtoembqyal.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.fzhhl.top/gtvmwuaazx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yj20258888.top/gtovdpvdrn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gthjuyubft.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.tanke756.top/gtgvyzudrv.html

================================================================================
来源：http://hz.xylfe.cn/gtugpojkjz.html

A. 基础语法与类型
来源：http://hz.shangyingyoupin.top/gtltiwrcht.html

================================================================================
来源：http://hz.52xcode.cn/gtxncdkrav.html

[A01] Hello World
来源：http://hz.jqgfzy.top/gtzzigfknq.html

Py:   print("Hello, World!")
来源：http://hz.ybcxt.top/gtnqoxfyea.html

PHP:  echo "Hello, World!";
来源：http://hz.bjfxy.top/gtolbwnqsh.html

JS:   console.log("Hello, World!");
来源：http://hz.c1oappe.top/gtiyiyynkz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cqqwz.cn/gtilazpraa.html

Java: System.out.println("Hello, World!");
来源：http://hz.jinyuanbaomall.cn/gtxyesgcjh.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.guowangkeji.top/gtejpodibc.html

Ruby: puts "Hello, World!"
来源：http://hz.shanyushiyangtech.top/gtvayjmfwd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yonumen.top/gtjiihrlpp.html

[A02] 变量声明与赋值
来源：http://hz.chenjidiqi.icu/gtquulkdui.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yanxiufei.cn/gtfmgvsoqs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yuxming.cn/gtjifkbriy.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.gotoacloud.top/gtzcaqwyce.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xuanzx.com/gtnwgpwtdl.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.pycfn.com/gtmaxfttob.html

Go:   name := "Alex"; age := 20
来源：http://hz.smart0.xyz/gtbjqworex.html

Ruby: name = "Alex"; age = 20
来源：http://hz.daxiang520.top/gtvhhlwebt.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.meibo888.top/gtonbqvhsk.html

[A03] 常量定义
来源：http://hz.hywenlv.cn/gtufsevfsg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.vqdsnc.cn/gtzipokito.html

PHP:  const PI = 3.14159;
来源：http://hz.redwolf501.top/gtwmturprx.html

JS:   const PI = 3.14159;
来源：http://hz.birdmap.top/gtzczsyhri.html

TS:   const PI: number = 3.14159;
来源：http://hz.havefunace.top/gtsbflozvt.html

Java: static final double PI = 3.14159;
来源：http://hz.sysykeji.top/gtkxdiziuh.html

Go:   const PI = 3.14159
来源：http://hz.hfpthk.cn/gtchxepyro.html

Ruby: PI = 3.14159
来源：http://hz.daxiang520.top/gtqonexfge.html

C#:   const double PI = 3.14159;
来源：http://hz.xylfe.cn/gtqmcaadso.html

[A04] 判断变量类型
来源：http://hz.ehwqpu.com/gtucbrqevk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.aibaodan.cn/gtvztqkiib.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ehwqpu.com/gtmvppbmum.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gzhubu.top/gtappqzeub.html

TS:   typeof x; x instanceof Date
来源：http://hz.316326.xyz/gtkroxszfd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hywenlv.cn/gtyawjlsju.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yuxming.cn/gtgjwgears.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gaohongyu789.top/gtqllmulwj.html

C#:   x.GetType().Name; x is int
来源：http://hz.hywenlv.cn/gthwfkxzxt.html

[A05] 整数除法与取模
来源：http://hz.smart0.xyz/gtspmalopt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.gaohongyu789.top/gtjfoksbog.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.pengpengdd.cyou/gtkpogkfrj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ivvv.top/gtjvtjshkl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtqwifjxcw.html

Java: 7 / 2; 7 % 2
来源：http://hz.ehwqpu.com/gttkvkjosy.html

Go:   7 / 2; 7 % 2
来源：http://hz.gogol.net.cn/gtreqenilj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.xziqi.cn/gtnneqgplt.html

C#:   7 / 2; 7 % 2
来源：http://hz.fzhhl.top/gtbsbfgugq.html

[A06] 字符串转数字
来源：http://hz.hnxiangtu.top/gtabpvhvtt.html

Py:   int("42"); float("3.14")
来源：http://hz.iojbl.cn/gtqpwqnjon.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.andypj.xyz/gtbgqdpxpv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cashguo.top/gtotgixoau.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jinqigufen.top/gtljaqvzqq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.wangdashe.top/gtxczfujgs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.zhoulong.xyz/gtgwvvfyrg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jlsjyb.cn/gtvtjnwwsy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.shzxlz.cn/gtihygsfdx.html

[A07] 数字转字符串
来源：http://hz.tian-w.cn/gtakrbasud.html

Py:   str(42)
来源：http://hz.chenjidiqi.icu/gtbzratoab.html

PHP:  (string) 42; strval(42)
来源：http://hz.havefunace.top/gtibqrdrnj.html

JS:   String(42); (42).toString()
来源：http://hz.iojbl.cn/gtxqcaymvp.html

TS:   String(42)
来源：http://hz.hnxiangtu.top/gtdijcwhcf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.quarkkingdee.top/gtwjkqhity.html

Go:   strconv.Itoa(42)
来源：http://hz.zhengqikj.top/gtcwbqopel.html

Ruby: 42.to_s
来源：http://hz.ehwqpu.com/gttxpooiwb.html

C#:   42.ToString()
来源：http://hz.havefunace.top/gtgdzzaswv.html

[A08] 取整与四舍五入
来源：http://hz.nanxinkj.top/gtorzhwbni.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.cqqwz.cn/gtfsghmyke.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.snrcjt.cn/gtmlhzlvjp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.cqqwz.cn/gttodljiva.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.quarkkingdee.top/gtwktbuydm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jqgufenzy.top/gtdfzgspmu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.cheryme.top/gtiwmewukd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.fengsongda.top/gtatpjdbvi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.ywan-chungtsiang.top/gtxewrozkd.html

[A09] 绝对值与最大最小值
来源：http://hz.jlsjyb.cn/gtfptjedxm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.sufxvd.cn/gtpwldhxjx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hammf.cn/gtbztlzbys.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.52xcode.cn/gtajvoycvy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.pengpengdd.cyou/gtqnqricdi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hfpthk.cn/gtmxxaxytf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.9152youxi.cn/gtwcgkfiwj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.xuetiantiany.cn/gtpxrmqfuq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.tianlin.xyz/gtvdfzecmu.html

[A10] 生成随机数
来源：http://hz.yj202588.top/gtncvujrcp.html

Py:   import random; random.randint(1, 100)
来源：http://hz.chenzaomai.com/gtcctvensh.html

PHP:  random_int(1, 100);
来源：http://hz.hywenlv.cn/gtszqkepjx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.andypj.xyz/gtlgxrzuwy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.xinyue.icu/gtirrvogfj.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yueranfly.top/gtjveewxwy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.andypj.xyz/gtcvlqahyv.html

Ruby: rand(1..100)
来源：http://hz.dashuyun.cn/gttywmkurv.html

C#:   new Random().Next(1, 101)
来源：http://hz.tianlin.xyz/gtcchisadu.html

[A11] 条件表达式（三元）
来源：http://hz.shanyushiyangkeji.top/gtlhrllpnr.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.xylfe.cn/gtuyebgpvt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.chenzaomai.com/gtqutjzxkc.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yueranfly.top/gtxaffmwsp.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.gzhubu.top/gtwojromzi.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.pycfn.com/gtqxyggkbu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.smart0.xyz/gtxyqqsowf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.xinyue.icu/gtpbyhfpcg.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.andypj.xyz/gtbvghglrd.html

[A12] 字符串插值 / 格式化
来源：http://hz.cqqwz.cn/gtuaeibosn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.yj20258.top/gtbjqtwwgk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.fzhhl.top/gtivxxojge.html

JS:   `Hello, ${name}!`
来源：http://hz.zhijiandao.cn/gtwuoaqswg.html

TS:   `Hello, ${name}!`
来源：http://hz.xylfe.cn/gtptyhbcsv.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.sysykeji.top/gtghrsfnsg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.52xcode.cn/gtdunezmuh.html

Ruby: "Hello, #{name}!"
来源：http://hz.vqdsnc.cn/gtufqothqv.html

C#:   $"Hello, {name}!"
来源：http://hz.jqgfzy.top/gtoucieyxq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.hysaishi.cn/gtznnddoqy.html

Py:   "第一行\n第二行"
来源：http://hz.tianlin.xyz/gtbeegsoux.html

PHP:  "第一行\n第二行"
来源：http://hz.wangdashe.top/gtalmujkvt.html

JS:   "第一行\n第二行"
来源：http://hz.quarkkingdee.top/gtstppisks.html

TS:   "第一行\n第二行"
来源：http://hz.ydjk.org.cn/gtrbmlhhlf.html

Java: "第一行\n第二行"
来源：http://hz.xziqi.cn/gtshngzguo.html

Go:   "第一行\n第二行"
来源：http://hz.hfpthk.cn/gtjvgqcwwv.html

Ruby: "第一行\n第二行"
来源：http://hz.yuanzhike.top/gtdzvhffiu.html

C#:   "第一行\n第二行"
来源：http://hz.bjfxy.top/gtusaaiart.html

[A14] 注释写法
来源：http://hz.hywenlv.cn/gtivozsssp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zycfv.cn/gtxffylujt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.tanke756.top/gtajialocl.html

JS:   // 单行；/* 多行 */
来源：http://hz.jinqigfzy.top/gtjtzejnjf.html

TS:   // 单行；/* 多行 */
来源：http://hz.wangdashe.top/gtssxcifmb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.yj20258888.top/gtkubbtxqr.html

Go:   // 单行；/* 多行 */
来源：http://hz.9152youxi.cn/gttfijsusv.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.zhiwuduotai.top/gtasmzpwxr.html

C#:   // 单行；/* 多行 */
来源：http://hz.hfpthk.cn/gtjwrrkqno.html

[A15] 空值判断与默认值
来源：http://hz.jinyuanbaomall.cn/gtokjlnepg.html

Py:   value = data or "默认值"
来源：http://hz.sysykeji.top/gtugdpinja.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.shanyushiyangkeji.top/gtlshtpdvy.html

JS:   const value = data ?? "默认值";
来源：http://hz.ydjk.org.cn/gttcfpyqwz.html

TS:   const value = data ?? "默认值";
来源：http://hz.jiagoushi.top/gtqgruqcyo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.hywenlv.cn/gthgbactrj.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.shzxlz.cn/gthcfcxiwe.html

Ruby: value = data || "默认值"
来源：http://hz.yongpay.top/gtrggdolbb.html

C#:   var value = data ?? "默认值";
来源：http://hz.aizwys.cn/gtkocwwxxy.html

[A16] 真假值判断规则
来源：http://hz.zhongyouzk.top/gtlieltyhx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yueranfly.top/gtojhmvhfb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.yvedp.cn/gtcbgiqjwm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.smart0.xyz/gtkjrdyank.html

TS:   if (!x) {}
来源：http://hz.0kj1m.cn/gtipwntmci.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.cucudq.cn/gtpsdysqmt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.shangyingyoupin.top/gthsncmbjx.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.wangshuangyany.cn/gtnsdmxeph.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.jinyuanbaomall.cn/gtkbmnhthd.html

[A17] 位运算
来源：http://hz.jinqigfzy.top/gtgjiazcug.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.pycfn.com/gtczznoztt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.xziqi.cn/gtnwsdbylb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuanzx.com/gtnuoaqser.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.hnqzz.top/gtebpettxo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gtximnyrrp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zdqjudy.top/gtfplgufbe.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.c1oappe.top/gtfdumasfn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fzhhl.top/gtnihlhihx.html

[A18] 字符与 ASCII 码互转
来源：http://hz.0kj1m.cn/gtprwjtcrt.html

Py:   ord("A"); chr(65)
来源：http://hz.cdnleiting.top/gtbgbfcgby.html

PHP:  ord("A"); chr(65)
来源：http://hz.yonumen.top/gtevqaqmfy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.cheryme.top/gtxlaoxkwz.html


<!-- 参考信息 -->