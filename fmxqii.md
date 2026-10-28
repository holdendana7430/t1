代发 wailian999

[U91] JS：对象键值遍历
来源：http://hz.hnxiangtu.top/gtctxphbcr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.sufxvd.cn/gtcmranpcj.html

[U92] JS：深拷贝
来源：http://hz.ehwqpu.com/gtbvfepkgm.html

structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtbprsyxax.html

[U93] JS：模板字符串
来源：http://hz.smart0.xyz/gtuvapmkqb.html

`共 ${n} 条`
来源：http://hz.316326.xyz/gtzuoffnnx.html

[U94] JS：箭头函数
来源：http://hz.cqqwz.cn/gtjopqlxtm.html

const double = x => x * 2;
来源：http://hz.ywan-chungtsiang.top/gtabzbephv.html

[U95] JS：Promise 包装
来源：http://hz.feifeiyinyue.top/gtuodfkebd.html

new Promise((resolve, reject) => {})
来源：http://hz.pycfn.com/gtgbzowswk.html

[U96] JS：async/await 与异常
来源：http://hz.fengsongda.top/gtlhvxvsxu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.shzxlz.cn/gtkjrkzgon.html

[U97] JS：并发请求
来源：http://hz.shanyushiyangkeji.top/gtlqrizgzm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtebssbcin.html

[U98] JS：fetch 带 JSON
来源：http://hz.tanke756.top/gtusiirqow.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.xuetiantiany.cn/gtukkisitx.html

[U99] JS：事件监听
来源：http://hz.ivvv.top/gtvwelkoxz.html

el.addEventListener("click", e => {})
来源：http://hz.ydzc1.top/gtibabvvkw.html

[U100] JS：DOM 查询
来源：http://hz.nanxuanxn.top/gtswfexfch.html

document.querySelector(".item")
来源：http://hz.daxiang520.top/gtbpfyxuer.html

[U101] JS：classList 操作
来源：http://hz.tianlin.xyz/gtfzcooiiw.html

el.classList.toggle("active")
来源：http://hz.hammf.cn/gtmieeeytv.html

[U102] JS：本地存储
来源：http://hz.wangdashe.top/gtpshrobwy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shangyingyoupin.top/gtoepgndsy.html

[U103] JS：定时器
来源：http://hz.jqgfzy.top/gtprzstdch.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.c1oappe.top/gtjkhsqlwm.html

[U104] JS：防抖
来源：http://hz.gogol.net.cn/gtdyxzgpyx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gtbchjedqp.html

[U105] JS：节流
来源：http://hz.cqqwz.cn/gtplotvcfo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenlongwang.top/gttwzretge.html

[U106] JS：日期格式化
来源：http://hz.andypj.xyz/gtmjekvfnd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jiagoushi.top/gtwsahfeki.html

[U107] JS：数字千分位
来源：http://hz.daxiang520.top/gtkvylppsr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.haohaochexian.top/gtqgunqqha.html

[U108] JS：随机整数
来源：http://hz.zycfv.cn/gtvpkrwrcz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shangyingyoupin.top/gtbmrfnhfh.html

[U109] JS：数组分组
来源：http://hz.smart0.xyz/gtkypcvdew.html

Object.groupBy(arr, x => x.type)
来源：http://hz.wangdashe.top/gtkhwenctu.html

[U110] JS：数组分块
来源：http://hz.dianchejie.cn/gtasoquppd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.iojbl.cn/gtgbomfqws.html

[U111] JS：对象转 Map
来源：http://hz.snrcjt.cn/gtnqtznvdj.html

new Map(Object.entries(obj))
来源：http://hz.xziqi.cn/gtvigafbsd.html

[U112] JS：字符串补位
来源：http://hz.feifeiyinyue.top/gtkgtiloyu.html

"7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtodmhrmsv.html

[U113] JS：正则替换全部
来源：http://hz.haohaochexian.top/gtufcxnwxo.html

s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gtxdpzxars.html

[U114] JS：JSON 深比较
来源：http://hz.ivvv.top/gtjyuvgato.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yonumen.top/gtcdeblldi.html

[U115] JS：生成 UUID
来源：http://hz.hnxiangtu.top/gtrvdydapb.html

crypto.randomUUID()
来源：http://hz.ybcxt.top/gteqtdqjap.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.kuanghao11.cn/gtnezcujsd.html

/** @param {string} name */ function f(name) {}
来源：http://hz.snrcjt.cn/gtjzdwoqdv.html

[U117] JS：单元测试
来源：http://hz.sufxvd.cn/gtmrwtnyym.html

npm i -D vitest;  npx vitest
来源：http://hz.xuetiantiany.cn/gtijdaajvy.html

[U118] JS：开发服务器
来源：http://hz.sysykeji.top/gtvuqscerv.html

npm i -D vite;  npx vite
来源：http://hz.nanxinkj.top/gtlwzbbybi.html

[U119] JS：生产构建
来源：http://hz.shuidangran.top/gtmvtavmqb.html

npx vite build
来源：http://hz.yanxiufei.cn/gtsxjegtaw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.smart0.xyz/gtteelhsar.html

import.meta.env.VITE_API_URL
来源：http://hz.wangshuangyany.cn/gttfmxfslt.html

================================================================================
来源：http://hz.hfpthk.cn/gtuexxruui.html

统计汇总
来源：http://hz.zdqjudy.top/gtqszcaife.html

================================================================================
来源：http://hz.meibo888.top/gtjdbxftmg.html

按语言统计（条）：
来源：http://hz.9152youxi.cn/gtqwipdglx.html

Python ......... 252
来源：http://hz.xinyue.icu/gtqabnftnd.html

PHP ............ 252
来源：http://hz.jinghuilouyu.cn/gtnpqqrkgl.html

JavaScript ..... 252
来源：http://hz.chenlongwang.top/gtsmvluswc.html

TypeScript ..... 212
来源：http://hz.birdmap.top/gtguxmevoh.html

Java ........... 212
来源：http://hz.gogol.net.cn/gtsrwncygd.html

Go ............. 212
来源：http://hz.ybcxt.top/gtfokrmbtw.html

Ruby ........... 212
来源：http://hz.smart0.xyz/gtewqmvpmq.html

C# ............. 212
来源：http://hz.hammf.cn/gtlmkuyozv.html

C .............. 30
来源：http://hz.ydzc1.top/gtlkhmuill.html

C++ ............ 30
来源：http://hz.daxiang520.top/gtufxdebot.html

SQL ............ 90
来源：http://hz.daxiang520.top/gtpgcxzhah.html

Bash ........... 80
来源：http://hz.cdnleiting.top/gtqstefyff.html

Kotlin ......... 15
来源：http://hz.ivvv.top/gtzxlflnfb.html

Swift .......... 15
来源：http://hz.meibo888.top/gtolkceipg.html

Lua ............ 10
来源：http://hz.jinqigufen.top/gtuzdfgsll.html

Perl ........... 10
来源：http://hz.gzhubu.top/gtdmtazmxs.html

Scala .......... 10
来源：http://hz.yj20258.top/gtgugqlyka.html

------------------------------------
来源：http://hz.guannengcc.top/gtqpossugm.html

合计 ........... 2106 条
来源：http://hz.zhixingplan.top/gtuhmvbsmj.html

按章节统计：
来源：http://hz.fzhhl.top/gtqjkyxkxo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhoulong.xyz/gtpnewrgqo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.nwbrower.top/gtmrvzbuxm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.wangshuangyany.cn/gtvkruveey.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.kuanghao11.cn/gtjhrwscki.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhongyouzk.top/gtwvoxhxmn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.zhixingplan.top/gtcfidncgz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jianghu66.top/gtpuxczsoi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.9152youxi.cn/gtkapgpbbt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtnxbkiaoi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.tian-w.cn/gtuosvgmck.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hongshengwenyu.top/gtxjwezvax.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtxjldklrs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtlzvvckis.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shuidangran.top/gtaezgqlgj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yvedp.cn/gtwgylzzmu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtcrrfilcl.html

Q SQL 专题                              90
来源：http://hz.c1oappe.top/gtcahtasbc.html

R Bash 专题                             80
来源：http://hz.daxiang520.top/gtdgcytegl.html

S C / C++ 专题                          60
来源：http://hz.yj202588.top/gtfxchsgns.html

T 其他语言补充                          60
来源：http://hz.pycfn.com/gtkjhlrjjo.html

U 高频实用片段                         120
来源：http://hz.zdqjudy.top/gtrmblmbbm.html

------------------------------------
来源：http://hz.sxryk.cn/gtxlmewauu.html

合计                                  2106 条
来源：http://hz.birdmap.top/gtcrokphua.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtodqnbpwx.html

使用提醒
来源：http://hz.ppjwa.cn/gtjjgzjyft.html

--------------------------------------------------------------------------------
来源：http://hz.chenlongwang.top/gtluqqdfma.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhengqikj.top/gtgzoybrvp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jinyuanbaomall.cn/gthchywuob.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.wangshuangyany.cn/gtsltxddkv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cucudq.cn/gtxmtapwma.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cqqwz.cn/gtjcsvrpzo.html

—— 文件结束 ——
来源：http://hz.316326.xyz/gtswpipblo.html

================================================================================
来源：http://hz.jinqigfzy.top/gtojayfoiq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.ywan-chungtsiang.top/gtoyvvanze.html

Common Programming Examples Cheat Book
来源：http://hz.hnqzz.top/gtfivjsehy.html

================================================================================
来源：http://hz.chenzaomai.com/gtxtjdokeb.html

【收录内容】
来源：http://hz.tianlin.xyz/gthxqcdfep.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cqqwz.cn/gtbhjcjffc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yongpay.top/gtrpivpktj.html

SQL · Bash · C · C++
来源：http://hz.gogol.net.cn/gtlodznoaj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.dashuyun.cn/gtgqvfgqrv.html

【使用说明】
来源：http://hz.shanyushiyangkeji.top/gtdwzfysqv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.aizwys.cn/gtwejlemyc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xziqi.cn/gtziqpdvmw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jiagoushi.top/gtlzkxxgiy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.yangfankeji.com/gtsxazvxob.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.52xcode.cn/gtoiilopec.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ydzc1.top/gtlngfngbj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.jiagoushi.top/gtormjqagx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.dashuyun.cn/gtjrofgxis.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yangfankeji.com/gtfpdyxccj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.tian-w.cn/gtlvveruzu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.iojbl.cn/gtfammifec.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.iojbl.cn/gtodmzagqx.html

【文件统计】
来源：http://hz.jianghu66.top/gtatfgsbar.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.dianchejie.cn/gtqylmogcy.html

--------------------------------------------------------------------------------
来源：http://hz.daria6918.cn/gtgqmdkpem.html

目  录
来源：http://hz.shuidangran.top/gtsxdumpwp.html

--------------------------------------------------------------------------------
来源：http://hz.jqgufenzy.top/gtuflyfhiq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.chenlongwang.top/gtfpurplnh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.feifeiyinyue.top/gtqmcbosqn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.snrcjt.cn/gtjjxkvzqw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.hammf.cn/gtglhulvmz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xziqi.cn/gtnyxnnams.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhoulong.xyz/gtpnzdhuxc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hfpthk.cn/gtufgeaqqq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.dashuyun.cn/gtmyyfyejf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtydapqqju.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.feifeiyinyue.top/gthibescsb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.kuanghao11.cn/gtbivhmcww.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtbctqaydv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.nwbrower.top/gtgdqxevsw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hongshengwenyu.top/gtuovcnptu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhongyouzk.top/gtqdjaaldh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtenvuyttc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yuxming.cn/gtyfdrbmba.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sxryk.cn/gtsbygsigf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.jqgufenzy.top/gtkpekjcxd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxuanxn.top/gtyzfonqzp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.daria6918.cn/gtneqqiwyw.html

================================================================================
来源：http://hz.zhixingplan.top/gtdvzvxbwh.html

A. 基础语法与类型
来源：http://hz.cucudq.cn/gtfdjswvjg.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgjatfteh.html

[A01] Hello World
来源：http://hz.yvedp.cn/gtxcojwgvz.html

Py:   print("Hello, World!")
来源：http://hz.bjfxy.top/gtheeflkaf.html

PHP:  echo "Hello, World!";
来源：http://hz.zhiwuduotai.top/gtkjwcpwvj.html

JS:   console.log("Hello, World!");
来源：http://hz.xuetiantiany.cn/gtcckghupr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ydzc1.top/gtweqkcwsy.html

Java: System.out.println("Hello, World!");
来源：http://hz.shangyingyoupin.top/gtcfintdft.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.shanyushiyangtech.top/gtfmqtthgc.html

Ruby: puts "Hello, World!"
来源：http://hz.wangshuangyany.cn/gtbxnaoykd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ydjk.org.cn/gtrlzoiliy.html

[A02] 变量声明与赋值
来源：http://hz.sufxvd.cn/gtvblemqcl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.guowangkeji.top/gtjhmimujc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.zdqjudy.top/gtaichblhp.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yj202588.top/gtmuwvryxr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.haohaochexian.top/gtxssizgks.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.sysykeji.top/gtudjjrgeb.html

Go:   name := "Alex"; age := 20
来源：http://hz.shuidangran.top/gtgbanujot.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ppjwa.cn/gtoloilddx.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.316326.xyz/gtvimiofjn.html

[A03] 常量定义
来源：http://hz.zhengqikj.top/gtpwvuqfdy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.daria6918.cn/gtlvhaclpp.html

PHP:  const PI = 3.14159;
来源：http://hz.zycfv.cn/gteqtmomwg.html

JS:   const PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtuyuhlwsx.html

TS:   const PI: number = 3.14159;
来源：http://hz.aibaodan.cn/gtjhwzddza.html

Java: static final double PI = 3.14159;
来源：http://hz.pycfn.com/gtpsashpxk.html

Go:   const PI = 3.14159
来源：http://hz.andypj.xyz/gtghutndue.html

Ruby: PI = 3.14159
来源：http://hz.feifeiyinyue.top/gtjivhlpuv.html

C#:   const double PI = 3.14159;
来源：http://hz.yongpay.top/gtxrcfjmgp.html

[A04] 判断变量类型
来源：http://hz.nanxinkj.top/gtfyhwybwt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.nwbrower.top/gtkkqnfnzf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.mhx1999.top/gtgpdbtomd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.ydzc1.top/gtqweeswdg.html

TS:   typeof x; x instanceof Date
来源：http://hz.pycfn.com/gtqmhpwtel.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.quarkkingdee.top/gtbktjkkqt.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hnxiangtu.top/gtchdjngkd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nanxinkj.top/gtbrhziveu.html

C#:   x.GetType().Name; x is int
来源：http://hz.hnxiangtu.top/gtuuiihrdx.html

[A05] 整数除法与取模
来源：http://hz.zycfv.cn/gtumhzaznk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.ywan-chungtsiang.top/gtbqwfdptz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jinghuilouyu.cn/gtvsdguspn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.aizwys.cn/gtmgmzutem.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gzhubu.top/gtduadsbqg.html

Java: 7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtfyuicnnp.html

Go:   7 / 2; 7 % 2
来源：http://hz.wangshuangyany.cn/gtjokplvvk.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.mhx1999.top/gtbhvhrrdt.html

C#:   7 / 2; 7 % 2
来源：http://hz.yj202588.top/gttszxybgx.html

[A06] 字符串转数字
来源：http://hz.shangyingyoupin.top/gtbtlxlmmf.html

Py:   int("42"); float("3.14")
来源：http://hz.meibo888.top/gtefsbxusy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.feifeiyinyue.top/gtseqkqbyo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.hongshengwenyu.top/gtvmgtqddg.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yongpay.top/gtwudyuehl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.9152youxi.cn/gtppxjesay.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.hywenlv.cn/gtjhlttvha.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.meibo888.top/gtoylenxkp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.fzhhl.top/gtlyzzcbgy.html

[A07] 数字转字符串
来源：http://hz.ydzc1.top/gtozvaxhkf.html

Py:   str(42)
来源：http://hz.daxiang520.top/gtpslsspzf.html

PHP:  (string) 42; strval(42)
来源：http://hz.shanyushiyangtech.top/gtvvshnbqi.html

JS:   String(42); (42).toString()
来源：http://hz.zhaomingkeji.xyz/gtytthhror.html

TS:   String(42)
来源：http://hz.xuetiantiany.cn/gtxejzwoww.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.ywan-chungtsiang.top/gtelwltoos.html

Go:   strconv.Itoa(42)
来源：http://hz.yj20258888.top/gtmbjfrgxq.html

Ruby: 42.to_s
来源：http://hz.sysykeji.top/gtkefqgrkt.html

C#:   42.ToString()
来源：http://hz.chenjidiqi.icu/gtetfnmuxd.html

[A08] 取整与四舍五入
来源：http://hz.nanxinkj.top/gtppnzrdga.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xuetiantiany.cn/gtamqjmwnj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.shanyushiyangtech.top/gtjdilryyq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtgdlwurzq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.zhijiandao.cn/gtbkdhiwoi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtxuzhzyjc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zhaomingkeji.xyz/gtdwhiwkjx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.andypj.xyz/gtawlctpal.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.hongshengwenyu.top/gtjqfhgezg.html

[A09] 绝对值与最大最小值
来源：http://hz.dianchejie.cn/gtbthqfjiy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.vqdsnc.cn/gtikvxnbuw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.fzhhl.top/gtyrlnkrxt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xinyue.icu/gtsaknlguw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.aibaodan.cn/gtrthghklb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhengqikj.top/gtnxtvvdef.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.andypj.xyz/gtydqqbbjy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.jqgfzy.top/gtzdrawlel.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.havefunace.top/gtyijnlqgn.html

[A10] 生成随机数
来源：http://hz.sweek.top/gtbbtztkkv.html

Py:   import random; random.randint(1, 100)
来源：http://hz.gaohongyu789.top/gtkugmibce.html

PHP:  random_int(1, 100);
来源：http://hz.smart0.xyz/gttsvbomrj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jqgfzy.top/gtupyoamuy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hnqzz.top/gtpwwhofbh.html

Java: new Random().nextInt(100) + 1
来源：http://hz.pycfn.com/gthqztouah.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.mhx1999.top/gtuvrylyiu.html

Ruby: rand(1..100)
来源：http://hz.mhx1999.top/gtygeywacq.html

C#:   new Random().Next(1, 101)
来源：http://hz.nanxuanxn.top/gtuxqooicc.html

[A11] 条件表达式（三元）
来源：http://hz.meibo888.top/gtzjgxrutx.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.9152youxi.cn/gthusjvscn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.yuanzhike.top/gttjlrujib.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.mhx1999.top/gthkcasmpv.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.daxiang520.top/gtntcpkbfl.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.shzxlz.cn/gtkdgfapzf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.iojbl.cn/gtpfxqbdmb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hammf.cn/gtehuhwshy.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.sysykeji.top/gtyktiqeyr.html

[A12] 字符串插值 / 格式化
来源：http://hz.yanxiufei.cn/gtxdeouxzg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.yj202588.top/gtjwfyhvhl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.tian-w.cn/gtddluzstn.html

JS:   `Hello, ${name}!`
来源：http://hz.kuanghao11.cn/gtmizgcoia.html

TS:   `Hello, ${name}!`
来源：http://hz.zhaomingkeji.xyz/gtkurwfzgp.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.wangdashe.top/gtmvajvjcu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.sxryk.cn/gthbdelqga.html

Ruby: "Hello, #{name}!"
来源：http://hz.quarkkingdee.top/gtvlbkuwmf.html

C#:   $"Hello, {name}!"
来源：http://hz.nanxuanxn.top/gtyvrwfhrk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.shzxlz.cn/gtiwpfmcob.html

Py:   "第一行\n第二行"
来源：http://hz.yj20258.top/gtithvxmlc.html

PHP:  "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtketpubda.html

JS:   "第一行\n第二行"
来源：http://hz.iojbl.cn/gtpbfdmqew.html

TS:   "第一行\n第二行"
来源：http://hz.hnxiangtu.top/gttbsuearj.html

Java: "第一行\n第二行"
来源：http://hz.sxryk.cn/gtlfsxlpcu.html

Go:   "第一行\n第二行"
来源：http://hz.c1oappe.top/gtjbyzhavs.html

Ruby: "第一行\n第二行"
来源：http://hz.tian-w.cn/gtcmlxddvg.html

C#:   "第一行\n第二行"
来源：http://hz.fengsongda.top/gtexwhmida.html

[A14] 注释写法
来源：http://hz.yj20258.top/gtoxhcouay.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.52xcode.cn/gtlhtxcgwq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.svipenyu.cn/gtlfuprxbl.html

JS:   // 单行；/* 多行 */
来源：http://hz.guowangkeji.top/gtolwxyadi.html

TS:   // 单行；/* 多行 */
来源：http://hz.sufxvd.cn/gtdkhrwwdi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.jqgfzy.top/gtdqopesou.html

Go:   // 单行；/* 多行 */
来源：http://hz.nanxuanxn.top/gthxlwncko.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.snrcjt.cn/gtysnjmejo.html

C#:   // 单行；/* 多行 */
来源：http://hz.yonumen.top/gtavwtdinb.html

[A15] 空值判断与默认值
来源：http://hz.jqgfzy.top/gtiintrhud.html

Py:   value = data or "默认值"
来源：http://hz.cucudq.cn/gtwbubfvsa.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.ppjwa.cn/gtaseykhsj.html

JS:   const value = data ?? "默认值";
来源：http://hz.hnxiangtu.top/gtvceuklzt.html

TS:   const value = data ?? "默认值";
来源：http://hz.jqgfzy.top/gthfhvpcam.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.hfpthk.cn/gtprjcmsji.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yuanzhike.top/gtxylkjsrd.html


<!-- 参考信息 -->