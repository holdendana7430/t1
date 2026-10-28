代发 wailian999

[U93] JS：模板字符串
来源：http://hz.shanyushiyangkeji.top/gtseksdbga.html

`共 ${n} 条`
来源：http://hz.yj20258888.top/gtvyxtgnqg.html

[U94] JS：箭头函数
来源：http://hz.52xcode.cn/gtssmrfasr.html

const double = x => x * 2;
来源：http://hz.shzxlz.cn/gtrowtqsio.html

[U95] JS：Promise 包装
来源：http://hz.ivvv.top/gtsmxxeaez.html

new Promise((resolve, reject) => {})
来源：http://hz.yuxming.cn/gtcygdbbac.html

[U96] JS：async/await 与异常
来源：http://hz.cqqwz.cn/gtwcrwjxsu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shzxlz.cn/gtcycodpkq.html

[U97] JS：并发请求
来源：http://hz.zycfv.cn/gtzpezwsyz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gthntyqqlu.html

[U98] JS：fetch 带 JSON
来源：http://hz.jinyuanbaomall.cn/gtwcbxdpvy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.guannengcc.top/gtvgytupop.html

[U99] JS：事件监听
来源：http://hz.xuanzx.com/gtwgmncpse.html

el.addEventListener("click", e => {})
来源：http://hz.haohaochexian.top/gtubdhnfgb.html

[U100] JS：DOM 查询
来源：http://hz.yangfankeji.com/gtlusaiawq.html

document.querySelector(".item")
来源：http://hz.feifeiyinyue.top/gtwivkazok.html

[U101] JS：classList 操作
来源：http://hz.yongpay.top/gtpxkrlizs.html

el.classList.toggle("active")
来源：http://hz.shanyushiyangkeji.top/gtjxwuloqx.html

[U102] JS：本地存储
来源：http://hz.tanke756.top/gtjwmosqcs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhixingplan.top/gtnmghmhup.html

[U103] JS：定时器
来源：http://hz.c1oappe.top/gtxajgkkei.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.havefunace.top/gtvnwdwtjh.html

[U104] JS：防抖
来源：http://hz.jinyuanbaomall.cn/gtuqrmhbxa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xuetiantiany.cn/gtwyfgiuqr.html

[U105] JS：节流
来源：http://hz.chenzaomai.com/gtrjisnhbj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenjidiqi.icu/gtwydprsuq.html

[U106] JS：日期格式化
来源：http://hz.zhongyouzk.top/gtvqpxqlsj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.zhixingplan.top/gtrkhpmyby.html

[U107] JS：数字千分位
来源：http://hz.ivvv.top/gtorztjzao.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yangfankeji.com/gtmsuoismz.html

[U108] JS：随机整数
来源：http://hz.xuanzx.com/gtmdxixgau.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.aibaodan.cn/gtooactwxl.html

[U109] JS：数组分组
来源：http://hz.cqqwz.cn/gtusezecoo.html

Object.groupBy(arr, x => x.type)
来源：http://hz.tian-w.cn/gtucsgujzu.html

[U110] JS：数组分块
来源：http://hz.ppjwa.cn/gtybztuzhl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hysaishi.cn/gthjgayxye.html

[U111] JS：对象转 Map
来源：http://hz.cdnleiting.top/gtubbmxsvl.html

new Map(Object.entries(obj))
来源：http://hz.ydjk.org.cn/gtdsqqjjcw.html

[U112] JS：字符串补位
来源：http://hz.aizwys.cn/gtctxgpbxk.html

"7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtzqfmbuqo.html

[U113] JS：正则替换全部
来源：http://hz.jqgfzy.top/gtnzrmcoek.html

s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtfaydwubo.html

[U114] JS：JSON 深比较
来源：http://hz.jianghu66.top/gtjrutczlv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.mhx1999.top/gtuoflvofm.html

[U115] JS：生成 UUID
来源：http://hz.jqgufenzy.top/gtrnafcqhf.html

crypto.randomUUID()
来源：http://hz.ybcxt.top/gtqynrbsey.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinqigufen.top/gtmcrzdeai.html

/** @param {string} name */ function f(name) {}
来源：http://hz.pengpengdd.cyou/gtddmwianp.html

[U117] JS：单元测试
来源：http://hz.9152youxi.cn/gtuumqaavl.html

npm i -D vitest;  npx vitest
来源：http://hz.xylfe.cn/gtbzswollu.html

[U118] JS：开发服务器
来源：http://hz.jianghu66.top/gtlgvnoihr.html

npm i -D vite;  npx vite
来源：http://hz.ehwqpu.com/gtioyfkffs.html

[U119] JS：生产构建
来源：http://hz.daria6918.cn/gtmyasqwcp.html

npx vite build
来源：http://hz.guannengcc.top/gtsjszeczs.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ywan-chungtsiang.top/gtpjesvhcz.html

import.meta.env.VITE_API_URL
来源：http://hz.0kj1m.cn/gtmxwqtisj.html

================================================================================
来源：http://hz.meibo888.top/gtiviinjpl.html

统计汇总
来源：http://hz.cashguo.top/gtmjzqspuu.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtjiistjew.html

按语言统计（条）：
来源：http://hz.jiagoushi.top/gtajmmmxcw.html

Python ......... 252
来源：http://hz.yj20258.top/gtmeepyyyy.html

PHP ............ 252
来源：http://hz.mhx1999.top/gtwupavmxm.html

JavaScript ..... 252
来源：http://hz.tanke756.top/gtucvbausc.html

TypeScript ..... 212
来源：http://hz.pengpengdd.cyou/gtgjzenljo.html

Java ........... 212
来源：http://hz.snrcjt.cn/gtlrsvssaz.html

Go ............. 212
来源：http://hz.cqqwz.cn/gtxznziemf.html

Ruby ........... 212
来源：http://hz.gaohongyu789.top/gtqziztikm.html

C# ............. 212
来源：http://hz.hfpthk.cn/gtggsiucpj.html

C .............. 30
来源：http://hz.gzhubu.top/gtndlsrkym.html

C++ ............ 30
来源：http://hz.chenlongwang.top/gtlbqekqlg.html

SQL ............ 90
来源：http://hz.shangyingyoupin.top/gtydvbcroc.html

Bash ........... 80
来源：http://hz.smart0.xyz/gtrgdaijey.html

Kotlin ......... 15
来源：http://hz.52xcode.cn/gtemuaxhvm.html

Swift .......... 15
来源：http://hz.gaohongyu789.top/gttehrrrpi.html

Lua ............ 10
来源：http://hz.tianlin.xyz/gtzugpaktp.html

Perl ........... 10
来源：http://hz.jinqigfzy.top/gtrmupdjmu.html

Scala .......... 10
来源：http://hz.ppjwa.cn/gtdxnnykhw.html

------------------------------------
来源：http://hz.dianchejie.cn/gtefyxypjx.html

合计 ........... 2106 条
来源：http://hz.yanxiufei.cn/gtsvgasutv.html

按章节统计：
来源：http://hz.yuxming.cn/gtvihakhrz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xinyue.icu/gtfzohwqwx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gthiqfhjob.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.nanxuanxn.top/gtfndqoiun.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jqgfzy.top/gtikdxazgo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hongshengwenyu.top/gtoqwaqbah.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.aizwys.cn/gtudiebojk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sysykeji.top/gthbtzcobi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nanxuanxn.top/gtxxhztaxx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtwpcwufgi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.ybcxt.top/gtsfnkgymh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.fengsongda.top/gtnwsxpgkr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtedqtwzta.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shanyushiyangtech.top/gtjskzzzdx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hongshengwenyu.top/gtjwkirrvz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.quarkkingdee.top/gtdwuynbvo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gttoegslrm.html

Q SQL 专题                              90
来源：http://hz.jinyuanbaomall.cn/gtwbyvpbvl.html

R Bash 专题                             80
来源：http://hz.cqqwz.cn/gtuvvnlgce.html

S C / C++ 专题                          60
来源：http://hz.shanyushiyangtech.top/gtxdkyqqdh.html

T 其他语言补充                          60
来源：http://hz.tian-w.cn/gtnwdpitqf.html

U 高频实用片段                         120
来源：http://hz.shangyingyoupin.top/gtoasfopie.html

------------------------------------
来源：http://hz.yangfankeji.com/gtoodmemvy.html

合计                                  2106 条
来源：http://hz.shanyushiyangkeji.top/gtfujofvwx.html

--------------------------------------------------------------------------------
来源：http://hz.ydjk.org.cn/gtlafkdnol.html

使用提醒
来源：http://hz.bjfxy.top/gtlbgeogmk.html

--------------------------------------------------------------------------------
来源：http://hz.jyoumei.cn/gtvyflaouq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.chenlongwang.top/gtcvwvxmmg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.vqdsnc.cn/gtvgtcofna.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yongpay.top/gtllajsbqv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.shzxlz.cn/gtkbrmbgtx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.shangyingyoupin.top/gtwutvqufy.html

—— 文件结束 ——
来源：http://hz.cheryme.top/gtflgdlrje.html

================================================================================
来源：http://hz.zhoulong.xyz/gtevkpxjlx.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zhijiandao.cn/gtsaatkbpm.html

Common Programming Examples Cheat Book
来源：http://hz.ydjk.org.cn/gtarafeuoe.html

================================================================================
来源：http://hz.snrcjt.cn/gtkjhqdykh.html

【收录内容】
来源：http://hz.shanyushiyangtech.top/gtitjhqlaf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.c1oappe.top/gtnbrtxbwq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.tian-w.cn/gtcqtqcocb.html

SQL · Bash · C · C++
来源：http://hz.yj20258888.top/gtzvzdbmnk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.vqdsnc.cn/gtawskkrfk.html

【使用说明】
来源：http://hz.zhongyouzk.top/gtxwerfgst.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.nwbrower.top/gtjdwtgnpv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.svipenyu.cn/gtbznrnohr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.svipenyu.cn/gtbtxdgute.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xziqi.cn/gtcpaeeybw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ivvv.top/gtonltqczj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.wangshuangyany.cn/gtyfjblyvn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jqgfzy.top/gtigsqvrpc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hywenlv.cn/gtvvcrknxp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xylfe.cn/gtktvviins.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.wangshuangyany.cn/gtlirbkfhw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.pengpengdd.cyou/gtxeltxbbw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.jqgfzy.top/gtmmswvcql.html

【文件统计】
来源：http://hz.sysykeji.top/gtinacjcnt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jqgufenzy.top/gtjbtsdjyr.html

--------------------------------------------------------------------------------
来源：http://hz.wangdashe.top/gttjfueden.html

目  录
来源：http://hz.ybcxt.top/gtwabdojoh.html

--------------------------------------------------------------------------------
来源：http://hz.zhongyouzk.top/gtfbnvivnj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.c1oappe.top/gtaihwekal.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.bjfxy.top/gtieciyubj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zhongyouzk.top/gtffryvaqy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ydzc1.top/gttbgqnqog.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.jqgfzy.top/gtmzbopcgj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xylfe.cn/gtlgakltmu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.nanxinkj.top/gtgfwvugsi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hywenlv.cn/gtwqcqkxnt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtyistllon.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.52xcode.cn/gtqxduwffc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtjeirjeem.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.wangdashe.top/gtykrfemfc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtikjavyub.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.ydzc1.top/gttpbjasvy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shzxlz.cn/gtgwfntpmk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.cqqwz.cn/gtxerkohvm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xylfe.cn/gtrejgvsle.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.andypj.xyz/gtdiqabrkb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yj202588.top/gtwsoqsawc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhongyouzk.top/gtjwjzdorc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.gaohongyu789.top/gtcdkvyswx.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtootlzwva.html

A. 基础语法与类型
来源：http://hz.jinghuilouyu.cn/gtnhliufeh.html

================================================================================
来源：http://hz.wangdashe.top/gthtdmmgvg.html

[A01] Hello World
来源：http://hz.iojbl.cn/gtwjkswggk.html

Py:   print("Hello, World!")
来源：http://hz.mhx1999.top/gtewpkohpo.html

PHP:  echo "Hello, World!";
来源：http://hz.smart0.xyz/gtyaxfqfrw.html

JS:   console.log("Hello, World!");
来源：http://hz.wangshuangyany.cn/gtvnypfjet.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cheryme.top/gtvjrrshse.html

Java: System.out.println("Hello, World!");
来源：http://hz.cheryme.top/gtwtimimyc.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.cashguo.top/gtxlllghpv.html

Ruby: puts "Hello, World!"
来源：http://hz.c1oappe.top/gtjlczqndb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhengqikj.top/gtnixnrxhw.html

[A02] 变量声明与赋值
来源：http://hz.mhx1999.top/gtljyqnzfl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.jyoumei.cn/gtdgvgtguh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ppjwa.cn/gticnfmrzc.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jqgfzy.top/gthqwhxunn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ydjk.org.cn/gttzdupclr.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yvedp.cn/gtgjqerujt.html

Go:   name := "Alex"; age := 20
来源：http://hz.chenzaomai.com/gtnmacpiys.html

Ruby: name = "Alex"; age = 20
来源：http://hz.nanxuanxn.top/gteyaxuohc.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.cashguo.top/gtjpexptfk.html

[A03] 常量定义
来源：http://hz.feifeiyinyue.top/gtrsgiwvcg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.fzhhl.top/gthlsmwtam.html

PHP:  const PI = 3.14159;
来源：http://hz.yangfankeji.com/gtzmijqtfm.html

JS:   const PI = 3.14159;
来源：http://hz.vqdsnc.cn/gtybgcvdlb.html

TS:   const PI: number = 3.14159;
来源：http://hz.yj202588.top/gtspgdfnay.html

Java: static final double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtmbxjubma.html

Go:   const PI = 3.14159
来源：http://hz.dashuyun.cn/gtruvemaju.html

Ruby: PI = 3.14159
来源：http://hz.ivvv.top/gtgrgawcim.html

C#:   const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtfafqptvh.html

[A04] 判断变量类型
来源：http://hz.smart0.xyz/gtwfpzgprf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.aizwys.cn/gtdyevjcyp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jqgufenzy.top/gtdfusqszz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.xylfe.cn/gtpleifrki.html

TS:   typeof x; x instanceof Date
来源：http://hz.fzhhl.top/gtlhdbkrux.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hnqzz.top/gtpwnwhwqq.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.vqdsnc.cn/gttlegzusy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.zhoulong.xyz/gtudaedilf.html

C#:   x.GetType().Name; x is int
来源：http://hz.jinqigufen.top/gtezjammoc.html

[A05] 整数除法与取模
来源：http://hz.chenlongwang.top/gtytxqbzzq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.wangshuangyany.cn/gtprrjkbvu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jqgfzy.top/gtebpcmycc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shanyushiyangtech.top/gtdigyjqjw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.haohaochexian.top/gtsvrjgsje.html

Java: 7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gtzjujluto.html

Go:   7 / 2; 7 % 2
来源：http://hz.zhaomingkeji.xyz/gtmrsdccge.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.tian-w.cn/gtxnydyysj.html

C#:   7 / 2; 7 % 2
来源：http://hz.yuxming.cn/gtfgscdikx.html

[A06] 字符串转数字
来源：http://hz.cqqwz.cn/gtceequjkx.html

Py:   int("42"); float("3.14")
来源：http://hz.nwbrower.top/gtwponhgxv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhiwuduotai.top/gtlqneusud.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.haohaochexian.top/gtvysxzpqd.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.fzhhl.top/gtluuabiyi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.vqdsnc.cn/gtrbrppbwu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.wangdashe.top/gtcvwtgrfj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.hammf.cn/gtrigyeqnc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yangfankeji.com/gttgmaxnzq.html

[A07] 数字转字符串
来源：http://hz.jianghu66.top/gtooheambk.html

Py:   str(42)
来源：http://hz.zhongyouzk.top/gtulfwxirb.html

PHP:  (string) 42; strval(42)
来源：http://hz.jyoumei.cn/gttjzjhebp.html

JS:   String(42); (42).toString()
来源：http://hz.ppjwa.cn/gtzculoubh.html

TS:   String(42)
来源：http://hz.fzhhl.top/gtazkrjvow.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhaomingkeji.xyz/gthsskzgkn.html

Go:   strconv.Itoa(42)
来源：http://hz.jqgufenzy.top/gtoiwtefip.html

Ruby: 42.to_s
来源：http://hz.yuxming.cn/gtsvanatkz.html

C#:   42.ToString()
来源：http://hz.jyoumei.cn/gtinoemaqe.html

[A08] 取整与四舍五入
来源：http://hz.yj20258888.top/gtbgiwvmsq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtzsprgqqd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.dashuyun.cn/gtubpcfmuk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.316326.xyz/gtxshhwhdi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.cdnleiting.top/gtlqgbhwtz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.ivvv.top/gtsloekjrs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yj202588.top/gtpfefcuye.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.0kj1m.cn/gtvfqssnic.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.nanxinkj.top/gtztqxjloj.html

[A09] 绝对值与最大最小值
来源：http://hz.daxiang520.top/gtirwsebjm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.c1oappe.top/gtqacvujak.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jinyuanbaomall.cn/gtwwszgxii.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hammf.cn/gtsyconopa.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yangfankeji.com/gtutvkikdc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.wangdashe.top/gtytwrpcll.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.svipenyu.cn/gthmjtccyt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.cqqwz.cn/gtkfugwlrt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.sweek.top/gtreojtoju.html

[A10] 生成随机数
来源：http://hz.jinyuanbaomall.cn/gtjzgswzzh.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ivvv.top/gtedfzpgls.html

PHP:  random_int(1, 100);
来源：http://hz.zycfv.cn/gtgbsfyflm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.aizwys.cn/gtgqndcvtr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shuidangran.top/gtqpkbhfyt.html

Java: new Random().nextInt(100) + 1
来源：http://hz.hongshengwenyu.top/gtccavspwp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.yj20258888.top/gtzuwepkut.html

Ruby: rand(1..100)
来源：http://hz.hnxiangtu.top/gtrksrlhlu.html

C#:   new Random().Next(1, 101)
来源：http://hz.zhongyouzk.top/gtbvudcexz.html

[A11] 条件表达式（三元）
来源：http://hz.hfpthk.cn/gtedzlbqsr.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.0kj1m.cn/gtilxyarbd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.gogol.net.cn/gtorkzakld.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.52xcode.cn/gtgmevotyc.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.smart0.xyz/gtwzgrhnfp.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yonumen.top/gtwqxhgzrl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.ywan-chungtsiang.top/gtfvyypvuf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.ppjwa.cn/gtvnfyimmp.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.tian-w.cn/gtuvfnzwop.html

[A12] 字符串插值 / 格式化
来源：http://hz.svipenyu.cn/gtzrctxcqg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.hysaishi.cn/gtxxewvwlp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.sxryk.cn/gthxwujuhl.html

JS:   `Hello, ${name}!`
来源：http://hz.c1oappe.top/gtlvsjywyi.html

TS:   `Hello, ${name}!`
来源：http://hz.andypj.xyz/gtgmeklyot.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.cucudq.cn/gtryqsnzts.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.ehwqpu.com/gtpoyiyqtv.html

Ruby: "Hello, #{name}!"
来源：http://hz.xinyue.icu/gtidsnmjnz.html

C#:   $"Hello, {name}!"
来源：http://hz.cashguo.top/gtbznqsyvx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.sweek.top/gtyyjqkvds.html

Py:   "第一行\n第二行"
来源：http://hz.mhx1999.top/gtdqvzakiu.html

PHP:  "第一行\n第二行"
来源：http://hz.daxiang520.top/gtoylmktyw.html

JS:   "第一行\n第二行"
来源：http://hz.redwolf501.top/gtoulwuheb.html

TS:   "第一行\n第二行"
来源：http://hz.jqgfzy.top/gtttcglbcm.html

Java: "第一行\n第二行"
来源：http://hz.fengsongda.top/gtsjmhimhs.html

Go:   "第一行\n第二行"
来源：http://hz.jiagoushi.top/gtzzjdfovi.html

Ruby: "第一行\n第二行"
来源：http://hz.zhengqikj.top/gttnhphxpe.html

C#:   "第一行\n第二行"
来源：http://hz.52xcode.cn/gtrnqmfrka.html

[A14] 注释写法
来源：http://hz.fzhhl.top/gtcspdtzzc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zhijiandao.cn/gtskqmgtxe.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.0kj1m.cn/gtvrphvqsp.html

JS:   // 单行；/* 多行 */
来源：http://hz.smart0.xyz/gtakgnripu.html

TS:   // 单行；/* 多行 */
来源：http://hz.shzxlz.cn/gtkipdojht.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.nanxuanxn.top/gtxvretasq.html

Go:   // 单行；/* 多行 */
来源：http://hz.mhx1999.top/gttqtywdlo.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.ivvv.top/gtexmaiwtk.html

C#:   // 单行；/* 多行 */
来源：http://hz.smart0.xyz/gtykgbxrpq.html

[A15] 空值判断与默认值
来源：http://hz.hysaishi.cn/gtmecuhsip.html

Py:   value = data or "默认值"
来源：http://hz.ppjwa.cn/gtuqebjkxn.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.jinqigufen.top/gttejfdtga.html

JS:   const value = data ?? "默认值";
来源：http://hz.xuanzx.com/gtypadmzrw.html

TS:   const value = data ?? "默认值";
来源：http://hz.sufxvd.cn/gtwilehozo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.zhengqikj.top/gtahjrbqkm.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.ybcxt.top/gtxipqtgse.html

Ruby: value = data || "默认值"
来源：http://hz.yj202588.top/gtbmncqksc.html

C#:   var value = data ?? "默认值";
来源：http://hz.tanke756.top/gthswwlviw.html

[A16] 真假值判断规则
来源：http://hz.tianlin.xyz/gtnqfbrofl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.ydzc1.top/gtsybsgjwy.html


<!-- 参考信息 -->