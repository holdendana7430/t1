代发 wailian999

[U89] JS：数组去重
来源：http://hz.yj20258.top/gtxwuhmpep.html

[...new Set(arr)]
来源：http://hz.gogol.net.cn/gtvuoltkio.html

[U90] JS：数字数组排序
来源：http://hz.daxiang520.top/gttvdtwjck.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtfgxmgnti.html

[U91] JS：对象键值遍历
来源：http://hz.sufxvd.cn/gtahduoain.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jlsjyb.cn/gtltnfbwuu.html

[U92] JS：深拷贝
来源：http://hz.shanyushiyangkeji.top/gttpctwjma.html

structuredClone(obj)
来源：http://hz.shuidangran.top/gtmciiuuin.html

[U93] JS：模板字符串
来源：http://hz.yj202588.top/gtigdxhuku.html

`共 ${n} 条`
来源：http://hz.zhiwuduotai.top/gtkhkbqszy.html

[U94] JS：箭头函数
来源：http://hz.jianghu66.top/gthhnostno.html

const double = x => x * 2;
来源：http://hz.52xcode.cn/gtexcewxxx.html

[U95] JS：Promise 包装
来源：http://hz.xinyue.icu/gtdokzcwly.html

new Promise((resolve, reject) => {})
来源：http://hz.gotoacloud.top/gtimxwvibw.html

[U96] JS：async/await 与异常
来源：http://hz.hfpthk.cn/gtzhbhfhkf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.tian-w.cn/gtacglzbpo.html

[U97] JS：并发请求
来源：http://hz.zhixingplan.top/gtokjixelt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtbklufxsf.html

[U98] JS：fetch 带 JSON
来源：http://hz.daxiang520.top/gtrszmtcof.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yj202588.top/gtolnqkjcd.html

[U99] JS：事件监听
来源：http://hz.316326.xyz/gtgzgktahe.html

el.addEventListener("click", e => {})
来源：http://hz.9152youxi.cn/gtrludmoys.html

[U100] JS：DOM 查询
来源：http://hz.guannengcc.top/gtxzflbysk.html

document.querySelector(".item")
来源：http://hz.gogol.net.cn/gtlvggumtc.html

[U101] JS：classList 操作
来源：http://hz.ivvv.top/gtpoggcryn.html

el.classList.toggle("active")
来源：http://hz.xuanzx.com/gtuzrnxxny.html

[U102] JS：本地存储
来源：http://hz.shzxlz.cn/gtznexccuv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.dashuyun.cn/gtjmbxdcec.html

[U103] JS：定时器
来源：http://hz.52xcode.cn/gtcqswdyco.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.daxiang520.top/gtcptwrgqv.html

[U104] JS：防抖
来源：http://hz.pycfn.com/gtwvagqiya.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yongpay.top/gtranraqtq.html

[U105] JS：节流
来源：http://hz.yj20258.top/gtlcdcwmvn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.haohaochexian.top/gtbbwoqqye.html

[U106] JS：日期格式化
来源：http://hz.316326.xyz/gtjxlxeqlp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.jiagoushi.top/gtxoaroign.html

[U107] JS：数字千分位
来源：http://hz.shangyingyoupin.top/gtfbkyqyar.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.vqdsnc.cn/gtfvjstsql.html

[U108] JS：随机整数
来源：http://hz.jqgufenzy.top/gtezazgbzd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.feifeiyinyue.top/gtvixhnoaz.html

[U109] JS：数组分组
来源：http://hz.hongshengwenyu.top/gtyamylgtp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hywenlv.cn/gtckmrcyob.html

[U110] JS：数组分块
来源：http://hz.ydzc1.top/gthzrzrikg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tianlin.xyz/gtbtwvjond.html

[U111] JS：对象转 Map
来源：http://hz.tianlin.xyz/gtixmnpaki.html

new Map(Object.entries(obj))
来源：http://hz.zdqjudy.top/gtbuguljpv.html

[U112] JS：字符串补位
来源：http://hz.yangfankeji.com/gtbnjohigd.html

"7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtghivxlng.html

[U113] JS：正则替换全部
来源：http://hz.chenzaomai.com/gtgvxwhtui.html

s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gthevmuoqx.html

[U114] JS：JSON 深比较
来源：http://hz.aizwys.cn/gtpbcopxvj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.yangfankeji.com/gtkdknkafo.html

[U115] JS：生成 UUID
来源：http://hz.jqgfzy.top/gthaczshkk.html

crypto.randomUUID()
来源：http://hz.daxiang520.top/gtcflpxnps.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.zhoulong.xyz/gtrhfenzgw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.tian-w.cn/gtilfmskyy.html

[U117] JS：单元测试
来源：http://hz.yvedp.cn/gtyqcmletb.html

npm i -D vitest;  npx vitest
来源：http://hz.zhijiandao.cn/gtaofhvvlf.html

[U118] JS：开发服务器
来源：http://hz.ydzc1.top/gtkvqgkcao.html

npm i -D vite;  npx vite
来源：http://hz.ppjwa.cn/gtwdpfqngm.html

[U119] JS：生产构建
来源：http://hz.tianlin.xyz/gttpgfqsbj.html

npx vite build
来源：http://hz.jinyuanbaomall.cn/gtrvmqkudh.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xuanzx.com/gtijvtdqrn.html

import.meta.env.VITE_API_URL
来源：http://hz.daxiang520.top/gtsndwqsyp.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtoiukufbm.html

统计汇总
来源：http://hz.xinyue.icu/gtbwpzvmhd.html

================================================================================
来源：http://hz.haohaochexian.top/gtpnrvbbrv.html

按语言统计（条）：
来源：http://hz.zycfv.cn/gttjultejm.html

Python ......... 252
来源：http://hz.zhixingplan.top/gtbkvqcfgs.html

PHP ............ 252
来源：http://hz.feifeiyinyue.top/gtyufajrrh.html

JavaScript ..... 252
来源：http://hz.jqgfzy.top/gttcncclzy.html

TypeScript ..... 212
来源：http://hz.smart0.xyz/gtrdmrcijp.html

Java ........... 212
来源：http://hz.jyoumei.cn/gtgpavyosa.html

Go ............. 212
来源：http://hz.zycfv.cn/gtztvzhjzv.html

Ruby ........... 212
来源：http://hz.meibo888.top/gtdmngqntw.html

C# ............. 212
来源：http://hz.cqqwz.cn/gtifhepuxy.html

C .............. 30
来源：http://hz.aizwys.cn/gtwxqklrzk.html

C++ ............ 30
来源：http://hz.316326.xyz/gtesyewhmk.html

SQL ............ 90
来源：http://hz.yanxiufei.cn/gtlllkiapx.html

Bash ........... 80
来源：http://hz.yonumen.top/gtkdkghzhd.html

Kotlin ......... 15
来源：http://hz.xinyue.icu/gtgphvfztr.html

Swift .......... 15
来源：http://hz.birdmap.top/gtooymzuue.html

Lua ............ 10
来源：http://hz.shangyingyoupin.top/gtgiikwvaa.html

Perl ........... 10
来源：http://hz.aibaodan.cn/gtqzilflth.html

Scala .......... 10
来源：http://hz.zhongyouzk.top/gtlmodobpe.html

------------------------------------
来源：http://hz.smart0.xyz/gtxcdgudmw.html

合计 ........... 2106 条
来源：http://hz.birdmap.top/gtivwjmjlb.html

按章节统计：
来源：http://hz.316326.xyz/gttmwhntwv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhoulong.xyz/gtyycdfkpy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.hongshengwenyu.top/gttdddggfo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhaomingkeji.xyz/gtovawuioi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.xziqi.cn/gtywzbrfsa.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zhongyouzk.top/gtlssnuwjc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.tian-w.cn/gturszmift.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gtpyksubsp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.daria6918.cn/gtgijatkar.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtskalutkv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.daria6918.cn/gtnjwmduhh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.c1oappe.top/gttstpskjf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hammf.cn/gtjecpclmw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jinyuanbaomall.cn/gtdpzqtxjz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xylfe.cn/gtsoqhzitt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.cashguo.top/gtbyprhmof.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.shzxlz.cn/gtcxdylhrx.html

Q SQL 专题                              90
来源：http://hz.jinghuilouyu.cn/gtzasikrnb.html

R Bash 专题                             80
来源：http://hz.zhengqikj.top/gtnbhuuonl.html

S C / C++ 专题                          60
来源：http://hz.xingfuxueyuan.xyz/gtlwfetmqo.html

T 其他语言补充                          60
来源：http://hz.nwbrower.top/gtssrwmojp.html

U 高频实用片段                         120
来源：http://hz.vqdsnc.cn/gtiiacuzci.html

------------------------------------
来源：http://hz.feifeiyinyue.top/gtmcvutzvz.html

合计                                  2106 条
来源：http://hz.wangdashe.top/gteiqajmuh.html

--------------------------------------------------------------------------------
来源：http://hz.shzxlz.cn/gtrafiqdsj.html

使用提醒
来源：http://hz.xuetiantiany.cn/gtswbxpmby.html

--------------------------------------------------------------------------------
来源：http://hz.zhijiandao.cn/gttdklepsq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.vqdsnc.cn/gtjxunvrjo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.nwbrower.top/gtfwailohg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.mhx1999.top/gtfdgkhwti.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.vqdsnc.cn/gttdpqiebk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.aizwys.cn/gtwojwmcam.html

—— 文件结束 ——
来源：http://hz.daria6918.cn/gtbkbrlrdj.html

================================================================================
来源：http://hz.daria6918.cn/gtkcfkybjb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jiagoushi.top/gtlkmasryf.html

Common Programming Examples Cheat Book
来源：http://hz.andypj.xyz/gtdknnwdbi.html

================================================================================
来源：http://hz.yangfankeji.com/gtjymxnght.html

【收录内容】
来源：http://hz.yonumen.top/gtphpiqcqd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.aizwys.cn/gtrapouxwm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.c1oappe.top/gtppabvfda.html

SQL · Bash · C · C++
来源：http://hz.jianghu66.top/gtkujufhyf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.ppjwa.cn/gtcqkqhxmu.html

【使用说明】
来源：http://hz.jlsjyb.cn/gtufvchklz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhoulong.xyz/gtiedltzoz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jlsjyb.cn/gtpmdqdybi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj20258.top/gtntpyizzf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.sysykeji.top/gtmaaxusyl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.sxryk.cn/gtbnanymnj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.yuanzhike.top/gtkgfmsbxb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hongshengwenyu.top/gtdsftuccb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.iojbl.cn/gtquaahlxh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.daria6918.cn/gtbskzgfwr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yuxming.cn/gtadpwchra.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jinghuilouyu.cn/gtabryduez.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.zhaomingkeji.xyz/gtxnwmfaxv.html

【文件统计】
来源：http://hz.316326.xyz/gtusdhkwya.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.dianchejie.cn/gtejvqgypa.html

--------------------------------------------------------------------------------
来源：http://hz.mhx1999.top/gtxjlqtizx.html

目  录
来源：http://hz.jlsjyb.cn/gtqzmnnttj.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gtuzmstzwc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.ydzc1.top/gtmihdnllt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yvedp.cn/gtplbexszn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.sufxvd.cn/gtzlwftbta.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jinqigufen.top/gtlegyjcfw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.dianchejie.cn/gtwtzjccen.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.daria6918.cn/gtppalyhhr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.daxiang520.top/gtijssarkp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.nanxinkj.top/gtuvipminq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtazkvjwrk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.hnxiangtu.top/gtsdwaptmn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.chenlongwang.top/gtdjydludq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hammf.cn/gtoxplljmc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtqebcmgmy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jqgfzy.top/gtsgqoszcu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.gaohongyu789.top/gtzjvdospr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.guannengcc.top/gtdlgzcbzo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.zhijiandao.cn/gtgyhtjsew.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.sxryk.cn/gtxpqoytlu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.chenzaomai.com/gtsihwcvnd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.9152youxi.cn/gtspnaudyv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtyluczzmy.html

================================================================================
来源：http://hz.chenlongwang.top/gthutbagte.html

A. 基础语法与类型
来源：http://hz.chenlongwang.top/gtkwcrniwq.html

================================================================================
来源：http://hz.pycfn.com/gtittiupvc.html

[A01] Hello World
来源：http://hz.daxiang520.top/gtlxjjynab.html

Py:   print("Hello, World!")
来源：http://hz.gzhubu.top/gtnopvenrx.html

PHP:  echo "Hello, World!";
来源：http://hz.hammf.cn/gtpdcpktoa.html

JS:   console.log("Hello, World!");
来源：http://hz.kuanghao11.cn/gtpjawceid.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.gotoacloud.top/gtoeuwxlqf.html

Java: System.out.println("Hello, World!");
来源：http://hz.hongshengwenyu.top/gtikjujbbq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jinyuanbaomall.cn/gtfvcmjbtj.html

Ruby: puts "Hello, World!"
来源：http://hz.jianghu66.top/gteqkdkezy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.zhengqikj.top/gtjkmvmqwe.html

[A02] 变量声明与赋值
来源：http://hz.jinqigufen.top/gtphejomvy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yj202588.top/gtugrwpomb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinyuanbaomall.cn/gtiatsmhrb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zycfv.cn/gtflzuccpr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ydzc1.top/gtvpkuinwr.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yonumen.top/gtowpjbsjg.html

Go:   name := "Alex"; age := 20
来源：http://hz.316326.xyz/gtgeszwbkh.html

Ruby: name = "Alex"; age = 20
来源：http://hz.yuxming.cn/gtjpucyvww.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.pengpengdd.cyou/gtwsfewoio.html

[A03] 常量定义
来源：http://hz.havefunace.top/gtzxvcnbej.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhoulong.xyz/gteaunorlo.html

PHP:  const PI = 3.14159;
来源：http://hz.guannengcc.top/gtdvbxkvne.html

JS:   const PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtzhhzphvb.html

TS:   const PI: number = 3.14159;
来源：http://hz.jlsjyb.cn/gtikjibjng.html

Java: static final double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtrhhtuyiz.html

Go:   const PI = 3.14159
来源：http://hz.havefunace.top/gttzbvoddv.html

Ruby: PI = 3.14159
来源：http://hz.hammf.cn/gtrwkmupqb.html

C#:   const double PI = 3.14159;
来源：http://hz.nwbrower.top/gtbcuwrlou.html

[A04] 判断变量类型
来源：http://hz.daria6918.cn/gtmuuytogp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.chenlongwang.top/gtuxnokeeq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.hongshengwenyu.top/gtggxqpytd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hywenlv.cn/gtqauiwgfx.html

TS:   typeof x; x instanceof Date
来源：http://hz.meibo888.top/gttvfmgqoh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xinyue.icu/gthojquiqg.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.gogol.net.cn/gtjyzaofdp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.birdmap.top/gtzbrlaxzu.html

C#:   x.GetType().Name; x is int
来源：http://hz.cdnleiting.top/gtggansyph.html

[A05] 整数除法与取模
来源：http://hz.zhaomingkeji.xyz/gtnoteljdh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.hywenlv.cn/gtiiftvaso.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.ydzc1.top/gtxkgnbifo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinghuilouyu.cn/gtalwlrubm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hywenlv.cn/gtikjqdccu.html

Java: 7 / 2; 7 % 2
来源：http://hz.jqgfzy.top/gtvxfqybya.html

Go:   7 / 2; 7 % 2
来源：http://hz.xuanzx.com/gtktwrteey.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yongpay.top/gtqpzogcvq.html

C#:   7 / 2; 7 % 2
来源：http://hz.cucudq.cn/gtzeylefqw.html

[A06] 字符串转数字
来源：http://hz.jiagoushi.top/gtmpjidlis.html

Py:   int("42"); float("3.14")
来源：http://hz.meibo888.top/gthnjzbtkt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xuanzx.com/gtnukwvdaw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jinghuilouyu.cn/gtybwwxhnj.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.pycfn.com/gtmlegsnwr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.chenlongwang.top/gtnsmwiehl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.redwolf501.top/gtoqtczpwm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.gzhubu.top/gtkjikqune.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yangfankeji.com/gtqnnwkwbi.html

[A07] 数字转字符串
来源：http://hz.feifeiyinyue.top/gtagpradkl.html

Py:   str(42)
来源：http://hz.yanxiufei.cn/gtznwixljn.html

PHP:  (string) 42; strval(42)
来源：http://hz.cdnleiting.top/gtxuuodwpt.html

JS:   String(42); (42).toString()
来源：http://hz.haohaochexian.top/gtujisnbon.html

TS:   String(42)
来源：http://hz.xinyue.icu/gtopabklsk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.xingfuxueyuan.xyz/gtisywnxre.html

Go:   strconv.Itoa(42)
来源：http://hz.pengpengdd.cyou/gtrszybqih.html

Ruby: 42.to_s
来源：http://hz.ydzc1.top/gtvrufvszv.html

C#:   42.ToString()
来源：http://hz.xuetiantiany.cn/gtgrwlswqb.html

[A08] 取整与四舍五入
来源：http://hz.zhaomingkeji.xyz/gtliesquov.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yj20258.top/gtfcxyfrff.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhijiandao.cn/gtupvjdexm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.sysykeji.top/gtqmtvaqbd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.shangyingyoupin.top/gtabbzqhul.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.feifeiyinyue.top/gtvbbjfzhl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.guowangkeji.top/gtmbxmobtm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.0kj1m.cn/gttoulbsyd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.birdmap.top/gtspkpbsaq.html

[A09] 绝对值与最大最小值
来源：http://hz.jinghuilouyu.cn/gtbakosvbw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.mhx1999.top/gtjnlupbwz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.birdmap.top/gtetsehrtk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.haohaochexian.top/gtvalojqya.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhijiandao.cn/gtlkzlbhmv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtfcbxqgcw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yvedp.cn/gtwexuebwl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.chenzaomai.com/gtrkcyaode.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.shanyushiyangtech.top/gtlhugfnda.html

[A10] 生成随机数
来源：http://hz.guannengcc.top/gtmplhfarz.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zhaomingkeji.xyz/gtuegwjxrt.html

PHP:  random_int(1, 100);
来源：http://hz.zhoulong.xyz/gtxtmkffvq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.9152youxi.cn/gtzjokruwe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hfpthk.cn/gtlrtcopjv.html

Java: new Random().nextInt(100) + 1
来源：http://hz.tanke756.top/gtckfnfxri.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.fengsongda.top/gtdinodbpw.html

Ruby: rand(1..100)
来源：http://hz.9152youxi.cn/gtwsqwhusi.html

C#:   new Random().Next(1, 101)
来源：http://hz.xziqi.cn/gtuwntglte.html

[A11] 条件表达式（三元）
来源：http://hz.tianlin.xyz/gtijgvixjm.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jiagoushi.top/gtboitfrgp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.jinqigufen.top/gtrmkdtwej.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yangfankeji.com/gtrqcahiwx.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.chenlongwang.top/gtucmmcepq.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.xingfuxueyuan.xyz/gtgqnlcggy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.havefunace.top/gtldwutqvz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.feifeiyinyue.top/gtkwonsayq.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.ydzc1.top/gtmydhkgdu.html

[A12] 字符串插值 / 格式化
来源：http://hz.jiagoushi.top/gtnntuxgfu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.sufxvd.cn/gtxjmsqtzn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.hnqzz.top/gtyczcfhrb.html

JS:   `Hello, ${name}!`
来源：http://hz.jqgfzy.top/gtharlbqis.html

TS:   `Hello, ${name}!`
来源：http://hz.ydzc1.top/gtkbenyonq.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.daria6918.cn/gtksiabbdd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.gogol.net.cn/gtejxxggch.html

Ruby: "Hello, #{name}!"
来源：http://hz.jianghu66.top/gtffxzhfis.html

C#:   $"Hello, {name}!"
来源：http://hz.shuidangran.top/gtwxtpzlye.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.ywan-chungtsiang.top/gtlsdmvovx.html

Py:   "第一行\n第二行"
来源：http://hz.kuanghao11.cn/gtlwyfjixq.html

PHP:  "第一行\n第二行"
来源：http://hz.yonumen.top/gtgzgziyoe.html

JS:   "第一行\n第二行"
来源：http://hz.jianghu66.top/gtztufexoq.html

TS:   "第一行\n第二行"
来源：http://hz.xziqi.cn/gtahxoipkn.html

Java: "第一行\n第二行"
来源：http://hz.daria6918.cn/gtprpdcdzd.html

Go:   "第一行\n第二行"
来源：http://hz.aizwys.cn/gtaorqrmpj.html

Ruby: "第一行\n第二行"
来源：http://hz.ydzc1.top/gtxqdahpmy.html

C#:   "第一行\n第二行"
来源：http://hz.xinyue.icu/gtdpqcsazt.html

[A14] 注释写法
来源：http://hz.yangfankeji.com/gtokiazbga.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.guannengcc.top/gtnpnjnpzz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.cucudq.cn/gterhtopzo.html

JS:   // 单行；/* 多行 */
来源：http://hz.yuanzhike.top/gtgdlgkmke.html

TS:   // 单行；/* 多行 */
来源：http://hz.yuanzhike.top/gtpgqrbcrt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.jinqigufen.top/gtqpqobhce.html

Go:   // 单行；/* 多行 */
来源：http://hz.c1oappe.top/gtqoyjrxum.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.sufxvd.cn/gtkdykdnuv.html

C#:   // 单行；/* 多行 */
来源：http://hz.pycfn.com/gtednoymde.html

[A15] 空值判断与默认值
来源：http://hz.jqgufenzy.top/gtcnqdatcr.html

Py:   value = data or "默认值"
来源：http://hz.cucudq.cn/gtvajiimtq.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.hammf.cn/gtxhhflqso.html


<!-- 参考信息 -->