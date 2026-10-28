代发 wailian999

[U93] JS：模板字符串
来源：http://hz.aibaodan.cn/gtpckxtkjo.html

`共 ${n} 条`
来源：http://hz.sysykeji.top/gtiuyulhtf.html

[U94] JS：箭头函数
来源：http://hz.aibaodan.cn/gtnieovpiz.html

const double = x => x * 2;
来源：http://hz.pycfn.com/gtqihvinld.html

[U95] JS：Promise 包装
来源：http://hz.svipenyu.cn/gthupwjung.html

new Promise((resolve, reject) => {})
来源：http://hz.chenlongwang.top/gtduggzmgt.html

[U96] JS：async/await 与异常
来源：http://hz.zhaomingkeji.xyz/gtmnofyisn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtgocjmzxs.html

[U97] JS：并发请求
来源：http://hz.guowangkeji.top/gtqrtbvpru.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sweek.top/gtgzizncjo.html

[U98] JS：fetch 带 JSON
来源：http://hz.quarkkingdee.top/gtzndveeqw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.redwolf501.top/gtsanyolvv.html

[U99] JS：事件监听
来源：http://hz.9152youxi.cn/gtizhojowh.html

el.addEventListener("click", e => {})
来源：http://hz.ybcxt.top/gtuqusppxe.html

[U100] JS：DOM 查询
来源：http://hz.cheryme.top/gtxqhessph.html

document.querySelector(".item")
来源：http://hz.gaohongyu789.top/gtozlxxoec.html

[U101] JS：classList 操作
来源：http://hz.meibo888.top/gtkoajtbjf.html

el.classList.toggle("active")
来源：http://hz.dashuyun.cn/gtaxmwomiw.html

[U102] JS：本地存储
来源：http://hz.wangdashe.top/gtbgxstcwj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ydzc1.top/gtprjpnqlk.html

[U103] JS：定时器
来源：http://hz.tianlin.xyz/gtdwvoxevr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.52xcode.cn/gtcieigmre.html

[U104] JS：防抖
来源：http://hz.jinqigufen.top/gtsxxxuozi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.svipenyu.cn/gtwmewqwbs.html

[U105] JS：节流
来源：http://hz.fzhhl.top/gttcspfzxj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.nanxinkj.top/gtpvotsdly.html

[U106] JS：日期格式化
来源：http://hz.zhixingplan.top/gtmkcbpfkl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hongshengwenyu.top/gtihhziujr.html

[U107] JS：数字千分位
来源：http://hz.gogol.net.cn/gtzpvzdbvd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hnxiangtu.top/gtoudkyfov.html

[U108] JS：随机整数
来源：http://hz.zhaomingkeji.xyz/gttoathzbi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.gzhubu.top/gtafwgpfgh.html

[U109] JS：数组分组
来源：http://hz.52xcode.cn/gtjjwtyyar.html

Object.groupBy(arr, x => x.type)
来源：http://hz.9152youxi.cn/gtekeylssl.html

[U110] JS：数组分块
来源：http://hz.ydzc1.top/gtpbjtzicb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hnxiangtu.top/gtkmuetsuu.html

[U111] JS：对象转 Map
来源：http://hz.zhengqikj.top/gttrazftui.html

new Map(Object.entries(obj))
来源：http://hz.mhx1999.top/gtpjrlhzgb.html

[U112] JS：字符串补位
来源：http://hz.svipenyu.cn/gtzbokccyq.html

"7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtzqbxumjk.html

[U113] JS：正则替换全部
来源：http://hz.jyoumei.cn/gtwucljngf.html

s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtjjxaerad.html

[U114] JS：JSON 深比较
来源：http://hz.pycfn.com/gtkjyynkhw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangshuangyany.cn/gtwlwtjiqh.html

[U115] JS：生成 UUID
来源：http://hz.316326.xyz/gtpakrdyue.html

crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtikvfhxsr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.smart0.xyz/gtnjicjqql.html

/** @param {string} name */ function f(name) {}
来源：http://hz.316326.xyz/gtxarxwkbh.html

[U117] JS：单元测试
来源：http://hz.zhengqikj.top/gtqmrhntjk.html

npm i -D vitest;  npx vitest
来源：http://hz.kuanghao11.cn/gtdmpdtebf.html

[U118] JS：开发服务器
来源：http://hz.xuetiantiany.cn/gtrkvdnxoz.html

npm i -D vite;  npx vite
来源：http://hz.daria6918.cn/gtbwwsvnga.html

[U119] JS：生产构建
来源：http://hz.jinghuilouyu.cn/gtssiwycpl.html

npx vite build
来源：http://hz.haohaochexian.top/gtdeeuoshp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.0kj1m.cn/gtbuxebmto.html

import.meta.env.VITE_API_URL
来源：http://hz.cucudq.cn/gtwvwfnnjt.html

================================================================================
来源：http://hz.316326.xyz/gtfgrkgtxw.html

统计汇总
来源：http://hz.jinqigufen.top/gtlporsrad.html

================================================================================
来源：http://hz.dashuyun.cn/gtkannoett.html

按语言统计（条）：
来源：http://hz.52xcode.cn/gtvrhbnhau.html

Python ......... 252
来源：http://hz.nanxuanxn.top/gtytaopcrq.html

PHP ............ 252
来源：http://hz.vqdsnc.cn/gtfevwmfnv.html

JavaScript ..... 252
来源：http://hz.jqgufenzy.top/gtaibkaixc.html

TypeScript ..... 212
来源：http://hz.iojbl.cn/gtapwwiqcc.html

Java ........... 212
来源：http://hz.dianchejie.cn/gtjuvqywaq.html

Go ............. 212
来源：http://hz.gzhubu.top/gtqxamtzel.html

Ruby ........... 212
来源：http://hz.guannengcc.top/gtigvqysqw.html

C# ............. 212
来源：http://hz.yanxiufei.cn/gtzktorksc.html

C .............. 30
来源：http://hz.zhaomingkeji.xyz/gtqlvesoha.html

C++ ............ 30
来源：http://hz.zhaomingkeji.xyz/gtfkglstlt.html

SQL ............ 90
来源：http://hz.meibo888.top/gtzfxtxwtr.html

Bash ........... 80
来源：http://hz.pengpengdd.cyou/gtjkbkqbjp.html

Kotlin ......... 15
来源：http://hz.yueranfly.top/gtsdjmlaeo.html

Swift .......... 15
来源：http://hz.bjfxy.top/gtuhmkzqnr.html

Lua ............ 10
来源：http://hz.zhijiandao.cn/gtlnwkmcbv.html

Perl ........... 10
来源：http://hz.yj202588.top/gtktwlvmss.html

Scala .......... 10
来源：http://hz.ydjk.org.cn/gtogxhwwwg.html

------------------------------------
来源：http://hz.birdmap.top/gtbmtmwaoi.html

合计 ........... 2106 条
来源：http://hz.xinyue.icu/gtqyxmfjjm.html

按章节统计：
来源：http://hz.chenzaomai.com/gtrizcthed.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yueranfly.top/gtetapchut.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hongshengwenyu.top/gtfcpliphm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gtuebjcimf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jyoumei.cn/gtcoqbeuap.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hywenlv.cn/gtfrkrrtcm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.jiagoushi.top/gtbqdespts.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jqgfzy.top/gtssknfbev.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.tianlin.xyz/gthhwzjgvq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hongshengwenyu.top/gtsactrkeg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.havefunace.top/gtvthuvpfc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.feifeiyinyue.top/gtnyrhuqar.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtsjxfhkml.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtozrkkcpv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jinghuilouyu.cn/gtnhyebttk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jianghu66.top/gtwwazulyf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtdifpwbzu.html

Q SQL 专题                              90
来源：http://hz.sweek.top/gtcbxgrozi.html

R Bash 专题                             80
来源：http://hz.feifeiyinyue.top/gtruwmoetb.html

S C / C++ 专题                          60
来源：http://hz.quarkkingdee.top/gtkaqrunpz.html

T 其他语言补充                          60
来源：http://hz.gogol.net.cn/gtftyljlxs.html

U 高频实用片段                         120
来源：http://hz.jinghuilouyu.cn/gtqlvkbrcy.html

------------------------------------
来源：http://hz.zhiwuduotai.top/gtpbntsdrg.html

合计                                  2106 条
来源：http://hz.jinqigufen.top/gtlbmipgog.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtcuquxqnv.html

使用提醒
来源：http://hz.mhx1999.top/gtbuylsabt.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtcduvkhsc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.fzhhl.top/gtnazlwzpg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.cucudq.cn/gtoxcvnupq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.vqdsnc.cn/gtnmvsliws.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.ydjk.org.cn/gtrkrxwrhe.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.birdmap.top/gtjpqzotrz.html

—— 文件结束 ——
来源：http://hz.aibaodan.cn/gtgcbimhtw.html

================================================================================
来源：http://hz.chenzaomai.com/gtjfqeovcp.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ydzc1.top/gthekaqsoz.html

Common Programming Examples Cheat Book
来源：http://hz.hysaishi.cn/gtvulkctsr.html

================================================================================
来源：http://hz.aibaodan.cn/gtnzljnsbb.html

【收录内容】
来源：http://hz.vqdsnc.cn/gtdfleyoqf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.dashuyun.cn/gtfxrowrfc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.aibaodan.cn/gtjpmabxsf.html

SQL · Bash · C · C++
来源：http://hz.hysaishi.cn/gtdbgvazaw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.316326.xyz/gtympftkkg.html

【使用说明】
来源：http://hz.bjfxy.top/gtoxgpiqhf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.wangdashe.top/gtnssqsqjm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.ydjk.org.cn/gtfylczgar.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.shuidangran.top/gtpxjwzbyl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenjidiqi.icu/gtyqscfjyb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.0kj1m.cn/gtvstpexhn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yj202588.top/gtexfpeoda.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.snrcjt.cn/gthcvyadne.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.pengpengdd.cyou/gtgmnghzuu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.wangshuangyany.cn/gtqkupmdmo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.pycfn.com/gtnezddsgk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.feifeiyinyue.top/gtadylcjer.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.nwbrower.top/gthzioxldm.html

【文件统计】
来源：http://hz.zhixingplan.top/gtgjqvajwo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.meibo888.top/gtzhuhiibi.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtolzedbim.html

目  录
来源：http://hz.zhaomingkeji.xyz/gtuoqizrag.html

--------------------------------------------------------------------------------
来源：http://hz.ivvv.top/gtnqvzetaq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.redwolf501.top/gtrqalftzu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.daria6918.cn/gtbnfuaaxz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zycfv.cn/gtdfribttr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.xuanzx.com/gtznazbgca.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.havefunace.top/gtwszwedli.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.feifeiyinyue.top/gtzfqhrote.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xylfe.cn/gttvdqtsib.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.vqdsnc.cn/gtqqyrpgvh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shanyushiyangtech.top/gtpefafqga.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.dianchejie.cn/gtgdnnolwm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtcakfdmbm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gtsmqesvrc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.gotoacloud.top/gthdivsitr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.shanyushiyangkeji.top/gtmfjhjqnu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhaomingkeji.xyz/gtqugpaafd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtdlfnvgvn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhengqikj.top/gtctmrmzzb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.ydjk.org.cn/gtcmkbfzyi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.sxryk.cn/gtdtruxbpv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gtpckgycub.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.xylfe.cn/gtmcfgvojg.html

================================================================================
来源：http://hz.jyoumei.cn/gtsghpbfxk.html

A. 基础语法与类型
来源：http://hz.jinqigfzy.top/gthwuyitww.html

================================================================================
来源：http://hz.sweek.top/gtknopzgtg.html

[A01] Hello World
来源：http://hz.bjfxy.top/gtkaudgzrp.html

Py:   print("Hello, World!")
来源：http://hz.yangfankeji.com/gtkqygcztb.html

PHP:  echo "Hello, World!";
来源：http://hz.yuanzhike.top/gtmeelsjhg.html

JS:   console.log("Hello, World!");
来源：http://hz.hysaishi.cn/gtyvyciizw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhengqikj.top/gtbsshvfra.html

Java: System.out.println("Hello, World!");
来源：http://hz.zhijiandao.cn/gtuudpyjyd.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zhengqikj.top/gtprzxkbjg.html

Ruby: puts "Hello, World!"
来源：http://hz.svipenyu.cn/gtcufieaif.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.guowangkeji.top/gtqexyvfgc.html

[A02] 变量声明与赋值
来源：http://hz.xinyue.icu/gtzcskkqma.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zycfv.cn/gtuchmcbru.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.nwbrower.top/gtxprmfekw.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.52xcode.cn/gtzgtdkazz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jqgfzy.top/gtywbsabus.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.dashuyun.cn/gtbnozphjs.html

Go:   name := "Alex"; age := 20
来源：http://hz.shangyingyoupin.top/gtoqemgmei.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ehwqpu.com/gtkllmlhwe.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zycfv.cn/gtmbgrcdwn.html

[A03] 常量定义
来源：http://hz.yuxming.cn/gtxovqqqqd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhijiandao.cn/gtoswqtjjb.html

PHP:  const PI = 3.14159;
来源：http://hz.dashuyun.cn/gtoaiwooio.html

JS:   const PI = 3.14159;
来源：http://hz.daria6918.cn/gtraasdrpb.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhoulong.xyz/gtsjtthpqq.html

Java: static final double PI = 3.14159;
来源：http://hz.zhengqikj.top/gtxkhmtgga.html

Go:   const PI = 3.14159
来源：http://hz.zhixingplan.top/gtpvafenib.html

Ruby: PI = 3.14159
来源：http://hz.hfpthk.cn/gtsjtjxyta.html

C#:   const double PI = 3.14159;
来源：http://hz.xinyue.icu/gtholnjfxx.html

[A04] 判断变量类型
来源：http://hz.tianlin.xyz/gtaiiesqpv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yuanzhike.top/gtoymgsjkg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ybcxt.top/gtxefrjdin.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yangfankeji.com/gtofdpylwa.html

TS:   typeof x; x instanceof Date
来源：http://hz.fzhhl.top/gtycbetzcl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.hnqzz.top/gtdnltzbsg.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yj202588.top/gtxtsynztz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gogol.net.cn/gtpsvqocqu.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhijiandao.cn/gtnjbsvwio.html

[A05] 整数除法与取模
来源：http://hz.haohaochexian.top/gtufslvjah.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.cashguo.top/gtjdtihcao.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.ydjk.org.cn/gtbfrugyeo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xuanzx.com/gtkldadjkc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtcpqxycua.html

Java: 7 / 2; 7 % 2
来源：http://hz.zycfv.cn/gtywpumbhi.html

Go:   7 / 2; 7 % 2
来源：http://hz.chenlongwang.top/gtnftaqlga.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.xinyue.icu/gtotdgqsdx.html

C#:   7 / 2; 7 % 2
来源：http://hz.nwbrower.top/gtvzzygyzv.html

[A06] 字符串转数字
来源：http://hz.shzxlz.cn/gtsigcelbp.html

Py:   int("42"); float("3.14")
来源：http://hz.jinqigfzy.top/gtcpainupl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jianghu66.top/gthmxmujfj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jiagoushi.top/gtphyhqmwi.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.redwolf501.top/gtkqsylnnx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.nanxinkj.top/gtwidbpkeg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.quarkkingdee.top/gtnzxfshsi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.shangyingyoupin.top/gtfejeljwa.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.redwolf501.top/gtstmofpnb.html

[A07] 数字转字符串
来源：http://hz.birdmap.top/gtbyozswwl.html

Py:   str(42)
来源：http://hz.yj20258888.top/gtiurvflno.html

PHP:  (string) 42; strval(42)
来源：http://hz.yueranfly.top/gtjopkqpwq.html

JS:   String(42); (42).toString()
来源：http://hz.zdqjudy.top/gtsohrephv.html

TS:   String(42)
来源：http://hz.havefunace.top/gthxvaagwe.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.gotoacloud.top/gthxcqdkee.html

Go:   strconv.Itoa(42)
来源：http://hz.gogol.net.cn/gtikicnkzf.html

Ruby: 42.to_s
来源：http://hz.gaohongyu789.top/gtshriwjrz.html

C#:   42.ToString()
来源：http://hz.hywenlv.cn/gtemgazovl.html

[A08] 取整与四舍五入
来源：http://hz.cqqwz.cn/gtmmanbxgj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.nanxinkj.top/gtufbxtjlo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.haohaochexian.top/gtwtzakhgg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jinqigfzy.top/gtdzrccbdl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.xylfe.cn/gtuzczwivl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.pycfn.com/gtyxrxxzcw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.tanke756.top/gtfcviqykv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.cheryme.top/gtclgcgdke.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.gzhubu.top/gtchponxeu.html

[A09] 绝对值与最大最小值
来源：http://hz.vqdsnc.cn/gttphnuzya.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ydjk.org.cn/gtraxgxiwd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.dashuyun.cn/gtogqdjthn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.zycfv.cn/gtagvfuyrz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.nwbrower.top/gtatqbsdhm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.chenlongwang.top/gthxfusyqn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.tanke756.top/gtdgawqbyn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.jinqigfzy.top/gtmphjjtqm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yvedp.cn/gtiighvmnk.html

[A10] 生成随机数
来源：http://hz.guannengcc.top/gtlmuwvzkx.html

Py:   import random; random.randint(1, 100)
来源：http://hz.guannengcc.top/gtvdmbkxif.html

PHP:  random_int(1, 100);
来源：http://hz.kuanghao11.cn/gtzuxxvcim.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zdqjudy.top/gtsisximxa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hywenlv.cn/gtfkmaghpm.html

Java: new Random().nextInt(100) + 1
来源：http://hz.guowangkeji.top/gttpaqyrmf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.vqdsnc.cn/gtkblsnsez.html

Ruby: rand(1..100)
来源：http://hz.havefunace.top/gtejroxuka.html

C#:   new Random().Next(1, 101)
来源：http://hz.yueranfly.top/gtjpaptioj.html

[A11] 条件表达式（三元）
来源：http://hz.wangdashe.top/gtzcurmokb.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.ivvv.top/gtbtfnowwq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.quarkkingdee.top/gtrzkfvqpx.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jinghuilouyu.cn/gtpencbavt.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zhiwuduotai.top/gtdoefiqti.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.bjfxy.top/gtbdltbdqe.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.iojbl.cn/gtxwfjzhhi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.zhengqikj.top/gtiydpdwqb.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gtjgpdaywe.html

[A12] 字符串插值 / 格式化
来源：http://hz.zhijiandao.cn/gthdqbtgyv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.hfpthk.cn/gtgtrpewyg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.hammf.cn/gtvypanqmt.html

JS:   `Hello, ${name}!`
来源：http://hz.quarkkingdee.top/gtbjoyrloo.html

TS:   `Hello, ${name}!`
来源：http://hz.gzhubu.top/gtveteqiik.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zhongyouzk.top/gtusfktxdp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.mhx1999.top/gtaerryzkz.html

Ruby: "Hello, #{name}!"
来源：http://hz.zhixingplan.top/gttyqjuvau.html

C#:   $"Hello, {name}!"
来源：http://hz.jqgufenzy.top/gteaowfbhi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.hywenlv.cn/gtgahwfmzk.html

Py:   "第一行\n第二行"
来源：http://hz.kuanghao11.cn/gtyynrngvi.html

PHP:  "第一行\n第二行"
来源：http://hz.guannengcc.top/gtvksanaqc.html

JS:   "第一行\n第二行"
来源：http://hz.tianlin.xyz/gtwrkefhiy.html

TS:   "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtxshuypyd.html

Java: "第一行\n第二行"
来源：http://hz.xziqi.cn/gtowkrzlmw.html

Go:   "第一行\n第二行"
来源：http://hz.ywan-chungtsiang.top/gtfngvcwwm.html

Ruby: "第一行\n第二行"
来源：http://hz.sxryk.cn/gtbalivqut.html

C#:   "第一行\n第二行"
来源：http://hz.0kj1m.cn/gtuiyhgdtq.html

[A14] 注释写法
来源：http://hz.haohaochexian.top/gtoddljhwr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.ybcxt.top/gtgamilkmt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.zycfv.cn/gtjmwrhfhw.html

JS:   // 单行；/* 多行 */
来源：http://hz.svipenyu.cn/gtxvxmgoay.html

TS:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangkeji.top/gtexaleeym.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhiwuduotai.top/gtdvonzngw.html

Go:   // 单行；/* 多行 */
来源：http://hz.c1oappe.top/gtbjflzhqt.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.yj202588.top/gtogyjdplq.html

C#:   // 单行；/* 多行 */
来源：http://hz.ppjwa.cn/gtgzstmtuq.html

[A15] 空值判断与默认值
来源：http://hz.hywenlv.cn/gtjpxtzfbf.html

Py:   value = data or "默认值"
来源：http://hz.nanxinkj.top/gtyyqduxbg.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zhaomingkeji.xyz/gtuixkgsib.html

JS:   const value = data ?? "默认值";
来源：http://hz.haohaochexian.top/gtyisyfvvx.html

TS:   const value = data ?? "默认值";
来源：http://hz.jinqigufen.top/gtvitjqjiq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.wangdashe.top/gtpvmsdxwz.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.cashguo.top/gtyfyectfq.html

Ruby: value = data || "默认值"
来源：http://hz.ehwqpu.com/gtzyjswfzh.html

C#:   var value = data ?? "默认值";
来源：http://hz.yvedp.cn/gtbtiaxvtl.html

[A16] 真假值判断规则
来源：http://hz.havefunace.top/gtgbrbynmw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.fzhhl.top/gtiskmoyrz.html


<!-- 参考信息 -->