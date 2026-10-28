代发 wailian999

[U79] PHP：静态分析
来源：http://hz.chenjidiqi.icu/gtlkigxado.html

composer require --dev phpstan/phpstan
来源：http://hz.andypj.xyz/gtrsdbylgv.html

[U80] PHP：代码规范修复
来源：http://hz.quarkkingdee.top/gtbtibowxc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cheryme.top/gtwggkzazl.html

[U81] JS：初始化项目
来源：http://hz.yanxiufei.cn/gtaspxayzb.html

npm init -y;  npm i express
来源：http://hz.shangyingyoupin.top/gtndxtgvwi.html

[U82] JS：package.json 脚本
来源：http://hz.yongpay.top/gtrbfzsaou.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yangfankeji.com/gtaqbylknu.html

[U83] JS：ES Module 导入导出
来源：http://hz.dashuyun.cn/gtlvhqbhvn.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jyoumei.cn/gtudayxkhr.html

[U84] JS：CommonJS 写法
来源：http://hz.dianchejie.cn/gtqanbeduc.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.dashuyun.cn/gtnofxlcuq.html

[U85] JS：可选链
来源：http://hz.gogol.net.cn/gtwjojkgiv.html

a?.b?.c
来源：http://hz.cdnleiting.top/gtfkeacqif.html

[U86] JS：空值合并
来源：http://hz.cheryme.top/gtxblzjhul.html

a ?? b
来源：http://hz.bjfxy.top/gtihsmsphb.html

[U87] JS：解构默认值
来源：http://hz.hammf.cn/gtgqielfse.html

const { a = 1, b = 2 } = obj;
来源：http://hz.gogol.net.cn/gtssfxgsnd.html

[U88] JS：对象展开合并
来源：http://hz.pengpengdd.cyou/gtznxhqsri.html

{ ...a, ...b }
来源：http://hz.nanxuanxn.top/gtjtsncafy.html

[U89] JS：数组去重
来源：http://hz.0kj1m.cn/gthsavzxuv.html

[...new Set(arr)]
来源：http://hz.birdmap.top/gtfgbngfxh.html

[U90] JS：数字数组排序
来源：http://hz.9152youxi.cn/gtxgqjsjpj.html

[...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtkseumztf.html

[U91] JS：对象键值遍历
来源：http://hz.hfpthk.cn/gtcntqawrv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.tian-w.cn/gtrazcylfs.html

[U92] JS：深拷贝
来源：http://hz.fzhhl.top/gtcfzcvhdt.html

structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtlspolzvz.html

[U93] JS：模板字符串
来源：http://hz.cucudq.cn/gtcxlxzvyw.html

`共 ${n} 条`
来源：http://hz.yj202588.top/gtwjpwvabj.html

[U94] JS：箭头函数
来源：http://hz.zhaomingkeji.xyz/gtdfoovqta.html

const double = x => x * 2;
来源：http://hz.zhoulong.xyz/gthfotdnqi.html

[U95] JS：Promise 包装
来源：http://hz.dianchejie.cn/gtirkjnetr.html

new Promise((resolve, reject) => {})
来源：http://hz.yuxming.cn/gtnodordmt.html

[U96] JS：async/await 与异常
来源：http://hz.shuidangran.top/gtmtdbaxpx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhongyouzk.top/gtmplofhwk.html

[U97] JS：并发请求
来源：http://hz.chenlongwang.top/gtjtimejaq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtvgodmptz.html

[U98] JS：fetch 带 JSON
来源：http://hz.hnqzz.top/gtvkohdjyb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.shanyushiyangtech.top/gthybavtlk.html

[U99] JS：事件监听
来源：http://hz.jianghu66.top/gtjtekvnof.html

el.addEventListener("click", e => {})
来源：http://hz.nanxinkj.top/gtvbkksphs.html

[U100] JS：DOM 查询
来源：http://hz.chenlongwang.top/gtytsmdcwy.html

document.querySelector(".item")
来源：http://hz.feifeiyinyue.top/gtetysjutd.html

[U101] JS：classList 操作
来源：http://hz.sxryk.cn/gtrfnkgrcm.html

el.classList.toggle("active")
来源：http://hz.birdmap.top/gtapzervjn.html

[U102] JS：本地存储
来源：http://hz.cucudq.cn/gtsvlfcjbn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.gzhubu.top/gtiomgeuyq.html

[U103] JS：定时器
来源：http://hz.yanxiufei.cn/gtlsjztxsy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.yonumen.top/gtykcktccg.html

[U104] JS：防抖
来源：http://hz.yangfankeji.com/gtbnznqfgz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yvedp.cn/gtxfsrkszr.html

[U105] JS：节流
来源：http://hz.gogol.net.cn/gtwvliccbl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hfpthk.cn/gtiovgwzji.html

[U106] JS：日期格式化
来源：http://hz.jqgfzy.top/gtcgjzgrfn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.ybcxt.top/gtifnqnpir.html

[U107] JS：数字千分位
来源：http://hz.birdmap.top/gtjnvhcimf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.ivvv.top/gtpnwhdyui.html

[U108] JS：随机整数
来源：http://hz.yj20258.top/gtlvowhmsk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.hywenlv.cn/gthfybrsej.html

[U109] JS：数组分组
来源：http://hz.cucudq.cn/gtkiuqhqdm.html

Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gttlaftavm.html

[U110] JS：数组分块
来源：http://hz.52xcode.cn/gtzeogqvwf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.pengpengdd.cyou/gtemzoeugi.html

[U111] JS：对象转 Map
来源：http://hz.birdmap.top/gtyjrhyzam.html

new Map(Object.entries(obj))
来源：http://hz.nanxinkj.top/gtwiwkbbjg.html

[U112] JS：字符串补位
来源：http://hz.zdqjudy.top/gtxumeoinc.html

"7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtvyiizxft.html

[U113] JS：正则替换全部
来源：http://hz.sweek.top/gtenikqnjf.html

s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtcnqlgahz.html

[U114] JS：JSON 深比较
来源：http://hz.jiagoushi.top/gtrlcdnqib.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hysaishi.cn/gtmkpidbkh.html

[U115] JS：生成 UUID
来源：http://hz.xinyue.icu/gtbhjfinkd.html

crypto.randomUUID()
来源：http://hz.316326.xyz/gtelxtgdlf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jlsjyb.cn/gtuumuktmq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.wangshuangyany.cn/gtmdjfxavq.html

[U117] JS：单元测试
来源：http://hz.wangdashe.top/gtcyjbabun.html

npm i -D vitest;  npx vitest
来源：http://hz.yanxiufei.cn/gtalkcslsm.html

[U118] JS：开发服务器
来源：http://hz.cucudq.cn/gtuzpdkhws.html

npm i -D vite;  npx vite
来源：http://hz.52xcode.cn/gtonoqmzbc.html

[U119] JS：生产构建
来源：http://hz.shangyingyoupin.top/gtqkkynilv.html

npx vite build
来源：http://hz.aibaodan.cn/gtyhkgdpvy.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.feifeiyinyue.top/gtqbmipwte.html

import.meta.env.VITE_API_URL
来源：http://hz.hywenlv.cn/gtorcxrjwz.html

================================================================================
来源：http://hz.aibaodan.cn/gtcaemckxr.html

统计汇总
来源：http://hz.gogol.net.cn/gtqdoocbqu.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjhqwfmqn.html

按语言统计（条）：
来源：http://hz.cheryme.top/gtzvrpipmz.html

Python ......... 252
来源：http://hz.ppjwa.cn/gtsbrjscnx.html

PHP ............ 252
来源：http://hz.svipenyu.cn/gtysiztcbu.html

JavaScript ..... 252
来源：http://hz.jinghuilouyu.cn/gthzqnllts.html

TypeScript ..... 212
来源：http://hz.hfpthk.cn/gtzwfuywjl.html

Java ........... 212
来源：http://hz.ppjwa.cn/gtkeszxvfg.html

Go ............. 212
来源：http://hz.nwbrower.top/gtrtubeuxw.html

Ruby ........... 212
来源：http://hz.52xcode.cn/gtpusgeyum.html

C# ............. 212
来源：http://hz.guannengcc.top/gtznhauqrq.html

C .............. 30
来源：http://hz.feifeiyinyue.top/gtzqrevniu.html

C++ ............ 30
来源：http://hz.ydjk.org.cn/gtzwzgyedo.html

SQL ............ 90
来源：http://hz.birdmap.top/gtvfbuybql.html

Bash ........... 80
来源：http://hz.svipenyu.cn/gtgstnklbr.html

Kotlin ......... 15
来源：http://hz.9152youxi.cn/gteskauwoo.html

Swift .......... 15
来源：http://hz.bjfxy.top/gtnsiteckw.html

Lua ............ 10
来源：http://hz.316326.xyz/gtkytmrhta.html

Perl ........... 10
来源：http://hz.jyoumei.cn/gttlklujdf.html

Scala .......... 10
来源：http://hz.jinqigfzy.top/gtjkzfqpzs.html

------------------------------------
来源：http://hz.pengpengdd.cyou/gtrztzkvhr.html

合计 ........... 2106 条
来源：http://hz.zhoulong.xyz/gtzpekpflc.html

按章节统计：
来源：http://hz.zdqjudy.top/gtqowqlicg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.yangfankeji.com/gtjndvbbpx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhixingplan.top/gtdbmagoxy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.gogol.net.cn/gtncicvwny.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.aibaodan.cn/gthsvoojve.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hongshengwenyu.top/gtghijwcqu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.chenjidiqi.icu/gtoxrglqrd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.9152youxi.cn/gtukmmudsu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nanxinkj.top/gtpvhvoqkw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtomjyakpp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.pycfn.com/gtehfrjbxw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtccpowhqo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.fzhhl.top/gturstkrzj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gtwofdtmts.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.gotoacloud.top/gtntnaxcta.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.nanxinkj.top/gtyzokrymq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.jlsjyb.cn/gttxsmrfec.html

Q SQL 专题                              90
来源：http://hz.wangshuangyany.cn/gtjkhtmckw.html

R Bash 专题                             80
来源：http://hz.pycfn.com/gthyekpgzh.html

S C / C++ 专题                          60
来源：http://hz.zdqjudy.top/gtsnttpsqo.html

T 其他语言补充                          60
来源：http://hz.hammf.cn/gtnzqidygn.html

U 高频实用片段                         120
来源：http://hz.dianchejie.cn/gtujlioowu.html

------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtqszossws.html

合计                                  2106 条
来源：http://hz.xylfe.cn/gtrruppgjo.html

--------------------------------------------------------------------------------
来源：http://hz.gaohongyu789.top/gtrnizkgrf.html

使用提醒
来源：http://hz.hongshengwenyu.top/gttdryboxq.html

--------------------------------------------------------------------------------
来源：http://hz.xylfe.cn/gtdakrnpni.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.guowangkeji.top/gtwdtdllsd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.shangyingyoupin.top/gtbapqpsng.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.316326.xyz/gtxowijznr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.nanxinkj.top/gtvkxjjrgr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.9152youxi.cn/gtddfepvsy.html

—— 文件结束 ——
来源：http://hz.sysykeji.top/gtijqpfuik.html

================================================================================
来源：http://hz.birdmap.top/gtujawrmvr.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xuetiantiany.cn/gtnsrragph.html

Common Programming Examples Cheat Book
来源：http://hz.sweek.top/gtmyicmhpj.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtijlehsjf.html

【收录内容】
来源：http://hz.shangyingyoupin.top/gtmpjnrjvf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cheryme.top/gtqhhzimpn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.yangfankeji.com/gtugytddnb.html

SQL · Bash · C · C++
来源：http://hz.jqgfzy.top/gtxzwzrogu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yj20258.top/gtadoczxpu.html

【使用说明】
来源：http://hz.shanyushiyangkeji.top/gtvmwthejb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.aizwys.cn/gtgvjrpuuv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.daxiang520.top/gtkniofqmi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jyoumei.cn/gthaajbzpu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.xinyue.icu/gtnlhzztme.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ydjk.org.cn/gtcdyfhdht.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.birdmap.top/gtgsnagacv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yj202588.top/gtzrijhaep.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ivvv.top/gtsrkoslon.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zycfv.cn/gtuwspvnlg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.daxiang520.top/gtnpanfcdn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.wangdashe.top/gtjbbpzbmh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ivvv.top/gtovzmxczj.html

【文件统计】
来源：http://hz.zhaomingkeji.xyz/gtdhpruwhi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.chenzaomai.com/gtndgrjsnm.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtuatiadfk.html

目  录
来源：http://hz.zhengqikj.top/gtaxipzssp.html

--------------------------------------------------------------------------------
来源：http://hz.shangyingyoupin.top/gtrzawqxgn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhaomingkeji.xyz/gtxctiapih.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhengqikj.top/gtfgyikljz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yj20258888.top/gtaygelkkp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.c1oappe.top/gtzgecwzze.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.nanxuanxn.top/gtsxiwmkve.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.fengsongda.top/gtybrdmwls.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.316326.xyz/gthnurwcdv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhaomingkeji.xyz/gtzyopusea.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtlgvgwnnb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jiagoushi.top/gtibdgiiwv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.wangshuangyany.cn/gtnksfkakd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.havefunace.top/gtbfqmoajq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gtmwxlqkfp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.sweek.top/gtcqjigaxq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.52xcode.cn/gtwszluanr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtvwmpwlmx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.fzhhl.top/gtbianskdm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.fzhhl.top/gtxicavljn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.xingfuxueyuan.xyz/gtxnhmaakj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhaomingkeji.xyz/gtsfakpqfn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydzc1.top/gtfgpvxmql.html

================================================================================
来源：http://hz.cheryme.top/gtahyuamgq.html

A. 基础语法与类型
来源：http://hz.yanxiufei.cn/gtdxeujlnm.html

================================================================================
来源：http://hz.bjfxy.top/gtnzeeieny.html

[A01] Hello World
来源：http://hz.dianchejie.cn/gtmehvhldp.html

Py:   print("Hello, World!")
来源：http://hz.iojbl.cn/gtwdgfozzr.html

PHP:  echo "Hello, World!";
来源：http://hz.nanxinkj.top/gtptvbgpuk.html

JS:   console.log("Hello, World!");
来源：http://hz.ivvv.top/gtbtyqiznw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.ybcxt.top/gtiaupvzjx.html

Java: System.out.println("Hello, World!");
来源：http://hz.sweek.top/gtdsbtcczc.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.jinyuanbaomall.cn/gtnpgxrtag.html

Ruby: puts "Hello, World!"
来源：http://hz.zhongyouzk.top/gtdedyfsaa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cheryme.top/gtpealvnum.html

[A02] 变量声明与赋值
来源：http://hz.9152youxi.cn/gtgggruvhh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shzxlz.cn/gtkwwhqafc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jinghuilouyu.cn/gtuhcuqvup.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.shanyushiyangkeji.top/gtkbbasmqq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jyoumei.cn/gtehjdmbxg.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xingfuxueyuan.xyz/gteoomlnjr.html

Go:   name := "Alex"; age := 20
来源：http://hz.guannengcc.top/gtkiqhmvgd.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ydjk.org.cn/gttiqomcte.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ivvv.top/gtflvoawho.html

[A03] 常量定义
来源：http://hz.sweek.top/gtqwdagxux.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.kuanghao11.cn/gtbuuukhwa.html

PHP:  const PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gttxtqvdkn.html

JS:   const PI = 3.14159;
来源：http://hz.sxryk.cn/gtemdnagnk.html

TS:   const PI: number = 3.14159;
来源：http://hz.52xcode.cn/gtgdqnsokv.html

Java: static final double PI = 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtwsinirpk.html

Go:   const PI = 3.14159
来源：http://hz.havefunace.top/gtgdevvgrh.html

Ruby: PI = 3.14159
来源：http://hz.0kj1m.cn/gtyxciqvci.html

C#:   const double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtwgyaamya.html

[A04] 判断变量类型
来源：http://hz.jqgfzy.top/gtmdpyzwyc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinghuilouyu.cn/gttevitrcm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.zhiwuduotai.top/gtvcksixok.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.xziqi.cn/gtqkgijien.html

TS:   typeof x; x instanceof Date
来源：http://hz.daria6918.cn/gtxaiguctx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jlsjyb.cn/gtaefapnwn.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhijiandao.cn/gtilrzmrnu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.yj20258.top/gtfqudwhzq.html

C#:   x.GetType().Name; x is int
来源：http://hz.ppjwa.cn/gtdjtficsl.html

[A05] 整数除法与取模
来源：http://hz.nanxinkj.top/gtrbrorlaf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.yanxiufei.cn/gtofdmxcqz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yj20258.top/gtcmhrmgpb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.sxryk.cn/gtlaygtull.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.52xcode.cn/gtioycljov.html

Java: 7 / 2; 7 % 2
来源：http://hz.hywenlv.cn/gtdfbfcqyg.html

Go:   7 / 2; 7 % 2
来源：http://hz.nwbrower.top/gtmmjfsvvh.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.guowangkeji.top/gthnbjydyy.html

C#:   7 / 2; 7 % 2
来源：http://hz.hysaishi.cn/gthbxoehcw.html

[A06] 字符串转数字
来源：http://hz.cashguo.top/gtnrgjpgwv.html

Py:   int("42"); float("3.14")
来源：http://hz.hnqzz.top/gtvpmxcmuy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.hnqzz.top/gtnagidfcu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.yvedp.cn/gtrgipavvz.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.zhongyouzk.top/gttisqfejk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yangfankeji.com/gtbwwgweam.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.daxiang520.top/gtjzfpmxqs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.zhongyouzk.top/gtmyfqpnlp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yanxiufei.cn/gtckktppco.html

[A07] 数字转字符串
来源：http://hz.chenjidiqi.icu/gtcyybgfcn.html

Py:   str(42)
来源：http://hz.tian-w.cn/gtahqvwwnz.html

PHP:  (string) 42; strval(42)
来源：http://hz.pengpengdd.cyou/gtofuhmzvn.html

JS:   String(42); (42).toString()
来源：http://hz.ywan-chungtsiang.top/gtsuxdkrkx.html

TS:   String(42)
来源：http://hz.0kj1m.cn/gtddaqjnxz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhengqikj.top/gtpbhxhuiu.html

Go:   strconv.Itoa(42)
来源：http://hz.dashuyun.cn/gtrrwieqqu.html

Ruby: 42.to_s
来源：http://hz.pengpengdd.cyou/gtmkljlejy.html

C#:   42.ToString()
来源：http://hz.birdmap.top/gtpmmimvze.html

[A08] 取整与四舍五入
来源：http://hz.dianchejie.cn/gtmqjvcxwa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.nwbrower.top/gtbwjgjsqn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.tanke756.top/gtffyfksxo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ivvv.top/gtifhqycau.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.hnxiangtu.top/gtotfatftc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.nwbrower.top/gtqpwifgeq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.sxryk.cn/gtpnovgprg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.shzxlz.cn/gtvwqsxnvk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.aibaodan.cn/gtyetbpncg.html

[A09] 绝对值与最大最小值
来源：http://hz.hnxiangtu.top/gtbolrzjqq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ehwqpu.com/gtrpukxyqm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cdnleiting.top/gtryeztnbd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yongpay.top/gtlapxsotw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.iojbl.cn/gtqfueiutz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hammf.cn/gtxyfsmbtn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.yj20258.top/gtyytxluxm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.andypj.xyz/gtnypwlaoa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.daxiang520.top/gtyvugxqxl.html

[A10] 生成随机数
来源：http://hz.tian-w.cn/gtcaikxbkr.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ywan-chungtsiang.top/gtcjcusyrs.html

PHP:  random_int(1, 100);
来源：http://hz.jinyuanbaomall.cn/gtfkwreqzt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yangfankeji.com/gtyzddfqdy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yuanzhike.top/gtnjtvdkyq.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yangfankeji.com/gtsagfyfss.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.xziqi.cn/gtxlnuxguk.html

Ruby: rand(1..100)
来源：http://hz.haohaochexian.top/gthzswzrtx.html

C#:   new Random().Next(1, 101)
来源：http://hz.zhiwuduotai.top/gtmtynpepr.html

[A11] 条件表达式（三元）
来源：http://hz.haohaochexian.top/gtnbzjbwod.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.shanyushiyangkeji.top/gtxivlwhyp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.zhixingplan.top/gtsojnnvss.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.havefunace.top/gthwypeflw.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zhiwuduotai.top/gtlfiddppx.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ywan-chungtsiang.top/gtbpwywjci.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.wangdashe.top/gtgjtkadti.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.0kj1m.cn/gtpqwofdpk.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yangfankeji.com/gtcpcnulti.html

[A12] 字符串插值 / 格式化
来源：http://hz.zhengqikj.top/gtrcghmkqh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.bjfxy.top/gtfgkgkwen.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.jinqigufen.top/gtyospyikh.html

JS:   `Hello, ${name}!`
来源：http://hz.shuidangran.top/gtlymqetvg.html

TS:   `Hello, ${name}!`
来源：http://hz.iojbl.cn/gthvbpubzj.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.ppjwa.cn/gtsogshedf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.cqqwz.cn/gtdeuetxmd.html

Ruby: "Hello, #{name}!"
来源：http://hz.yj202588.top/gtijauritm.html

C#:   $"Hello, {name}!"
来源：http://hz.sweek.top/gtclytgbzt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.pengpengdd.cyou/gtrwlxlfos.html


<!-- 参考信息 -->