代发 wailian999

[U105] JS：节流
来源：http://hz.ppjwa.cn/gthwvsxrcn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.jianghu66.top/gtbwgjrkqk.html

[U106] JS：日期格式化
来源：http://hz.zycfv.cn/gtxqnppzmh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yvedp.cn/gtdtzijwwh.html

[U107] JS：数字千分位
来源：http://hz.ydjk.org.cn/gtxrjvoodp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.xziqi.cn/gteopbyqgk.html

[U108] JS：随机整数
来源：http://hz.zhijiandao.cn/gttlpkjwch.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hywenlv.cn/gtzezppfaf.html

[U109] JS：数组分组
来源：http://hz.meibo888.top/gtyzbfhqmc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gthyskrgvn.html

[U110] JS：数组分块
来源：http://hz.guannengcc.top/gtdanvzfeq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jiagoushi.top/gtroimnqhv.html

[U111] JS：对象转 Map
来源：http://hz.yj202588.top/gtgoqlgdph.html

new Map(Object.entries(obj))
来源：http://hz.sysykeji.top/gtypmculko.html

[U112] JS：字符串补位
来源：http://hz.shanyushiyangtech.top/gtgmjpktyl.html

"7".padStart(3, "0")
来源：http://hz.ybcxt.top/gtpzcaidbb.html

[U113] JS：正则替换全部
来源：http://hz.yj202588.top/gtgwsutpzg.html

s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gttosjocwh.html

[U114] JS：JSON 深比较
来源：http://hz.gzhubu.top/gtnswzcwjw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhijiandao.cn/gtwkvvjfej.html

[U115] JS：生成 UUID
来源：http://hz.hnqzz.top/gtcaoywvia.html

crypto.randomUUID()
来源：http://hz.yonumen.top/gtbuwronld.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.hongshengwenyu.top/gtzkytwgmp.html

/** @param {string} name */ function f(name) {}
来源：http://hz.kuanghao11.cn/gtihgjzrkf.html

[U117] JS：单元测试
来源：http://hz.quarkkingdee.top/gtzwkowfox.html

npm i -D vitest;  npx vitest
来源：http://hz.chenlongwang.top/gtuncudkzv.html

[U118] JS：开发服务器
来源：http://hz.yj20258888.top/gtnblgsnyy.html

npm i -D vite;  npx vite
来源：http://hz.tian-w.cn/gtzqilbgnw.html

[U119] JS：生产构建
来源：http://hz.yueranfly.top/gtvngydnyo.html

npx vite build
来源：http://hz.tianlin.xyz/gtcmzpmbaz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.sweek.top/gtlqqfejoa.html

import.meta.env.VITE_API_URL
来源：http://hz.zhengqikj.top/gtuwbmuief.html

================================================================================
来源：http://hz.jqgfzy.top/gtyrkscmjc.html

统计汇总
来源：http://hz.dashuyun.cn/gtotubraxx.html

================================================================================
来源：http://hz.xuanzx.com/gtxpviahto.html

按语言统计（条）：
来源：http://hz.hnqzz.top/gtxrbuloql.html

Python ......... 252
来源：http://hz.quarkkingdee.top/gtuwvpigml.html

PHP ............ 252
来源：http://hz.shzxlz.cn/gtuxjhxhel.html

JavaScript ..... 252
来源：http://hz.gogol.net.cn/gtazzqkxlm.html

TypeScript ..... 212
来源：http://hz.wangdashe.top/gtqvcumudj.html

Java ........... 212
来源：http://hz.aibaodan.cn/gtjcsybycc.html

Go ............. 212
来源：http://hz.guannengcc.top/gtuceybojx.html

Ruby ........... 212
来源：http://hz.jinqigfzy.top/gtakmbtbkd.html

C# ............. 212
来源：http://hz.havefunace.top/gtamqdniji.html

C .............. 30
来源：http://hz.chenjidiqi.icu/gtclthkhua.html

C++ ............ 30
来源：http://hz.ivvv.top/gtrjpptjsy.html

SQL ............ 90
来源：http://hz.guannengcc.top/gtwfnjpuwm.html

Bash ........... 80
来源：http://hz.yj20258.top/gtvguujlkb.html

Kotlin ......... 15
来源：http://hz.tian-w.cn/gtveqklazb.html

Swift .......... 15
来源：http://hz.fengsongda.top/gtwwwsttdb.html

Lua ............ 10
来源：http://hz.xylfe.cn/gtxgtoojfx.html

Perl ........... 10
来源：http://hz.shanyushiyangtech.top/gtrjfovmfu.html

Scala .......... 10
来源：http://hz.jinqigufen.top/gtvufyldlz.html

------------------------------------
来源：http://hz.cqqwz.cn/gtpjvgsxmx.html

合计 ........... 2106 条
来源：http://hz.zhongyouzk.top/gtmoshydjm.html

按章节统计：
来源：http://hz.hongshengwenyu.top/gtyzwidfjf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yvedp.cn/gtdkjhapht.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.jinqigufen.top/gtxcmgsvkk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xuetiantiany.cn/gtpdaqudvd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.hongshengwenyu.top/gtzrjqzgrp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.aizwys.cn/gtgjmlzffj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.xingfuxueyuan.xyz/gtqhbdmmoa.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.nanxuanxn.top/gtccrpbnug.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hysaishi.cn/gtkiktxpjo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jianghu66.top/gtlogbtdjs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtktxggmxe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtxhnylwcg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtnnvjxvmy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtchrslafg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.svipenyu.cn/gtrhihgmuf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shangyingyoupin.top/gtkxsfvkez.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtmnmpusqz.html

Q SQL 专题                              90
来源：http://hz.sysykeji.top/gtemrfbscr.html

R Bash 专题                             80
来源：http://hz.c1oappe.top/gtzjonknbe.html

S C / C++ 专题                          60
来源：http://hz.ehwqpu.com/gtgzinjumb.html

T 其他语言补充                          60
来源：http://hz.cdnleiting.top/gtejbvudzs.html

U 高频实用片段                         120
来源：http://hz.feifeiyinyue.top/gtesvvuavs.html

------------------------------------
来源：http://hz.zhixingplan.top/gtlxavxetr.html

合计                                  2106 条
来源：http://hz.cucudq.cn/gtckbqsqam.html

--------------------------------------------------------------------------------
来源：http://hz.hongshengwenyu.top/gtompztecu.html

使用提醒
来源：http://hz.bjfxy.top/gtocumiiaw.html

--------------------------------------------------------------------------------
来源：http://hz.bjfxy.top/gtzgpqlgqu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.quarkkingdee.top/gtpkzgugoi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.chenjidiqi.icu/gtbzizghat.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hnxiangtu.top/gtutsfahry.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xuetiantiany.cn/gtgybkcuvk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.hnqzz.top/gtvqxmmvpo.html

—— 文件结束 ——
来源：http://hz.iojbl.cn/gtjouxxqdh.html

================================================================================
来源：http://hz.ybcxt.top/gttgrtcbaz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ydjk.org.cn/gtnvdmfwvl.html

Common Programming Examples Cheat Book
来源：http://hz.yuxming.cn/gtfobaoqdf.html

================================================================================
来源：http://hz.sysykeji.top/gtmordlvpx.html

【收录内容】
来源：http://hz.kuanghao11.cn/gtzaydlrbg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.snrcjt.cn/gtgkolfmhi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.iojbl.cn/gtiyyijxsz.html

SQL · Bash · C · C++
来源：http://hz.yonumen.top/gtmkmgntqj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.wangshuangyany.cn/gtiiiajiyq.html

【使用说明】
来源：http://hz.zhaomingkeji.xyz/gthpoumhax.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.guowangkeji.top/gtgddoecdt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.daxiang520.top/gtdkmjocun.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ywan-chungtsiang.top/gtyukhmskw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.kuanghao11.cn/gtfjkgmpry.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ydzc1.top/gtqqqgjhpg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gotoacloud.top/gthjucuuvp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ehwqpu.com/gtllccjxjp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.9152youxi.cn/gtzzrkxjyk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.tanke756.top/gtxwzlitnz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yonumen.top/gtnwqgizio.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.yj20258888.top/gtamkipgad.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ywan-chungtsiang.top/gtbnbjdtms.html

【文件统计】
来源：http://hz.hnqzz.top/gtilbzlfwm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.sxryk.cn/gtqplthqtu.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtyhfqndhp.html

目  录
来源：http://hz.yj20258.top/gtotjauypr.html

--------------------------------------------------------------------------------
来源：http://hz.316326.xyz/gtrjvtdeos.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.cdnleiting.top/gtuizxpuro.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.guowangkeji.top/gtmqrmzyqf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hysaishi.cn/gthmrjlgep.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.cqqwz.cn/gtehbatswd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ywan-chungtsiang.top/gtzjrfpngh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.gzhubu.top/gtxueydxlw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hysaishi.cn/gtdstykbyw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.redwolf501.top/gttrvwrnqf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtqrjrfkis.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shuidangran.top/gtkvyhicfi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.dianchejie.cn/gtjqkvvoyt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtwmkzsvzi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtxjsxshxc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.nwbrower.top/gtfikxdfyr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.0kj1m.cn/gtxgmtphuq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.fengsongda.top/gtvpqevmzl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jianghu66.top/gtffmzpetd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.xylfe.cn/gtmomrnxde.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.nanxuanxn.top/gtxujznwfo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hongshengwenyu.top/gtzeelsxcz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.tianlin.xyz/gtdypxfymn.html

================================================================================
来源：http://hz.ivvv.top/gtydeptdob.html

A. 基础语法与类型
来源：http://hz.nanxuanxn.top/gtgjywzkvp.html

================================================================================
来源：http://hz.iojbl.cn/gtuanlyvbx.html

[A01] Hello World
来源：http://hz.sysykeji.top/gtgspasoqb.html

Py:   print("Hello, World!")
来源：http://hz.shanyushiyangtech.top/gtbgeedmid.html

PHP:  echo "Hello, World!";
来源：http://hz.gogol.net.cn/gtvknfjpml.html

JS:   console.log("Hello, World!");
来源：http://hz.jyoumei.cn/gtclixjfwx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.fzhhl.top/gtjgkogdks.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenjidiqi.icu/gtwzbimuum.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.cucudq.cn/gtxzgiqiha.html

Ruby: puts "Hello, World!"
来源：http://hz.hnqzz.top/gtczsgnhgv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.shanyushiyangtech.top/gttwkjzzaj.html

[A02] 变量声明与赋值
来源：http://hz.nanxinkj.top/gtnbiwnccy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jianghu66.top/gtkotqjydx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yueranfly.top/gtkrefwuuj.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.xuetiantiany.cn/gtwlhkwcxm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.chenjidiqi.icu/gtyltpgxdm.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.9152youxi.cn/gtnqobzdap.html

Go:   name := "Alex"; age := 20
来源：http://hz.yuanzhike.top/gtwoehevvo.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cdnleiting.top/gtegaysjmr.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.52xcode.cn/gthygldxmx.html

[A03] 常量定义
来源：http://hz.shuidangran.top/gtfbexjsdx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.yongpay.top/gtcbiycubb.html

PHP:  const PI = 3.14159;
来源：http://hz.gogol.net.cn/gtmsfsqxcj.html

JS:   const PI = 3.14159;
来源：http://hz.shzxlz.cn/gtjstfreuw.html

TS:   const PI: number = 3.14159;
来源：http://hz.tanke756.top/gtbmqirnfr.html

Java: static final double PI = 3.14159;
来源：http://hz.havefunace.top/gtfrphooai.html

Go:   const PI = 3.14159
来源：http://hz.daxiang520.top/gtiszllabh.html

Ruby: PI = 3.14159
来源：http://hz.zhixingplan.top/gtmzlyfzpn.html

C#:   const double PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gttuyeftcm.html

[A04] 判断变量类型
来源：http://hz.yuxming.cn/gtlnmichwz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.fzhhl.top/gtqxyxhrys.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.xylfe.cn/gtunilzxdf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.chenzaomai.com/gtpcyjobxm.html

TS:   typeof x; x instanceof Date
来源：http://hz.xziqi.cn/gtvidzemam.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xuetiantiany.cn/gtsqubpgvw.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhoulong.xyz/gtqdfaeapi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.tian-w.cn/gtwrssmocf.html

C#:   x.GetType().Name; x is int
来源：http://hz.nwbrower.top/gtqpbvsbfj.html

[A05] 整数除法与取模
来源：http://hz.xuanzx.com/gtwbjijxgb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.hfpthk.cn/gtwczumlqs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.chenzaomai.com/gtlvcltaxa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.guowangkeji.top/gtjsfsnndb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.redwolf501.top/gtiodxsrfd.html

Java: 7 / 2; 7 % 2
来源：http://hz.shanyushiyangkeji.top/gtzpeyeipw.html

Go:   7 / 2; 7 % 2
来源：http://hz.zhengqikj.top/gtvazscvcb.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.hammf.cn/gtghkmqamp.html

C#:   7 / 2; 7 % 2
来源：http://hz.zycfv.cn/gtootozqfn.html

[A06] 字符串转数字
来源：http://hz.ydzc1.top/gtbfeppdzg.html

Py:   int("42"); float("3.14")
来源：http://hz.redwolf501.top/gttaiixwxo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.cashguo.top/gtlqtsxxpc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jiagoushi.top/gtcssaqlle.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.bjfxy.top/gtrddlujfd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.xuetiantiany.cn/gtpbgeojef.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.chenzaomai.com/gtbuplmtun.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.sufxvd.cn/gtnkfdehml.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.ywan-chungtsiang.top/gtzmoexwwp.html

[A07] 数字转字符串
来源：http://hz.fengsongda.top/gtexecrozk.html

Py:   str(42)
来源：http://hz.xinyue.icu/gtricklclt.html

PHP:  (string) 42; strval(42)
来源：http://hz.gaohongyu789.top/gtzgufrrwm.html

JS:   String(42); (42).toString()
来源：http://hz.shanyushiyangkeji.top/gtpntfigqy.html

TS:   String(42)
来源：http://hz.ehwqpu.com/gtqnnawryv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.sysykeji.top/gtrmvwpaea.html

Go:   strconv.Itoa(42)
来源：http://hz.0kj1m.cn/gtiwhxvavy.html

Ruby: 42.to_s
来源：http://hz.aizwys.cn/gtkjvktmcq.html

C#:   42.ToString()
来源：http://hz.zhijiandao.cn/gtgnvzmkiw.html

[A08] 取整与四舍五入
来源：http://hz.vqdsnc.cn/gtrxyeoqws.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.cucudq.cn/gtolrtbgeg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.birdmap.top/gtxpjpcjdv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yj20258888.top/gtylfwiczk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zdqjudy.top/gtfpxrpfak.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.daria6918.cn/gtpsxlakij.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jinghuilouyu.cn/gtobmcgvyu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.hnxiangtu.top/gtxuqhyiza.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.daria6918.cn/gtomntpbuk.html

[A09] 绝对值与最大最小值
来源：http://hz.gogol.net.cn/gtpymenpoq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cheryme.top/gtuwzwafvh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.feifeiyinyue.top/gtadecqxwk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.52xcode.cn/gtelokmpvf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yongpay.top/gtkmxaztoz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.ehwqpu.com/gtcajqxgfa.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zhoulong.xyz/gtfwbyiyxk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.c1oappe.top/gtgzigdmpu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.hfpthk.cn/gtwspokalg.html

[A10] 生成随机数
来源：http://hz.sweek.top/gtsdpfygzi.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zycfv.cn/gtksupzlmv.html

PHP:  random_int(1, 100);
来源：http://hz.redwolf501.top/gtwzqdoass.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.tanke756.top/gtgniqjukt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.iojbl.cn/gtmabjqqoh.html

Java: new Random().nextInt(100) + 1
来源：http://hz.hongshengwenyu.top/gtmtxzonnk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jinqigufen.top/gtubbwjixr.html

Ruby: rand(1..100)
来源：http://hz.dianchejie.cn/gtzuscaijd.html

C#:   new Random().Next(1, 101)
来源：http://hz.daria6918.cn/gtyfdaumkd.html

[A11] 条件表达式（三元）
来源：http://hz.jlsjyb.cn/gtqzyfelxg.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.sufxvd.cn/gtqukhdwmo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.yuxming.cn/gtullddbdd.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.vqdsnc.cn/gtipgrnesx.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.hfpthk.cn/gtlybcpspe.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.jinghuilouyu.cn/gtqnioybjt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.aizwys.cn/gthtllelwb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.aibaodan.cn/gtoobtfkmb.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.jinyuanbaomall.cn/gtkxqzbbqo.html

[A12] 字符串插值 / 格式化
来源：http://hz.wangshuangyany.cn/gtevqpdycj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jinqigfzy.top/gtiuaeidwj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.daxiang520.top/gtkscjcauq.html

JS:   `Hello, ${name}!`
来源：http://hz.aizwys.cn/gthufugekl.html

TS:   `Hello, ${name}!`
来源：http://hz.shanyushiyangtech.top/gttpazoqhc.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zhengqikj.top/gteoxofnis.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.xuetiantiany.cn/gtdnfmzcjr.html

Ruby: "Hello, #{name}!"
来源：http://hz.jqgfzy.top/gthzuzntud.html

C#:   $"Hello, {name}!"
来源：http://hz.zhoulong.xyz/gtujplqbjf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.zhiwuduotai.top/gthaoszjtc.html

Py:   "第一行\n第二行"
来源：http://hz.yangfankeji.com/gtariwpkkj.html

PHP:  "第一行\n第二行"
来源：http://hz.cqqwz.cn/gtpueqwhoy.html

JS:   "第一行\n第二行"
来源：http://hz.sxryk.cn/gtkcttmqrr.html

TS:   "第一行\n第二行"
来源：http://hz.yonumen.top/gteoauqcro.html

Java: "第一行\n第二行"
来源：http://hz.hysaishi.cn/gtnnkrzqky.html

Go:   "第一行\n第二行"
来源：http://hz.fengsongda.top/gtumgmwfpw.html

Ruby: "第一行\n第二行"
来源：http://hz.ydzc1.top/gtgusplyfa.html

C#:   "第一行\n第二行"
来源：http://hz.yangfankeji.com/gtpiemgokk.html

[A14] 注释写法
来源：http://hz.hnxiangtu.top/gtvfjqsvvk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zhengqikj.top/gtgrzfzoep.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.ivvv.top/gtftfjbfoc.html

JS:   // 单行；/* 多行 */
来源：http://hz.jiagoushi.top/gtemrqptdp.html

TS:   // 单行；/* 多行 */
来源：http://hz.hnqzz.top/gtryzutfoi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.sysykeji.top/gtssyculol.html

Go:   // 单行；/* 多行 */
来源：http://hz.jiagoushi.top/gtfhyzjvwf.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jinqigufen.top/gtkffbcdck.html

C#:   // 单行；/* 多行 */
来源：http://hz.shuidangran.top/gtoxhwdrbp.html

[A15] 空值判断与默认值
来源：http://hz.hfpthk.cn/gtrrfyxitw.html

Py:   value = data or "默认值"
来源：http://hz.aibaodan.cn/gtbunwvsaq.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.hywenlv.cn/gtpjxceioo.html

JS:   const value = data ?? "默认值";
来源：http://hz.ydzc1.top/gtimuzwlfu.html

TS:   const value = data ?? "默认值";
来源：http://hz.jinyuanbaomall.cn/gtngfzzase.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.pycfn.com/gtxxbzgwoz.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.sufxvd.cn/gteybpihkl.html

Ruby: value = data || "默认值"
来源：http://hz.birdmap.top/gteimuocrj.html

C#:   var value = data ?? "默认值";
来源：http://hz.haohaochexian.top/gtrbllbldw.html

[A16] 真假值判断规则
来源：http://hz.ydzc1.top/gtqfbckoqx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.shangyingyoupin.top/gtkavpxudt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.meibo888.top/gtevaomtzc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.zycfv.cn/gtidbqoklu.html

TS:   if (!x) {}
来源：http://hz.pengpengdd.cyou/gtmbaoqlwt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.gzhubu.top/gtnfpuqwlg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.zhixingplan.top/gtzjradtmf.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.ppjwa.cn/gtrlooovrr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.vqdsnc.cn/gtxvvxqqky.html

[A17] 位运算
来源：http://hz.zhiwuduotai.top/gtbjqbgcpp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhiwuduotai.top/gthajpxbpm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yj20258.top/gteznkluly.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydzc1.top/gthqhhyrgr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.zhoulong.xyz/gtaayaijym.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hongshengwenyu.top/gtiouamjqj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.guowangkeji.top/gtwtqtnkkz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.snrcjt.cn/gtxrtfoagr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cheryme.top/gtptoatmoy.html

[A18] 字符与 ASCII 码互转
来源：http://hz.cheryme.top/gtfsbjxbot.html

Py:   ord("A"); chr(65)
来源：http://hz.svipenyu.cn/gtdrhzghha.html

PHP:  ord("A"); chr(65)
来源：http://hz.ehwqpu.com/gtjlecdwjg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.9152youxi.cn/gtnansljve.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.dianchejie.cn/gtumhyiojw.html

Java: (int) 'A'; (char) 65
来源：http://hz.tianlin.xyz/gtdrkjckca.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.nanxuanxn.top/gtweawktwi.html

Ruby: "A".ord; 65.chr
来源：http://hz.mhx1999.top/gtwyolndmw.html


<!-- 参考信息 -->