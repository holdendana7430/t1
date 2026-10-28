代发 wailian999

[U93] JS：模板字符串
来源：http://hz.haohaochexian.top/gtnnnktkey.html

`共 ${n} 条`
来源：http://hz.yonumen.top/gtjlbmvsdq.html

[U94] JS：箭头函数
来源：http://hz.9152youxi.cn/gtivjiwjsm.html

const double = x => x * 2;
来源：http://hz.ydjk.org.cn/gtczzylnzu.html

[U95] JS：Promise 包装
来源：http://hz.mhx1999.top/gtoimrrklq.html

new Promise((resolve, reject) => {})
来源：http://hz.ppjwa.cn/gtukvkefms.html

[U96] JS：async/await 与异常
来源：http://hz.shanyushiyangkeji.top/gttbcwdpix.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj202588.top/gttpgbinmk.html

[U97] JS：并发请求
来源：http://hz.ivvv.top/gtxikwlfsr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtwlpehrne.html

[U98] JS：fetch 带 JSON
来源：http://hz.jqgufenzy.top/gtbtlpejpl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jianghu66.top/gtmqgzedgh.html

[U99] JS：事件监听
来源：http://hz.cheryme.top/gtgjdxinba.html

el.addEventListener("click", e => {})
来源：http://hz.haohaochexian.top/gtnhrerdvv.html

[U100] JS：DOM 查询
来源：http://hz.shzxlz.cn/gtchwsomix.html

document.querySelector(".item")
来源：http://hz.hnxiangtu.top/gtiztnlcan.html

[U101] JS：classList 操作
来源：http://hz.yj20258888.top/gtnapnzsoj.html

el.classList.toggle("active")
来源：http://hz.yongpay.top/gtgndcwyvt.html

[U102] JS：本地存储
来源：http://hz.9152youxi.cn/gtivjknyhy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.gotoacloud.top/gtcwnfjybp.html

[U103] JS：定时器
来源：http://hz.zhaomingkeji.xyz/gtggapocpw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xuetiantiany.cn/gtxjreqygg.html

[U104] JS：防抖
来源：http://hz.cqqwz.cn/gtueknycmt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.havefunace.top/gttxmsqibw.html

[U105] JS：节流
来源：http://hz.zhoulong.xyz/gtiilsjzgn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hongshengwenyu.top/gtwlpdwxjc.html

[U106] JS：日期格式化
来源：http://hz.dashuyun.cn/gtrzjigrda.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yvedp.cn/gtgiyawppy.html

[U107] JS：数字千分位
来源：http://hz.xylfe.cn/gthcktgzzx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhengqikj.top/gtqxaskrpo.html

[U108] JS：随机整数
来源：http://hz.ybcxt.top/gtvchogrcp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guowangkeji.top/gtzvzyuhkl.html

[U109] JS：数组分组
来源：http://hz.yj20258888.top/gthdmgcqgf.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangtech.top/gtiabrmrwe.html

[U110] JS：数组分块
来源：http://hz.tianlin.xyz/gtahqfqvbd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.sysykeji.top/gtqsbiccoy.html

[U111] JS：对象转 Map
来源：http://hz.yuxming.cn/gtswvwyyge.html

new Map(Object.entries(obj))
来源：http://hz.shangyingyoupin.top/gtkkpwlxho.html

[U112] JS：字符串补位
来源：http://hz.xziqi.cn/gtifyjbsiz.html

"7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtxqajafkv.html

[U113] JS：正则替换全部
来源：http://hz.cashguo.top/gtzuhznmlk.html

s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtejzjfcdx.html

[U114] JS：JSON 深比较
来源：http://hz.xylfe.cn/gtriwjyoyj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jiagoushi.top/gtlgjeuhup.html

[U115] JS：生成 UUID
来源：http://hz.shuidangran.top/gtwxvkebeu.html

crypto.randomUUID()
来源：http://hz.dianchejie.cn/gthiwtyxbc.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.ppjwa.cn/gtprtifbgy.html

/** @param {string} name */ function f(name) {}
来源：http://hz.gaohongyu789.top/gtqmfzwgnv.html

[U117] JS：单元测试
来源：http://hz.gogol.net.cn/gtfzbqkize.html

npm i -D vitest;  npx vitest
来源：http://hz.snrcjt.cn/gtrftjxjxn.html

[U118] JS：开发服务器
来源：http://hz.zhixingplan.top/gtlokdswrx.html

npm i -D vite;  npx vite
来源：http://hz.ybcxt.top/gtbjhsmpje.html

[U119] JS：生产构建
来源：http://hz.yj20258.top/gtjvprhdfl.html

npx vite build
来源：http://hz.haohaochexian.top/gtbhtzztiw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.chenjidiqi.icu/gtixbqedyj.html

import.meta.env.VITE_API_URL
来源：http://hz.ybcxt.top/gthidpruex.html

================================================================================
来源：http://hz.zhixingplan.top/gtqkwndsao.html

统计汇总
来源：http://hz.gotoacloud.top/gtafiypzrn.html

================================================================================
来源：http://hz.jinqigufen.top/gtdjtnxqfy.html

按语言统计（条）：
来源：http://hz.ybcxt.top/gtgbeoxzhx.html

Python ......... 252
来源：http://hz.daria6918.cn/gtkdrazqkd.html

PHP ............ 252
来源：http://hz.jinghuilouyu.cn/gtrhjmjabr.html

JavaScript ..... 252
来源：http://hz.shanyushiyangtech.top/gtbfvrnegt.html

TypeScript ..... 212
来源：http://hz.xuetiantiany.cn/gtbasrpzsg.html

Java ........... 212
来源：http://hz.sysykeji.top/gtdaxsuthd.html

Go ............. 212
来源：http://hz.dashuyun.cn/gtvtbhidvp.html

Ruby ........... 212
来源：http://hz.fengsongda.top/gtvfqhlhyq.html

C# ............. 212
来源：http://hz.cucudq.cn/gtymkspypl.html

C .............. 30
来源：http://hz.aizwys.cn/gtlyddymef.html

C++ ............ 30
来源：http://hz.jiagoushi.top/gtittjxqbo.html

SQL ............ 90
来源：http://hz.cheryme.top/gtfhdgdatb.html

Bash ........... 80
来源：http://hz.daxiang520.top/gtkcgiqtrj.html

Kotlin ......... 15
来源：http://hz.yueranfly.top/gtcdephbhq.html

Swift .......... 15
来源：http://hz.jiagoushi.top/gtddepoxug.html

Lua ............ 10
来源：http://hz.shanyushiyangkeji.top/gtmatwpplh.html

Perl ........... 10
来源：http://hz.xylfe.cn/gtcvboepjg.html

Scala .......... 10
来源：http://hz.shangyingyoupin.top/gtimskgxze.html

------------------------------------
来源：http://hz.aizwys.cn/gteoxlympi.html

合计 ........... 2106 条
来源：http://hz.quarkkingdee.top/gtffucsqnq.html

按章节统计：
来源：http://hz.kuanghao11.cn/gtjxqtuvlc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.nanxuanxn.top/gtupppyxaa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ywan-chungtsiang.top/gtgisyjadq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cdnleiting.top/gtgebhpobn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.gzhubu.top/gtwsyhhpbh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.shzxlz.cn/gtuatgndje.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.sufxvd.cn/gtgbqxvycd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhongyouzk.top/gtgpnuulgy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yuanzhike.top/gtoxcsupry.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtepgvskid.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jinqigufen.top/gtyfqkwyxw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtxofaprph.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtcsecxksp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhengqikj.top/gtgvquhmpx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.kuanghao11.cn/gthwrlkwqn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.316326.xyz/gtkhswekcd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gtydpvirnw.html

Q SQL 专题                              90
来源：http://hz.xuetiantiany.cn/gtcyejmhfi.html

R Bash 专题                             80
来源：http://hz.pengpengdd.cyou/gtpwapyhxt.html

S C / C++ 专题                          60
来源：http://hz.jinqigufen.top/gtjnflzmoa.html

T 其他语言补充                          60
来源：http://hz.pengpengdd.cyou/gtncaidsnq.html

U 高频实用片段                         120
来源：http://hz.chenlongwang.top/gtselevnlm.html

------------------------------------
来源：http://hz.havefunace.top/gtniqpmvkt.html

合计                                  2106 条
来源：http://hz.yj20258888.top/gtbvijxzrz.html

--------------------------------------------------------------------------------
来源：http://hz.wangdashe.top/gthxsxxzzo.html

使用提醒
来源：http://hz.redwolf501.top/gtohcumlut.html

--------------------------------------------------------------------------------
来源：http://hz.hfpthk.cn/gtgwwvlzef.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.daria6918.cn/gtoyaoalpv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hnqzz.top/gtrdrrnzmk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.quarkkingdee.top/gttkvnamik.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.fzhhl.top/gtiwjjmzjz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.tian-w.cn/gtpvwkzxzo.html

—— 文件结束 ——
来源：http://hz.tian-w.cn/gtlukqvubp.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthvclgpxi.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.feifeiyinyue.top/gtbaukwamd.html

Common Programming Examples Cheat Book
来源：http://hz.feifeiyinyue.top/gtuwoulema.html

================================================================================
来源：http://hz.fzhhl.top/gtwtdnyiwy.html

【收录内容】
来源：http://hz.ehwqpu.com/gtzqzwnlzl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cheryme.top/gtjittdmdm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cheryme.top/gtgdiravap.html

SQL · Bash · C · C++
来源：http://hz.52xcode.cn/gtmkenigec.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.52xcode.cn/gtassxgclx.html

【使用说明】
来源：http://hz.gogol.net.cn/gthnmcgdah.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhaomingkeji.xyz/gtmsqlfcva.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ybcxt.top/gtzioukqcj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ywan-chungtsiang.top/gtjnmlufrg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.hongshengwenyu.top/gtslquhyos.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.gotoacloud.top/gtjwudgdtm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.cashguo.top/gtwnyliqfb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xuanzx.com/gtsaouetnd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.316326.xyz/gtkepzwajm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.sufxvd.cn/gtkavxkrxz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.iojbl.cn/gtrlpjkrhh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.xziqi.cn/gtjptihoev.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.aibaodan.cn/gtbwtckpst.html

【文件统计】
来源：http://hz.chenjidiqi.icu/gtjwwcqbwf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.316326.xyz/gtwlchncxj.html

--------------------------------------------------------------------------------
来源：http://hz.wangdashe.top/gtgelgjgxl.html

目  录
来源：http://hz.xingfuxueyuan.xyz/gtqelmilsx.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtudazctqb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xinyue.icu/gtmdwbfvsv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jqgufenzy.top/gtocrbelzf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.tanke756.top/gtwtpsisuo.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ywan-chungtsiang.top/gtsxnqtave.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.sufxvd.cn/gtznurikep.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cashguo.top/gtopypcsfk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xziqi.cn/gtiitqkabz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.andypj.xyz/gtrcyewfqf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtayaovlqf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yuanzhike.top/gtyvfkhptc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinqigfzy.top/gtxavkyxct.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gttvbabqwv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtaddrbswu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yangfankeji.com/gtwrbitndu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yonumen.top/gtehpbjgof.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtuyhsuyhq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.smart0.xyz/gtbeonkuhj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jianghu66.top/gtblovorzs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cucudq.cn/gtsgaipaer.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shzxlz.cn/gtgorffwcl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj20258.top/gtzkftwtsz.html

================================================================================
来源：http://hz.jiagoushi.top/gtjtqpjbeu.html

A. 基础语法与类型
来源：http://hz.andypj.xyz/gtztdngnhd.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtepcvtndz.html

[A01] Hello World
来源：http://hz.yj202588.top/gtydqaxijp.html

Py:   print("Hello, World!")
来源：http://hz.yuanzhike.top/gtiqvlcgex.html

PHP:  echo "Hello, World!";
来源：http://hz.mhx1999.top/gtubgatfyn.html

JS:   console.log("Hello, World!");
来源：http://hz.yvedp.cn/gtactmcima.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.sweek.top/gthzdtcawa.html

Java: System.out.println("Hello, World!");
来源：http://hz.hnqzz.top/gtwfjxfipo.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.shzxlz.cn/gtlihnyjew.html

Ruby: puts "Hello, World!"
来源：http://hz.hammf.cn/gtsqjncqqf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ywan-chungtsiang.top/gtvjqybyvs.html

[A02] 变量声明与赋值
来源：http://hz.redwolf501.top/gtcvwgmbvo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shanyushiyangkeji.top/gtnnhnwgix.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yueranfly.top/gtyqlrtrvl.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yangfankeji.com/gtqpuvvbap.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.pycfn.com/gtewtpmlhe.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ywan-chungtsiang.top/gtqxyexlnu.html

Go:   name := "Alex"; age := 20
来源：http://hz.jqgufenzy.top/gthiwhtrvr.html

Ruby: name = "Alex"; age = 20
来源：http://hz.gogol.net.cn/gtijugprgz.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hammf.cn/gtzjkhctsb.html

[A03] 常量定义
来源：http://hz.jqgufenzy.top/gtbtqyktpt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.tian-w.cn/gtdqonfqjz.html

PHP:  const PI = 3.14159;
来源：http://hz.yj20258888.top/gtjbpxxgfu.html

JS:   const PI = 3.14159;
来源：http://hz.cucudq.cn/gtgnnkocyt.html

TS:   const PI: number = 3.14159;
来源：http://hz.nanxuanxn.top/gtznuinkpm.html

Java: static final double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtlhrzaqml.html

Go:   const PI = 3.14159
来源：http://hz.zhijiandao.cn/gtddfgciqw.html

Ruby: PI = 3.14159
来源：http://hz.jqgfzy.top/gtavdvupdg.html

C#:   const double PI = 3.14159;
来源：http://hz.wangdashe.top/gtgfifasgs.html

[A04] 判断变量类型
来源：http://hz.aizwys.cn/gtaqttbygs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.pengpengdd.cyou/gttbnbqpsy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yvedp.cn/gttynxvout.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.shanyushiyangkeji.top/gtuiaokqug.html

TS:   typeof x; x instanceof Date
来源：http://hz.hammf.cn/gtukekihlo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.meibo888.top/gtmchukect.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.ivvv.top/gtdeqnwsxh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.dianchejie.cn/gtdqvyolvl.html

C#:   x.GetType().Name; x is int
来源：http://hz.daria6918.cn/gtsipawpqa.html

[A05] 整数除法与取模
来源：http://hz.nanxuanxn.top/gtzdyzaokt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jinghuilouyu.cn/gtbnqmdlpe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jlsjyb.cn/gtuqqkdfqe.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shangyingyoupin.top/gteycnigqz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhoulong.xyz/gtrrmukcay.html

Java: 7 / 2; 7 % 2
来源：http://hz.shuidangran.top/gtighvftgm.html

Go:   7 / 2; 7 % 2
来源：http://hz.yvedp.cn/gtjpmwkazp.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.pengpengdd.cyou/gttgxnosxp.html

C#:   7 / 2; 7 % 2
来源：http://hz.zhiwuduotai.top/gtmnlwctjb.html

[A06] 字符串转数字
来源：http://hz.quarkkingdee.top/gtnzssgywn.html

Py:   int("42"); float("3.14")
来源：http://hz.hysaishi.cn/gtfngqpjxw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.pycfn.com/gtuwislhia.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.pycfn.com/gtpajdjtav.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.redwolf501.top/gtieetucwc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.hnxiangtu.top/gtpqwqgntk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jiagoushi.top/gtfloaabyp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.feifeiyinyue.top/gtssuxkfso.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.kuanghao11.cn/gteydewzhb.html

[A07] 数字转字符串
来源：http://hz.xylfe.cn/gtrzogygrt.html

Py:   str(42)
来源：http://hz.zdqjudy.top/gtloalkylt.html

PHP:  (string) 42; strval(42)
来源：http://hz.bjfxy.top/gtgjhuceqs.html

JS:   String(42); (42).toString()
来源：http://hz.shanyushiyangtech.top/gtvwuxstri.html

TS:   String(42)
来源：http://hz.ybcxt.top/gttflrcppu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.birdmap.top/gtrhpahpfm.html

Go:   strconv.Itoa(42)
来源：http://hz.sxryk.cn/gtjkotfbxn.html

Ruby: 42.to_s
来源：http://hz.yj20258.top/gtmcepgrcn.html

C#:   42.ToString()
来源：http://hz.c1oappe.top/gtnwnffpzf.html

[A08] 取整与四舍五入
来源：http://hz.zdqjudy.top/gtfhcofizm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.sxryk.cn/gthcalhbxg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.ehwqpu.com/gtsoibthch.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.gotoacloud.top/gtubaatpvb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.shangyingyoupin.top/gtwucznvze.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.redwolf501.top/gtnpbrakyj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.ydjk.org.cn/gttdljornp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.nanxuanxn.top/gtgyimalcf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.hywenlv.cn/gtajyroixb.html

[A09] 绝对值与最大最小值
来源：http://hz.dianchejie.cn/gthzfzhsfv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.tianlin.xyz/gtuodpqijd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xuetiantiany.cn/gtxwakzflc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.cheryme.top/gtkkvkwiiy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.gaohongyu789.top/gtgjzknkun.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.shanyushiyangtech.top/gtiftbqnpi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zycfv.cn/gtucolwkhe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.ydjk.org.cn/gtdfgvmpfg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zhiwuduotai.top/gtmljgvtyy.html

[A10] 生成随机数
来源：http://hz.havefunace.top/gtmzzibkal.html

Py:   import random; random.randint(1, 100)
来源：http://hz.jinqigfzy.top/gtwiwayzvy.html

PHP:  random_int(1, 100);
来源：http://hz.guannengcc.top/gtajkffcin.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yuxming.cn/gtgkhiahja.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhongyouzk.top/gtgkgbvefc.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yonumen.top/gtbmlkogsb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.tianlin.xyz/gtiqnosvza.html

Ruby: rand(1..100)
来源：http://hz.jyoumei.cn/gtmfhrirmz.html

C#:   new Random().Next(1, 101)
来源：http://hz.zycfv.cn/gtgykuzpii.html

[A11] 条件表达式（三元）
来源：http://hz.xylfe.cn/gtcvjkczjk.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.cashguo.top/gtjqogbukg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.nanxinkj.top/gtkdxjelwq.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.snrcjt.cn/gthgcjjqll.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gthltulamy.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yanxiufei.cn/gtpkfwrduc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.gaohongyu789.top/gtdhzpdcmj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.cheryme.top/gtlovfrueq.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.sysykeji.top/gtdjmngxcj.html

[A12] 字符串插值 / 格式化
来源：http://hz.xuetiantiany.cn/gtfoqbrzjv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jyoumei.cn/gtqktcdmcj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.wangshuangyany.cn/gtgniggtmi.html

JS:   `Hello, ${name}!`
来源：http://hz.vqdsnc.cn/gtivqwibrw.html

TS:   `Hello, ${name}!`
来源：http://hz.chenzaomai.com/gtlprfrqey.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zycfv.cn/gtwhuqayjo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jyoumei.cn/gtsotvtmnl.html

Ruby: "Hello, #{name}!"
来源：http://hz.guowangkeji.top/gttmvbfbdi.html

C#:   $"Hello, {name}!"
来源：http://hz.chenlongwang.top/gtytvqzdtp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.fzhhl.top/gtfdhtgnpm.html

Py:   "第一行\n第二行"
来源：http://hz.yangfankeji.com/gtvektlrmj.html

PHP:  "第一行\n第二行"
来源：http://hz.shuidangran.top/gtbksvocgo.html

JS:   "第一行\n第二行"
来源：http://hz.quarkkingdee.top/gtsbtmyowu.html

TS:   "第一行\n第二行"
来源：http://hz.hongshengwenyu.top/gtymlikjci.html

Java: "第一行\n第二行"
来源：http://hz.yonumen.top/gtvxfljjek.html

Go:   "第一行\n第二行"
来源：http://hz.shangyingyoupin.top/gtxndpyeoq.html

Ruby: "第一行\n第二行"
来源：http://hz.jinqigufen.top/gtamrllklf.html

C#:   "第一行\n第二行"
来源：http://hz.nanxuanxn.top/gtiaxfwstn.html

[A14] 注释写法
来源：http://hz.yuxming.cn/gtthhwalre.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yonumen.top/gtmzxyltqt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.bjfxy.top/gtbcgumegd.html

JS:   // 单行；/* 多行 */
来源：http://hz.jqgfzy.top/gtfksyjire.html

TS:   // 单行；/* 多行 */
来源：http://hz.sufxvd.cn/gtykgshuzi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.jinqigufen.top/gtebdskssx.html

Go:   // 单行；/* 多行 */
来源：http://hz.gotoacloud.top/gtbecrqwxn.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.pengpengdd.cyou/gtlmzuvytv.html

C#:   // 单行；/* 多行 */
来源：http://hz.hnqzz.top/gtjeaedqss.html

[A15] 空值判断与默认值
来源：http://hz.hysaishi.cn/gtviwdtzsd.html

Py:   value = data or "默认值"
来源：http://hz.mhx1999.top/gtqpvwmjqt.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.feifeiyinyue.top/gtfwgxzhuj.html

JS:   const value = data ?? "默认值";
来源：http://hz.c1oappe.top/gtalblznee.html

TS:   const value = data ?? "默认值";
来源：http://hz.shzxlz.cn/gtanumzgqp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.zhoulong.xyz/gtgcyhzjlw.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.fengsongda.top/gtfmcsjgfs.html

Ruby: value = data || "默认值"
来源：http://hz.hnxiangtu.top/gtvfucoxxm.html

C#:   var value = data ?? "默认值";
来源：http://hz.yj20258.top/gtqwsnpgao.html

[A16] 真假值判断规则
来源：http://hz.svipenyu.cn/gtupnmgtrf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.ydjk.org.cn/gtnnzaggfd.html


<!-- 参考信息 -->