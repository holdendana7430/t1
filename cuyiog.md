代发 wailian999

[U101] JS：classList 操作
来源：http://hz.andypj.xyz/gtmouyaksx.html

el.classList.toggle("active")
来源：http://hz.sweek.top/gtcavdvphf.html

[U102] JS：本地存储
来源：http://hz.bjfxy.top/gtlhykxgjp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.tanke756.top/gtplndkzda.html

[U103] JS：定时器
来源：http://hz.0kj1m.cn/gtcgekiklc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.gaohongyu789.top/gtcahigtew.html

[U104] JS：防抖
来源：http://hz.jqgufenzy.top/gtkxrisgsf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtdtlltfsr.html

[U105] JS：节流
来源：http://hz.iojbl.cn/gtbwacjemi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shzxlz.cn/gtkxolcluf.html

[U106] JS：日期格式化
来源：http://hz.gogol.net.cn/gtalleobae.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yj20258888.top/gtjkglheld.html

[U107] JS：数字千分位
来源：http://hz.jinyuanbaomall.cn/gtabgpssyx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.gotoacloud.top/gtncggmitu.html

[U108] JS：随机整数
来源：http://hz.hammf.cn/gtjpdkiawr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.tian-w.cn/gtcvrpvttd.html

[U109] JS：数组分组
来源：http://hz.zhoulong.xyz/gtjmtfuonc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.pengpengdd.cyou/gtkblsixqf.html

[U110] JS：数组分块
来源：http://hz.cashguo.top/gttvfhedgj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yuanzhike.top/gtlutcdwpa.html

[U111] JS：对象转 Map
来源：http://hz.hfpthk.cn/gttnvjhlxh.html

new Map(Object.entries(obj))
来源：http://hz.zhijiandao.cn/gtklwbbluv.html

[U112] JS：字符串补位
来源：http://hz.cqqwz.cn/gtgozcqtqi.html

"7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtaskppeee.html

[U113] JS：正则替换全部
来源：http://hz.52xcode.cn/gtlemgccvr.html

s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtybkyntjb.html

[U114] JS：JSON 深比较
来源：http://hz.havefunace.top/gtgbodpill.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.cucudq.cn/gtyhajsklw.html

[U115] JS：生成 UUID
来源：http://hz.aibaodan.cn/gtytrfnmlm.html

crypto.randomUUID()
来源：http://hz.jiagoushi.top/gtbqltxtpa.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.pycfn.com/gtvijgcvfh.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xingfuxueyuan.xyz/gtgnkyulyb.html

[U117] JS：单元测试
来源：http://hz.gzhubu.top/gtqpwcqfiz.html

npm i -D vitest;  npx vitest
来源：http://hz.52xcode.cn/gtukumzzhc.html

[U118] JS：开发服务器
来源：http://hz.jinghuilouyu.cn/gtozvenloq.html

npm i -D vite;  npx vite
来源：http://hz.yuxming.cn/gtowuoiiqb.html

[U119] JS：生产构建
来源：http://hz.chenzaomai.com/gtkjkjrjfw.html

npx vite build
来源：http://hz.shanyushiyangkeji.top/gttubsocyz.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.52xcode.cn/gtpkqzndhs.html

import.meta.env.VITE_API_URL
来源：http://hz.yj20258.top/gtayepegwt.html

================================================================================
来源：http://hz.pycfn.com/gtwzrqwyej.html

统计汇总
来源：http://hz.shanyushiyangtech.top/gthbzkyklp.html

================================================================================
来源：http://hz.sxryk.cn/gtougciyjm.html

按语言统计（条）：
来源：http://hz.hysaishi.cn/gtcbgpuvez.html

Python ......... 252
来源：http://hz.hysaishi.cn/gtvkegdeqr.html

PHP ............ 252
来源：http://hz.gogol.net.cn/gtczncvujt.html

JavaScript ..... 252
来源：http://hz.zhongyouzk.top/gthocnwkws.html

TypeScript ..... 212
来源：http://hz.jinqigufen.top/gtejzupfom.html

Java ........... 212
来源：http://hz.jqgufenzy.top/gthkkdragp.html

Go ............. 212
来源：http://hz.yj20258888.top/gtdaogiaep.html

Ruby ........... 212
来源：http://hz.xinyue.icu/gtvkcljbqj.html

C# ............. 212
来源：http://hz.fzhhl.top/gtgyljdslt.html

C .............. 30
来源：http://hz.zhijiandao.cn/gtamuuuqso.html

C++ ............ 30
来源：http://hz.nanxuanxn.top/gtdcvnimra.html

SQL ............ 90
来源：http://hz.jinghuilouyu.cn/gtjdfmyzlf.html

Bash ........... 80
来源：http://hz.cashguo.top/gtlmhxevwj.html

Kotlin ......... 15
来源：http://hz.chenjidiqi.icu/gtufazkaai.html

Swift .......... 15
来源：http://hz.jqgfzy.top/gtfavbnzmb.html

Lua ............ 10
来源：http://hz.yueranfly.top/gtlkltsakh.html

Perl ........... 10
来源：http://hz.daxiang520.top/gtklnonpun.html

Scala .......... 10
来源：http://hz.c1oappe.top/gtmerypdov.html

------------------------------------
来源：http://hz.nanxinkj.top/gtzrxwrbcq.html

合计 ........... 2106 条
来源：http://hz.shangyingyoupin.top/gtdsykdfkn.html

按章节统计：
来源：http://hz.tian-w.cn/gtxpcwvdki.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.jinqigfzy.top/gtadjhxoin.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.sysykeji.top/gthhpfscep.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hysaishi.cn/gtqzcehxsc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.aizwys.cn/gtuqwiznqg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.nwbrower.top/gtdxfxjmdb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.chenzaomai.com/gtbwkpurqe.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jianghu66.top/gtpgsxmsvi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj20258888.top/gtkdmbgotv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtmcywejnv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shanyushiyangkeji.top/gtbzazcfyx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.cqqwz.cn/gtzidmedua.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtgnxxqwga.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hfpthk.cn/gthprzgrlm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.dashuyun.cn/gtoavirozi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jinqigfzy.top/gtsfmqklxl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.chenjidiqi.icu/gtolmohcqt.html

Q SQL 专题                              90
来源：http://hz.nanxuanxn.top/gtcsnbljqq.html

R Bash 专题                             80
来源：http://hz.daxiang520.top/gtgpkasalb.html

S C / C++ 专题                          60
来源：http://hz.sysykeji.top/gtcykgiiqw.html

T 其他语言补充                          60
来源：http://hz.wangshuangyany.cn/gtzzqkbhmb.html

U 高频实用片段                         120
来源：http://hz.jinyuanbaomall.cn/gtqsiqvlho.html

------------------------------------
来源：http://hz.hnxiangtu.top/gtscqvwueq.html

合计                                  2106 条
来源：http://hz.zhixingplan.top/gtmonmghxx.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtcowpsvoe.html

使用提醒
来源：http://hz.xinyue.icu/gtoxwssqnd.html

--------------------------------------------------------------------------------
来源：http://hz.jqgfzy.top/gtwlbiecgz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.aizwys.cn/gtqtrrcvyf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.yuxming.cn/gtddzyfslq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.ywan-chungtsiang.top/gteushapgl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hysaishi.cn/gterfqvnrc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shuidangran.top/gtqraqhcoe.html

—— 文件结束 ——
来源：http://hz.ydzc1.top/gtaniucvxz.html

================================================================================
来源：http://hz.sysykeji.top/gtfpzglewd.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.0kj1m.cn/gtqnvurwox.html

Common Programming Examples Cheat Book
来源：http://hz.hysaishi.cn/gtaojsgwdg.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtpwgtslnb.html

【收录内容】
来源：http://hz.ydzc1.top/gtcapidmqr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.0kj1m.cn/gtqealqbak.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shanyushiyangtech.top/gtzehxeokb.html

SQL · Bash · C · C++
来源：http://hz.c1oappe.top/gtfzqxeves.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.daxiang520.top/gthcdvnpdk.html

【使用说明】
来源：http://hz.yanxiufei.cn/gtemykwzjq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.ydzc1.top/gtmcdukaes.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.snrcjt.cn/gtxxamdajd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258888.top/gtgijrvqtn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.havefunace.top/gtujyoyffl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jlsjyb.cn/gtkrpbkszz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.kuanghao11.cn/gtcqjtggay.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.chenlongwang.top/gtsiwbjzyl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.aizwys.cn/gtlzsmcguv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jiagoushi.top/gtiyntcvvp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.cqqwz.cn/gtuunchdnt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.hongshengwenyu.top/gtlnkphbfb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zdqjudy.top/gtpudeeudy.html

【文件统计】
来源：http://hz.nanxuanxn.top/gtbjhethqb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.fengsongda.top/gtfsgqbqnv.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtvvjvlcgv.html

目  录
来源：http://hz.zhiwuduotai.top/gtwntrkcgf.html

--------------------------------------------------------------------------------
来源：http://hz.daria6918.cn/gtpndrakuu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jiagoushi.top/gtjruedhsa.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yj202588.top/gtpvfjvojn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtnehumklq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.vqdsnc.cn/gtciisbzmv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shuidangran.top/gtzctgnjpz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.fengsongda.top/gtfhgdnaay.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.gotoacloud.top/gtuxwheypb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.guannengcc.top/gtbqauooap.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtpjowietf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.pengpengdd.cyou/gtxupqkhem.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.wangdashe.top/gtnuzjffta.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gtwwbpkdau.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.sysykeji.top/gtjsrjjxbt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.havefunace.top/gtjxoywkfl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hnxiangtu.top/gtdnaeijcf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yueranfly.top/gtxndoubju.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.kuanghao11.cn/gtghirqwfu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.9152youxi.cn/gtqbevolbs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.sysykeji.top/gtkzrdsrot.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.kuanghao11.cn/gtwfyywfjt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhiwuduotai.top/gtjcewpaos.html

================================================================================
来源：http://hz.birdmap.top/gttbjulprm.html

A. 基础语法与类型
来源：http://hz.yangfankeji.com/gtexezzbdf.html

================================================================================
来源：http://hz.iojbl.cn/gtztlnfbhw.html

[A01] Hello World
来源：http://hz.xuanzx.com/gtdykwvtsg.html

Py:   print("Hello, World!")
来源：http://hz.bjfxy.top/gtorfvpuaa.html

PHP:  echo "Hello, World!";
来源：http://hz.xuanzx.com/gtzsbgjhst.html

JS:   console.log("Hello, World!");
来源：http://hz.fengsongda.top/gtcqwcztqy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhoulong.xyz/gtlevlivgj.html

Java: System.out.println("Hello, World!");
来源：http://hz.yuanzhike.top/gtqazgpdsx.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.quarkkingdee.top/gtobstcnbs.html

Ruby: puts "Hello, World!"
来源：http://hz.yongpay.top/gtafbpyqek.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ydjk.org.cn/gtzkmjnjbc.html

[A02] 变量声明与赋值
来源：http://hz.c1oappe.top/gttlqzhpio.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhixingplan.top/gtlabbxcgd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hnqzz.top/gtfamulyvf.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ppjwa.cn/gtxsogadfk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.aibaodan.cn/gtkyyxbcwk.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.havefunace.top/gttkydtxea.html

Go:   name := "Alex"; age := 20
来源：http://hz.wangshuangyany.cn/gtxikdlqcb.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zdqjudy.top/gtqisxfzlj.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.316326.xyz/gtipxnfwwl.html

[A03] 常量定义
来源：http://hz.yuanzhike.top/gtcvmqjgsd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.kuanghao11.cn/gtosqowwyq.html

PHP:  const PI = 3.14159;
来源：http://hz.zhengqikj.top/gtuotagtwi.html

JS:   const PI = 3.14159;
来源：http://hz.yonumen.top/gtxotpapaq.html

TS:   const PI: number = 3.14159;
来源：http://hz.hnqzz.top/gtyvkqbgyx.html

Java: static final double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtdssbvlwd.html

Go:   const PI = 3.14159
来源：http://hz.xuetiantiany.cn/gteoctsmap.html

Ruby: PI = 3.14159
来源：http://hz.fzhhl.top/gtvyarcxyr.html

C#:   const double PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtcxtxmzcb.html

[A04] 判断变量类型
来源：http://hz.havefunace.top/gtyytqmbop.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.iojbl.cn/gtglpvbkwe.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.52xcode.cn/gtcbrvzmlp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.redwolf501.top/gtblymogfl.html

TS:   typeof x; x instanceof Date
来源：http://hz.jiagoushi.top/gtarogrnjn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.sufxvd.cn/gtaelerelb.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yonumen.top/gtcbeuaxwj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yj20258888.top/gtkuptqkxk.html

C#:   x.GetType().Name; x is int
来源：http://hz.gzhubu.top/gtsumdbouk.html

[A05] 整数除法与取模
来源：http://hz.chenjidiqi.icu/gtpgzmzhvl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.cheryme.top/gtbtvkjukx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.wangdashe.top/gtnfxxfmhy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xylfe.cn/gtmqzqxcll.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.9152youxi.cn/gtrlmdhpud.html

Java: 7 / 2; 7 % 2
来源：http://hz.jinghuilouyu.cn/gtjcxbgsse.html

Go:   7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtyovhaykp.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.birdmap.top/gtiosbwizb.html

C#:   7 / 2; 7 % 2
来源：http://hz.52xcode.cn/gtycstacou.html

[A06] 字符串转数字
来源：http://hz.jqgufenzy.top/gtgxokzguh.html

Py:   int("42"); float("3.14")
来源：http://hz.c1oappe.top/gtcogbajiw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jinqigufen.top/gtrkylrmwt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.cheryme.top/gtdevzkoou.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.nanxinkj.top/gtujmoxjyf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zdqjudy.top/gtlilrkmxw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.nanxinkj.top/gtiixrfair.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jianghu66.top/gtcmfjbdgl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xuanzx.com/gtajwewsbq.html

[A07] 数字转字符串
来源：http://hz.tanke756.top/gtrzjlindy.html

Py:   str(42)
来源：http://hz.snrcjt.cn/gthqwshpov.html

PHP:  (string) 42; strval(42)
来源：http://hz.mhx1999.top/gtltbxlrmo.html

JS:   String(42); (42).toString()
来源：http://hz.nanxuanxn.top/gtursaqqqw.html

TS:   String(42)
来源：http://hz.wangshuangyany.cn/gtdhyuurun.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.feifeiyinyue.top/gthsqithdq.html

Go:   strconv.Itoa(42)
来源：http://hz.dianchejie.cn/gthauhnhet.html

Ruby: 42.to_s
来源：http://hz.xingfuxueyuan.xyz/gtkjcqrruu.html

C#:   42.ToString()
来源：http://hz.shanyushiyangtech.top/gttgjgjpza.html

[A08] 取整与四舍五入
来源：http://hz.chenzaomai.com/gtgfglqqyd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.kuanghao11.cn/gtvrdwawyw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.shanyushiyangkeji.top/gtdtjulpqm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yueranfly.top/gtvnxietcu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.shanyushiyangkeji.top/gtbjzsbxmq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.c1oappe.top/gtwwuuzzfy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yuanzhike.top/gthyxhprig.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.snrcjt.cn/gtjsaxctty.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.fengsongda.top/gtgqwoyjsw.html

[A09] 绝对值与最大最小值
来源：http://hz.feifeiyinyue.top/gtrcrylfke.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.nanxuanxn.top/gtwlmptrfl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.bjfxy.top/gtytkoxebw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.sxryk.cn/gtxerigyaf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.xuanzx.com/gtuokmjeoi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.meibo888.top/gteoswuqne.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.52xcode.cn/gtmqwqtdfl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.cashguo.top/gthiandqkl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yuxming.cn/gtkgadcorv.html

[A10] 生成随机数
来源：http://hz.snrcjt.cn/gtkwpjimjl.html

Py:   import random; random.randint(1, 100)
来源：http://hz.xingfuxueyuan.xyz/gthmneytbo.html

PHP:  random_int(1, 100);
来源：http://hz.xuetiantiany.cn/gtvtarvgjv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.nanxinkj.top/gtfcqddtyc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.redwolf501.top/gtddywpxkn.html

Java: new Random().nextInt(100) + 1
来源：http://hz.chenjidiqi.icu/gttsinqgkh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.sysykeji.top/gtgbatfjsx.html

Ruby: rand(1..100)
来源：http://hz.yvedp.cn/gtfczidtig.html

C#:   new Random().Next(1, 101)
来源：http://hz.yuxming.cn/gtazsgivbk.html

[A11] 条件表达式（三元）
来源：http://hz.9152youxi.cn/gtlrvxqxzn.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jinyuanbaomall.cn/gtqjsxyron.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.iojbl.cn/gtzkjuklsg.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.ivvv.top/gtytbjnovk.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jiagoushi.top/gtbwzfykdv.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gtqcjqqyju.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.yangfankeji.com/gtmxbenxae.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.zhiwuduotai.top/gtuybblxrl.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.gaohongyu789.top/gtgpbqzmtn.html

[A12] 字符串插值 / 格式化
来源：http://hz.cqqwz.cn/gtkdkwgqms.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.xziqi.cn/gtoolgdztb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.chenzaomai.com/gteiampuyl.html

JS:   `Hello, ${name}!`
来源：http://hz.ybcxt.top/gtmiobinka.html

TS:   `Hello, ${name}!`
来源：http://hz.dashuyun.cn/gtbomfjemk.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.nanxinkj.top/gtsnempkzt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.xuetiantiany.cn/gtezetknzx.html

Ruby: "Hello, #{name}!"
来源：http://hz.daria6918.cn/gtzuxbvhgb.html

C#:   $"Hello, {name}!"
来源：http://hz.gogol.net.cn/gtsafnlpgq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yongpay.top/gtvfwbwyhw.html

Py:   "第一行\n第二行"
来源：http://hz.ydjk.org.cn/gtowsazzcz.html

PHP:  "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtcuuguhif.html

JS:   "第一行\n第二行"
来源：http://hz.jqgufenzy.top/gtyvxqjjhc.html

TS:   "第一行\n第二行"
来源：http://hz.yj20258.top/gtolejqbde.html

Java: "第一行\n第二行"
来源：http://hz.jianghu66.top/gtufizxptx.html

Go:   "第一行\n第二行"
来源：http://hz.smart0.xyz/gtinpppxoz.html

Ruby: "第一行\n第二行"
来源：http://hz.fengsongda.top/gtljinvtwp.html

C#:   "第一行\n第二行"
来源：http://hz.quarkkingdee.top/gtkzfjohrc.html

[A14] 注释写法
来源：http://hz.cqqwz.cn/gtugmdmqrk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.aibaodan.cn/gtauntxfeg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.havefunace.top/gtweflwqni.html

JS:   // 单行；/* 多行 */
来源：http://hz.xuetiantiany.cn/gtqtajihhz.html

TS:   // 单行；/* 多行 */
来源：http://hz.tianlin.xyz/gticdkpbtc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.vqdsnc.cn/gtjtzghsxo.html

Go:   // 单行；/* 多行 */
来源：http://hz.316326.xyz/gtfoxcpeol.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.sweek.top/gtyjyssrlg.html

C#:   // 单行；/* 多行 */
来源：http://hz.tianlin.xyz/gtrmcyencn.html

[A15] 空值判断与默认值
来源：http://hz.pengpengdd.cyou/gthebckiqu.html

Py:   value = data or "默认值"
来源：http://hz.jinyuanbaomall.cn/gtxuadmpnc.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.shanyushiyangkeji.top/gtnqfuafsk.html

JS:   const value = data ?? "默认值";
来源：http://hz.daxiang520.top/gtghxqencl.html

TS:   const value = data ?? "默认值";
来源：http://hz.aibaodan.cn/gttmwlousa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.yuxming.cn/gttemynetu.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.gotoacloud.top/gtitxenxio.html

Ruby: value = data || "默认值"
来源：http://hz.xylfe.cn/gtcdrkqtvt.html

C#:   var value = data ?? "默认值";
来源：http://hz.hammf.cn/gtuznzwpim.html

[A16] 真假值判断规则
来源：http://hz.chenlongwang.top/gtkhyinfmj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.xuanzx.com/gtsrcneveq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.yj202588.top/gtopqwikdn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.shuidangran.top/gtekeduagq.html

TS:   if (!x) {}
来源：http://hz.meibo888.top/gtqtbxgcim.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.ppjwa.cn/gtiznrdcpw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.quarkkingdee.top/gtedtskati.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.guowangkeji.top/gtmxkaians.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.guannengcc.top/gtjahyaozv.html

[A17] 位运算
来源：http://hz.fzhhl.top/gtulokbpws.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.316326.xyz/gtqjfseidv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.aibaodan.cn/gtdvigdrcd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hywenlv.cn/gtpnpdybma.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.bjfxy.top/gtrvmgbsmq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gtheejlqwm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.fzhhl.top/gtpbercqfs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangshuangyany.cn/gtxguiswvj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cucudq.cn/gtorfnxljd.html


<!-- 参考信息 -->