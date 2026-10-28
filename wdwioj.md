代发 wailian999

[U93] JS：模板字符串
来源：http://hz.andypj.xyz/gtqnmnrqak.html

`共 ${n} 条`
来源：http://hz.jinyuanbaomall.cn/gtwyjrnkoi.html

[U94] JS：箭头函数
来源：http://hz.fzhhl.top/gtblribrhj.html

const double = x => x * 2;
来源：http://hz.jiagoushi.top/gtrizhlrvr.html

[U95] JS：Promise 包装
来源：http://hz.bjfxy.top/gttxtdvmcg.html

new Promise((resolve, reject) => {})
来源：http://hz.nanxuanxn.top/gtbqydukzx.html

[U96] JS：async/await 与异常
来源：http://hz.iojbl.cn/gtiqoiepfb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.smart0.xyz/gthquruuky.html

[U97] JS：并发请求
来源：http://hz.gaohongyu789.top/gtweobwmzf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtxrvogptl.html

[U98] JS：fetch 带 JSON
来源：http://hz.jianghu66.top/gtsjqghzuy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.snrcjt.cn/gtujmbggxi.html

[U99] JS：事件监听
来源：http://hz.jinqigfzy.top/gtwvyyosgf.html

el.addEventListener("click", e => {})
来源：http://hz.vqdsnc.cn/gtfvpzogqx.html

[U100] JS：DOM 查询
来源：http://hz.ppjwa.cn/gtzahqrser.html

document.querySelector(".item")
来源：http://hz.ivvv.top/gtpuhlnlsv.html

[U101] JS：classList 操作
来源：http://hz.kuanghao11.cn/gtzhzfekxa.html

el.classList.toggle("active")
来源：http://hz.quarkkingdee.top/gtrpexzxrq.html

[U102] JS：本地存储
来源：http://hz.zdqjudy.top/gtckgrispy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.cqqwz.cn/gtcdrlitfv.html

[U103] JS：定时器
来源：http://hz.hnqzz.top/gtarkkehns.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jlsjyb.cn/gtezeybchg.html

[U104] JS：防抖
来源：http://hz.yuxming.cn/gttsniyizh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtikalzvzx.html

[U105] JS：节流
来源：http://hz.hywenlv.cn/gtlwndewgj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.cqqwz.cn/gtlzqitevr.html

[U106] JS：日期格式化
来源：http://hz.gzhubu.top/gtsocqwnyp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yangfankeji.com/gtfbemqfkb.html

[U107] JS：数字千分位
来源：http://hz.yonumen.top/gtbsysuzoq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jlsjyb.cn/gtkezmdhza.html

[U108] JS：随机整数
来源：http://hz.jqgufenzy.top/gtmwjzmver.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yanxiufei.cn/gtgravudkw.html

[U109] JS：数组分组
来源：http://hz.wangdashe.top/gtyfthyecm.html

Object.groupBy(arr, x => x.type)
来源：http://hz.cdnleiting.top/gtrevqyhlh.html

[U110] JS：数组分块
来源：http://hz.hnxiangtu.top/gtuurwyrtp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tian-w.cn/gtuuaachen.html

[U111] JS：对象转 Map
来源：http://hz.shanyushiyangtech.top/gtuzctcatv.html

new Map(Object.entries(obj))
来源：http://hz.shanyushiyangkeji.top/gtelnnwiag.html

[U112] JS：字符串补位
来源：http://hz.sysykeji.top/gtpdjksjne.html

"7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtyeuarmxz.html

[U113] JS：正则替换全部
来源：http://hz.hongshengwenyu.top/gtecnpewjp.html

s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtbmqpiwgf.html

[U114] JS：JSON 深比较
来源：http://hz.chenlongwang.top/gtpfarqoma.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gteucokovr.html

[U115] JS：生成 UUID
来源：http://hz.jianghu66.top/gtgembeqxk.html

crypto.randomUUID()
来源：http://hz.xziqi.cn/gtfkskcfyd.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xziqi.cn/gtettmqpkl.html

/** @param {string} name */ function f(name) {}
来源：http://hz.havefunace.top/gtmrwiswum.html

[U117] JS：单元测试
来源：http://hz.jyoumei.cn/gtvutdkxmk.html

npm i -D vitest;  npx vitest
来源：http://hz.yuxming.cn/gtkvlwanym.html

[U118] JS：开发服务器
来源：http://hz.jinghuilouyu.cn/gtjgnxozjz.html

npm i -D vite;  npx vite
来源：http://hz.52xcode.cn/gtxqbqhrep.html

[U119] JS：生产构建
来源：http://hz.pycfn.com/gtehovmdvz.html

npx vite build
来源：http://hz.xylfe.cn/gtrefsbubu.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ybcxt.top/gtupfyudhz.html

import.meta.env.VITE_API_URL
来源：http://hz.daxiang520.top/gtlaoqzpxp.html

================================================================================
来源：http://hz.mhx1999.top/gtvburabab.html

统计汇总
来源：http://hz.haohaochexian.top/gtlkkyiszf.html

================================================================================
来源：http://hz.zdqjudy.top/gtrjoqqqit.html

按语言统计（条）：
来源：http://hz.316326.xyz/gtkvfwnwyi.html

Python ......... 252
来源：http://hz.xuetiantiany.cn/gtzbkdayjk.html

PHP ............ 252
来源：http://hz.dashuyun.cn/gteuzhnivw.html

JavaScript ..... 252
来源：http://hz.gaohongyu789.top/gtxmsplwku.html

TypeScript ..... 212
来源：http://hz.sufxvd.cn/gtqbkkbaqf.html

Java ........... 212
来源：http://hz.feifeiyinyue.top/gtqssvikid.html

Go ............. 212
来源：http://hz.shangyingyoupin.top/gtbrbsbpyj.html

Ruby ........... 212
来源：http://hz.ywan-chungtsiang.top/gtydivojvk.html

C# ............. 212
来源：http://hz.gzhubu.top/gtgxxktmhd.html

C .............. 30
来源：http://hz.yonumen.top/gtpmfjdlhn.html

C++ ............ 30
来源：http://hz.hysaishi.cn/gtghijqkef.html

SQL ............ 90
来源：http://hz.smart0.xyz/gtwdttzjig.html

Bash ........... 80
来源：http://hz.zhijiandao.cn/gtnmvobvyh.html

Kotlin ......... 15
来源：http://hz.daria6918.cn/gtrumamywd.html

Swift .......... 15
来源：http://hz.hongshengwenyu.top/gtirgpydqt.html

Lua ............ 10
来源：http://hz.0kj1m.cn/gtmajlrkbb.html

Perl ........... 10
来源：http://hz.jiagoushi.top/gtsjrbrios.html

Scala .......... 10
来源：http://hz.dianchejie.cn/gtqfwkhomh.html

------------------------------------
来源：http://hz.zhixingplan.top/gtvjkvkpyg.html

合计 ........... 2106 条
来源：http://hz.316326.xyz/gtqltcdhea.html

按章节统计：
来源：http://hz.yuxming.cn/gtzhkpxaxl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xziqi.cn/gtkwrleiok.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.ydjk.org.cn/gtjvkrfpkl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.chenlongwang.top/gtqcymxuzl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.52xcode.cn/gtiusbcrgv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zdqjudy.top/gtuocebxli.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jianghu66.top/gtdlqzrfua.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.svipenyu.cn/gtycgpckdm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.hammf.cn/gtnrwicomq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtskofhgqg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.xinyue.icu/gtjyjmtosj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtfrmcyywl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hfpthk.cn/gtxotroenn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gtldjjwkdw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.iojbl.cn/gtcdyvcpvg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.sufxvd.cn/gtwujmtopi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtntafqzgb.html

Q SQL 专题                              90
来源：http://hz.sysykeji.top/gtetbzmzop.html

R Bash 专题                             80
来源：http://hz.mhx1999.top/gtyqcoylmy.html

S C / C++ 专题                          60
来源：http://hz.havefunace.top/gtqkoakpcd.html

T 其他语言补充                          60
来源：http://hz.nwbrower.top/gtherwghsy.html

U 高频实用片段                         120
来源：http://hz.ehwqpu.com/gtvdqtmtpy.html

------------------------------------
来源：http://hz.wangshuangyany.cn/gtzwjxmojc.html

合计                                  2106 条
来源：http://hz.hfpthk.cn/gtottkyzzp.html

--------------------------------------------------------------------------------
来源：http://hz.yangfankeji.com/gtesalrnkn.html

使用提醒
来源：http://hz.zhixingplan.top/gtyxyuyabx.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtrahzbcxg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.quarkkingdee.top/gtewcxowwm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shuidangran.top/gtacvyyuph.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.gaohongyu789.top/gttyszfwpe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ppjwa.cn/gtaetzjbot.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.c1oappe.top/gtnhghruvl.html

—— 文件结束 ——
来源：http://hz.wangshuangyany.cn/gtfvlonrst.html

================================================================================
来源：http://hz.ivvv.top/gtsrkhiszh.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ydzc1.top/gtatxazkzc.html

Common Programming Examples Cheat Book
来源：http://hz.zhijiandao.cn/gtaqgwwtse.html

================================================================================
来源：http://hz.shzxlz.cn/gtjkixxkuw.html

【收录内容】
来源：http://hz.guannengcc.top/gterzrcish.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.bjfxy.top/gtqcwstgzw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.cucudq.cn/gtgddswfyd.html

SQL · Bash · C · C++
来源：http://hz.cdnleiting.top/gtsvxhight.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yueranfly.top/gtuyerdrkv.html

【使用说明】
来源：http://hz.gogol.net.cn/gtggurziym.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xinyue.icu/gtlyrsqoqk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.sysykeji.top/gtyltvlzmv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hongshengwenyu.top/gtssbpojzs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yj20258888.top/gtahqgywha.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jiagoushi.top/gtpjzrorlf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.9152youxi.cn/gtjqwbjjng.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.cqqwz.cn/gtxlynalbg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yuanzhike.top/gtgofdwqcu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.nwbrower.top/gtjtejrjlo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yueranfly.top/gtbjvdorbz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.pycfn.com/gttedvlvni.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.kuanghao11.cn/gtybbyifjz.html

【文件统计】
来源：http://hz.hnqzz.top/gtkxdmegub.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jinyuanbaomall.cn/gtdvlhnwel.html

--------------------------------------------------------------------------------
来源：http://hz.0kj1m.cn/gtnjqpxsck.html

目  录
来源：http://hz.jqgufenzy.top/gtdylcmjyt.html

--------------------------------------------------------------------------------
来源：http://hz.mhx1999.top/gtakszsjwf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ydzc1.top/gtrxngnxvl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shzxlz.cn/gtojahkkah.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shanyushiyangtech.top/gtgoceattz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.cucudq.cn/gtzrkgiuyq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hywenlv.cn/gtubdzzhpz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.dashuyun.cn/gtiewrpugz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shanyushiyangkeji.top/gtymfcfmce.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.smart0.xyz/gtooqljndi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtxkpcbufe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gtxfcobtvs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.snrcjt.cn/gtexshkrnx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhengqikj.top/gtngrmrqix.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtiaxqymje.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.fzhhl.top/gtqamyzxhz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.fzhhl.top/gtnzxajkzu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.iojbl.cn/gtcmskoihb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhongyouzk.top/gtbjbxmnac.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.cheryme.top/gtptpalzdz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.yanxiufei.cn/gtodymhxbu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxuanxn.top/gtqgjbnjaz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinyuanbaomall.cn/gtjmcnfbwt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtbsspsbhh.html

A. 基础语法与类型
来源：http://hz.xziqi.cn/gtjeilbhtf.html

================================================================================
来源：http://hz.jiagoushi.top/gtvbqyvfun.html

[A01] Hello World
来源：http://hz.yvedp.cn/gtykljqhcv.html

Py:   print("Hello, World!")
来源：http://hz.dashuyun.cn/gttbftxyxt.html

PHP:  echo "Hello, World!";
来源：http://hz.gaohongyu789.top/gthknjrvtu.html

JS:   console.log("Hello, World!");
来源：http://hz.nwbrower.top/gtkdwtntia.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yj202588.top/gthuwwgvct.html

Java: System.out.println("Hello, World!");
来源：http://hz.shanyushiyangkeji.top/gtggsdenzt.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.316326.xyz/gtkkbqfggm.html

Ruby: puts "Hello, World!"
来源：http://hz.fengsongda.top/gtohuuikbm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhijiandao.cn/gtoijryvux.html

[A02] 变量声明与赋值
来源：http://hz.cucudq.cn/gtxclllgyq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.dianchejie.cn/gtdgzqijqn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jqgfzy.top/gtqxhhgzkd.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jyoumei.cn/gtyikbjyze.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ydzc1.top/gtyvennjgn.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.redwolf501.top/gtonrrjsdb.html

Go:   name := "Alex"; age := 20
来源：http://hz.52xcode.cn/gtjzifpviw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yvedp.cn/gtiegswlvr.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.haohaochexian.top/gtcutnebkj.html

[A03] 常量定义
来源：http://hz.jianghu66.top/gtiyrqmjys.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.pengpengdd.cyou/gtruybaboz.html

PHP:  const PI = 3.14159;
来源：http://hz.cqqwz.cn/gtjgwerimm.html

JS:   const PI = 3.14159;
来源：http://hz.pycfn.com/gtqwgrnorh.html

TS:   const PI: number = 3.14159;
来源：http://hz.gotoacloud.top/gtffqihuck.html

Java: static final double PI = 3.14159;
来源：http://hz.ppjwa.cn/gtjjoenhgm.html

Go:   const PI = 3.14159
来源：http://hz.nwbrower.top/gthsnxjgdv.html

Ruby: PI = 3.14159
来源：http://hz.chenjidiqi.icu/gtcwizsqfr.html

C#:   const double PI = 3.14159;
来源：http://hz.nanxuanxn.top/gtzxkgiqyf.html

[A04] 判断变量类型
来源：http://hz.xinyue.icu/gtpqncezpv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.tian-w.cn/gtfbqukbiz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shzxlz.cn/gtmivqiqbs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hongshengwenyu.top/gtufaivehe.html

TS:   typeof x; x instanceof Date
来源：http://hz.sxryk.cn/gtctiuvhpc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.daria6918.cn/gtbbdjydeo.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zdqjudy.top/gteysygroa.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sufxvd.cn/gthebyyeui.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhijiandao.cn/gtugevrllg.html

[A05] 整数除法与取模
来源：http://hz.nanxuanxn.top/gtvzacprwt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.chenlongwang.top/gtmfklccgn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.feifeiyinyue.top/gtewnygrck.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yonumen.top/gtfqsdngpz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.mhx1999.top/gtdamhnecb.html

Java: 7 / 2; 7 % 2
来源：http://hz.zdqjudy.top/gtvqwgudjx.html

Go:   7 / 2; 7 % 2
来源：http://hz.hnxiangtu.top/gtehpdatut.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.0kj1m.cn/gtrqflzmxj.html

C#:   7 / 2; 7 % 2
来源：http://hz.daria6918.cn/gtwsszfhpq.html

[A06] 字符串转数字
来源：http://hz.hywenlv.cn/gtagvkncov.html

Py:   int("42"); float("3.14")
来源：http://hz.birdmap.top/gtscxcemkw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.guannengcc.top/gtwuzbsmnw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.zhoulong.xyz/gtydwgrnty.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yueranfly.top/gtsjrqaaac.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ydzc1.top/gtvjkvutfi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.daria6918.cn/gtwtpdaxfb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jyoumei.cn/gtriduqphk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.zycfv.cn/gtwmqxfjrq.html

[A07] 数字转字符串
来源：http://hz.andypj.xyz/gtopehgrrb.html

Py:   str(42)
来源：http://hz.nanxuanxn.top/gtphlvunin.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhoulong.xyz/gtgjttvyua.html

JS:   String(42); (42).toString()
来源：http://hz.guowangkeji.top/gtzdgxxerk.html

TS:   String(42)
来源：http://hz.feifeiyinyue.top/gthjmnkyrk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.chenjidiqi.icu/gtuixuqldv.html

Go:   strconv.Itoa(42)
来源：http://hz.shuidangran.top/gtvuzmksuv.html

Ruby: 42.to_s
来源：http://hz.zhiwuduotai.top/gtmhvxzvmy.html

C#:   42.ToString()
来源：http://hz.ydjk.org.cn/gtrpmuiuid.html

[A08] 取整与四舍五入
来源：http://hz.svipenyu.cn/gtcguiobpi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.ywan-chungtsiang.top/gtifubeisv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.dashuyun.cn/gtjkdklwoc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.andypj.xyz/gtbjybtslj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yangfankeji.com/gtyjefitql.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.zhijiandao.cn/gtcchqybtk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.ydzc1.top/gtpejydvxk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.fzhhl.top/gtlgrwhidk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.ppjwa.cn/gthzcdotya.html

[A09] 绝对值与最大最小值
来源：http://hz.sxryk.cn/gtnnjvqktf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xziqi.cn/gtiwrbyvqj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.chenlongwang.top/gtvggyckup.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zhiwuduotai.top/gtmpabtnjh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.chenlongwang.top/gthybytcbk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.xylfe.cn/gtfxjbvyyx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.aibaodan.cn/gtaiaapwkf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.shangyingyoupin.top/gtyowdsxdi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zhengqikj.top/gtxhnvfovp.html

[A10] 生成随机数
来源：http://hz.jyoumei.cn/gtiwectsdq.html

Py:   import random; random.randint(1, 100)
来源：http://hz.bjfxy.top/gtulbnnfvm.html

PHP:  random_int(1, 100);
来源：http://hz.yj20258888.top/gttkuthceq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.fzhhl.top/gtnimruolr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jqgfzy.top/gtnclnuqqj.html

Java: new Random().nextInt(100) + 1
来源：http://hz.hysaishi.cn/gtsdtyeabn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.kuanghao11.cn/gtpjcchqls.html

Ruby: rand(1..100)
来源：http://hz.pengpengdd.cyou/gtyxucdzwv.html

C#:   new Random().Next(1, 101)
来源：http://hz.guowangkeji.top/gtsojorpsk.html

[A11] 条件表达式（三元）
来源：http://hz.gotoacloud.top/gtygebagjr.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jlsjyb.cn/gtectquqvb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.tian-w.cn/gtqsndcegh.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.nanxuanxn.top/gtccimbzqo.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jinghuilouyu.cn/gtbvxwtxjt.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.bjfxy.top/gtgsswigrv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.sxryk.cn/gtxodicpwu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hammf.cn/gtzphbzgni.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.jinghuilouyu.cn/gtyknbmkwd.html

[A12] 字符串插值 / 格式化
来源：http://hz.yuxming.cn/gtxluaypsd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.ivvv.top/gtzjwigqzb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.shanyushiyangtech.top/gtjcdjqped.html

JS:   `Hello, ${name}!`
来源：http://hz.0kj1m.cn/gtinefobhi.html

TS:   `Hello, ${name}!`
来源：http://hz.shanyushiyangtech.top/gtzsdaxoei.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.shzxlz.cn/gtmppkhhdl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.sxryk.cn/gtqgtqvwsm.html

Ruby: "Hello, #{name}!"
来源：http://hz.vqdsnc.cn/gtzwouzfqd.html

C#:   $"Hello, {name}!"
来源：http://hz.pengpengdd.cyou/gtynxfekvb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yuanzhike.top/gtpwhxhees.html

Py:   "第一行\n第二行"
来源：http://hz.tian-w.cn/gtstzxzozo.html

PHP:  "第一行\n第二行"
来源：http://hz.shangyingyoupin.top/gtjlptujto.html

JS:   "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtafpnwuuv.html

TS:   "第一行\n第二行"
来源：http://hz.cdnleiting.top/gtdmuzxcjl.html

Java: "第一行\n第二行"
来源：http://hz.cucudq.cn/gtkgiulzhr.html

Go:   "第一行\n第二行"
来源：http://hz.tanke756.top/gtmpijkvqh.html

Ruby: "第一行\n第二行"
来源：http://hz.wangdashe.top/gtripgsadb.html

C#:   "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtcfwuynpt.html

[A14] 注释写法
来源：http://hz.svipenyu.cn/gtqfxyfqbo.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.shzxlz.cn/gtidcbifdn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.nwbrower.top/gtiklsxoow.html

JS:   // 单行；/* 多行 */
来源：http://hz.nwbrower.top/gtbzdlpkyw.html

TS:   // 单行；/* 多行 */
来源：http://hz.daria6918.cn/gtvvrgtsqu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.birdmap.top/gtfdwmpxcc.html

Go:   // 单行；/* 多行 */
来源：http://hz.vqdsnc.cn/gtptcanlkx.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.xziqi.cn/gtvsczilfo.html

C#:   // 单行；/* 多行 */
来源：http://hz.redwolf501.top/gtytporcjz.html

[A15] 空值判断与默认值
来源：http://hz.ydjk.org.cn/gtifuvfihi.html

Py:   value = data or "默认值"
来源：http://hz.zhaomingkeji.xyz/gtfxdmkgzy.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.gogol.net.cn/gtmczgubln.html

JS:   const value = data ?? "默认值";
来源：http://hz.snrcjt.cn/gthatlvejc.html

TS:   const value = data ?? "默认值";
来源：http://hz.svipenyu.cn/gtdgvjoaaa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.wangshuangyany.cn/gtwvqsogyu.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.cqqwz.cn/gtvxxbeulb.html

Ruby: value = data || "默认值"
来源：http://hz.jlsjyb.cn/gtlcxmbtyi.html

C#:   var value = data ?? "默认值";
来源：http://hz.gogol.net.cn/gtpriltrkg.html

[A16] 真假值判断规则
来源：http://hz.jiagoushi.top/gtzynluhej.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.aibaodan.cn/gttyuymqqx.html


<!-- 参考信息 -->