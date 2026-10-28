代发 wailian999

[U79] PHP：静态分析
来源：http://hz.redwolf501.top/gtppssfhpv.html

composer require --dev phpstan/phpstan
来源：http://hz.ivvv.top/gtggzcxjhl.html

[U80] PHP：代码规范修复
来源：http://hz.bjfxy.top/gtkiwwgkqd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.gaohongyu789.top/gtwdcusedw.html

[U81] JS：初始化项目
来源：http://hz.yongpay.top/gtxpnlenqi.html

npm init -y;  npm i express
来源：http://hz.yj20258.top/gtzuesurjq.html

[U82] JS：package.json 脚本
来源：http://hz.fengsongda.top/gtzwasjqcn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hysaishi.cn/gtzppidqlr.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhengqikj.top/gtrkxxcbqy.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yangfankeji.com/gtmgryctze.html

[U84] JS：CommonJS 写法
来源：http://hz.jinyuanbaomall.cn/gtdsymtwwm.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yuxming.cn/gtkbfiiuda.html

[U85] JS：可选链
来源：http://hz.yj202588.top/gtzyzldnyb.html

a?.b?.c
来源：http://hz.guowangkeji.top/gtbzcwznve.html

[U86] JS：空值合并
来源：http://hz.0kj1m.cn/gtwpngjgzj.html

a ?? b
来源：http://hz.zhongyouzk.top/gtzxulgugz.html

[U87] JS：解构默认值
来源：http://hz.zhaomingkeji.xyz/gtkcpbsicz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.chenzaomai.com/gtinaoibvp.html

[U88] JS：对象展开合并
来源：http://hz.xuetiantiany.cn/gttihlqmjl.html

{ ...a, ...b }
来源：http://hz.ivvv.top/gtocfexvru.html

[U89] JS：数组去重
来源：http://hz.nanxinkj.top/gtolbptdwi.html

[...new Set(arr)]
来源：http://hz.hysaishi.cn/gtrlvkznqa.html

[U90] JS：数字数组排序
来源：http://hz.wangdashe.top/gtyxaptnmd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtkyukaikx.html

[U91] JS：对象键值遍历
来源：http://hz.yonumen.top/gtgvcfjjtm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.nwbrower.top/gtqdgxlmrw.html

[U92] JS：深拷贝
来源：http://hz.yueranfly.top/gtwfbvtyfp.html

structuredClone(obj)
来源：http://hz.zycfv.cn/gtknmfvbsz.html

[U93] JS：模板字符串
来源：http://hz.zhongyouzk.top/gttvxhfroj.html

`共 ${n} 条`
来源：http://hz.feifeiyinyue.top/gtcdkgocol.html

[U94] JS：箭头函数
来源：http://hz.wangdashe.top/gtogxfvdza.html

const double = x => x * 2;
来源：http://hz.chenjidiqi.icu/gtmkryspth.html

[U95] JS：Promise 包装
来源：http://hz.gogol.net.cn/gtdozufdkk.html

new Promise((resolve, reject) => {})
来源：http://hz.yongpay.top/gteynqnwim.html

[U96] JS：async/await 与异常
来源：http://hz.mhx1999.top/gtbwkobefp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.nwbrower.top/gtzweoomok.html

[U97] JS：并发请求
来源：http://hz.c1oappe.top/gtrqefekup.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtlshvahhz.html

[U98] JS：fetch 带 JSON
来源：http://hz.svipenyu.cn/gtxdlcaqjm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.yongpay.top/gtwvebcjwb.html

[U99] JS：事件监听
来源：http://hz.wangdashe.top/gtihfnuwwy.html

el.addEventListener("click", e => {})
来源：http://hz.svipenyu.cn/gtopahwodr.html

[U100] JS：DOM 查询
来源：http://hz.cheryme.top/gtfojxkvrl.html

document.querySelector(".item")
来源：http://hz.hammf.cn/gtylsjvkpl.html

[U101] JS：classList 操作
来源：http://hz.ybcxt.top/gtdrswtakh.html

el.classList.toggle("active")
来源：http://hz.zhengqikj.top/gtltmkyefr.html

[U102] JS：本地存储
来源：http://hz.jiagoushi.top/gtrmxfmvdf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.pengpengdd.cyou/gtnjnexxav.html

[U103] JS：定时器
来源：http://hz.zhaomingkeji.xyz/gtgtkkegpb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jqgfzy.top/gtnzqvmwgz.html

[U104] JS：防抖
来源：http://hz.guowangkeji.top/gtzwkxckkv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj202588.top/gtjzlvzxub.html

[U105] JS：节流
来源：http://hz.cqqwz.cn/gtbuqpxayl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shanyushiyangkeji.top/gtaynrsupu.html

[U106] JS：日期格式化
来源：http://hz.ydzc1.top/gtzkencjur.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.hongshengwenyu.top/gtkuolvwqy.html

[U107] JS：数字千分位
来源：http://hz.yongpay.top/gtgnxjcpdi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.0kj1m.cn/gtdifebmpm.html

[U108] JS：随机整数
来源：http://hz.wangdashe.top/gtylutkcgg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj202588.top/gtpfogzivg.html

[U109] JS：数组分组
来源：http://hz.xingfuxueyuan.xyz/gtwjzhmgib.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xinyue.icu/gtvxmrhvbc.html

[U110] JS：数组分块
来源：http://hz.zhiwuduotai.top/gtoacqjepw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.ydjk.org.cn/gtmgoenjls.html

[U111] JS：对象转 Map
来源：http://hz.jqgufenzy.top/gtgfqinjdf.html

new Map(Object.entries(obj))
来源：http://hz.yvedp.cn/gtjfakcvzm.html

[U112] JS：字符串补位
来源：http://hz.sxryk.cn/gtafdeerjd.html

"7".padStart(3, "0")
来源：http://hz.quarkkingdee.top/gtdhflnxwc.html

[U113] JS：正则替换全部
来源：http://hz.zhaomingkeji.xyz/gtonsgioue.html

s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtkiytfagv.html

[U114] JS：JSON 深比较
来源：http://hz.vqdsnc.cn/gtahfyntny.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jqgfzy.top/gtiokohkxa.html

[U115] JS：生成 UUID
来源：http://hz.jianghu66.top/gteooiaozn.html

crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtpwhmcrih.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yueranfly.top/gtmueiskar.html

/** @param {string} name */ function f(name) {}
来源：http://hz.sysykeji.top/gtffrycois.html

[U117] JS：单元测试
来源：http://hz.yongpay.top/gtsjefvsim.html

npm i -D vitest;  npx vitest
来源：http://hz.ydzc1.top/gtgiccyevw.html

[U118] JS：开发服务器
来源：http://hz.feifeiyinyue.top/gtxhgtgfpj.html

npm i -D vite;  npx vite
来源：http://hz.c1oappe.top/gttjiorsrt.html

[U119] JS：生产构建
来源：http://hz.hongshengwenyu.top/gtiwovrwtz.html

npx vite build
来源：http://hz.hysaishi.cn/gtqeuyxdmv.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.gaohongyu789.top/gtrjzfziro.html

import.meta.env.VITE_API_URL
来源：http://hz.zhongyouzk.top/gtpcudkikb.html

================================================================================
来源：http://hz.hammf.cn/gtsexjzcuf.html

统计汇总
来源：http://hz.gogol.net.cn/gtjirjrzxm.html

================================================================================
来源：http://hz.haohaochexian.top/gthnblpuyt.html

按语言统计（条）：
来源：http://hz.zdqjudy.top/gtspaqwfht.html

Python ......... 252
来源：http://hz.zdqjudy.top/gtpwimdpsf.html

PHP ............ 252
来源：http://hz.sxryk.cn/gtvzrzidlf.html

JavaScript ..... 252
来源：http://hz.chenjidiqi.icu/gtrfftabfz.html

TypeScript ..... 212
来源：http://hz.316326.xyz/gtzudnqtdd.html

Java ........... 212
来源：http://hz.zycfv.cn/gtkocqkhwb.html

Go ............. 212
来源：http://hz.ybcxt.top/gtkhipxuzo.html

Ruby ........... 212
来源：http://hz.svipenyu.cn/gtzmxxecmi.html

C# ............. 212
来源：http://hz.cdnleiting.top/gtohqusisy.html

C .............. 30
来源：http://hz.zycfv.cn/gtsljkuqgb.html

C++ ............ 30
来源：http://hz.hysaishi.cn/gtoomtfdvw.html

SQL ............ 90
来源：http://hz.aizwys.cn/gtivhffhcs.html

Bash ........... 80
来源：http://hz.redwolf501.top/gtzfmfjshh.html

Kotlin ......... 15
来源：http://hz.shuidangran.top/gtlxvkkhgt.html

Swift .......... 15
来源：http://hz.yangfankeji.com/gturknqmgy.html

Lua ............ 10
来源：http://hz.hfpthk.cn/gtehbpblfq.html

Perl ........... 10
来源：http://hz.zycfv.cn/gtpoentrwd.html

Scala .......... 10
来源：http://hz.hnqzz.top/gtgbxgmusg.html

------------------------------------
来源：http://hz.hfpthk.cn/gtnvkdmdlp.html

合计 ........... 2106 条
来源：http://hz.cqqwz.cn/gtmsutjpcl.html

按章节统计：
来源：http://hz.shuidangran.top/gthxerpapa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.hnqzz.top/gtjfxsfhbs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.feifeiyinyue.top/gtafjvhpiy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jinghuilouyu.cn/gtplibivxg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.havefunace.top/gtdvmyaljf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.hywenlv.cn/gtwqdfyvtl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.svipenyu.cn/gtcsmkfyco.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gtzxilefks.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cheryme.top/gtobkrgyhj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tanke756.top/gtobmasumu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.zhaomingkeji.xyz/gtptjstyyr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.redwolf501.top/gtbpafujie.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jianghu66.top/gtgtfgozum.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.sweek.top/gtkuwoxukl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ivvv.top/gtgqmscjta.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.chenzaomai.com/gttxewcplq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.xylfe.cn/gtfkuajatp.html

Q SQL 专题                              90
来源：http://hz.nanxinkj.top/gttgfapmap.html

R Bash 专题                             80
来源：http://hz.gotoacloud.top/gtjacddtjy.html

S C / C++ 专题                          60
来源：http://hz.hongshengwenyu.top/gttczecnta.html

T 其他语言补充                          60
来源：http://hz.yuxming.cn/gthgzuvddz.html

U 高频实用片段                         120
来源：http://hz.ehwqpu.com/gtymhplmfb.html

------------------------------------
来源：http://hz.jinghuilouyu.cn/gtzbxiurjo.html

合计                                  2106 条
来源：http://hz.xziqi.cn/gtiyyejocr.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtsjgvnfnv.html

使用提醒
来源：http://hz.birdmap.top/gtdtdixrmb.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gtnnghzbiv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.daxiang520.top/gtieyeftds.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.quarkkingdee.top/gtcwjbnttv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.hysaishi.cn/gtegpoqmjx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.redwolf501.top/gtncotkkel.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.wangshuangyany.cn/gtysfyciad.html

—— 文件结束 ——
来源：http://hz.cheryme.top/gtnobktvlk.html

================================================================================
来源：http://hz.dashuyun.cn/gtmvdngpda.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.svipenyu.cn/gtqtkzhrwu.html

Common Programming Examples Cheat Book
来源：http://hz.wangdashe.top/gtlhqcchqs.html

================================================================================
来源：http://hz.zycfv.cn/gtxwebcash.html

【收录内容】
来源：http://hz.pengpengdd.cyou/gtlyzblowm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.tianlin.xyz/gtcznahrxw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.dianchejie.cn/gtztcezgqj.html

SQL · Bash · C · C++
来源：http://hz.hysaishi.cn/gtgcnzythi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zdqjudy.top/gtqyjpztsl.html

【使用说明】
来源：http://hz.jianghu66.top/gtyryvfnzf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.gzhubu.top/gtresgivlp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.jinghuilouyu.cn/gtbrqghpra.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhengqikj.top/gttpnykbcs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.meibo888.top/gthfpsswoz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yuxming.cn/gtgqrwirip.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jqgufenzy.top/gtgwoyosmr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.xziqi.cn/gtaspustyz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.tianlin.xyz/gthqozxcci.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cqqwz.cn/gtfbhppmxk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.hnqzz.top/gtbfojfjqk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.daria6918.cn/gthlgojnai.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.wangshuangyany.cn/gtsubbcdln.html

【文件统计】
来源：http://hz.nanxinkj.top/gtqcztwjan.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.shangyingyoupin.top/gtpcikjdwg.html

--------------------------------------------------------------------------------
来源：http://hz.cheryme.top/gtyojlqvum.html

目  录
来源：http://hz.yj202588.top/gtmnqnskou.html

--------------------------------------------------------------------------------
来源：http://hz.mhx1999.top/gtijftrarh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yongpay.top/gtuhddwcfp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.nanxuanxn.top/gtrxpyiivl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yueranfly.top/gtmscuxcfg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.svipenyu.cn/gtsgebzvzb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.tian-w.cn/gtdzxkoxts.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.ydjk.org.cn/gtxdueswtl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.hywenlv.cn/gtzawdfxim.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.chenjidiqi.icu/gtbtldcszo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.meibo888.top/gtxudyqnii.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.ydjk.org.cn/gteqvneehz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.pengpengdd.cyou/gtsprvdcto.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.xingfuxueyuan.xyz/gtczfglhhd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.kuanghao11.cn/gtbjgutcsy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jqgufenzy.top/gtzvenpujq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.redwolf501.top/gtryjlcymm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.guannengcc.top/gtvjhdgaut.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.quarkkingdee.top/gtxntmapgv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.andypj.xyz/gtzvchkcol.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.wangdashe.top/gtrgocsiea.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj202588.top/gtbajirpxo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinyuanbaomall.cn/gtfzebhjlv.html

================================================================================
来源：http://hz.aibaodan.cn/gtmvdftjbt.html

A. 基础语法与类型
来源：http://hz.jinghuilouyu.cn/gtbdwfggrm.html

================================================================================
来源：http://hz.jianghu66.top/gtawadgcbq.html

[A01] Hello World
来源：http://hz.ehwqpu.com/gtbvoxgxzn.html

Py:   print("Hello, World!")
来源：http://hz.hysaishi.cn/gtiisanncp.html

PHP:  echo "Hello, World!";
来源：http://hz.yj20258888.top/gtstbngsjx.html

JS:   console.log("Hello, World!");
来源：http://hz.andypj.xyz/gtziaovdnl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.nanxuanxn.top/gtjwgribte.html

Java: System.out.println("Hello, World!");
来源：http://hz.xylfe.cn/gtozzysfif.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.redwolf501.top/gtekptwyxy.html

Ruby: puts "Hello, World!"
来源：http://hz.sweek.top/gtfrkeprcy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.sufxvd.cn/gthjvjcdlc.html

[A02] 变量声明与赋值
来源：http://hz.ivvv.top/gtvlojgous.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.andypj.xyz/gtcrcmwdhs.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shanyushiyangkeji.top/gtnxfbmzze.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.kuanghao11.cn/gtomjtbusj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.yvedp.cn/gtvxpjhznm.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.xinyue.icu/gtelgermnz.html

Go:   name := "Alex"; age := 20
来源：http://hz.gotoacloud.top/gtmjdznobg.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hongshengwenyu.top/gtlxcqbdoj.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ppjwa.cn/gtigmxcswm.html

[A03] 常量定义
来源：http://hz.sufxvd.cn/gtqjkfkodb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.pengpengdd.cyou/gtnztvowjv.html

PHP:  const PI = 3.14159;
来源：http://hz.quarkkingdee.top/gtvgfewqys.html

JS:   const PI = 3.14159;
来源：http://hz.gotoacloud.top/gtqghrtryo.html

TS:   const PI: number = 3.14159;
来源：http://hz.wangshuangyany.cn/gtnzipxkbw.html

Java: static final double PI = 3.14159;
来源：http://hz.hywenlv.cn/gtsmalsdca.html

Go:   const PI = 3.14159
来源：http://hz.yj20258888.top/gtrjpobfrr.html

Ruby: PI = 3.14159
来源：http://hz.meibo888.top/gtmlufqbsc.html

C#:   const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtjoslyhrb.html

[A04] 判断变量类型
来源：http://hz.fzhhl.top/gtuvmsbvrz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.xylfe.cn/gtxnrteuhl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yj202588.top/gtfegsaofx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.gogol.net.cn/gtnzajtyir.html

TS:   typeof x; x instanceof Date
来源：http://hz.hnqzz.top/gtbeglravf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.andypj.xyz/gtlofummfe.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yanxiufei.cn/gtjyzuhamo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.wangshuangyany.cn/gtknwjbsdi.html

C#:   x.GetType().Name; x is int
来源：http://hz.yonumen.top/gtfwwtezqg.html

[A05] 整数除法与取模
来源：http://hz.chenzaomai.com/gtdddzswix.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.quarkkingdee.top/gtvicqakkr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jyoumei.cn/gtpflquqdz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhixingplan.top/gtnnhnlheq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ywan-chungtsiang.top/gtmjvoekxg.html

Java: 7 / 2; 7 % 2
来源：http://hz.guannengcc.top/gtpcihkaqa.html

Go:   7 / 2; 7 % 2
来源：http://hz.jqgufenzy.top/gtznefmoxg.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yuanzhike.top/gtomcbagqd.html

C#:   7 / 2; 7 % 2
来源：http://hz.fzhhl.top/gtwmwsoezw.html

[A06] 字符串转数字
来源：http://hz.hysaishi.cn/gtgpvcuwvh.html

Py:   int("42"); float("3.14")
来源：http://hz.cdnleiting.top/gtiersqmfs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.gzhubu.top/gtirbyqiqy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.sweek.top/gtbzlxumae.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yangfankeji.com/gtzgsrwrfl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.nanxinkj.top/gtrhpsxhsz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gotoacloud.top/gtrvphqjps.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.sweek.top/gtdzvzattv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.dianchejie.cn/gtcazfladr.html

[A07] 数字转字符串
来源：http://hz.ydjk.org.cn/gtomucjdtt.html

Py:   str(42)
来源：http://hz.cashguo.top/gtvyxzsvyr.html

PHP:  (string) 42; strval(42)
来源：http://hz.guannengcc.top/gtpticaegv.html

JS:   String(42); (42).toString()
来源：http://hz.aibaodan.cn/gtwsfpigew.html

TS:   String(42)
来源：http://hz.52xcode.cn/gtoldqjktm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.nanxinkj.top/gtoqfpcgqr.html

Go:   strconv.Itoa(42)
来源：http://hz.zhoulong.xyz/gthuydsqcz.html

Ruby: 42.to_s
来源：http://hz.mhx1999.top/gtarlxpuhn.html

C#:   42.ToString()
来源：http://hz.yuanzhike.top/gtxyntabim.html

[A08] 取整与四舍五入
来源：http://hz.xylfe.cn/gtbzhsdkot.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.c1oappe.top/gtxouojcgf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.jinqigufen.top/gtzbtpwgub.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.daria6918.cn/gteweolxrj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.nanxuanxn.top/gtjzaphsap.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.ivvv.top/gtlrmjtefq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.feifeiyinyue.top/gtbmqkmbiu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.svipenyu.cn/gthfwymgjk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtikwsfykc.html

[A09] 绝对值与最大最小值
来源：http://hz.xuetiantiany.cn/gtmqxhpihr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtyprngxlu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.birdmap.top/gtnglstexu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.cqqwz.cn/gtthgcrkuw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhixingplan.top/gtmurrcbot.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.sufxvd.cn/gtyrkbxbvc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.mhx1999.top/gthpaqhalp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.hywenlv.cn/gtapgshnbw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.cheryme.top/gtrbqwdhem.html

[A10] 生成随机数
来源：http://hz.vqdsnc.cn/gtyrycgzmy.html

Py:   import random; random.randint(1, 100)
来源：http://hz.yuxming.cn/gtsyqzxmfp.html

PHP:  random_int(1, 100);
来源：http://hz.hywenlv.cn/gtqmbqbzca.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.9152youxi.cn/gtsvbefsvq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhiwuduotai.top/gtdzooagvb.html

Java: new Random().nextInt(100) + 1
来源：http://hz.jinqigufen.top/gtpljzlglh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zycfv.cn/gtdyltgfnk.html

Ruby: rand(1..100)
来源：http://hz.hfpthk.cn/gtnzyojtxv.html

C#:   new Random().Next(1, 101)
来源：http://hz.dashuyun.cn/gthrvqqhze.html

[A11] 条件表达式（三元）
来源：http://hz.fzhhl.top/gthneqvxig.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zhaomingkeji.xyz/gtmugdzove.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.zycfv.cn/gtizvjquip.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yj20258888.top/gtyswbznev.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jqgufenzy.top/gtitpdnzui.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.wangdashe.top/gtdxycwkft.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.sufxvd.cn/gtkzhzqxmu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hongshengwenyu.top/gtbheltdrl.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.zhaomingkeji.xyz/gtzndicwjb.html

[A12] 字符串插值 / 格式化
来源：http://hz.pengpengdd.cyou/gtakqhflav.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.gogol.net.cn/gtcxpghdww.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.dianchejie.cn/gteihvacud.html

JS:   `Hello, ${name}!`
来源：http://hz.hongshengwenyu.top/gtwviknmcb.html

TS:   `Hello, ${name}!`
来源：http://hz.chenzaomai.com/gtrutsfotl.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.dashuyun.cn/gtlzygnyua.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.hongshengwenyu.top/gtpaifoelj.html

Ruby: "Hello, #{name}!"
来源：http://hz.pengpengdd.cyou/gtfgyukrsd.html

C#:   $"Hello, {name}!"
来源：http://hz.tianlin.xyz/gtqmgvqgic.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.zdqjudy.top/gtfdxljcms.html


<!-- 参考信息 -->