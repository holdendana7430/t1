代发 wailian999

[U79] PHP：静态分析
来源：http://hz.fzhhl.top/gtziplfure.html

composer require --dev phpstan/phpstan
来源：http://hz.hammf.cn/gtkfncglfv.html

[U80] PHP：代码规范修复
来源：http://hz.zdqjudy.top/gtegnfreql.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jianghu66.top/gtiggyagit.html

[U81] JS：初始化项目
来源：http://hz.haohaochexian.top/gtlqpugokf.html

npm init -y;  npm i express
来源：http://hz.bjfxy.top/gtfeguotnf.html

[U82] JS：package.json 脚本
来源：http://hz.xuetiantiany.cn/gtpdgoikxw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhaomingkeji.xyz/gtqpglwywa.html

[U83] JS：ES Module 导入导出
来源：http://hz.havefunace.top/gtglqmyhzh.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.nwbrower.top/gtniyhsbhp.html

[U84] JS：CommonJS 写法
来源：http://hz.mhx1999.top/gtowdvjzyb.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.shanyushiyangkeji.top/gttardvooq.html

[U85] JS：可选链
来源：http://hz.gotoacloud.top/gtamewfeam.html

a?.b?.c
来源：http://hz.zhixingplan.top/gtguhjmsug.html

[U86] JS：空值合并
来源：http://hz.cashguo.top/gtlcvsnqvx.html

a ?? b
来源：http://hz.chenlongwang.top/gtvtoejdfx.html

[U87] JS：解构默认值
来源：http://hz.dashuyun.cn/gtdjiswmvm.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhaomingkeji.xyz/gtpxlnmsgp.html

[U88] JS：对象展开合并
来源：http://hz.yonumen.top/gtyggjlwdn.html

{ ...a, ...b }
来源：http://hz.haohaochexian.top/gtsoytqviz.html

[U89] JS：数组去重
来源：http://hz.guannengcc.top/gtqcycimxj.html

[...new Set(arr)]
来源：http://hz.nanxuanxn.top/gtlrbinfdq.html

[U90] JS：数字数组排序
来源：http://hz.yj202588.top/gtppyfhuww.html

[...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gtqacphjff.html

[U91] JS：对象键值遍历
来源：http://hz.chenlongwang.top/gthzvklxsi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.tian-w.cn/gtukylthis.html

[U92] JS：深拷贝
来源：http://hz.yj202588.top/gthjfzhdfg.html

structuredClone(obj)
来源：http://hz.jinqigufen.top/gtctvqokqa.html

[U93] JS：模板字符串
来源：http://hz.bjfxy.top/gtfziommbg.html

`共 ${n} 条`
来源：http://hz.jinqigufen.top/gtfcanzriv.html

[U94] JS：箭头函数
来源：http://hz.haohaochexian.top/gtnvpfjign.html

const double = x => x * 2;
来源：http://hz.sweek.top/gtxkcwkkpy.html

[U95] JS：Promise 包装
来源：http://hz.zhijiandao.cn/gtwygrasfb.html

new Promise((resolve, reject) => {})
来源：http://hz.0kj1m.cn/gtdcbaqnqp.html

[U96] JS：async/await 与异常
来源：http://hz.cqqwz.cn/gtddgkchiu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtfhmfgzsw.html

[U97] JS：并发请求
来源：http://hz.yj202588.top/gtlgwufwmm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtpcozlpaz.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhoulong.xyz/gtbvdyiaze.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.nwbrower.top/gtvbwmlgmm.html

[U99] JS：事件监听
来源：http://hz.snrcjt.cn/gtziolyqhr.html

el.addEventListener("click", e => {})
来源：http://hz.mhx1999.top/gtbfrojltn.html

[U100] JS：DOM 查询
来源：http://hz.jinqigufen.top/gtkefcqhjp.html

document.querySelector(".item")
来源：http://hz.nanxuanxn.top/gttcdfvsmz.html

[U101] JS：classList 操作
来源：http://hz.xingfuxueyuan.xyz/gtozgkeerj.html

el.classList.toggle("active")
来源：http://hz.gzhubu.top/gtdnoncjiy.html

[U102] JS：本地存储
来源：http://hz.zhoulong.xyz/gtcknhmbmo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.redwolf501.top/gtehgecpdw.html

[U103] JS：定时器
来源：http://hz.shanyushiyangtech.top/gtcgjnoosh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jqgufenzy.top/gtbcchjwnu.html

[U104] JS：防抖
来源：http://hz.andypj.xyz/gtdwvhwfww.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.xziqi.cn/gtdtiosbib.html

[U105] JS：节流
来源：http://hz.pycfn.com/gtigekuvby.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.ywan-chungtsiang.top/gtmquoewsd.html

[U106] JS：日期格式化
来源：http://hz.sxryk.cn/gtjlmjvgfj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.9152youxi.cn/gtptcqxqho.html

[U107] JS：数字千分位
来源：http://hz.zdqjudy.top/gtfgyykoik.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.daria6918.cn/gtwbztueea.html

[U108] JS：随机整数
来源：http://hz.shanyushiyangtech.top/gtcnohnizw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yangfankeji.com/gtzklsshxt.html

[U109] JS：数组分组
来源：http://hz.cdnleiting.top/gtzzmjcfdc.html

Object.groupBy(arr, x => x.type)
来源：http://hz.andypj.xyz/gteihgqxtd.html

[U110] JS：数组分块
来源：http://hz.zhoulong.xyz/gtagghwigr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.zhixingplan.top/gtqkqcvhyc.html

[U111] JS：对象转 Map
来源：http://hz.yj20258.top/gtngzsaxwg.html

new Map(Object.entries(obj))
来源：http://hz.aizwys.cn/gtyjdqbiwa.html

[U112] JS：字符串补位
来源：http://hz.zhaomingkeji.xyz/gtmcjowgrq.html

"7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtytxeajwv.html

[U113] JS：正则替换全部
来源：http://hz.yonumen.top/gtkybgokvo.html

s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gttngafsvc.html

[U114] JS：JSON 深比较
来源：http://hz.ydjk.org.cn/gtfhrxgeyb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.gaohongyu789.top/gtxtiuxymz.html

[U115] JS：生成 UUID
来源：http://hz.iojbl.cn/gttmzzpuso.html

crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtqyscsrus.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.chenlongwang.top/gtuobdursj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.zhixingplan.top/gtahalrypt.html

[U117] JS：单元测试
来源：http://hz.wangshuangyany.cn/gtvqrwewpx.html

npm i -D vitest;  npx vitest
来源：http://hz.yongpay.top/gtqlknvbcw.html

[U118] JS：开发服务器
来源：http://hz.xziqi.cn/gtodewjqab.html

npm i -D vite;  npx vite
来源：http://hz.yuxming.cn/gtczfyhauh.html

[U119] JS：生产构建
来源：http://hz.bjfxy.top/gtpyzzypdq.html

npx vite build
来源：http://hz.vqdsnc.cn/gtvkfloqyr.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gogol.net.cn/gtoxrccywz.html

import.meta.env.VITE_API_URL
来源：http://hz.gotoacloud.top/gtufyxqrpe.html

================================================================================
来源：http://hz.jinqigufen.top/gtybcxcdnq.html

统计汇总
来源：http://hz.xziqi.cn/gtradqluhv.html

================================================================================
来源：http://hz.nanxuanxn.top/gtburayzsc.html

按语言统计（条）：
来源：http://hz.ppjwa.cn/gtazttgvhs.html

Python ......... 252
来源：http://hz.daria6918.cn/gtwcoxmwoq.html

PHP ............ 252
来源：http://hz.svipenyu.cn/gtiktvrupg.html

JavaScript ..... 252
来源：http://hz.gaohongyu789.top/gtumkwvtan.html

TypeScript ..... 212
来源：http://hz.ivvv.top/gteshdbaaq.html

Java ........... 212
来源：http://hz.svipenyu.cn/gtksgthual.html

Go ............. 212
来源：http://hz.feifeiyinyue.top/gtylfykvqz.html

Ruby ........... 212
来源：http://hz.0kj1m.cn/gtopxorirz.html

C# ............. 212
来源：http://hz.yj20258.top/gtvovwfygj.html

C .............. 30
来源：http://hz.yj20258888.top/gtydnqtydp.html

C++ ............ 30
来源：http://hz.yuanzhike.top/gteowexocb.html

SQL ............ 90
来源：http://hz.hywenlv.cn/gtihjnbury.html

Bash ........... 80
来源：http://hz.zdqjudy.top/gtobtpdlar.html

Kotlin ......... 15
来源：http://hz.quarkkingdee.top/gtkcbtdxso.html

Swift .......... 15
来源：http://hz.hywenlv.cn/gtotjkvhkl.html

Lua ............ 10
来源：http://hz.nwbrower.top/gtqbvmtxie.html

Perl ........... 10
来源：http://hz.nanxuanxn.top/gtwbfzieau.html

Scala .......... 10
来源：http://hz.jinqigufen.top/gtzlimirnk.html

------------------------------------
来源：http://hz.jinghuilouyu.cn/gtkxccuyql.html

合计 ........... 2106 条
来源：http://hz.tian-w.cn/gtrommmmyk.html

按章节统计：
来源：http://hz.shangyingyoupin.top/gtrphzrqmf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.gogol.net.cn/gtbgihznxj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gtnkrskogp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jianghu66.top/gtwriublbh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zycfv.cn/gtgvfgphmn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.cucudq.cn/gtzsrseazr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.smart0.xyz/gtwabnuohc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.ivvv.top/gtypnwgfhu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.tian-w.cn/gtjvvltlcl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.svipenyu.cn/gtxcikiucd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.dashuyun.cn/gtwhjsiifo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtctvuriha.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtkjcewlpd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.gzhubu.top/gtrxoudasy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.sxryk.cn/gtjpatmpip.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.svipenyu.cn/gtbwxtkjob.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtudoizsoj.html

Q SQL 专题                              90
来源：http://hz.daria6918.cn/gthqlvziyn.html

R Bash 专题                             80
来源：http://hz.bjfxy.top/gtglffjeuy.html

S C / C++ 专题                          60
来源：http://hz.aibaodan.cn/gtooqqgbjo.html

T 其他语言补充                          60
来源：http://hz.ydzc1.top/gtgizbtzgt.html

U 高频实用片段                         120
来源：http://hz.jinqigufen.top/gtfcfgkmux.html

------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtunjkofjg.html

合计                                  2106 条
来源：http://hz.yvedp.cn/gtsjyykoqg.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtvbzpxnkr.html

使用提醒
来源：http://hz.chenzaomai.com/gtjywwytna.html

--------------------------------------------------------------------------------
来源：http://hz.fzhhl.top/gtrfezwrma.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.hammf.cn/gtdsizxlhv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.xuetiantiany.cn/gtgvlabhsj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cashguo.top/gtthzeeuve.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sysykeji.top/gtuhwwnpzl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.sxryk.cn/gtuvviuafa.html

—— 文件结束 ——
来源：http://hz.sysykeji.top/gtquhozhou.html

================================================================================
来源：http://hz.gaohongyu789.top/gtletyhfqb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tanke756.top/gtipxsczxx.html

Common Programming Examples Cheat Book
来源：http://hz.vqdsnc.cn/gtoljedock.html

================================================================================
来源：http://hz.gaohongyu789.top/gtrevsjgol.html

【收录内容】
来源：http://hz.xuetiantiany.cn/gtstmxopul.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.svipenyu.cn/gtvydmeofq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zdqjudy.top/gtfkqypqao.html

SQL · Bash · C · C++
来源：http://hz.haohaochexian.top/gtpmphymka.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cucudq.cn/gtfjzpaqsn.html

【使用说明】
来源：http://hz.wangdashe.top/gtkrbwyuby.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.gzhubu.top/gtvhyakaxw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.yj20258.top/gthpzzzxdo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.sxryk.cn/gtdzngtcjj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.chenzaomai.com/gtsdpfvjzq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.hfpthk.cn/gtwumfmjjz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jinqigfzy.top/gtetlqhinj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yj202588.top/gtjqtrrbwk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jqgufenzy.top/gtwewufkak.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinqigfzy.top/gttdtmcovm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.haohaochexian.top/gtkvzuxqrx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.chenjidiqi.icu/gtkmsomdxw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.sweek.top/gtzgjecean.html

【文件统计】
来源：http://hz.316326.xyz/gtdkziftmk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.yvedp.cn/gtqmnoegxq.html

--------------------------------------------------------------------------------
来源：http://hz.vqdsnc.cn/gtemlkcpld.html

目  录
来源：http://hz.yueranfly.top/gtubqlxefu.html

--------------------------------------------------------------------------------
来源：http://hz.gaohongyu789.top/gtycagrkds.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.svipenyu.cn/gtjldnopnu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.vqdsnc.cn/gtvguvjcwe.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.shanyushiyangkeji.top/gtnspmcukn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.gaohongyu789.top/gtvcrfnsqw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.shangyingyoupin.top/gtqetdrwdx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhongyouzk.top/gtjgsqnqft.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yueranfly.top/gtumsrisga.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.hysaishi.cn/gtpavdfmho.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.quarkkingdee.top/gteriszdih.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jianghu66.top/gtgtlbnkff.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gtjgpufskg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.tian-w.cn/gtonajtuji.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhixingplan.top/gtzfvmxwrt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yonumen.top/gtyechdrfj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.316326.xyz/gtclbstngl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.c1oappe.top/gtzmkdqzhh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jinqigufen.top/gtjsohtywq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.shanyushiyangkeji.top/gtdotkaixm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.shangyingyoupin.top/gttbiwnttu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fzhhl.top/gtsgbzanam.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.mhx1999.top/gthzfgjkpx.html

================================================================================
来源：http://hz.vqdsnc.cn/gtngndgedl.html

A. 基础语法与类型
来源：http://hz.wangdashe.top/gtvfjmyqkk.html

================================================================================
来源：http://hz.zhengqikj.top/gtdgcvlwbw.html

[A01] Hello World
来源：http://hz.zhaomingkeji.xyz/gtisaoqabe.html

Py:   print("Hello, World!")
来源：http://hz.gogol.net.cn/gtgrxpzctz.html

PHP:  echo "Hello, World!";
来源：http://hz.jqgufenzy.top/gtybshmhaq.html

JS:   console.log("Hello, World!");
来源：http://hz.iojbl.cn/gtxdkdnjaz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.smart0.xyz/gtdlbidovm.html

Java: System.out.println("Hello, World!");
来源：http://hz.snrcjt.cn/gtzugdzjib.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.sufxvd.cn/gtnoggxvja.html

Ruby: puts "Hello, World!"
来源：http://hz.zhiwuduotai.top/gtxyrydmaq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ydjk.org.cn/gtvlotpfnk.html

[A02] 变量声明与赋值
来源：http://hz.yj20258888.top/gtbkeugvza.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.bjfxy.top/gtilsvxhlz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.yvedp.cn/gtjbjumqiv.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.cashguo.top/gtrhtlzkbc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jyoumei.cn/gttyxmotyb.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.dashuyun.cn/gtqzvuetuh.html

Go:   name := "Alex"; age := 20
来源：http://hz.zycfv.cn/gtlugayodb.html

Ruby: name = "Alex"; age = 20
来源：http://hz.xuetiantiany.cn/gtvywduoij.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.wangdashe.top/gtshbgpeaa.html

[A03] 常量定义
来源：http://hz.ywan-chungtsiang.top/gtuobxxnsp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhongyouzk.top/gtfktyymzz.html

PHP:  const PI = 3.14159;
来源：http://hz.daxiang520.top/gtggobqapo.html

JS:   const PI = 3.14159;
来源：http://hz.c1oappe.top/gtkszhdszw.html

TS:   const PI: number = 3.14159;
来源：http://hz.yuxming.cn/gtemcristy.html

Java: static final double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtawlcducw.html

Go:   const PI = 3.14159
来源：http://hz.cqqwz.cn/gtsrwjzolk.html

Ruby: PI = 3.14159
来源：http://hz.zycfv.cn/gtiwclmmxw.html

C#:   const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtizovtvik.html

[A04] 判断变量类型
来源：http://hz.hammf.cn/gtjclofpth.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.gogol.net.cn/gtrhqgkwqj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhoulong.xyz/gtrrgdxjlu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.haohaochexian.top/gtgabxsaah.html

TS:   typeof x; x instanceof Date
来源：http://hz.shzxlz.cn/gtacdxtoiv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.mhx1999.top/gtyeuphtcn.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.iojbl.cn/gtanupqdhe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.ydzc1.top/gtawuqshoi.html

C#:   x.GetType().Name; x is int
来源：http://hz.yvedp.cn/gttzkmchdt.html

[A05] 整数除法与取模
来源：http://hz.guowangkeji.top/gtsanpdslk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.mhx1999.top/gtxdjcyqjn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zycfv.cn/gtiehplunv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.52xcode.cn/gtqtjurahq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.fzhhl.top/gtguhpooof.html

Java: 7 / 2; 7 % 2
来源：http://hz.cucudq.cn/gtebicytsk.html

Go:   7 / 2; 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtxtnxnngx.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yuanzhike.top/gtjqktokdu.html

C#:   7 / 2; 7 % 2
来源：http://hz.cqqwz.cn/gtjygmveye.html

[A06] 字符串转数字
来源：http://hz.shzxlz.cn/gtlajxpfnl.html

Py:   int("42"); float("3.14")
来源：http://hz.guannengcc.top/gtasguimpr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.52xcode.cn/gtftxxbhlk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.sweek.top/gtxenvkbbz.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.svipenyu.cn/gtiywggcmo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.shangyingyoupin.top/gtxbrvgkqe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.316326.xyz/gtuwilzlkw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.0kj1m.cn/gtlfzzrzko.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.aizwys.cn/gtmwmsucqg.html

[A07] 数字转字符串
来源：http://hz.jinghuilouyu.cn/gtjjeizngu.html

Py:   str(42)
来源：http://hz.wangshuangyany.cn/gtzdexwbgd.html

PHP:  (string) 42; strval(42)
来源：http://hz.yonumen.top/gthxdhibal.html

JS:   String(42); (42).toString()
来源：http://hz.c1oappe.top/gtelrqayjc.html

TS:   String(42)
来源：http://hz.jlsjyb.cn/gtueugvhkj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.mhx1999.top/gtqrajnirn.html

Go:   strconv.Itoa(42)
来源：http://hz.sysykeji.top/gtfevejkdo.html

Ruby: 42.to_s
来源：http://hz.xuanzx.com/gttgesbzlf.html

C#:   42.ToString()
来源：http://hz.yuxming.cn/gtqinnmtov.html

[A08] 取整与四舍五入
来源：http://hz.cdnleiting.top/gtnwffgtoy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.316326.xyz/gtevpolwyu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yangfankeji.com/gtwdakjvnp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.snrcjt.cn/gtrhmnlrjr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yj20258888.top/gteuwxkslg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.bjfxy.top/gthzqhrayv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.bjfxy.top/gtzasoeauk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jinyuanbaomall.cn/gtxphugdpw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.cheryme.top/gtyyszbbeu.html

[A09] 绝对值与最大最小值
来源：http://hz.birdmap.top/gtpjuskxsc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cqqwz.cn/gtxetlecpo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.nwbrower.top/gtyogygxzo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.ivvv.top/gtsdsakoor.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhiwuduotai.top/gtgkyefbut.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.chenzaomai.com/gtncuosihv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yuanzhike.top/gtoypfnyqc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.xuanzx.com/gtnqngwowe.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zhongyouzk.top/gtyrprhynn.html

[A10] 生成随机数
来源：http://hz.feifeiyinyue.top/gtxyxgtbqz.html

Py:   import random; random.randint(1, 100)
来源：http://hz.yuanzhike.top/gtkmdocozp.html

PHP:  random_int(1, 100);
来源：http://hz.hysaishi.cn/gtvupdvcin.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.nanxuanxn.top/gtnjkkqdka.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.daria6918.cn/gtcvifszex.html

Java: new Random().nextInt(100) + 1
来源：http://hz.zhixingplan.top/gtiykzcxya.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.xziqi.cn/gtgbrhdxam.html

Ruby: rand(1..100)
来源：http://hz.yueranfly.top/gtwcjsjzdb.html

C#:   new Random().Next(1, 101)
来源：http://hz.chenjidiqi.icu/gtkyhcduvf.html

[A11] 条件表达式（三元）
来源：http://hz.meibo888.top/gtnandszwo.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.feifeiyinyue.top/gtcznpeyeq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.vqdsnc.cn/gtkivlflig.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jyoumei.cn/gtpnogganw.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.hysaishi.cn/gttgxolvjj.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.havefunace.top/gtwgaxhtgo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.daria6918.cn/gtugoevwgb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.cheryme.top/gtfqpovbhw.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.bjfxy.top/gtexpepruz.html

[A12] 字符串插值 / 格式化
来源：http://hz.jyoumei.cn/gthfxggsav.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.cheryme.top/gtuwkwgkdg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.kuanghao11.cn/gtggwprvwd.html

JS:   `Hello, ${name}!`
来源：http://hz.zhijiandao.cn/gthpbymmtv.html

TS:   `Hello, ${name}!`
来源：http://hz.0kj1m.cn/gtdwwbwaes.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.hfpthk.cn/gtpbqqmmbc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.c1oappe.top/gtxjwwbkap.html

Ruby: "Hello, #{name}!"
来源：http://hz.bjfxy.top/gtvhkssdpu.html

C#:   $"Hello, {name}!"
来源：http://hz.birdmap.top/gtjbknhzhc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.iojbl.cn/gtgblynawe.html


<!-- 参考信息 -->