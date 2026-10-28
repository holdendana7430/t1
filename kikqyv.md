代发 wailian999

[U91] JS：对象键值遍历
来源：http://hz.fengsongda.top/gtlnovnfdr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jianghu66.top/gtydchyzow.html

[U92] JS：深拷贝
来源：http://hz.sweek.top/gtlgzzmfkj.html

structuredClone(obj)
来源：http://hz.pycfn.com/gtlzjwugte.html

[U93] JS：模板字符串
来源：http://hz.yanxiufei.cn/gtimqbjqns.html

`共 ${n} 条`
来源：http://hz.zhijiandao.cn/gthqpqkvlm.html

[U94] JS：箭头函数
来源：http://hz.chenzaomai.com/gtageekgfl.html

const double = x => x * 2;
来源：http://hz.hnqzz.top/gtnallvfad.html

[U95] JS：Promise 包装
来源：http://hz.zycfv.cn/gtjolwjmqg.html

new Promise((resolve, reject) => {})
来源：http://hz.hammf.cn/gtjjglxwiy.html

[U96] JS：async/await 与异常
来源：http://hz.pengpengdd.cyou/gtmsseqynv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtlkjokgrj.html

[U97] JS：并发请求
来源：http://hz.shangyingyoupin.top/gtgzldnnpy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.snrcjt.cn/gtpvycnxim.html

[U98] JS：fetch 带 JSON
来源：http://hz.haohaochexian.top/gtvnxubmfu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.jinghuilouyu.cn/gthkhvzyam.html

[U99] JS：事件监听
来源：http://hz.birdmap.top/gtgphnmsae.html

el.addEventListener("click", e => {})
来源：http://hz.zhoulong.xyz/gtrlvqfley.html

[U100] JS：DOM 查询
来源：http://hz.iojbl.cn/gtezjfezwv.html

document.querySelector(".item")
来源：http://hz.ppjwa.cn/gtcpvrklld.html

[U101] JS：classList 操作
来源：http://hz.nanxinkj.top/gtrghqefwo.html

el.classList.toggle("active")
来源：http://hz.guowangkeji.top/gtqhbuclmi.html

[U102] JS：本地存储
来源：http://hz.havefunace.top/gtwvtbwzvc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.chenlongwang.top/gtkwszkbmw.html

[U103] JS：定时器
来源：http://hz.chenjidiqi.icu/gtfvzysnwi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yj20258888.top/gtptholdel.html

[U104] JS：防抖
来源：http://hz.hfpthk.cn/gtevsmqqse.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.cdnleiting.top/gtdufpcrtg.html

[U105] JS：节流
来源：http://hz.hfpthk.cn/gtstliuwbd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.xinyue.icu/gtjmkoxzez.html

[U106] JS：日期格式化
来源：http://hz.yvedp.cn/gtdimhhimu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.dianchejie.cn/gttqlhijmz.html

[U107] JS：数字千分位
来源：http://hz.tian-w.cn/gtiqnqkhdq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yanxiufei.cn/gtcccftgqj.html

[U108] JS：随机整数
来源：http://hz.cashguo.top/gtwktbwzkp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.nanxinkj.top/gtczwvngiz.html

[U109] JS：数组分组
来源：http://hz.bjfxy.top/gtvbylepau.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangkeji.top/gtgheynnqh.html

[U110] JS：数组分块
来源：http://hz.pycfn.com/gtdbikogjr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.xylfe.cn/gtrdjavbtz.html

[U111] JS：对象转 Map
来源：http://hz.ydjk.org.cn/gtrmokzjtl.html

new Map(Object.entries(obj))
来源：http://hz.shangyingyoupin.top/gtubnbzmve.html

[U112] JS：字符串补位
来源：http://hz.svipenyu.cn/gtrqgxljja.html

"7".padStart(3, "0")
来源：http://hz.shuidangran.top/gtxtxnhbju.html

[U113] JS：正则替换全部
来源：http://hz.haohaochexian.top/gtyndmidvk.html

s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtqcyqfwqg.html

[U114] JS：JSON 深比较
来源：http://hz.xuetiantiany.cn/gtkwkxbpcf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.chenzaomai.com/gtmfnwdajj.html

[U115] JS：生成 UUID
来源：http://hz.cucudq.cn/gtgyaqplai.html

crypto.randomUUID()
来源：http://hz.yj20258888.top/gtljjgmxsh.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.meibo888.top/gtsuvodknd.html

/** @param {string} name */ function f(name) {}
来源：http://hz.chenlongwang.top/gtobqiwdnt.html

[U117] JS：单元测试
来源：http://hz.cheryme.top/gtnjyzekfp.html

npm i -D vitest;  npx vitest
来源：http://hz.pengpengdd.cyou/gtrtvijrnv.html

[U118] JS：开发服务器
来源：http://hz.zhaomingkeji.xyz/gtlmpgwhtm.html

npm i -D vite;  npx vite
来源：http://hz.nanxinkj.top/gtstzfyujx.html

[U119] JS：生产构建
来源：http://hz.jqgufenzy.top/gtyjrgsxgj.html

npx vite build
来源：http://hz.chenlongwang.top/gthjjszwty.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gotoacloud.top/gtnybnqqhl.html

import.meta.env.VITE_API_URL
来源：http://hz.ivvv.top/gtbpzyuahp.html

================================================================================
来源：http://hz.yj202588.top/gthrcpzyfn.html

统计汇总
来源：http://hz.fzhhl.top/gtvcdreadl.html

================================================================================
来源：http://hz.hnxiangtu.top/gtcwgbpyxm.html

按语言统计（条）：
来源：http://hz.jianghu66.top/gtzczznuib.html

Python ......... 252
来源：http://hz.jyoumei.cn/gtimezdcjd.html

PHP ............ 252
来源：http://hz.ppjwa.cn/gtwvhkgovh.html

JavaScript ..... 252
来源：http://hz.snrcjt.cn/gtutgmhens.html

TypeScript ..... 212
来源：http://hz.havefunace.top/gtypjlywmg.html

Java ........... 212
来源：http://hz.nwbrower.top/gtvgrjlade.html

Go ............. 212
来源：http://hz.fengsongda.top/gtjnbvpgol.html

Ruby ........... 212
来源：http://hz.shuidangran.top/gtgozfonrc.html

C# ............. 212
来源：http://hz.kuanghao11.cn/gtjetdcusa.html

C .............. 30
来源：http://hz.shangyingyoupin.top/gtryxtijfh.html

C++ ............ 30
来源：http://hz.sufxvd.cn/gtygktsnlw.html

SQL ............ 90
来源：http://hz.ybcxt.top/gtojummdjb.html

Bash ........... 80
来源：http://hz.jqgfzy.top/gtwrcjnyox.html

Kotlin ......... 15
来源：http://hz.hnxiangtu.top/gtgbexhbzq.html

Swift .......... 15
来源：http://hz.dianchejie.cn/gtogrsdada.html

Lua ............ 10
来源：http://hz.zhengqikj.top/gtdvryivwd.html

Perl ........... 10
来源：http://hz.zhixingplan.top/gtsxznbmod.html

Scala .......... 10
来源：http://hz.zhijiandao.cn/gtkltixbts.html

------------------------------------
来源：http://hz.tianlin.xyz/gtamfttknd.html

合计 ........... 2106 条
来源：http://hz.gotoacloud.top/gtcwmjccuj.html

按章节统计：
来源：http://hz.haohaochexian.top/gtqsfogaxj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenzaomai.com/gteanxfnio.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.birdmap.top/gtdhwdygej.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yuanzhike.top/gttqrpvztd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.nanxinkj.top/gtyyeatceh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.andypj.xyz/gtonrxtqtj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yj202588.top/gtwurvhzsq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtjpnticep.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.52xcode.cn/gtvedttfip.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtgkbgborz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.aibaodan.cn/gtkalejnxk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtlvoyajep.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtxphpdswu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sysykeji.top/gtjgrjvxwa.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.wangdashe.top/gthhikceso.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.shanyushiyangtech.top/gtksderdom.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.ywan-chungtsiang.top/gtakgnfyev.html

Q SQL 专题                              90
来源：http://hz.yj20258888.top/gtlwaxltwt.html

R Bash 专题                             80
来源：http://hz.xuanzx.com/gtcovorzze.html

S C / C++ 专题                          60
来源：http://hz.jyoumei.cn/gtscrimetq.html

T 其他语言补充                          60
来源：http://hz.hnxiangtu.top/gtxpfuuyep.html

U 高频实用片段                         120
来源：http://hz.fengsongda.top/gtnvwqdlsq.html

------------------------------------
来源：http://hz.cqqwz.cn/gtrvqdnvko.html

合计                                  2106 条
来源：http://hz.nanxuanxn.top/gtlqooxwre.html

--------------------------------------------------------------------------------
来源：http://hz.ydjk.org.cn/gttiltucjc.html

使用提醒
来源：http://hz.redwolf501.top/gteqgordbw.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtipjnqzes.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.vqdsnc.cn/gtadnkwxcm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zdqjudy.top/gtslpqvlyk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jianghu66.top/gtgugfbyki.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.dashuyun.cn/gtmjctatml.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhiwuduotai.top/gtfieibpka.html

—— 文件结束 ——
来源：http://hz.vqdsnc.cn/gtgvszqlng.html

================================================================================
来源：http://hz.gaohongyu789.top/gtuqmeepid.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.andypj.xyz/gtdlueexty.html

Common Programming Examples Cheat Book
来源：http://hz.chenjidiqi.icu/gtxyhyereu.html

================================================================================
来源：http://hz.xylfe.cn/gtytuhfeom.html

【收录内容】
来源：http://hz.52xcode.cn/gttnjwlewh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.daria6918.cn/gtwumcknxc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.iojbl.cn/gtbpcmgtpr.html

SQL · Bash · C · C++
来源：http://hz.yj20258888.top/gtmygmkdof.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.jinghuilouyu.cn/gtolefhmhc.html

【使用说明】
来源：http://hz.birdmap.top/gtjulhdsvv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jinqigfzy.top/gtvqmcyckn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.nwbrower.top/gtjwhdhqro.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.xziqi.cn/gtxhyrchvl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.haohaochexian.top/gthhqmfqhh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jqgfzy.top/gtflxypkmm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.zycfv.cn/gtjaqhhnbr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.zhijiandao.cn/gtbxmpuuzo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yj20258888.top/gtdsfawzyz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yuxming.cn/gtrdfflcvg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yueranfly.top/gtokesvjrq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.nwbrower.top/gtqfszxcic.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.fzhhl.top/gtwyexrbyn.html

【文件统计】
来源：http://hz.9152youxi.cn/gtdqrvdrzg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zhijiandao.cn/gtsehtccly.html

--------------------------------------------------------------------------------
来源：http://hz.cucudq.cn/gtxekprrwq.html

目  录
来源：http://hz.fengsongda.top/gtcgahfvyh.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gttgznhirm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.wangdashe.top/gtsfgafjpk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jqgufenzy.top/gtiypoldui.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.nanxuanxn.top/gtgitcupuf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.zycfv.cn/gtmrkcugod.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.aizwys.cn/gtbvkdlymn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.shzxlz.cn/gtqeokctbl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.svipenyu.cn/gthvkerjtu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhiwuduotai.top/gtsivlluiu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cucudq.cn/gtlildcahj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.xuetiantiany.cn/gtdrjzcuip.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gtcwwlsrvv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtptilgifw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.sysykeji.top/gtyqgekzei.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yuanzhike.top/gtpzacrixt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.ydjk.org.cn/gtwbazcsfl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jqgufenzy.top/gtjkrjaglt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.aizwys.cn/gttsixwgji.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.quarkkingdee.top/gtfsowcjvh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.smart0.xyz/gtabnmjmeh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.svipenyu.cn/gtkzspxpte.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.nwbrower.top/gthsfxdvqa.html

================================================================================
来源：http://hz.zycfv.cn/gtfzwidiqe.html

A. 基础语法与类型
来源：http://hz.shzxlz.cn/gtfqfxaxfg.html

================================================================================
来源：http://hz.cucudq.cn/gtgbnlzdvv.html

[A01] Hello World
来源：http://hz.quarkkingdee.top/gtfomlntul.html

Py:   print("Hello, World!")
来源：http://hz.shanyushiyangkeji.top/gtjlaesunf.html

PHP:  echo "Hello, World!";
来源：http://hz.zycfv.cn/gtpuvknuxj.html

JS:   console.log("Hello, World!");
来源：http://hz.andypj.xyz/gtmfxestyx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ppjwa.cn/gtcjnkdxde.html

Java: System.out.println("Hello, World!");
来源：http://hz.gotoacloud.top/gtdfiwovfw.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zdqjudy.top/gtcfcinjaa.html

Ruby: puts "Hello, World!"
来源：http://hz.hysaishi.cn/gtjyabgour.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.wangdashe.top/gtzxwjugga.html

[A02] 变量声明与赋值
来源：http://hz.feifeiyinyue.top/gtmnsfzcpw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.fzhhl.top/gtvdmjlrzp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.sysykeji.top/gtslqgnzey.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.dianchejie.cn/gtinleqmqe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xylfe.cn/gtqnxtxsnt.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hongshengwenyu.top/gtnbmpmvln.html

Go:   name := "Alex"; age := 20
来源：http://hz.hongshengwenyu.top/gtvzyyfamw.html

Ruby: name = "Alex"; age = 20
来源：http://hz.mhx1999.top/gtzkdrmyvn.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.0kj1m.cn/gtnunqzdbv.html

[A03] 常量定义
来源：http://hz.cucudq.cn/gtvrvoyloo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.wangdashe.top/gttrthtced.html

PHP:  const PI = 3.14159;
来源：http://hz.zdqjudy.top/gtpczicbak.html

JS:   const PI = 3.14159;
来源：http://hz.yongpay.top/gtwqwapydh.html

TS:   const PI: number = 3.14159;
来源：http://hz.hnxiangtu.top/gtimypbzsv.html

Java: static final double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gthfznsthw.html

Go:   const PI = 3.14159
来源：http://hz.hnxiangtu.top/gtmuewpfdo.html

Ruby: PI = 3.14159
来源：http://hz.zhijiandao.cn/gtfxbueogd.html

C#:   const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtvjjycbpo.html

[A04] 判断变量类型
来源：http://hz.feifeiyinyue.top/gtfaghogaw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ehwqpu.com/gtelhmulrh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ywan-chungtsiang.top/gtplunmxoc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gogol.net.cn/gttxqlqars.html

TS:   typeof x; x instanceof Date
来源：http://hz.gzhubu.top/gtmqhjfsin.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.xingfuxueyuan.xyz/gtdalyucgb.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.sweek.top/gtvqxtmfet.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xylfe.cn/gtfxhcjxyq.html

C#:   x.GetType().Name; x is int
来源：http://hz.chenzaomai.com/gtdouiahnp.html

[A05] 整数除法与取模
来源：http://hz.cashguo.top/gtkitqmzqu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.chenzaomai.com/gtdkxyvjio.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.chenlongwang.top/gtdevetmoy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.tanke756.top/gtyompgklo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hfpthk.cn/gtrfnrwvcf.html

Java: 7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gtrzzqumtk.html

Go:   7 / 2; 7 % 2
来源：http://hz.yj20258.top/gtyxmppycz.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtqoazywwd.html

C#:   7 / 2; 7 % 2
来源：http://hz.havefunace.top/gtpaouiozx.html

[A06] 字符串转数字
来源：http://hz.nanxuanxn.top/gtjcygkxeu.html

Py:   int("42"); float("3.14")
来源：http://hz.jiagoushi.top/gteeameufw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.shanyushiyangkeji.top/gtizmflkzk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.quarkkingdee.top/gtonmwlpni.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ywan-chungtsiang.top/gtdtlojsfa.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.cdnleiting.top/gtreeiawzj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gzhubu.top/gtwcehbvsd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.yueranfly.top/gtuheppsth.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.pycfn.com/gtkhnpcqwo.html

[A07] 数字转字符串
来源：http://hz.cdnleiting.top/gtfmgupemz.html

Py:   str(42)
来源：http://hz.andypj.xyz/gtesbnkbno.html

PHP:  (string) 42; strval(42)
来源：http://hz.vqdsnc.cn/gtaqolvhak.html

JS:   String(42); (42).toString()
来源：http://hz.chenlongwang.top/gtusocchoo.html

TS:   String(42)
来源：http://hz.hnqzz.top/gthkbwwjih.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.fengsongda.top/gtenenfhpv.html

Go:   strconv.Itoa(42)
来源：http://hz.yj202588.top/gtsxlybjxr.html

Ruby: 42.to_s
来源：http://hz.hysaishi.cn/gtklnzmuzj.html

C#:   42.ToString()
来源：http://hz.fzhhl.top/gtbonpnfod.html

[A08] 取整与四舍五入
来源：http://hz.9152youxi.cn/gtmgugcmxv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.tanke756.top/gtzhzvlmni.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.jinghuilouyu.cn/gtdwydeylx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ehwqpu.com/gtnpbltgqc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.aizwys.cn/gtfkhauvot.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.ehwqpu.com/gtueeljwrg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.shuidangran.top/gtnkjtdcme.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.cucudq.cn/gtvfhurdhb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.tanke756.top/gtycphfxsv.html

[A09] 绝对值与最大最小值
来源：http://hz.chenlongwang.top/gtdnvgfbsf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ehwqpu.com/gtzymbuhch.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shanyushiyangtech.top/gtokgjdszt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.jqgfzy.top/gtyyadmcfh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shuidangran.top/gtadoudjoh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.zdqjudy.top/gtveyacwfp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.cqqwz.cn/gtlhwoeznh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.dianchejie.cn/gtiqedvzcf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.vqdsnc.cn/gtysqnfxrn.html

[A10] 生成随机数
来源：http://hz.cqqwz.cn/gtqcrqyvbd.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zycfv.cn/gtantihtmf.html

PHP:  random_int(1, 100);
来源：http://hz.ivvv.top/gthrfznxae.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yanxiufei.cn/gtvystekly.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhengqikj.top/gtmtpinnlf.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yj20258.top/gtcbhsjgbv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.daxiang520.top/gtiddqpqoh.html

Ruby: rand(1..100)
来源：http://hz.quarkkingdee.top/gttcdpgesp.html

C#:   new Random().Next(1, 101)
来源：http://hz.cashguo.top/gtexemzrbs.html

[A11] 条件表达式（三元）
来源：http://hz.sxryk.cn/gtxuocjjtq.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zycfv.cn/gtfiqsvpkt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.52xcode.cn/gtqbfkkutr.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yonumen.top/gtsgxyvyzr.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.bjfxy.top/gtkviycmgb.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.zycfv.cn/gtwwbtpuuu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.shanyushiyangkeji.top/gtbncaqfjx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.zdqjudy.top/gtmjrwrgbw.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.0kj1m.cn/gthjymkxzv.html

[A12] 字符串插值 / 格式化
来源：http://hz.0kj1m.cn/gtcydklyqu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.chenjidiqi.icu/gtvvfslhtx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.ydjk.org.cn/gtdepxzhuw.html

JS:   `Hello, ${name}!`
来源：http://hz.jinyuanbaomall.cn/gtjhsizyue.html

TS:   `Hello, ${name}!`
来源：http://hz.yangfankeji.com/gtalyddcew.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.redwolf501.top/gtxcgthmnl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.ydzc1.top/gtipmdmeys.html

Ruby: "Hello, #{name}!"
来源：http://hz.redwolf501.top/gteirdnhco.html

C#:   $"Hello, {name}!"
来源：http://hz.9152youxi.cn/gthifydggi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yongpay.top/gtybfrksko.html

Py:   "第一行\n第二行"
来源：http://hz.yj20258.top/gtvdfkbuml.html

PHP:  "第一行\n第二行"
来源：http://hz.fzhhl.top/gtxdhqezdp.html

JS:   "第一行\n第二行"
来源：http://hz.hnqzz.top/gtvfgoxslq.html

TS:   "第一行\n第二行"
来源：http://hz.cucudq.cn/gtkufaymxm.html

Java: "第一行\n第二行"
来源：http://hz.wangdashe.top/gtdporoqap.html

Go:   "第一行\n第二行"
来源：http://hz.yangfankeji.com/gtuekhrnzb.html

Ruby: "第一行\n第二行"
来源：http://hz.xingfuxueyuan.xyz/gtpnmrcygn.html

C#:   "第一行\n第二行"
来源：http://hz.ywan-chungtsiang.top/gtmrvnvbnf.html

[A14] 注释写法
来源：http://hz.ehwqpu.com/gtnlccvzcj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.hfpthk.cn/gtgkcpyjkn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.shangyingyoupin.top/gtnylymxlc.html

JS:   // 单行；/* 多行 */
来源：http://hz.shzxlz.cn/gtybsekymu.html

TS:   // 单行；/* 多行 */
来源：http://hz.birdmap.top/gtumbgslac.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.wangshuangyany.cn/gtpjtsskod.html

Go:   // 单行；/* 多行 */
来源：http://hz.316326.xyz/gtedypymlo.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.zhaomingkeji.xyz/gtfkozctsn.html

C#:   // 单行；/* 多行 */
来源：http://hz.cashguo.top/gteftycuen.html

[A15] 空值判断与默认值
来源：http://hz.nanxinkj.top/gtvtxfgtbg.html

Py:   value = data or "默认值"
来源：http://hz.gogol.net.cn/gthmaqfulg.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zhoulong.xyz/gtbupfffgg.html

JS:   const value = data ?? "默认值";
来源：http://hz.zhiwuduotai.top/gtyvtbyuql.html

TS:   const value = data ?? "默认值";
来源：http://hz.shangyingyoupin.top/gtwiitajmc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.nanxuanxn.top/gtrmqywzsx.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.xinyue.icu/gtoitffgku.html


<!-- 参考信息 -->