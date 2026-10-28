代发 wailian999

[U85] JS：可选链
来源：http://hz.pycfn.com/gtesrbogti.html

a?.b?.c
来源：http://hz.ybcxt.top/gtfvurgkqd.html

[U86] JS：空值合并
来源：http://hz.316326.xyz/gttvjrsrsd.html

a ?? b
来源：http://hz.ywan-chungtsiang.top/gtwohdfyfj.html

[U87] JS：解构默认值
来源：http://hz.yj202588.top/gtemsiwfbk.html

const { a = 1, b = 2 } = obj;
来源：http://hz.andypj.xyz/gtraezwkjn.html

[U88] JS：对象展开合并
来源：http://hz.zdqjudy.top/gttspnrbyp.html

{ ...a, ...b }
来源：http://hz.zhongyouzk.top/gttinlphqs.html

[U89] JS：数组去重
来源：http://hz.hywenlv.cn/gtbwektxvp.html

[...new Set(arr)]
来源：http://hz.havefunace.top/gtkixourxt.html

[U90] JS：数字数组排序
来源：http://hz.jqgfzy.top/gtyahmlest.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtajgkxypm.html

[U91] JS：对象键值遍历
来源：http://hz.nanxinkj.top/gtlhkvfink.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hongshengwenyu.top/gtfeijnlwz.html

[U92] JS：深拷贝
来源：http://hz.xuanzx.com/gtlnmsrgap.html

structuredClone(obj)
来源：http://hz.daria6918.cn/gtvygqeros.html

[U93] JS：模板字符串
来源：http://hz.hysaishi.cn/gtqnpdapin.html

`共 ${n} 条`
来源：http://hz.tianlin.xyz/gtqkzkmtgs.html

[U94] JS：箭头函数
来源：http://hz.ybcxt.top/gthxnmrctr.html

const double = x => x * 2;
来源：http://hz.ybcxt.top/gtiarcurls.html

[U95] JS：Promise 包装
来源：http://hz.jinyuanbaomall.cn/gtydktvufc.html

new Promise((resolve, reject) => {})
来源：http://hz.chenzaomai.com/gtasgijdky.html

[U96] JS：async/await 与异常
来源：http://hz.chenjidiqi.icu/gtmdqfjkls.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ybcxt.top/gttanqeknr.html

[U97] JS：并发请求
来源：http://hz.ydzc1.top/gtdvbogrhe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.snrcjt.cn/gtvvuykcib.html

[U98] JS：fetch 带 JSON
来源：http://hz.gzhubu.top/gthavsainr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.iojbl.cn/gtpdonpfzw.html

[U99] JS：事件监听
来源：http://hz.vqdsnc.cn/gtnbgqrewf.html

el.addEventListener("click", e => {})
来源：http://hz.jqgfzy.top/gtmekfqrtk.html

[U100] JS：DOM 查询
来源：http://hz.ydzc1.top/gtgldipnae.html

document.querySelector(".item")
来源：http://hz.zhijiandao.cn/gthygktdva.html

[U101] JS：classList 操作
来源：http://hz.chenjidiqi.icu/gturugtkyg.html

el.classList.toggle("active")
来源：http://hz.smart0.xyz/gtfwuiavlu.html

[U102] JS：本地存储
来源：http://hz.hongshengwenyu.top/gtucybomfj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.iojbl.cn/gthwkygart.html

[U103] JS：定时器
来源：http://hz.ybcxt.top/gtwfzaerkt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sweek.top/gtzetinfhi.html

[U104] JS：防抖
来源：http://hz.ydzc1.top/gtdukplwxb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jinyuanbaomall.cn/gtjomertje.html

[U105] JS：节流
来源：http://hz.sxryk.cn/gtltedsedq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.nwbrower.top/gtmfkoyshv.html

[U106] JS：日期格式化
来源：http://hz.yangfankeji.com/gtoavmovry.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jinyuanbaomall.cn/gtwmbgfxgc.html

[U107] JS：数字千分位
来源：http://hz.yonumen.top/gtjyqmaoqr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shzxlz.cn/gtegllbjjk.html

[U108] JS：随机整数
来源：http://hz.9152youxi.cn/gteqddiywk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.zhongyouzk.top/gtihzxtacj.html

[U109] JS：数组分组
来源：http://hz.ivvv.top/gtvgoeppda.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hnqzz.top/gtrbbucwke.html

[U110] JS：数组分块
来源：http://hz.hammf.cn/gtbshhkzwd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ydjk.org.cn/gtidtpcxxx.html

[U111] JS：对象转 Map
来源：http://hz.gotoacloud.top/gtvxjjkvlh.html

new Map(Object.entries(obj))
来源：http://hz.c1oappe.top/gtnkgappyy.html

[U112] JS：字符串补位
来源：http://hz.tianlin.xyz/gtgwmlrdlt.html

"7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtouhmsorl.html

[U113] JS：正则替换全部
来源：http://hz.daria6918.cn/gtkgvrgktt.html

s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtkxichreg.html

[U114] JS：JSON 深比较
来源：http://hz.yj20258.top/gtyoosjpek.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.sxryk.cn/gtzlsxhkus.html

[U115] JS：生成 UUID
来源：http://hz.iojbl.cn/gtmntuyzto.html

crypto.randomUUID()
来源：http://hz.jinghuilouyu.cn/gtvzxmvtdz.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.wangdashe.top/gttgwuebgn.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yonumen.top/gtticjljrv.html

[U117] JS：单元测试
来源：http://hz.tanke756.top/gthbvlltqx.html

npm i -D vitest;  npx vitest
来源：http://hz.feifeiyinyue.top/gtcnenoqif.html

[U118] JS：开发服务器
来源：http://hz.jinghuilouyu.cn/gtdwbeyvzi.html

npm i -D vite;  npx vite
来源：http://hz.cqqwz.cn/gtcqgkenon.html

[U119] JS：生产构建
来源：http://hz.snrcjt.cn/gtcfudhpbl.html

npx vite build
来源：http://hz.hammf.cn/gtnufylgbh.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.aibaodan.cn/gtrfqhroev.html

import.meta.env.VITE_API_URL
来源：http://hz.yangfankeji.com/gtbflfncoe.html

================================================================================
来源：http://hz.guannengcc.top/gtwnvgnwzv.html

统计汇总
来源：http://hz.0kj1m.cn/gtbqldwmmp.html

================================================================================
来源：http://hz.ydjk.org.cn/gtkxmrrupu.html

按语言统计（条）：
来源：http://hz.yanxiufei.cn/gttfcfrmtm.html

Python ......... 252
来源：http://hz.meibo888.top/gtrpenmxdy.html

PHP ............ 252
来源：http://hz.tianlin.xyz/gtqmtzjuzw.html

JavaScript ..... 252
来源：http://hz.redwolf501.top/gtipvmoxod.html

TypeScript ..... 212
来源：http://hz.shanyushiyangtech.top/gtcnchqube.html

Java ........... 212
来源：http://hz.svipenyu.cn/gtlcvxwifv.html

Go ............. 212
来源：http://hz.316326.xyz/gtzqpbyuzc.html

Ruby ........... 212
来源：http://hz.pengpengdd.cyou/gtqpvestfw.html

C# ............. 212
来源：http://hz.ivvv.top/gtxcdexbgv.html

C .............. 30
来源：http://hz.xingfuxueyuan.xyz/gtqrrmciyt.html

C++ ............ 30
来源：http://hz.hnxiangtu.top/gtmmbueraq.html

SQL ............ 90
来源：http://hz.zhaomingkeji.xyz/gtmqjghowb.html

Bash ........... 80
来源：http://hz.c1oappe.top/gtjtzqsurd.html

Kotlin ......... 15
来源：http://hz.zhongyouzk.top/gtsfhqfymu.html

Swift .......... 15
来源：http://hz.kuanghao11.cn/gtdvhctnom.html

Lua ............ 10
来源：http://hz.wangshuangyany.cn/gttokxteud.html

Perl ........... 10
来源：http://hz.svipenyu.cn/gtsnkcnbaq.html

Scala .......... 10
来源：http://hz.hnqzz.top/gtradfpmex.html

------------------------------------
来源：http://hz.yj20258.top/gtclcyibrl.html

合计 ........... 2106 条
来源：http://hz.fengsongda.top/gtpyisdwig.html

按章节统计：
来源：http://hz.daxiang520.top/gttcsjeucs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.dianchejie.cn/gtgyzonocz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.guowangkeji.top/gtyhegtuaw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yuxming.cn/gtskiochfc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.redwolf501.top/gtzumiknlx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.tianlin.xyz/gtivgjyeyn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.52xcode.cn/gttejvlkua.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.cucudq.cn/gtzftwmbyg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.316326.xyz/gtxjtjndqf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtudtjzhpo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.guannengcc.top/gtnjhbiyme.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.jqgfzy.top/gtcojihtnh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtmdsqrqsy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtqyizudwm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sxryk.cn/gttlrfainh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zycfv.cn/gtkthogbfp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gtnspqfltr.html

Q SQL 专题                              90
来源：http://hz.feifeiyinyue.top/gtdqzupyua.html

R Bash 专题                             80
来源：http://hz.c1oappe.top/gtdhftaqak.html

S C / C++ 专题                          60
来源：http://hz.zhongyouzk.top/gteaersrms.html

T 其他语言补充                          60
来源：http://hz.yuxming.cn/gtxaxnaedg.html

U 高频实用片段                         120
来源：http://hz.yj20258888.top/gtpcxybenl.html

------------------------------------
来源：http://hz.aibaodan.cn/gtqrpxnsqv.html

合计                                  2106 条
来源：http://hz.0kj1m.cn/gthhrazkti.html

--------------------------------------------------------------------------------
来源：http://hz.jinqigufen.top/gtdxzicvch.html

使用提醒
来源：http://hz.cashguo.top/gtjlljusgq.html

--------------------------------------------------------------------------------
来源：http://hz.shangyingyoupin.top/gtedbmriap.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.chenjidiqi.icu/gtdbfuugoi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.gaohongyu789.top/gtplpvvehx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.fengsongda.top/gtajybxccr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.hysaishi.cn/gtxnbkjjxz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zdqjudy.top/gtoziwnaxq.html

—— 文件结束 ——
来源：http://hz.chenlongwang.top/gtazdamzqo.html

================================================================================
来源：http://hz.tian-w.cn/gtleqtipow.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.gzhubu.top/gtthlvmifd.html

Common Programming Examples Cheat Book
来源：http://hz.tianlin.xyz/gtnlrivwoo.html

================================================================================
来源：http://hz.9152youxi.cn/gtkvxtmqjy.html

【收录内容】
来源：http://hz.daxiang520.top/gtxtejrhyi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.9152youxi.cn/gtcozivmlw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yvedp.cn/gtpgzalllv.html

SQL · Bash · C · C++
来源：http://hz.pycfn.com/gtoobzcysr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.gaohongyu789.top/gthlqlyavd.html

【使用说明】
来源：http://hz.mhx1999.top/gtrhdfvkxv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.0kj1m.cn/gtoeqxlfkc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.c1oappe.top/gtcxvhoqpc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhoulong.xyz/gtnkgwvhrx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cheryme.top/gtktslrdfh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ehwqpu.com/gtcycwandt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.shzxlz.cn/gtytwzvezu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yangfankeji.com/gtanjqbzfb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.52xcode.cn/gtxqmdtbqz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hammf.cn/gtictnfxgt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.ivvv.top/gtryighsce.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinyuanbaomall.cn/gtzsvbaabg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhixingplan.top/gtxfbuykre.html

【文件统计】
来源：http://hz.yuanzhike.top/gtisfvqkyd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yj20258.top/gthwdsbssm.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gthqqyjjsy.html

目  录
来源：http://hz.zhiwuduotai.top/gtbhujroms.html

--------------------------------------------------------------------------------
来源：http://hz.bjfxy.top/gtczlmbyxb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hywenlv.cn/gtosmdggvo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.mhx1999.top/gtfkfdanzx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zhiwuduotai.top/gtejcqnhbk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.pycfn.com/gtbwqmcxse.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.gotoacloud.top/gtdllkxqca.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.sweek.top/gthajezcxr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.fzhhl.top/gtjdteavzj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ppjwa.cn/gtvsvxccal.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ybcxt.top/gtsveukrgv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.kuanghao11.cn/gtkvywnbhk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtxnlkveix.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.tanke756.top/gtqjirsmwj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.sufxvd.cn/gtvlpfdmxr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.dashuyun.cn/gtpdyszbfa.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.feifeiyinyue.top/gttozifbtv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jinghuilouyu.cn/gtnonylrtt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ywan-chungtsiang.top/gtzjnweyjw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.andypj.xyz/gtzlofogck.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.316326.xyz/gtyjzrirdv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xziqi.cn/gtmeytlmhv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gtvydznsrd.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbrrsqjaa.html

A. 基础语法与类型
来源：http://hz.hfpthk.cn/gtyicjcgfa.html

================================================================================
来源：http://hz.yongpay.top/gtuwzycvbq.html

[A01] Hello World
来源：http://hz.chenzaomai.com/gtvnrdysyi.html

Py:   print("Hello, World!")
来源：http://hz.hammf.cn/gtblykljxr.html

PHP:  echo "Hello, World!";
来源：http://hz.zycfv.cn/gtejsrshwl.html

JS:   console.log("Hello, World!");
来源：http://hz.chenjidiqi.icu/gtlyxtizsh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.316326.xyz/gttkaqcnec.html

Java: System.out.println("Hello, World!");
来源：http://hz.feifeiyinyue.top/gtmxzctsao.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jianghu66.top/gtlqvxzemh.html

Ruby: puts "Hello, World!"
来源：http://hz.cdnleiting.top/gtedsyzlen.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.dianchejie.cn/gtixrkmjuk.html

[A02] 变量声明与赋值
来源：http://hz.cashguo.top/gtnhrckjuq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.zhoulong.xyz/gtkhyqklts.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.guannengcc.top/gtnzgnsxkp.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.haohaochexian.top/gtevibotre.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yanxiufei.cn/gtnfwadkzo.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.bjfxy.top/gtopvlmfga.html

Go:   name := "Alex"; age := 20
来源：http://hz.feifeiyinyue.top/gtvblhnzwp.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hysaishi.cn/gthhubgvgt.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.chenjidiqi.icu/gtkgkpipkx.html

[A03] 常量定义
来源：http://hz.tanke756.top/gtcvlrfbra.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.havefunace.top/gtagahcjyl.html

PHP:  const PI = 3.14159;
来源：http://hz.xuanzx.com/gtwihqivpx.html

JS:   const PI = 3.14159;
来源：http://hz.redwolf501.top/gtjnizasyw.html

TS:   const PI: number = 3.14159;
来源：http://hz.ybcxt.top/gtrqzxmvvy.html

Java: static final double PI = 3.14159;
来源：http://hz.52xcode.cn/gtuivnebkq.html

Go:   const PI = 3.14159
来源：http://hz.fengsongda.top/gtnddshxhq.html

Ruby: PI = 3.14159
来源：http://hz.quarkkingdee.top/gtopxighah.html

C#:   const double PI = 3.14159;
来源：http://hz.pycfn.com/gtfawsvywd.html

[A04] 判断变量类型
来源：http://hz.yuanzhike.top/gtrnauende.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhongyouzk.top/gtapgrsquw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hnxiangtu.top/gtiktzxukh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yueranfly.top/gtxccgnaij.html

TS:   typeof x; x instanceof Date
来源：http://hz.hywenlv.cn/gttdowyiad.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.gaohongyu789.top/gtpfqmurru.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.ydjk.org.cn/gtaskxldmc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gogol.net.cn/gtgtuebeyb.html

C#:   x.GetType().Name; x is int
来源：http://hz.hnxiangtu.top/gtywnwsnly.html

[A05] 整数除法与取模
来源：http://hz.yuanzhike.top/gtnbscnnmv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.wangdashe.top/gtlejilkrm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.xziqi.cn/gtwkptbxly.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj20258.top/gtzyktbkma.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.bjfxy.top/gtboitrfkr.html

Java: 7 / 2; 7 % 2
来源：http://hz.xinyue.icu/gtrsbmshft.html

Go:   7 / 2; 7 % 2
来源：http://hz.hnxiangtu.top/gtvgyskmrh.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.zhengqikj.top/gteelcrrgr.html

C#:   7 / 2; 7 % 2
来源：http://hz.hywenlv.cn/gtxuahqsfh.html

[A06] 字符串转数字
来源：http://hz.c1oappe.top/gtpwvvhurv.html

Py:   int("42"); float("3.14")
来源：http://hz.zhiwuduotai.top/gtdfkgvfll.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.chenjidiqi.icu/gtjcrctnhm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ehwqpu.com/gtnocubhug.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.havefunace.top/gtlpxajakh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.52xcode.cn/gtfobrosjp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.tanke756.top/gtuxixjhzs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.shangyingyoupin.top/gtvpnpyydo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jyoumei.cn/gthepxtgrm.html

[A07] 数字转字符串
来源：http://hz.svipenyu.cn/gtzzpkwwty.html

Py:   str(42)
来源：http://hz.tianlin.xyz/gtfqcyhkeh.html

PHP:  (string) 42; strval(42)
来源：http://hz.yuanzhike.top/gtxegdwrha.html

JS:   String(42); (42).toString()
来源：http://hz.yangfankeji.com/gtpjmpsdji.html

TS:   String(42)
来源：http://hz.nwbrower.top/gtmniplhsh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.jlsjyb.cn/gtbruazmtp.html

Go:   strconv.Itoa(42)
来源：http://hz.cucudq.cn/gtwhomfymf.html

Ruby: 42.to_s
来源：http://hz.hysaishi.cn/gtijmxecrh.html

C#:   42.ToString()
来源：http://hz.dianchejie.cn/gtmvczrgaz.html

[A08] 取整与四舍五入
来源：http://hz.xylfe.cn/gtzerlltps.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.vqdsnc.cn/gtftzpursz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.sufxvd.cn/gtdnsqhvxp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.wangshuangyany.cn/gtowssmiaq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.tianlin.xyz/gtkfishhgz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yj202588.top/gtlkivqifa.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.52xcode.cn/gtamzxlokd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.gotoacloud.top/gtptwmprxu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.shzxlz.cn/gtvdkczpch.html

[A09] 绝对值与最大最小值
来源：http://hz.gogol.net.cn/gtnpeyhshe.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cheryme.top/gtwnmsjdsx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shuidangran.top/gtqcdpuxex.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.dashuyun.cn/gtzdyllwnp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.ydzc1.top/gtxymnizyo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.gzhubu.top/gtrmfwehqa.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.sweek.top/gtpsrfmsqu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.cqqwz.cn/gtharwbdsp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.redwolf501.top/gtmlrqcoph.html

[A10] 生成随机数
来源：http://hz.nwbrower.top/gtttplppwd.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hfpthk.cn/gtzgimepmm.html

PHP:  random_int(1, 100);
来源：http://hz.yvedp.cn/gtjlzlbkow.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.gogol.net.cn/gtpfauibvj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.xinyue.icu/gttkffaexw.html

Java: new Random().nextInt(100) + 1
来源：http://hz.cashguo.top/gtodxgrwei.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jinghuilouyu.cn/gtxqcynubd.html

Ruby: rand(1..100)
来源：http://hz.guowangkeji.top/gtxzpenwlf.html

C#:   new Random().Next(1, 101)
来源：http://hz.jlsjyb.cn/gtxavrjncb.html

[A11] 条件表达式（三元）
来源：http://hz.ivvv.top/gtffprfikc.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jinqigfzy.top/gtrxpufhdg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.zhengqikj.top/gttdmhgjoh.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.haohaochexian.top/gtikpuoiau.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.chenjidiqi.icu/gtrynwjzgt.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gtcodjvqhl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.xziqi.cn/gtxmoohtpm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.ppjwa.cn/gtcsluutlg.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.fengsongda.top/gtfthpftxq.html

[A12] 字符串插值 / 格式化
来源：http://hz.sysykeji.top/gtyzyeffye.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.hnxiangtu.top/gtamrrcmkx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yonumen.top/gtcljwtlrh.html

JS:   `Hello, ${name}!`
来源：http://hz.yj20258888.top/gttklrjlyh.html

TS:   `Hello, ${name}!`
来源：http://hz.nanxinkj.top/gtbqmojlaf.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zdqjudy.top/gtjbqimoob.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.chenlongwang.top/gtrhugzrby.html

Ruby: "Hello, #{name}!"
来源：http://hz.chenjidiqi.icu/gthlqqvpaa.html

C#:   $"Hello, {name}!"
来源：http://hz.dashuyun.cn/gtznclvqsq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.ybcxt.top/gtjkfbgpyf.html

Py:   "第一行\n第二行"
来源：http://hz.shangyingyoupin.top/gtcjalqtce.html

PHP:  "第一行\n第二行"
来源：http://hz.yueranfly.top/gtgwhdegvg.html

JS:   "第一行\n第二行"
来源：http://hz.yuanzhike.top/gttubdklio.html

TS:   "第一行\n第二行"
来源：http://hz.jinqigufen.top/gturhotzjj.html

Java: "第一行\n第二行"
来源：http://hz.chenlongwang.top/gtugrlcfdd.html

Go:   "第一行\n第二行"
来源：http://hz.xziqi.cn/gtiyjhzriy.html

Ruby: "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtcfgashun.html

C#:   "第一行\n第二行"
来源：http://hz.nwbrower.top/gtesulzyzg.html

[A14] 注释写法
来源：http://hz.jinqigufen.top/gtrmywkqix.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yj202588.top/gtccqqnmww.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.tianlin.xyz/gthtrtcijj.html

JS:   // 单行；/* 多行 */
来源：http://hz.tanke756.top/gttqqmsbph.html


<!-- 参考信息 -->