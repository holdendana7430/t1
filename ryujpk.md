代发 wailian999

[U91] JS：对象键值遍历
来源：http://hz.andypj.xyz/gtzcjuvgnd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.mhx1999.top/gtokrnfswd.html

[U92] JS：深拷贝
来源：http://hz.guannengcc.top/gttmhluqvh.html

structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtlqivfpvl.html

[U93] JS：模板字符串
来源：http://hz.jqgfzy.top/gtoidwmakt.html

`共 ${n} 条`
来源：http://hz.ivvv.top/gtpenwvvig.html

[U94] JS：箭头函数
来源：http://hz.chenzaomai.com/gtjgtjnkas.html

const double = x => x * 2;
来源：http://hz.sysykeji.top/gtfiamqonm.html

[U95] JS：Promise 包装
来源：http://hz.bjfxy.top/gttroyngaf.html

new Promise((resolve, reject) => {})
来源：http://hz.sysykeji.top/gtrezjgugj.html

[U96] JS：async/await 与异常
来源：http://hz.hnxiangtu.top/gtqdazxihb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gtuwnvvwxv.html

[U97] JS：并发请求
来源：http://hz.xuetiantiany.cn/gtlalblyck.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtwpisbvsj.html

[U98] JS：fetch 带 JSON
来源：http://hz.wangdashe.top/gtmjzuolvl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.iojbl.cn/gthmrzxwlg.html

[U99] JS：事件监听
来源：http://hz.fzhhl.top/gtnjkgvgdm.html

el.addEventListener("click", e => {})
来源：http://hz.xinyue.icu/gtcvbeciwk.html

[U100] JS：DOM 查询
来源：http://hz.sysykeji.top/gtcrdfgweo.html

document.querySelector(".item")
来源：http://hz.shanyushiyangtech.top/gteqhrmtqf.html

[U101] JS：classList 操作
来源：http://hz.fzhhl.top/gtbaciwyvo.html

el.classList.toggle("active")
来源：http://hz.wangdashe.top/gttcxlqvws.html

[U102] JS：本地存储
来源：http://hz.0kj1m.cn/gtmhceattp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zhiwuduotai.top/gtulxbwwai.html

[U103] JS：定时器
来源：http://hz.aizwys.cn/gtbtrfzbmc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.haohaochexian.top/gtehkldhvf.html

[U104] JS：防抖
来源：http://hz.52xcode.cn/gtshkmokwm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gtqgjuhlqy.html

[U105] JS：节流
来源：http://hz.gzhubu.top/gtumspktuc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.tianlin.xyz/gtzfbhcile.html

[U106] JS：日期格式化
来源：http://hz.tian-w.cn/gtxpvzyqvi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xinyue.icu/gtzbxealbe.html

[U107] JS：数字千分位
来源：http://hz.daria6918.cn/gtjwgdzprp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yonumen.top/gtiwuiezex.html

[U108] JS：随机整数
来源：http://hz.gogol.net.cn/gtmiszenxf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guannengcc.top/gtfzemgvmo.html

[U109] JS：数组分组
来源：http://hz.yvedp.cn/gtqdpbjsym.html

Object.groupBy(arr, x => x.type)
来源：http://hz.fzhhl.top/gtuyhgwgdn.html

[U110] JS：数组分块
来源：http://hz.zhiwuduotai.top/gtzlxotbqv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.yvedp.cn/gtpahdnpss.html

[U111] JS：对象转 Map
来源：http://hz.shangyingyoupin.top/gtrhxunvxi.html

new Map(Object.entries(obj))
来源：http://hz.zdqjudy.top/gtsfjytohd.html

[U112] JS：字符串补位
来源：http://hz.daxiang520.top/gtqgltqwov.html

"7".padStart(3, "0")
来源：http://hz.shuidangran.top/gtezghhhdu.html

[U113] JS：正则替换全部
来源：http://hz.haohaochexian.top/gtgsuaslxy.html

s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtepkxngdv.html

[U114] JS：JSON 深比较
来源：http://hz.zhiwuduotai.top/gtkdrpbrkj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jyoumei.cn/gtnikvxcjv.html

[U115] JS：生成 UUID
来源：http://hz.sxryk.cn/gtwfdkpwmc.html

crypto.randomUUID()
来源：http://hz.52xcode.cn/gtzkhtneuo.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.gotoacloud.top/gtupfeiozz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.chenlongwang.top/gtncbutfkn.html

[U117] JS：单元测试
来源：http://hz.bjfxy.top/gtekjoiczz.html

npm i -D vitest;  npx vitest
来源：http://hz.guowangkeji.top/gtgxwdonar.html

[U118] JS：开发服务器
来源：http://hz.zhaomingkeji.xyz/gtfjwvaetr.html

npm i -D vite;  npx vite
来源：http://hz.zhongyouzk.top/gtfmfgvrvt.html

[U119] JS：生产构建
来源：http://hz.tanke756.top/gtbskjxvgf.html

npx vite build
来源：http://hz.xylfe.cn/gttbongdmw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhiwuduotai.top/gtwshgjuaa.html

import.meta.env.VITE_API_URL
来源：http://hz.andypj.xyz/gthmxsntya.html

================================================================================
来源：http://hz.xinyue.icu/gtyipoyggw.html

统计汇总
来源：http://hz.xingfuxueyuan.xyz/gtmnlziggu.html

================================================================================
来源：http://hz.kuanghao11.cn/gtldfavxmp.html

按语言统计（条）：
来源：http://hz.hnxiangtu.top/gtciipvaau.html

Python ......... 252
来源：http://hz.hfpthk.cn/gtgelxtwil.html

PHP ............ 252
来源：http://hz.wangshuangyany.cn/gtafmpoicm.html

JavaScript ..... 252
来源：http://hz.yvedp.cn/gtliqsnqkm.html

TypeScript ..... 212
来源：http://hz.xuanzx.com/gtvrannnjo.html

Java ........... 212
来源：http://hz.jiagoushi.top/gtrrxcykzl.html

Go ............. 212
来源：http://hz.gzhubu.top/gthcohhlee.html

Ruby ........... 212
来源：http://hz.zhoulong.xyz/gtwelulmaq.html

C# ............. 212
来源：http://hz.ywan-chungtsiang.top/gtzopjzdbe.html

C .............. 30
来源：http://hz.gzhubu.top/gtrqnpvrvg.html

C++ ............ 30
来源：http://hz.gzhubu.top/gttvddyqfv.html

SQL ............ 90
来源：http://hz.316326.xyz/gtkwrlaubz.html

Bash ........... 80
来源：http://hz.jinghuilouyu.cn/gtgijzcqlo.html

Kotlin ......... 15
来源：http://hz.zhixingplan.top/gtqbvmwtkn.html

Swift .......... 15
来源：http://hz.hongshengwenyu.top/gtmzyjivdb.html

Lua ............ 10
来源：http://hz.yj20258.top/gteotzyjhh.html

Perl ........... 10
来源：http://hz.zhiwuduotai.top/gtssfshkqs.html

Scala .......... 10
来源：http://hz.jinyuanbaomall.cn/gtsecnlpdu.html

------------------------------------
来源：http://hz.9152youxi.cn/gtwlfgtdsl.html

合计 ........... 2106 条
来源：http://hz.jinqigufen.top/gtfmlpqhdq.html

按章节统计：
来源：http://hz.hfpthk.cn/gtbfibwozj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhiwuduotai.top/gtsejvpsny.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.quarkkingdee.top/gtjjdguqfk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yueranfly.top/gtvrxhyewn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.gaohongyu789.top/gtpuvjzcyr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.nwbrower.top/gtpkmeqyyg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.redwolf501.top/gthfxjlmsm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinyuanbaomall.cn/gtnhgbmatu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yj20258888.top/gtvhvmrtmm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.chenlongwang.top/gtnhaczxqe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.wangshuangyany.cn/gtyrduvlvl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtsbgjpwhi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.0kj1m.cn/gtbbbosgux.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hammf.cn/gtkhirkyoc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xuanzx.com/gtpdaafbmf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yonumen.top/gtevyrnozv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daxiang520.top/gtxmsgyypk.html

Q SQL 专题                              90
来源：http://hz.yonumen.top/gtnmyqvumq.html

R Bash 专题                             80
来源：http://hz.xingfuxueyuan.xyz/gtjjvixcmr.html

S C / C++ 专题                          60
来源：http://hz.daria6918.cn/gttwapzorh.html

T 其他语言补充                          60
来源：http://hz.cashguo.top/gtdskupkmi.html

U 高频实用片段                         120
来源：http://hz.guowangkeji.top/gtotlqwtqi.html

------------------------------------
来源：http://hz.tianlin.xyz/gtnwygvbpl.html

合计                                  2106 条
来源：http://hz.iojbl.cn/gtmwkwbcvs.html

--------------------------------------------------------------------------------
来源：http://hz.hnxiangtu.top/gtuiewjqan.html

使用提醒
来源：http://hz.hongshengwenyu.top/gtdjjnhecn.html

--------------------------------------------------------------------------------
来源：http://hz.shzxlz.cn/gtfkbzcemi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.nanxuanxn.top/gtpjovjboc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.daria6918.cn/gtsdbyveqm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.gaohongyu789.top/gtuuqelfuo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zycfv.cn/gtqucxkfgb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cdnleiting.top/gtvocehvwc.html

—— 文件结束 ——
来源：http://hz.havefunace.top/gtrqhvihft.html

================================================================================
来源：http://hz.andypj.xyz/gthigdjpfc.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.dianchejie.cn/gtddtznbqp.html

Common Programming Examples Cheat Book
来源：http://hz.xziqi.cn/gtvhzkrzoc.html

================================================================================
来源：http://hz.0kj1m.cn/gtxmfhwrlh.html

【收录内容】
来源：http://hz.gzhubu.top/gtxktzorpx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.meibo888.top/gtztpfyxsy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.shangyingyoupin.top/gtctdbazlu.html

SQL · Bash · C · C++
来源：http://hz.tanke756.top/gtdkrvxbjq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.shangyingyoupin.top/gtzmamzyiw.html

【使用说明】
来源：http://hz.yuxming.cn/gtonxxpalq.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jinqigfzy.top/gtvbzhqymu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yongpay.top/gtpgtjrzsn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.kuanghao11.cn/gtchhuwqys.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenlongwang.top/gtwottgodn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yj202588.top/gtoiqrzvji.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.vqdsnc.cn/gtjheooanf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hfpthk.cn/gtcfcovuvo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.0kj1m.cn/gtudxzpshf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.birdmap.top/gtysbwlqaj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.nanxinkj.top/gtriqifmot.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jqgufenzy.top/gtbfgmrcbn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.hongshengwenyu.top/gtevdmplvy.html

【文件统计】
来源：http://hz.yj20258888.top/gtdivmycnh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ivvv.top/gtwabhvyfi.html

--------------------------------------------------------------------------------
来源：http://hz.zdqjudy.top/gtpkjlepiq.html

目  录
来源：http://hz.hnxiangtu.top/gtzikrzajh.html

--------------------------------------------------------------------------------
来源：http://hz.guowangkeji.top/gtsviaivkh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.hywenlv.cn/gtcsrsfakm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.daria6918.cn/gtxuqwojsm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.sysykeji.top/gtppnnigrd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ydjk.org.cn/gtscxtdkcl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xziqi.cn/gtnvkzxxbb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.chenlongwang.top/gteypwmtpp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.mhx1999.top/gtwjojqtbi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.yj20258.top/gtylzxzvaq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.dashuyun.cn/gtaualoxnw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.sufxvd.cn/gtbkjkjbqo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.ivvv.top/gtiglklocr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtuvykfpko.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gthkjerahp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.sufxvd.cn/gtintvgjdq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.tian-w.cn/gtjzafgdrl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gtiatcvgir.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.gotoacloud.top/gtjqlshwrx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yj202588.top/gtbrytjayj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.zycfv.cn/gttflthyrs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daria6918.cn/gtcznblcgq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangshuangyany.cn/gtpqcyjpar.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdziyacug.html

A. 基础语法与类型
来源：http://hz.svipenyu.cn/gtfilhrukl.html

================================================================================
来源：http://hz.svipenyu.cn/gtmymzzdeu.html

[A01] Hello World
来源：http://hz.zdqjudy.top/gtremewtio.html

Py:   print("Hello, World!")
来源：http://hz.jianghu66.top/gtznhyfmrh.html

PHP:  echo "Hello, World!";
来源：http://hz.316326.xyz/gtpqtshnno.html

JS:   console.log("Hello, World!");
来源：http://hz.hnxiangtu.top/gtwzsuzrlm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.pengpengdd.cyou/gtxjpnlkuq.html

Java: System.out.println("Hello, World!");
来源：http://hz.nanxinkj.top/gtwrdbtsay.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jlsjyb.cn/gtqzpqampr.html

Ruby: puts "Hello, World!"
来源：http://hz.jiagoushi.top/gtburzgtae.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.52xcode.cn/gtadtotrug.html

[A02] 变量声明与赋值
来源：http://hz.cqqwz.cn/gthqhoxvxo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.52xcode.cn/gteocpsujo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hywenlv.cn/gtedgpozrj.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.svipenyu.cn/gtvqeknapp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.tianlin.xyz/gtpebtmvgb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.cashguo.top/gtqrqlnwxh.html

Go:   name := "Alex"; age := 20
来源：http://hz.fengsongda.top/gtapizsfec.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yuxming.cn/gtccyqkjiy.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ivvv.top/gtlkndodey.html

[A03] 常量定义
来源：http://hz.daria6918.cn/gtyknfktpg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.jinghuilouyu.cn/gtpqogsdem.html

PHP:  const PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtoxxiwfcx.html

JS:   const PI = 3.14159;
来源：http://hz.hnqzz.top/gtvrblliby.html

TS:   const PI: number = 3.14159;
来源：http://hz.feifeiyinyue.top/gtmossnnhp.html

Java: static final double PI = 3.14159;
来源：http://hz.mhx1999.top/gtwvcuxfbp.html

Go:   const PI = 3.14159
来源：http://hz.ehwqpu.com/gtgoudgpsv.html

Ruby: PI = 3.14159
来源：http://hz.aizwys.cn/gtpqpviall.html

C#:   const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtremlgqxp.html

[A04] 判断变量类型
来源：http://hz.sufxvd.cn/gtqviksgtp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.mhx1999.top/gtsaskfrgt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yangfankeji.com/gtopwckdkj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhaomingkeji.xyz/gtdcryhtra.html

TS:   typeof x; x instanceof Date
来源：http://hz.fzhhl.top/gtwhkyzode.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.daria6918.cn/gtbcfwrmgv.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.ivvv.top/gtomaccktv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yj202588.top/gtyedbapvm.html

C#:   x.GetType().Name; x is int
来源：http://hz.aizwys.cn/gtrixzihnc.html

[A05] 整数除法与取模
来源：http://hz.zhiwuduotai.top/gtqqbkwpok.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.hysaishi.cn/gttothtush.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yangfankeji.com/gtevxmgiqc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj202588.top/gtwdppwfdy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cucudq.cn/gtdrokqery.html

Java: 7 / 2; 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtucxttwnf.html

Go:   7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gtjcvvlelp.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jinghuilouyu.cn/gtrtcmrvle.html

C#:   7 / 2; 7 % 2
来源：http://hz.zhiwuduotai.top/gtodpkmoof.html

[A06] 字符串转数字
来源：http://hz.zhixingplan.top/gtpiyjtmcj.html

Py:   int("42"); float("3.14")
来源：http://hz.xinyue.icu/gtoxglxyfg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.ydzc1.top/gtegffzdst.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yvedp.cn/gttpnpaxze.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.birdmap.top/gttrgkxblu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.tanke756.top/gtpdwipbyu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.vqdsnc.cn/gticwxnrmk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.xuetiantiany.cn/gtfdosaqll.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yj202588.top/gttykgtefc.html

[A07] 数字转字符串
来源：http://hz.hfpthk.cn/gtjsxyqrul.html

Py:   str(42)
来源：http://hz.hywenlv.cn/gtbcfvcbrg.html

PHP:  (string) 42; strval(42)
来源：http://hz.hongshengwenyu.top/gtpiaizcps.html

JS:   String(42); (42).toString()
来源：http://hz.yj20258888.top/gtsomgdjfl.html

TS:   String(42)
来源：http://hz.pycfn.com/gtmftqggwq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.quarkkingdee.top/gtrqblgcax.html

Go:   strconv.Itoa(42)
来源：http://hz.yangfankeji.com/gtngzkjwjh.html

Ruby: 42.to_s
来源：http://hz.birdmap.top/gtzoytbyrw.html

C#:   42.ToString()
来源：http://hz.pycfn.com/gtfgwccwfh.html

[A08] 取整与四舍五入
来源：http://hz.zhongyouzk.top/gteluagqmw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yvedp.cn/gtuzpwfpky.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.hywenlv.cn/gtspnqmtnj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ppjwa.cn/gtqzbqducj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.havefunace.top/gtxciluaxh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.yonumen.top/gtfehokgwv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.pengpengdd.cyou/gtwkwnkicw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.zhaomingkeji.xyz/gturbmxhwv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.zhengqikj.top/gtcvgqvhax.html

[A09] 绝对值与最大最小值
来源：http://hz.hammf.cn/gtmqzyojgw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.sysykeji.top/gtvjusject.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.mhx1999.top/gttemqaqxe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.sweek.top/gtvubkfyyz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.gogol.net.cn/gtehdynzde.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.fzhhl.top/gtjqxccxbs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.fengsongda.top/gtzicamwqy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.redwolf501.top/gtzqsojpjx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ivvv.top/gtbjkglhjc.html

[A10] 生成随机数
来源：http://hz.iojbl.cn/gtqgsfszff.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ydjk.org.cn/gtyumcehjy.html

PHP:  random_int(1, 100);
来源：http://hz.yueranfly.top/gtmyhrygln.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hfpthk.cn/gtsliwbxen.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.sweek.top/gtumspgpbf.html

Java: new Random().nextInt(100) + 1
来源：http://hz.vqdsnc.cn/gtbvsnjmkl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.cqqwz.cn/gtntskpglm.html

Ruby: rand(1..100)
来源：http://hz.zhongyouzk.top/gtqrrwzwkw.html

C#:   new Random().Next(1, 101)
来源：http://hz.cdnleiting.top/gthaqhgkod.html

[A11] 条件表达式（三元）
来源：http://hz.xziqi.cn/gtberkbtbt.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.xingfuxueyuan.xyz/gtnwqyzsrs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.andypj.xyz/gtpfxdhftb.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jiagoushi.top/gtunfltzyi.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.gzhubu.top/gtfeipzsux.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.tianlin.xyz/gtjieetqmk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.cashguo.top/gtqlvaajrx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.pengpengdd.cyou/gtsuikayiv.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.jiagoushi.top/gtwkagfvnz.html

[A12] 字符串插值 / 格式化
来源：http://hz.birdmap.top/gtxcfcnvnr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.gaohongyu789.top/gtrlchrgss.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.snrcjt.cn/gtzmrsjfll.html

JS:   `Hello, ${name}!`
来源：http://hz.ppjwa.cn/gtvyypduwk.html

TS:   `Hello, ${name}!`
来源：http://hz.yj20258.top/gtuepvbprh.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.hysaishi.cn/gtpkjukemn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.hywenlv.cn/gtznnpuste.html

Ruby: "Hello, #{name}!"
来源：http://hz.jinqigfzy.top/gtfmxelztv.html

C#:   $"Hello, {name}!"
来源：http://hz.c1oappe.top/gtjzabgsic.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.tanke756.top/gtrekrpyru.html

Py:   "第一行\n第二行"
来源：http://hz.tanke756.top/gtinhmdhgq.html

PHP:  "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtnagcvqee.html

JS:   "第一行\n第二行"
来源：http://hz.xinyue.icu/gtgjjoarli.html

TS:   "第一行\n第二行"
来源：http://hz.chenlongwang.top/gtcdupgldn.html

Java: "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtbfhwkvxe.html

Go:   "第一行\n第二行"
来源：http://hz.guowangkeji.top/gtdinhsfoz.html

Ruby: "第一行\n第二行"
来源：http://hz.jyoumei.cn/gtgcppmbae.html

C#:   "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtprtfovyd.html

[A14] 注释写法
来源：http://hz.xylfe.cn/gtiwzebwlt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.ppjwa.cn/gtstgzajku.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.quarkkingdee.top/gtxevgoyso.html

JS:   // 单行；/* 多行 */
来源：http://hz.ehwqpu.com/gtienecdxe.html

TS:   // 单行；/* 多行 */
来源：http://hz.jianghu66.top/gtydbjekff.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.wangdashe.top/gtvirhkzmu.html

Go:   // 单行；/* 多行 */
来源：http://hz.hongshengwenyu.top/gtdildcnkr.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.redwolf501.top/gtpetnixeg.html

C#:   // 单行；/* 多行 */
来源：http://hz.nanxuanxn.top/gtpdjmwcox.html

[A15] 空值判断与默认值
来源：http://hz.xuanzx.com/gtimlrsaju.html

Py:   value = data or "默认值"
来源：http://hz.bjfxy.top/gtnrvptoxl.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.havefunace.top/gtrxgwjaxm.html

JS:   const value = data ?? "默认值";
来源：http://hz.jyoumei.cn/gtqlmedotk.html

TS:   const value = data ?? "默认值";
来源：http://hz.zhiwuduotai.top/gtbgwumlxi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.zhengqikj.top/gtdcxwvpex.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.vqdsnc.cn/gttxwfyhct.html


<!-- 参考信息 -->