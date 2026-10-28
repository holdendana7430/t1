代发 wailian999

[U91] JS：对象键值遍历
来源：http://hz.0kj1m.cn/gtbrediaac.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.52xcode.cn/gtrvpyiyao.html

[U92] JS：深拷贝
来源：http://hz.svipenyu.cn/gtoysnyrrr.html

structuredClone(obj)
来源：http://hz.yj20258.top/gtdndklouo.html

[U93] JS：模板字符串
来源：http://hz.jqgufenzy.top/gttcboachy.html

`共 ${n} 条`
来源：http://hz.dashuyun.cn/gtcwihbwza.html

[U94] JS：箭头函数
来源：http://hz.shzxlz.cn/gtzobfxuzc.html

const double = x => x * 2;
来源：http://hz.zycfv.cn/gtlygcbkod.html

[U95] JS：Promise 包装
来源：http://hz.cucudq.cn/gtwzcgoukw.html

new Promise((resolve, reject) => {})
来源：http://hz.yongpay.top/gtxnmzrjts.html

[U96] JS：async/await 与异常
来源：http://hz.redwolf501.top/gtlsrkzncr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.iojbl.cn/gtjvmcmtav.html

[U97] JS：并发请求
来源：http://hz.tian-w.cn/gtafqinoas.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gtypmrxhqm.html

[U98] JS：fetch 带 JSON
来源：http://hz.kuanghao11.cn/gtmsvjcuin.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.dashuyun.cn/gtpaqyulcv.html

[U99] JS：事件监听
来源：http://hz.zhongyouzk.top/gtrtmzglqj.html

el.addEventListener("click", e => {})
来源：http://hz.iojbl.cn/gtupbzgvwr.html

[U100] JS：DOM 查询
来源：http://hz.hysaishi.cn/gtkggyzovr.html

document.querySelector(".item")
来源：http://hz.zhiwuduotai.top/gtnxxcmkyr.html

[U101] JS：classList 操作
来源：http://hz.quarkkingdee.top/gtqnidgrin.html

el.classList.toggle("active")
来源：http://hz.ybcxt.top/gtztttnobo.html

[U102] JS：本地存储
来源：http://hz.316326.xyz/gtjtuxfklz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ppjwa.cn/gtddsfugem.html

[U103] JS：定时器
来源：http://hz.jlsjyb.cn/gtxzesjggl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.shanyushiyangtech.top/gtikwxsxbi.html

[U104] JS：防抖
来源：http://hz.zhiwuduotai.top/gtjesrzfpv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.sufxvd.cn/gtnaeogela.html

[U105] JS：节流
来源：http://hz.shzxlz.cn/gtyzqdinil.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhengqikj.top/gtjbedfuyw.html

[U106] JS：日期格式化
来源：http://hz.hywenlv.cn/gtubcpbtmr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shangyingyoupin.top/gtsoxkzjei.html

[U107] JS：数字千分位
来源：http://hz.dianchejie.cn/gtjlkrxqsp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinghuilouyu.cn/gtwxwoknwu.html

[U108] JS：随机整数
来源：http://hz.chenjidiqi.icu/gtnehnmoiu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sysykeji.top/gtylpbhnoz.html

[U109] JS：数组分组
来源：http://hz.hysaishi.cn/gthwrefpdj.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jinghuilouyu.cn/gtmrspqgsn.html

[U110] JS：数组分块
来源：http://hz.52xcode.cn/gtxsyizdus.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.shzxlz.cn/gtwbcaojug.html

[U111] JS：对象转 Map
来源：http://hz.pengpengdd.cyou/gtszpjtjsr.html

new Map(Object.entries(obj))
来源：http://hz.hnqzz.top/gturvwifqe.html

[U112] JS：字符串补位
来源：http://hz.jqgfzy.top/gtmssysneu.html

"7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtswcvdmdx.html

[U113] JS：正则替换全部
来源：http://hz.nanxuanxn.top/gtjpvuurtg.html

s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtdnvvepdf.html

[U114] JS：JSON 深比较
来源：http://hz.shangyingyoupin.top/gthxhztzgc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sufxvd.cn/gttadoiewi.html

[U115] JS：生成 UUID
来源：http://hz.hnqzz.top/gthhdiqfby.html

crypto.randomUUID()
来源：http://hz.sufxvd.cn/gttwuaxanv.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cheryme.top/gthdfudjab.html

/** @param {string} name */ function f(name) {}
来源：http://hz.guannengcc.top/gttjuxdigw.html

[U117] JS：单元测试
来源：http://hz.52xcode.cn/gtmuqtxmbp.html

npm i -D vitest;  npx vitest
来源：http://hz.cqqwz.cn/gtemfjeitg.html

[U118] JS：开发服务器
来源：http://hz.tianlin.xyz/gtzwftysqh.html

npm i -D vite;  npx vite
来源：http://hz.shanyushiyangtech.top/gtrkuddzda.html

[U119] JS：生产构建
来源：http://hz.yj20258888.top/gtllsirghz.html

npx vite build
来源：http://hz.dashuyun.cn/gtsefdnfwt.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.jqgufenzy.top/gtghchbhvp.html

import.meta.env.VITE_API_URL
来源：http://hz.xziqi.cn/gtktgtoxuk.html

================================================================================
来源：http://hz.tanke756.top/gtuikbklqs.html

统计汇总
来源：http://hz.smart0.xyz/gtzphxvjjp.html

================================================================================
来源：http://hz.zhixingplan.top/gtirunsvpb.html

按语言统计（条）：
来源：http://hz.yj202588.top/gtdwuippqu.html

Python ......... 252
来源：http://hz.ehwqpu.com/gtzdjpkaoq.html

PHP ............ 252
来源：http://hz.xinyue.icu/gtggmoydaa.html

JavaScript ..... 252
来源：http://hz.zhengqikj.top/gtdwtnuern.html

TypeScript ..... 212
来源：http://hz.aizwys.cn/gtlcsanomj.html

Java ........... 212
来源：http://hz.sxryk.cn/gtjxicvbjf.html

Go ............. 212
来源：http://hz.zhijiandao.cn/gtymzolele.html

Ruby ........... 212
来源：http://hz.tianlin.xyz/gtlchxnpbb.html

C# ............. 212
来源：http://hz.yuanzhike.top/gtpbnkxahk.html

C .............. 30
来源：http://hz.xingfuxueyuan.xyz/gtiilnvowx.html

C++ ............ 30
来源：http://hz.yj202588.top/gtnzywzbhd.html

SQL ............ 90
来源：http://hz.guannengcc.top/gtljxgkvbn.html

Bash ........... 80
来源：http://hz.52xcode.cn/gtynamfadm.html

Kotlin ......... 15
来源：http://hz.shuidangran.top/gtuloyxzxm.html

Swift .......... 15
来源：http://hz.zhengqikj.top/gtwznoczpq.html

Lua ............ 10
来源：http://hz.zhoulong.xyz/gtzcwbvvvb.html

Perl ........... 10
来源：http://hz.havefunace.top/gtdpzkitkj.html

Scala .......... 10
来源：http://hz.hywenlv.cn/gtgmodotlx.html

------------------------------------
来源：http://hz.ivvv.top/gtcozvykoa.html

合计 ........... 2106 条
来源：http://hz.ydjk.org.cn/gttmndmxwx.html

按章节统计：
来源：http://hz.316326.xyz/gtivrfzeht.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.dashuyun.cn/gtlfunkzou.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nanxinkj.top/gtitqhxrgy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sxryk.cn/gthzyquzvz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sysykeji.top/gtxkfagnku.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cdnleiting.top/gtygimdohj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.havefunace.top/gtbzxxekcz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hongshengwenyu.top/gtjyhchwhh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.kuanghao11.cn/gtyifivylf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtjvnsoijt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.aizwys.cn/gtnstachgr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.haohaochexian.top/gtmrhcqpyv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtnwojszes.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtmahixjzc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yongpay.top/gtxqgejzog.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.svipenyu.cn/gtqjvhpysb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtqikteexn.html

Q SQL 专题                              90
来源：http://hz.gotoacloud.top/gtoyhtvubu.html

R Bash 专题                             80
来源：http://hz.zhiwuduotai.top/gtbzajhkyi.html

S C / C++ 专题                          60
来源：http://hz.jinqigfzy.top/gtnqvfvzhk.html

T 其他语言补充                          60
来源：http://hz.gaohongyu789.top/gtfxjoardy.html

U 高频实用片段                         120
来源：http://hz.nwbrower.top/gtftuwglnp.html

------------------------------------
来源：http://hz.shuidangran.top/gtmumgmhrc.html

合计                                  2106 条
来源：http://hz.redwolf501.top/gtngnjpkrb.html

--------------------------------------------------------------------------------
来源：http://hz.zhoulong.xyz/gtpyszxhml.html

使用提醒
来源：http://hz.shanyushiyangtech.top/gtyxuyichb.html

--------------------------------------------------------------------------------
来源：http://hz.cdnleiting.top/gtzppcnuyd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zycfv.cn/gtifopwyzd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.chenzaomai.com/gtdgvzqzro.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yj202588.top/gtarbvuttm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.tanke756.top/gtoegurxqa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.yj20258.top/gtztyjghch.html

—— 文件结束 ——
来源：http://hz.yj202588.top/gtjdbmvjeh.html

================================================================================
来源：http://hz.fengsongda.top/gthscgiemu.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.vqdsnc.cn/gtlyjyrira.html

Common Programming Examples Cheat Book
来源：http://hz.jinqigufen.top/gtkllbzbtg.html

================================================================================
来源：http://hz.chenlongwang.top/gtyiuscwfn.html

【收录内容】
来源：http://hz.yuxming.cn/gtzotzbbol.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.pengpengdd.cyou/gthjxsfglt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.9152youxi.cn/gtqtalxkkl.html

SQL · Bash · C · C++
来源：http://hz.gotoacloud.top/gtmimxqnar.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.9152youxi.cn/gtlvizgyij.html

【使用说明】
来源：http://hz.xuanzx.com/gtbzpiugmp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.chenlongwang.top/gtikcglhhv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.cheryme.top/gtlaarioqv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hnqzz.top/gttnrpqpjq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.smart0.xyz/gtdhounpmj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hfpthk.cn/gtufxiuddt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.chenzaomai.com/gtmuscvhfh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.nanxinkj.top/gthvszbppf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.sufxvd.cn/gtwyvuorpp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.nanxinkj.top/gtrddqdcrc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ydzc1.top/gtrmgzhfkd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.havefunace.top/gtjraurzsl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.yuxming.cn/gtnpfanfyf.html

【文件统计】
来源：http://hz.shanyushiyangkeji.top/gtwiuszjya.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.andypj.xyz/gtqydhiyvv.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtkmaatgwy.html

目  录
来源：http://hz.xinyue.icu/gtpyydsgva.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtwtpwwxab.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xinyue.icu/gtktmyxtmi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ivvv.top/gttjkxvliu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.xuanzx.com/gtmjlmliff.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.daxiang520.top/gtvflljqas.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.gzhubu.top/gtxcfhntiw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ivvv.top/gtnnyypyrs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jinghuilouyu.cn/gtmtuxasbt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yongpay.top/gtmxvlblbn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtawghtjyg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.c1oappe.top/gtrlgkrnbm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtwwexyoug.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.nwbrower.top/gturerbjdn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtzkuxlmsh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shanyushiyangtech.top/gtyjkmyehz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yonumen.top/gtatfahlcq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.52xcode.cn/gtzpwfoxet.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.meibo888.top/gtjisjiazc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.chenlongwang.top/gttdyzivgh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hywenlv.cn/gtlozlcxhn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.9152youxi.cn/gtaeuojjnu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuxming.cn/gtbosderlp.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtzuhrmbqh.html

A. 基础语法与类型
来源：http://hz.nwbrower.top/gtxsnyqblr.html

================================================================================
来源：http://hz.bjfxy.top/gtswhlvmlx.html

[A01] Hello World
来源：http://hz.yuanzhike.top/gtjjbmflol.html

Py:   print("Hello, World!")
来源：http://hz.xinyue.icu/gtkbwokcfv.html

PHP:  echo "Hello, World!";
来源：http://hz.gzhubu.top/gtsmteahus.html

JS:   console.log("Hello, World!");
来源：http://hz.bjfxy.top/gtmnyueifp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.svipenyu.cn/gtkpqptsum.html

Java: System.out.println("Hello, World!");
来源：http://hz.dianchejie.cn/gtjlfchkyr.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ivvv.top/gtixejjtei.html

Ruby: puts "Hello, World!"
来源：http://hz.xuanzx.com/gttdzxcgvb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ybcxt.top/gtyyatydsz.html

[A02] 变量声明与赋值
来源：http://hz.dashuyun.cn/gtrybknvhc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.quarkkingdee.top/gtgylauvdk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hnqzz.top/gtomtwcyft.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.smart0.xyz/gtyinovxta.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.redwolf501.top/gttdzdjmzz.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhiwuduotai.top/gtntwidcau.html

Go:   name := "Alex"; age := 20
来源：http://hz.gogol.net.cn/gtauzkaofd.html

Ruby: name = "Alex"; age = 20
来源：http://hz.quarkkingdee.top/gtqnvoqqcb.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.pengpengdd.cyou/gtzyjdbyvu.html

[A03] 常量定义
来源：http://hz.zhoulong.xyz/gtcuxfgmga.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhoulong.xyz/gtihxwjvbv.html

PHP:  const PI = 3.14159;
来源：http://hz.hfpthk.cn/gtvetlmbjn.html

JS:   const PI = 3.14159;
来源：http://hz.ppjwa.cn/gtvmcybwut.html

TS:   const PI: number = 3.14159;
来源：http://hz.pycfn.com/gtjskwuwlr.html

Java: static final double PI = 3.14159;
来源：http://hz.tianlin.xyz/gtgllrwbbe.html

Go:   const PI = 3.14159
来源：http://hz.shanyushiyangkeji.top/gtyqqfvqgg.html

Ruby: PI = 3.14159
来源：http://hz.jinghuilouyu.cn/gtndvwqifa.html

C#:   const double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtuwycejhy.html

[A04] 判断变量类型
来源：http://hz.shangyingyoupin.top/gtpdsbzyla.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.dianchejie.cn/gtcxwbzzit.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.snrcjt.cn/gtwvmwghnb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.chenlongwang.top/gtjramqtgm.html

TS:   typeof x; x instanceof Date
来源：http://hz.jinyuanbaomall.cn/gtzrhusdsi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ybcxt.top/gtmmksrprc.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yonumen.top/gtigqortls.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sxryk.cn/gtrdwnnzwr.html

C#:   x.GetType().Name; x is int
来源：http://hz.hongshengwenyu.top/gtkzguuzph.html

[A05] 整数除法与取模
来源：http://hz.ydzc1.top/gtzlxmjdmn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.quarkkingdee.top/gtmxlowerh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.aizwys.cn/gtrqrpgesg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.svipenyu.cn/gtqxuvezui.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.daxiang520.top/gtjdxktyml.html

Java: 7 / 2; 7 % 2
来源：http://hz.ydzc1.top/gtllxnepdx.html

Go:   7 / 2; 7 % 2
来源：http://hz.andypj.xyz/gtkjijxumj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.redwolf501.top/gtqdajphqp.html

C#:   7 / 2; 7 % 2
来源：http://hz.iojbl.cn/gtuqhbnmxe.html

[A06] 字符串转数字
来源：http://hz.cheryme.top/gtaaflaamk.html

Py:   int("42"); float("3.14")
来源：http://hz.sysykeji.top/gttuklwqsh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.yj202588.top/gtjzxfnvkf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.smart0.xyz/gtefktcpwx.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.tianlin.xyz/gtbmoxxebw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yuxming.cn/gtoozuqadh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.pengpengdd.cyou/gtzkssdtmc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.316326.xyz/gtfdfpmzup.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yuxming.cn/gtokbnrcky.html

[A07] 数字转字符串
来源：http://hz.jianghu66.top/gtnihkxdzh.html

Py:   str(42)
来源：http://hz.dianchejie.cn/gtcskseuti.html

PHP:  (string) 42; strval(42)
来源：http://hz.nanxinkj.top/gtvreeushu.html

JS:   String(42); (42).toString()
来源：http://hz.yj20258888.top/gtqyleuniw.html

TS:   String(42)
来源：http://hz.hammf.cn/gtlyyjvbwb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.0kj1m.cn/gtegjxauii.html

Go:   strconv.Itoa(42)
来源：http://hz.cdnleiting.top/gtietkzzao.html

Ruby: 42.to_s
来源：http://hz.ywan-chungtsiang.top/gtscaekqrd.html

C#:   42.ToString()
来源：http://hz.zycfv.cn/gtishiypun.html

[A08] 取整与四舍五入
来源：http://hz.hnxiangtu.top/gteixzbnro.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xuetiantiany.cn/gtxdahdusj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.gaohongyu789.top/gtzhibsdnd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hnxiangtu.top/gtsroguyga.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jinghuilouyu.cn/gtsodzhmiy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.jinqigufen.top/gtwvvsijns.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.c1oappe.top/gtjhtnggjj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.daxiang520.top/gtzkdiuiwv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.shzxlz.cn/gtoebbmraa.html

[A09] 绝对值与最大最小值
来源：http://hz.ydzc1.top/gtmojnmuso.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.daxiang520.top/gtygsqkhcw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cheryme.top/gtbxhosuxu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hnqzz.top/gtqvjcixqr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.tian-w.cn/gtzldercdr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hongshengwenyu.top/gtzhiqgtqo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zycfv.cn/gtsyeirfvl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.fzhhl.top/gtxuwaurcq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.pengpengdd.cyou/gtkptsfsaq.html

[A10] 生成随机数
来源：http://hz.jqgfzy.top/gtkkllfmqh.html

Py:   import random; random.randint(1, 100)
来源：http://hz.xingfuxueyuan.xyz/gtufgvybmg.html

PHP:  random_int(1, 100);
来源：http://hz.yj20258888.top/gtygjhdpad.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jianghu66.top/gtdpgejgky.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.nanxuanxn.top/gtlbfvcqvk.html

Java: new Random().nextInt(100) + 1
来源：http://hz.ehwqpu.com/gtwdcpuokr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.tianlin.xyz/gtmyusfmzg.html

Ruby: rand(1..100)
来源：http://hz.nwbrower.top/gtpxlwacsi.html

C#:   new Random().Next(1, 101)
来源：http://hz.yj20258.top/gtbdwbfffh.html

[A11] 条件表达式（三元）
来源：http://hz.dashuyun.cn/gtufklmutf.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jianghu66.top/gtqtsyrfpc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.xingfuxueyuan.xyz/gtncemgyhp.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.pengpengdd.cyou/gtcqsqjxfq.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.xylfe.cn/gtizqlfsaq.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.zycfv.cn/gtrgtvhhrw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.ybcxt.top/gtzlolisfo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.cashguo.top/gttwjhyesk.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.daxiang520.top/gtlgjiobns.html

[A12] 字符串插值 / 格式化
来源：http://hz.jiagoushi.top/gtvuauvpad.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jqgufenzy.top/gtagjezdoi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhixingplan.top/gtmsyewtwy.html

JS:   `Hello, ${name}!`
来源：http://hz.shanyushiyangkeji.top/gttofexjgw.html

TS:   `Hello, ${name}!`
来源：http://hz.9152youxi.cn/gtmqrglqpe.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.shanyushiyangkeji.top/gtycwkpvmv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.nanxuanxn.top/gtkifcnszv.html

Ruby: "Hello, #{name}!"
来源：http://hz.gotoacloud.top/gtsgajpamy.html

C#:   $"Hello, {name}!"
来源：http://hz.jinyuanbaomall.cn/gtcdcpbhew.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.316326.xyz/gtebblixrg.html

Py:   "第一行\n第二行"
来源：http://hz.yangfankeji.com/gtwytkvciw.html

PHP:  "第一行\n第二行"
来源：http://hz.xylfe.cn/gtmuvzbcar.html

JS:   "第一行\n第二行"
来源：http://hz.haohaochexian.top/gtaowcfncj.html

TS:   "第一行\n第二行"
来源：http://hz.ywan-chungtsiang.top/gtvvskadlm.html

Java: "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtegorwbfz.html

Go:   "第一行\n第二行"
来源：http://hz.yj202588.top/gtszuxtvll.html

Ruby: "第一行\n第二行"
来源：http://hz.wangdashe.top/gtqtvyxxwy.html

C#:   "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtjdujaliq.html

[A14] 注释写法
来源：http://hz.smart0.xyz/gtqpirnmjv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.sweek.top/gtjtxforrk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.snrcjt.cn/gtrcekumsw.html

JS:   // 单行；/* 多行 */
来源：http://hz.guannengcc.top/gtdwnmimwy.html

TS:   // 单行；/* 多行 */
来源：http://hz.xylfe.cn/gtpylbpibd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhongyouzk.top/gtqltvwwoj.html

Go:   // 单行；/* 多行 */
来源：http://hz.cashguo.top/gtzgcohpie.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.ehwqpu.com/gthdeexhcd.html

C#:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangkeji.top/gtbwznsafe.html

[A15] 空值判断与默认值
来源：http://hz.fengsongda.top/gtkmdgdbei.html

Py:   value = data or "默认值"
来源：http://hz.feifeiyinyue.top/gtjxcvqckc.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.dianchejie.cn/gtxvolulvl.html

JS:   const value = data ?? "默认值";
来源：http://hz.fzhhl.top/gtcmiukbso.html

TS:   const value = data ?? "默认值";
来源：http://hz.cashguo.top/gtabdqmuiz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.ehwqpu.com/gtqjteezsi.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.hysaishi.cn/gtgkpjnirf.html


<!-- 参考信息 -->