代发 wailian999

[U105] JS：节流
来源：http://hz.tian-w.cn/gtrikwzxbf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ywan-chungtsiang.top/gtjgouozhf.html

[U106] JS：日期格式化
来源：http://hz.hywenlv.cn/gtwsmddaeb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shanyushiyangkeji.top/gthhciiowl.html

[U107] JS：数字千分位
来源：http://hz.wangshuangyany.cn/gtoaccpzca.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.nanxinkj.top/gtycctonwl.html

[U108] JS：随机整数
来源：http://hz.cucudq.cn/gtazpcrqoe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.vqdsnc.cn/gtkiyulcft.html

[U109] JS：数组分组
来源：http://hz.ywan-chungtsiang.top/gtomhnjknq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gtdrctppho.html

[U110] JS：数组分块
来源：http://hz.yongpay.top/gtvnqywnnk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.dashuyun.cn/gtosoucjxp.html

[U111] JS：对象转 Map
来源：http://hz.meibo888.top/gtxjovvhbv.html

new Map(Object.entries(obj))
来源：http://hz.jlsjyb.cn/gtrbzfvepp.html

[U112] JS：字符串补位
来源：http://hz.zhengqikj.top/gtjzvzjske.html

"7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtdbuiixmv.html

[U113] JS：正则替换全部
来源：http://hz.yuanzhike.top/gteqzrqmxn.html

s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gthjqtnlre.html

[U114] JS：JSON 深比较
来源：http://hz.yongpay.top/gtochmcvfl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.havefunace.top/gtqhjlmtly.html

[U115] JS：生成 UUID
来源：http://hz.ydzc1.top/gtqmmmfxjs.html

crypto.randomUUID()
来源：http://hz.c1oappe.top/gtjyomyqjd.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhaomingkeji.xyz/gtmvrgiyxp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.pycfn.com/gtyztbduvf.html

[U117] JS：单元测试
来源：http://hz.nwbrower.top/gtwknycwcw.html

npm i -D vitest;  npx vitest
来源：http://hz.havefunace.top/gtorobnswq.html

[U118] JS：开发服务器
来源：http://hz.daxiang520.top/gtqxrugyqa.html

npm i -D vite;  npx vite
来源：http://hz.shzxlz.cn/gthvesfhao.html

[U119] JS：生产构建
来源：http://hz.gzhubu.top/gtntpmwvol.html

npx vite build
来源：http://hz.hammf.cn/gtspqgbwzt.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.nanxuanxn.top/gtdhkiwwei.html

import.meta.env.VITE_API_URL
来源：http://hz.hammf.cn/gtzhobjgxo.html

================================================================================
来源：http://hz.gaohongyu789.top/gtfwxvwfby.html

统计汇总
来源：http://hz.xuetiantiany.cn/gtoaofzfff.html

================================================================================
来源：http://hz.fengsongda.top/gtiqwtjigj.html

按语言统计（条）：
来源：http://hz.guowangkeji.top/gteznnnlds.html

Python ......... 252
来源：http://hz.smart0.xyz/gtmsydmoti.html

PHP ............ 252
来源：http://hz.guannengcc.top/gtfczpteif.html

JavaScript ..... 252
来源：http://hz.zycfv.cn/gtigmmhdwm.html

TypeScript ..... 212
来源：http://hz.fengsongda.top/gtdnrpnnuf.html

Java ........... 212
来源：http://hz.daria6918.cn/gtbknzmnbg.html

Go ............. 212
来源：http://hz.sufxvd.cn/gtvswvbeed.html

Ruby ........... 212
来源：http://hz.smart0.xyz/gtuodpfwsj.html

C# ............. 212
来源：http://hz.xuanzx.com/gtcghbphzg.html

C .............. 30
来源：http://hz.ydzc1.top/gtmagtqyjl.html

C++ ............ 30
来源：http://hz.zhongyouzk.top/gtvblvzybn.html

SQL ............ 90
来源：http://hz.ppjwa.cn/gtretyswba.html

Bash ........... 80
来源：http://hz.gogol.net.cn/gtyzmrsgdo.html

Kotlin ......... 15
来源：http://hz.cashguo.top/gtlgboucfr.html

Swift .......... 15
来源：http://hz.ivvv.top/gtgqvpeyio.html

Lua ............ 10
来源：http://hz.c1oappe.top/gtamiytnvz.html

Perl ........... 10
来源：http://hz.52xcode.cn/gtqorhklgg.html

Scala .......... 10
来源：http://hz.gzhubu.top/gtdcpjuykh.html

------------------------------------
来源：http://hz.quarkkingdee.top/gtrkvqywlh.html

合计 ........... 2106 条
来源：http://hz.jqgfzy.top/gtkpfxxwgd.html

按章节统计：
来源：http://hz.xuanzx.com/gtowxepueo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.sysykeji.top/gtgtksdcvg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.quarkkingdee.top/gtvtpmohvy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cucudq.cn/gtiwnjxdrv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zdqjudy.top/gtcefuwqpf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.mhx1999.top/gtoimmtgdz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhengqikj.top/gtdgjwlfyo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.haohaochexian.top/gtbiucbaxl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sweek.top/gtnjffilhf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yonumen.top/gtsquqekgr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.chenzaomai.com/gtefsoxfer.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.chenzaomai.com/gtfcuodmgx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtxmsecrgs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hnxiangtu.top/gtiraejhqz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jlsjyb.cn/gtuorhxqur.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.tianlin.xyz/gtdodroqif.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtdsosbjcw.html

Q SQL 专题                              90
来源：http://hz.wangshuangyany.cn/gttqwsydxe.html

R Bash 专题                             80
来源：http://hz.kuanghao11.cn/gtxaomfuvq.html

S C / C++ 专题                          60
来源：http://hz.wangshuangyany.cn/gtaszfbdnc.html

T 其他语言补充                          60
来源：http://hz.aibaodan.cn/gtcxoenypf.html

U 高频实用片段                         120
来源：http://hz.zhiwuduotai.top/gtykrosgpj.html

------------------------------------
来源：http://hz.c1oappe.top/gtgmpqpzhf.html

合计                                  2106 条
来源：http://hz.jinyuanbaomall.cn/gtxziydcpc.html

--------------------------------------------------------------------------------
来源：http://hz.bjfxy.top/gtsmgzqxob.html

使用提醒
来源：http://hz.aizwys.cn/gtrrkkdiei.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtmipuytky.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cqqwz.cn/gtdqnlafce.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ehwqpu.com/gtdjbxglle.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hnqzz.top/gtzosomoyw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.haohaochexian.top/gtvuzwzdqf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hywenlv.cn/gtrohjymxu.html

—— 文件结束 ——
来源：http://hz.jinyuanbaomall.cn/gtaqycumgr.html

================================================================================
来源：http://hz.ppjwa.cn/gtqovkmzbw.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xinyue.icu/gtbhkxvwpc.html

Common Programming Examples Cheat Book
来源：http://hz.snrcjt.cn/gtrogwrgdx.html

================================================================================
来源：http://hz.cucudq.cn/gtzqhlggqt.html

【收录内容】
来源：http://hz.havefunace.top/gtefpyfbjw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj202588.top/gtjsotsqyd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhijiandao.cn/gtqvipyaqs.html

SQL · Bash · C · C++
来源：http://hz.xuetiantiany.cn/gttxoypcrz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.havefunace.top/gthrykaedp.html

【使用说明】
来源：http://hz.hfpthk.cn/gtypvfweyb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xuetiantiany.cn/gtxgrxnbau.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.gzhubu.top/gtqdkuxuke.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hnxiangtu.top/gtgitouvej.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.snrcjt.cn/gtwqtiiasy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yj20258.top/gtpzjewmna.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gaohongyu789.top/gtobnhlhre.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.vqdsnc.cn/gttohfexap.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.iojbl.cn/gtixhilygr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jyoumei.cn/gtockdyprq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.guowangkeji.top/gtfdvnaubk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.dianchejie.cn/gtdaifjvik.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shzxlz.cn/gtswhzramc.html

【文件统计】
来源：http://hz.daxiang520.top/gtmpljydrd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.dianchejie.cn/gtlvppyifz.html

--------------------------------------------------------------------------------
来源：http://hz.ydzc1.top/gtfbdjhdzc.html

目  录
来源：http://hz.jqgfzy.top/gtdnbwwler.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gtwgmpioom.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.shanyushiyangtech.top/gtxfugqolk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.c1oappe.top/gtwohuupuu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zycfv.cn/gtkmadpfkm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ivvv.top/gtvpihnncv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jinghuilouyu.cn/gtfctgvqqv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.chenzaomai.com/gtymxocxrq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shangyingyoupin.top/gtnwtbxqvw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ydzc1.top/gtpqypqgyy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.fengsongda.top/gttaqastaf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.xylfe.cn/gtzzzjqmhm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jianghu66.top/gtcjzmuerd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.sufxvd.cn/gttcvhuqnc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.xylfe.cn/gtwixkbyik.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yj202588.top/gtnafxhhon.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.jinghuilouyu.cn/gtpemepnfp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.andypj.xyz/gtzrycblzq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nanxuanxn.top/gtammrguif.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.chenlongwang.top/gtzavjttvz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yuxming.cn/gtvoqvlmvs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jyoumei.cn/gtqjittaxu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.cashguo.top/gtwehhdwzk.html

================================================================================
来源：http://hz.jianghu66.top/gtwsqaohhv.html

A. 基础语法与类型
来源：http://hz.yj202588.top/gtmfweadnf.html

================================================================================
来源：http://hz.daria6918.cn/gtgieexxay.html

[A01] Hello World
来源：http://hz.fzhhl.top/gtbzzrqcpc.html

Py:   print("Hello, World!")
来源：http://hz.tianlin.xyz/gtfhfiqayl.html

PHP:  echo "Hello, World!";
来源：http://hz.iojbl.cn/gtsdpkwwgw.html

JS:   console.log("Hello, World!");
来源：http://hz.bjfxy.top/gtvxnuufbf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jqgfzy.top/gtbaaaahkk.html

Java: System.out.println("Hello, World!");
来源：http://hz.yonumen.top/gtlhbrixtk.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zhoulong.xyz/gtpcoqvafb.html

Ruby: puts "Hello, World!"
来源：http://hz.0kj1m.cn/gtgqizzqar.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ywan-chungtsiang.top/gthwhzrtcj.html

[A02] 变量声明与赋值
来源：http://hz.chenlongwang.top/gtnwmxqpuv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zycfv.cn/gtgemdcanh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ivvv.top/gtfivnmref.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.pengpengdd.cyou/gtbmewyryq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.meibo888.top/gttpzkukal.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.havefunace.top/gtaffjjosl.html

Go:   name := "Alex"; age := 20
来源：http://hz.zhengqikj.top/gtfhhjleop.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yuxming.cn/gtskvtdopy.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jinqigufen.top/gttmdtovjg.html

[A03] 常量定义
来源：http://hz.gogol.net.cn/gtyjyhkotx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jinyuanbaomall.cn/gtpavizdql.html

PHP:  const PI = 3.14159;
来源：http://hz.guannengcc.top/gtvnfymwpi.html

JS:   const PI = 3.14159;
来源：http://hz.iojbl.cn/gtutjpdwtp.html

TS:   const PI: number = 3.14159;
来源：http://hz.cdnleiting.top/gtedodzbzj.html

Java: static final double PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtmaqkwbab.html

Go:   const PI = 3.14159
来源：http://hz.svipenyu.cn/gtshwprfcq.html

Ruby: PI = 3.14159
来源：http://hz.daxiang520.top/gtltkzcnav.html

C#:   const double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtkdekkexe.html

[A04] 判断变量类型
来源：http://hz.sxryk.cn/gtkcqfjpvh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yonumen.top/gtonkyqdmm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hysaishi.cn/gtodzwbqsm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.jinyuanbaomall.cn/gtzbqpxxjg.html

TS:   typeof x; x instanceof Date
来源：http://hz.aizwys.cn/gtryfvsxyy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jianghu66.top/gtherfgawz.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.cashguo.top/gtrhjipwsh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yvedp.cn/gtwkajqjnp.html

C#:   x.GetType().Name; x is int
来源：http://hz.hammf.cn/gtvyldkirl.html

[A05] 整数除法与取模
来源：http://hz.yueranfly.top/gtlwfachuo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.nanxinkj.top/gtfyijrpwz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.shuidangran.top/gtyiqpuvon.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xylfe.cn/gtjxfworvb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yangfankeji.com/gtwdzhkikj.html

Java: 7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtwoqvxiyf.html

Go:   7 / 2; 7 % 2
来源：http://hz.gotoacloud.top/gtqlrzsjqw.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.sysykeji.top/gtnlzdbsmo.html

C#:   7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gtqgquhbrc.html

[A06] 字符串转数字
来源：http://hz.52xcode.cn/gtkbslxqdf.html

Py:   int("42"); float("3.14")
来源：http://hz.c1oappe.top/gtsnetdujj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.redwolf501.top/gtvfxpybmy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.pengpengdd.cyou/gtzzyaiydz.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.dianchejie.cn/gthtlusipg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.haohaochexian.top/gtslqasfqs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.hfpthk.cn/gtyuamlkal.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.9152youxi.cn/gtgfhducoh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.guowangkeji.top/gtcsrwjbdq.html

[A07] 数字转字符串
来源：http://hz.yj202588.top/gtevqurfna.html

Py:   str(42)
来源：http://hz.kuanghao11.cn/gtkyxvkppe.html

PHP:  (string) 42; strval(42)
来源：http://hz.jiagoushi.top/gteslvqadm.html

JS:   String(42); (42).toString()
来源：http://hz.jiagoushi.top/gtdyjiuecr.html

TS:   String(42)
来源：http://hz.9152youxi.cn/gtkpkfqaby.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.shanyushiyangtech.top/gtbviibufl.html

Go:   strconv.Itoa(42)
来源：http://hz.gogol.net.cn/gteyamihho.html

Ruby: 42.to_s
来源：http://hz.dianchejie.cn/gtyfavbqrf.html

C#:   42.ToString()
来源：http://hz.shuidangran.top/gttepvsjxw.html

[A08] 取整与四舍五入
来源：http://hz.yvedp.cn/gtxunsbeju.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jyoumei.cn/gtgevfosod.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.gotoacloud.top/gtzvryepzo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.vqdsnc.cn/gtkyopvhqr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.gaohongyu789.top/gtkjajihtl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jinyuanbaomall.cn/gtiyqumsfg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.dashuyun.cn/gtbueodriv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.chenzaomai.com/gtyxgtsimk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.52xcode.cn/gttwjptzag.html

[A09] 绝对值与最大最小值
来源：http://hz.redwolf501.top/gtzcfhytcg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cheryme.top/gtthcvzkrv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhongyouzk.top/gtkkuhlogs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhengqikj.top/gtulimqbix.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.redwolf501.top/gtebbaxumb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jinyuanbaomall.cn/gtqwrgbjil.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.dianchejie.cn/gtrzcmatno.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.tianlin.xyz/gtiyjiwjis.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.sufxvd.cn/gtjajgazgj.html

[A10] 生成随机数
来源：http://hz.andypj.xyz/gtokknrohr.html

Py:   import random; random.randint(1, 100)
来源：http://hz.dianchejie.cn/gtrnggxatj.html

PHP:  random_int(1, 100);
来源：http://hz.ppjwa.cn/gtbxbfxkeq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.daria6918.cn/gtgcrpovfr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.bjfxy.top/gtxzexjabu.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yuanzhike.top/gtkjjmeimf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.bjfxy.top/gtanxzqolj.html

Ruby: rand(1..100)
来源：http://hz.316326.xyz/gtckyiicgp.html

C#:   new Random().Next(1, 101)
来源：http://hz.tianlin.xyz/gtizppuuyi.html

[A11] 条件表达式（三元）
来源：http://hz.gotoacloud.top/gtopwnflsn.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.xuanzx.com/gtvpecehqb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.cheryme.top/gtuitloyzd.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gtltiruden.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.ppjwa.cn/gtxoxajirf.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yj20258.top/gtkjjbuvin.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.ydjk.org.cn/gtltczidnj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.daxiang520.top/gtcmjabxvy.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gthxuojlqn.html

[A12] 字符串插值 / 格式化
来源：http://hz.hysaishi.cn/gthdlszntg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.chenlongwang.top/gtorwtwkbc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.ppjwa.cn/gtlynfpjzw.html

JS:   `Hello, ${name}!`
来源：http://hz.52xcode.cn/gtbjkdhzzg.html

TS:   `Hello, ${name}!`
来源：http://hz.dianchejie.cn/gtrpgfqojo.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.ywan-chungtsiang.top/gtpfsppodt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jqgufenzy.top/gtmqoyhkvg.html

Ruby: "Hello, #{name}!"
来源：http://hz.jianghu66.top/gtwbowskfi.html

C#:   $"Hello, {name}!"
来源：http://hz.yj20258888.top/gtawoazutf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.daxiang520.top/gtxfsaiquu.html

Py:   "第一行\n第二行"
来源：http://hz.yangfankeji.com/gtgtppgbvm.html

PHP:  "第一行\n第二行"
来源：http://hz.mhx1999.top/gtfzpchnjf.html

JS:   "第一行\n第二行"
来源：http://hz.ydjk.org.cn/gtswejesoq.html

TS:   "第一行\n第二行"
来源：http://hz.birdmap.top/gtqqddiwso.html

Java: "第一行\n第二行"
来源：http://hz.wangshuangyany.cn/gthfrcfjih.html

Go:   "第一行\n第二行"
来源：http://hz.yuxming.cn/gtwnzdvqjo.html

Ruby: "第一行\n第二行"
来源：http://hz.iojbl.cn/gtrmknyuty.html

C#:   "第一行\n第二行"
来源：http://hz.316326.xyz/gtkwtpwvwu.html

[A14] 注释写法
来源：http://hz.guowangkeji.top/gtbcgxbpqi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.wangdashe.top/gtlfbulmsf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.xingfuxueyuan.xyz/gtxsnnihsj.html

JS:   // 单行；/* 多行 */
来源：http://hz.chenjidiqi.icu/gtmfzbktet.html

TS:   // 单行；/* 多行 */
来源：http://hz.hfpthk.cn/gtkugqonur.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.fzhhl.top/gtiqqynngs.html

Go:   // 单行；/* 多行 */
来源：http://hz.kuanghao11.cn/gtwfgmabea.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.haohaochexian.top/gtcnkctxay.html

C#:   // 单行；/* 多行 */
来源：http://hz.cashguo.top/gtviaweytc.html

[A15] 空值判断与默认值
来源：http://hz.shangyingyoupin.top/gthmxwmpca.html

Py:   value = data or "默认值"
来源：http://hz.hywenlv.cn/gtalfukjqz.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.yvedp.cn/gttedizdwz.html

JS:   const value = data ?? "默认值";
来源：http://hz.zhaomingkeji.xyz/gtnvsvrrtj.html

TS:   const value = data ?? "默认值";
来源：http://hz.xingfuxueyuan.xyz/gtdxfhznww.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.hysaishi.cn/gtuecroklz.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.daria6918.cn/gtyfvqfiou.html

Ruby: value = data || "默认值"
来源：http://hz.ppjwa.cn/gtldxobowq.html

C#:   var value = data ?? "默认值";
来源：http://hz.yj20258888.top/gtsbawmapw.html

[A16] 真假值判断规则
来源：http://hz.hongshengwenyu.top/gtielsrgir.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.xylfe.cn/gtkjswmliq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.fzhhl.top/gtckflgufh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.chenjidiqi.icu/gtcmqbltcj.html

TS:   if (!x) {}
来源：http://hz.jlsjyb.cn/gtuxanbmnp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.0kj1m.cn/gtfzkrljig.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.xylfe.cn/gtlxijavxh.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.xziqi.cn/gtnrybnugt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.fzhhl.top/gtuivzzwoy.html

[A17] 位运算
来源：http://hz.zhoulong.xyz/gtdbgazjqf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gttuwyrvld.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yj20258.top/gtkjhiprcc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sufxvd.cn/gtaysrorhe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.cqqwz.cn/gtvlcyjevj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenlongwang.top/gtpivgooxm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.wangshuangyany.cn/gtcrcqvzed.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gtczumvfsw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtuemcygtd.html

[A18] 字符与 ASCII 码互转
来源：http://hz.yanxiufei.cn/gtqbezhyvb.html

Py:   ord("A"); chr(65)
来源：http://hz.jiagoushi.top/gtkxpcipjd.html

PHP:  ord("A"); chr(65)
来源：http://hz.snrcjt.cn/gtkdhujhtg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jyoumei.cn/gtfpynzzzi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.daria6918.cn/gtxpseusyo.html

Java: (int) 'A'; (char) 65
来源：http://hz.jiagoushi.top/gtfflhkuup.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.jqgufenzy.top/gtqoiqkewm.html

Ruby: "A".ord; 65.chr
来源：http://hz.iojbl.cn/gtrrrngbcr.html


<!-- 参考信息 -->