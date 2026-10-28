代发 wailian999

[U93] JS：模板字符串
来源：http://hz.jlsjyb.cn/gtwqlcylsm.html

`共 ${n} 条`
来源：http://hz.chenzaomai.com/gtqoewlxtr.html

[U94] JS：箭头函数
来源：http://hz.tian-w.cn/gtyrccbcsv.html

const double = x => x * 2;
来源：http://hz.hammf.cn/gtgeauprjk.html

[U95] JS：Promise 包装
来源：http://hz.zhoulong.xyz/gturwtaizz.html

new Promise((resolve, reject) => {})
来源：http://hz.wangshuangyany.cn/gtjhstwzuk.html

[U96] JS：async/await 与异常
来源：http://hz.yueranfly.top/gtnrhxrqzc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtulrxrjwd.html

[U97] JS：并发请求
来源：http://hz.yj202588.top/gtwpdwtkfk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtecbhxnmz.html

[U98] JS：fetch 带 JSON
来源：http://hz.havefunace.top/gtvsyvpzrz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.52xcode.cn/gtuzojdlii.html

[U99] JS：事件监听
来源：http://hz.meibo888.top/gtyajveiem.html

el.addEventListener("click", e => {})
来源：http://hz.zhiwuduotai.top/gtgjwdedzo.html

[U100] JS：DOM 查询
来源：http://hz.zhiwuduotai.top/gtpyaoyejp.html

document.querySelector(".item")
来源：http://hz.wangdashe.top/gtxtgjiviv.html

[U101] JS：classList 操作
来源：http://hz.hysaishi.cn/gtpyxjrmhq.html

el.classList.toggle("active")
来源：http://hz.meibo888.top/gtkpixidjs.html

[U102] JS：本地存储
来源：http://hz.guowangkeji.top/gtdoernrzc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.mhx1999.top/gtscetjqip.html

[U103] JS：定时器
来源：http://hz.zhoulong.xyz/gttjxzekxd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.smart0.xyz/gtcqjpzvbf.html

[U104] JS：防抖
来源：http://hz.zhixingplan.top/gtivjrxjhx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangtech.top/gtkmnrfpzv.html

[U105] JS：节流
来源：http://hz.xylfe.cn/gttysoymdv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.wangdashe.top/gtzksbxket.html

[U106] JS：日期格式化
来源：http://hz.snrcjt.cn/gtbcyvwfbm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.shangyingyoupin.top/gtskvaqtfc.html

[U107] JS：数字千分位
来源：http://hz.c1oappe.top/gtzaszwmun.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jlsjyb.cn/gtsoyyouuu.html

[U108] JS：随机整数
来源：http://hz.ppjwa.cn/gtygbjeaep.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jlsjyb.cn/gtnxonltxb.html

[U109] JS：数组分组
来源：http://hz.fengsongda.top/gtkobbxpms.html

Object.groupBy(arr, x => x.type)
来源：http://hz.sufxvd.cn/gtjetlxnkr.html

[U110] JS：数组分块
来源：http://hz.redwolf501.top/gtiwoulhjk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinqigfzy.top/gtmsydrekw.html

[U111] JS：对象转 Map
来源：http://hz.smart0.xyz/gtrwxyihqj.html

new Map(Object.entries(obj))
来源：http://hz.chenjidiqi.icu/gtkdbcvhvo.html

[U112] JS：字符串补位
来源：http://hz.yvedp.cn/gtxuwfrqdm.html

"7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gtposunkda.html

[U113] JS：正则替换全部
来源：http://hz.316326.xyz/gtutvmybch.html

s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtwsnukchx.html

[U114] JS：JSON 深比较
来源：http://hz.bjfxy.top/gtaiaeicip.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtomnxxbkk.html

[U115] JS：生成 UUID
来源：http://hz.zycfv.cn/gtzegbojdj.html

crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtmpxzwhsf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.cashguo.top/gtspihrxcl.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xinyue.icu/gtouucbizs.html

[U117] JS：单元测试
来源：http://hz.snrcjt.cn/gtkndcgcgq.html

npm i -D vitest;  npx vitest
来源：http://hz.zhengqikj.top/gtisyixamx.html

[U118] JS：开发服务器
来源：http://hz.wangshuangyany.cn/gtafurqtvo.html

npm i -D vite;  npx vite
来源：http://hz.birdmap.top/gtwtjrgdbe.html

[U119] JS：生产构建
来源：http://hz.gzhubu.top/gttapsxyea.html

npx vite build
来源：http://hz.chenlongwang.top/gtjkkjfixu.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ydjk.org.cn/gtlllerexx.html

import.meta.env.VITE_API_URL
来源：http://hz.cheryme.top/gttseecvmq.html

================================================================================
来源：http://hz.svipenyu.cn/gtjokimzez.html

统计汇总
来源：http://hz.jianghu66.top/gtsjjxqrhr.html

================================================================================
来源：http://hz.ydjk.org.cn/gtwzigjhwa.html

按语言统计（条）：
来源：http://hz.sweek.top/gtobhbxfyi.html

Python ......... 252
来源：http://hz.guannengcc.top/gtenvvquri.html

PHP ............ 252
来源：http://hz.yuxming.cn/gtawsabvpo.html

JavaScript ..... 252
来源：http://hz.zhengqikj.top/gtlzuanoea.html

TypeScript ..... 212
来源：http://hz.xziqi.cn/gtawooobfh.html

Java ........... 212
来源：http://hz.andypj.xyz/gtvbsjvqvp.html

Go ............. 212
来源：http://hz.yj20258.top/gtzlgrcbea.html

Ruby ........... 212
来源：http://hz.jqgufenzy.top/gtbznpwtev.html

C# ............. 212
来源：http://hz.dashuyun.cn/gtydwukhla.html

C .............. 30
来源：http://hz.vqdsnc.cn/gtakyfhulq.html

C++ ............ 30
来源：http://hz.wangshuangyany.cn/gtswbxjact.html

SQL ............ 90
来源：http://hz.tianlin.xyz/gtbrobxupu.html

Bash ........... 80
来源：http://hz.cdnleiting.top/gtwmgrqngf.html

Kotlin ......... 15
来源：http://hz.jlsjyb.cn/gtroihvlzl.html

Swift .......... 15
来源：http://hz.zhongyouzk.top/gtlovldwjj.html

Lua ............ 10
来源：http://hz.guowangkeji.top/gtshhbizfi.html

Perl ........... 10
来源：http://hz.svipenyu.cn/gtkurkjnfj.html

Scala .......... 10
来源：http://hz.wangdashe.top/gtpcibyixx.html

------------------------------------
来源：http://hz.jianghu66.top/gtaoenvfxl.html

合计 ........... 2106 条
来源：http://hz.ehwqpu.com/gtsemzbepu.html

按章节统计：
来源：http://hz.dianchejie.cn/gtgefswuqm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhijiandao.cn/gtlofeuxyf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.pycfn.com/gtwabclxwj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xinyue.icu/gtqqjdxblw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.gaohongyu789.top/gtwvnkirlt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.yj20258888.top/gtlgayukkz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.nanxinkj.top/gtuqiuynjx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.fzhhl.top/gtjsshdtqf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yanxiufei.cn/gtaxjpuwgd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtruxuxwbr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.52xcode.cn/gtvzvariqd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hammf.cn/gtklpbnzeo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhaomingkeji.xyz/gtccjttxew.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtjhpbmhjl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.nanxuanxn.top/gtnruwxuke.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.haohaochexian.top/gtblayaofj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtgvnlwztk.html

Q SQL 专题                              90
来源：http://hz.jqgfzy.top/gtamamppqx.html

R Bash 专题                             80
来源：http://hz.tianlin.xyz/gtiozjulqj.html

S C / C++ 专题                          60
来源：http://hz.yangfankeji.com/gtimfpelnx.html

T 其他语言补充                          60
来源：http://hz.hnxiangtu.top/gtipmnquaj.html

U 高频实用片段                         120
来源：http://hz.ehwqpu.com/gtpmcvhleq.html

------------------------------------
来源：http://hz.daxiang520.top/gtidjzdtnw.html

合计                                  2106 条
来源：http://hz.aizwys.cn/gteyqeqpqx.html

--------------------------------------------------------------------------------
来源：http://hz.hammf.cn/gtrthpdqjn.html

使用提醒
来源：http://hz.yj20258888.top/gtibskjamu.html

--------------------------------------------------------------------------------
来源：http://hz.cashguo.top/gtmdxwzydf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shuidangran.top/gthlvwxfke.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.52xcode.cn/gtobiokgmj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.tian-w.cn/gtlepibrhf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jianghu66.top/gtrokznyma.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cqqwz.cn/gtnkfnyybx.html

—— 文件结束 ——
来源：http://hz.tian-w.cn/gtrkvhxddi.html

================================================================================
来源：http://hz.dianchejie.cn/gtscwywnnz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.cheryme.top/gtqdhtsetr.html

Common Programming Examples Cheat Book
来源：http://hz.aibaodan.cn/gthdklxflh.html

================================================================================
来源：http://hz.hfpthk.cn/gtzvansdyz.html

【收录内容】
来源：http://hz.yj20258.top/gtoohcbjvl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yanxiufei.cn/gtbyxtfuph.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jiagoushi.top/gtbzvoooqh.html

SQL · Bash · C · C++
来源：http://hz.vqdsnc.cn/gtrdabnrng.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.meibo888.top/gtcgxqugva.html

【使用说明】
来源：http://hz.nwbrower.top/gtcsokwzju.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.guowangkeji.top/gtpkmavzzr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.shuidangran.top/gtblzpkefd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.cdnleiting.top/gtjtjkuirz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jinyuanbaomall.cn/gtagyiayju.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jqgufenzy.top/gtyqdvwjdb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zhengqikj.top/gtweqgoloz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ppjwa.cn/gtrijmkqjh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.daria6918.cn/gtfrpqlxnd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.xylfe.cn/gteuhuqbxa.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.daxiang520.top/gtqowonwol.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.chenlongwang.top/gtusmnogsq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.haohaochexian.top/gtfftmpfsz.html

【文件统计】
来源：http://hz.meibo888.top/gtbtbfvpww.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.svipenyu.cn/gttscybruz.html

--------------------------------------------------------------------------------
来源：http://hz.cdnleiting.top/gtfgpsoigf.html

目  录
来源：http://hz.shangyingyoupin.top/gtgrorfqqe.html

--------------------------------------------------------------------------------
来源：http://hz.aizwys.cn/gtgpbzvklz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.c1oappe.top/gtjqruzwnb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinghuilouyu.cn/gtzsejhilu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yonumen.top/gtzqqymrje.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zhaomingkeji.xyz/gtoglzorvp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ybcxt.top/gttdqzadvb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhoulong.xyz/gtjupeydar.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.zhijiandao.cn/gtydekwltp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sxryk.cn/gtlphxtadb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ppjwa.cn/gtvnxdcgvu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.shzxlz.cn/gtmeosfxcw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtpbyinxax.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtfspsttkk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.bjfxy.top/gtufgwvlrq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.316326.xyz/gtyjocvleg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zycfv.cn/gtlrwmyzee.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gthmkgbbiw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhengqikj.top/gtqjbtasbt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.bjfxy.top/gtpicawayg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.ydjk.org.cn/gtsgxxakio.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dashuyun.cn/gtaimqntuv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.bjfxy.top/gtelunddxe.html

================================================================================
来源：http://hz.yangfankeji.com/gtcdgoskrk.html

A. 基础语法与类型
来源：http://hz.jqgufenzy.top/gtkmustzcu.html

================================================================================
来源：http://hz.andypj.xyz/gteaihkdto.html

[A01] Hello World
来源：http://hz.zhoulong.xyz/gtsuuxbegd.html

Py:   print("Hello, World!")
来源：http://hz.kuanghao11.cn/gtevxepxue.html

PHP:  echo "Hello, World!";
来源：http://hz.gogol.net.cn/gtgxbhflrl.html

JS:   console.log("Hello, World!");
来源：http://hz.quarkkingdee.top/gtsoqdvtsf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.cheryme.top/gtvbbspcib.html

Java: System.out.println("Hello, World!");
来源：http://hz.gogol.net.cn/gtjcwucivd.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.pengpengdd.cyou/gtfhvtqtlz.html

Ruby: puts "Hello, World!"
来源：http://hz.haohaochexian.top/gtmhrfqcxn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.gaohongyu789.top/gtltxkaebh.html

[A02] 变量声明与赋值
来源：http://hz.yj20258.top/gtpuqpzzzt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.cdnleiting.top/gtzhqrneys.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shangyingyoupin.top/gtbnmvbwyu.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.52xcode.cn/gtnketzbek.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.hongshengwenyu.top/gtaxibctmq.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.dianchejie.cn/gtawtpwieg.html

Go:   name := "Alex"; age := 20
来源：http://hz.xingfuxueyuan.xyz/gtwqgsigsc.html

Ruby: name = "Alex"; age = 20
来源：http://hz.shzxlz.cn/gtogsvqyiy.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.sufxvd.cn/gtemdnhynk.html

[A03] 常量定义
来源：http://hz.hysaishi.cn/gtgwmwglqs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ppjwa.cn/gtzeupewjm.html

PHP:  const PI = 3.14159;
来源：http://hz.hongshengwenyu.top/gtkjzhjlem.html

JS:   const PI = 3.14159;
来源：http://hz.wangdashe.top/gteevpfskc.html

TS:   const PI: number = 3.14159;
来源：http://hz.andypj.xyz/gtswrzhkxd.html

Java: static final double PI = 3.14159;
来源：http://hz.zhiwuduotai.top/gtshwqkklq.html

Go:   const PI = 3.14159
来源：http://hz.guannengcc.top/gtecstafot.html

Ruby: PI = 3.14159
来源：http://hz.yvedp.cn/gttuksjhlt.html

C#:   const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtiargxfhf.html

[A04] 判断变量类型
来源：http://hz.shangyingyoupin.top/gthgvflgve.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.chenzaomai.com/gtggncjwcf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ydjk.org.cn/gtrdrosoip.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yueranfly.top/gtmrepiscb.html

TS:   typeof x; x instanceof Date
来源：http://hz.hfpthk.cn/gttjduoulk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.cqqwz.cn/gtrswcjhbo.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yj20258888.top/gthajvasks.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yvedp.cn/gtpeingxqx.html

C#:   x.GetType().Name; x is int
来源：http://hz.jqgfzy.top/gtldbpiwkt.html

[A05] 整数除法与取模
来源：http://hz.cqqwz.cn/gtazavsutc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.pycfn.com/gtbekscdmq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.wangshuangyany.cn/gtinvtklgp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ybcxt.top/gtcvqhhtot.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jiagoushi.top/gttafplpmf.html

Java: 7 / 2; 7 % 2
来源：http://hz.jinghuilouyu.cn/gtozhdvppd.html

Go:   7 / 2; 7 % 2
来源：http://hz.shanyushiyangkeji.top/gtonktjtlv.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.havefunace.top/gtpuoqejtr.html

C#:   7 / 2; 7 % 2
来源：http://hz.jiagoushi.top/gtylbloylr.html

[A06] 字符串转数字
来源：http://hz.daxiang520.top/gtkmfpiehr.html

Py:   int("42"); float("3.14")
来源：http://hz.ywan-chungtsiang.top/gtaxtlmdcc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.0kj1m.cn/gtrxazwtsm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jinyuanbaomall.cn/gtyirrjuav.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jyoumei.cn/gteqvhgnov.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.shangyingyoupin.top/gtyljutoce.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.hnxiangtu.top/gtsdkaeskj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.sweek.top/gtlfjkwfmn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.fengsongda.top/gtjotniest.html

[A07] 数字转字符串
来源：http://hz.dashuyun.cn/gtwkgzqkdt.html

Py:   str(42)
来源：http://hz.yj202588.top/gtiwhiskbm.html

PHP:  (string) 42; strval(42)
来源：http://hz.iojbl.cn/gtjzuctgpg.html

JS:   String(42); (42).toString()
来源：http://hz.jinqigufen.top/gtaijgvwuo.html

TS:   String(42)
来源：http://hz.jinghuilouyu.cn/gtrlrrcccc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.nanxuanxn.top/gtsnoyfdrl.html

Go:   strconv.Itoa(42)
来源：http://hz.gzhubu.top/gtkqpuxhab.html

Ruby: 42.to_s
来源：http://hz.andypj.xyz/gtyxgiuprb.html

C#:   42.ToString()
来源：http://hz.jinqigfzy.top/gtyupdpukp.html

[A08] 取整与四舍五入
来源：http://hz.jinghuilouyu.cn/gtjcciaexp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.0kj1m.cn/gtaihoujxz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.xuetiantiany.cn/gtlukzibrf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.dianchejie.cn/gtfgrtjxtz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jyoumei.cn/gtapsrxioy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.vqdsnc.cn/gtayngbkye.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.tian-w.cn/gtmlckoncb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yj202588.top/gtxlwmkmek.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.daria6918.cn/gtmuolijgs.html

[A09] 绝对值与最大最小值
来源：http://hz.zhongyouzk.top/gtclmbydiw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cdnleiting.top/gtxcnqjiws.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhoulong.xyz/gtplshmrgv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xylfe.cn/gtyhegxiph.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shzxlz.cn/gturlempox.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hammf.cn/gtmfjjrdlt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.xingfuxueyuan.xyz/gtlpftsnwx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.wangdashe.top/gtahvurwhb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ybcxt.top/gtecafmknf.html

[A10] 生成随机数
来源：http://hz.gotoacloud.top/gtvvsyervj.html

Py:   import random; random.randint(1, 100)
来源：http://hz.jqgufenzy.top/gtwfpxcvye.html

PHP:  random_int(1, 100);
来源：http://hz.zdqjudy.top/gtboklrfhr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.daria6918.cn/gtrmnzhsxy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yvedp.cn/gtiexvvwzc.html

Java: new Random().nextInt(100) + 1
来源：http://hz.zhoulong.xyz/gttnjzyqbo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.bjfxy.top/gtydzpnyhz.html

Ruby: rand(1..100)
来源：http://hz.jinghuilouyu.cn/gtccjyvbkq.html

C#:   new Random().Next(1, 101)
来源：http://hz.yuxming.cn/gtklutljjs.html

[A11] 条件表达式（三元）
来源：http://hz.hfpthk.cn/gtihopbuoo.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.redwolf501.top/gtjakbhtpd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangtech.top/gtscairfyi.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.xingfuxueyuan.xyz/gthcpcslis.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zhongyouzk.top/gtagyrnfat.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gtsydpbiha.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.guowangkeji.top/gtxpsvlszq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.jqgfzy.top/gttifqneuu.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yonumen.top/gtspuxqkzm.html

[A12] 字符串插值 / 格式化
来源：http://hz.chenlongwang.top/gtjnpzkbas.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.daxiang520.top/gtqrabecpv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhoulong.xyz/gtaqutyhtu.html

JS:   `Hello, ${name}!`
来源：http://hz.tanke756.top/gthxpmxpjt.html

TS:   `Hello, ${name}!`
来源：http://hz.yanxiufei.cn/gtwbflkitw.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.yvedp.cn/gtejsvexcm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.0kj1m.cn/gtxuppxnvy.html

Ruby: "Hello, #{name}!"
来源：http://hz.nanxuanxn.top/gtfjevoiov.html

C#:   $"Hello, {name}!"
来源：http://hz.daxiang520.top/gtzwurewcd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.ppjwa.cn/gtuxoiahxx.html

Py:   "第一行\n第二行"
来源：http://hz.yvedp.cn/gtavdkfzzc.html

PHP:  "第一行\n第二行"
来源：http://hz.cqqwz.cn/gtfzqebzbp.html

JS:   "第一行\n第二行"
来源：http://hz.chenjidiqi.icu/gtovcftrqs.html

TS:   "第一行\n第二行"
来源：http://hz.hammf.cn/gtxzcfsplq.html

Java: "第一行\n第二行"
来源：http://hz.jqgfzy.top/gtzijbzwxv.html

Go:   "第一行\n第二行"
来源：http://hz.hysaishi.cn/gtafapxisq.html

Ruby: "第一行\n第二行"
来源：http://hz.yongpay.top/gtielpxwvp.html

C#:   "第一行\n第二行"
来源：http://hz.hongshengwenyu.top/gtismghjga.html

[A14] 注释写法
来源：http://hz.jinqigufen.top/gtclgealzt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.hywenlv.cn/gthfcjirbl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.nanxinkj.top/gttmngswar.html

JS:   // 单行；/* 多行 */
来源：http://hz.cdnleiting.top/gtlitnrohx.html

TS:   // 单行；/* 多行 */
来源：http://hz.shuidangran.top/gtkvfuyjaa.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.snrcjt.cn/gtivcxhsei.html

Go:   // 单行；/* 多行 */
来源：http://hz.hongshengwenyu.top/gtypmathqy.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.gogol.net.cn/gtyleortdj.html

C#:   // 单行；/* 多行 */
来源：http://hz.zycfv.cn/gtlipgarto.html

[A15] 空值判断与默认值
来源：http://hz.cashguo.top/gtnbivxwpw.html

Py:   value = data or "默认值"
来源：http://hz.feifeiyinyue.top/gtasezzjfj.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zycfv.cn/gtzwzyppzf.html

JS:   const value = data ?? "默认值";
来源：http://hz.bjfxy.top/gtgwvkjukg.html

TS:   const value = data ?? "默认值";
来源：http://hz.pengpengdd.cyou/gtdjscckbl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.tianlin.xyz/gtbthinpjp.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.jinyuanbaomall.cn/gttdhukbpf.html

Ruby: value = data || "默认值"
来源：http://hz.316326.xyz/gtgdnfqppp.html

C#:   var value = data ?? "默认值";
来源：http://hz.nanxuanxn.top/gtsiafliaz.html

[A16] 真假值判断规则
来源：http://hz.jinqigufen.top/gtnsclhpzm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.wangdashe.top/gtkfwrdgho.html


<!-- 参考信息 -->