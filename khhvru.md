代发 wailian999

[U77] PHP：模板渲染
来源：http://hz.tianlin.xyz/gtfnnzifzy.html

composer require twig/twig
来源：http://hz.kuanghao11.cn/gtcdciaido.html

[U78] PHP：单元测试
来源：http://hz.guowangkeji.top/gtzaetysqg.html

composer require --dev phpunit/phpunit
来源：http://hz.ydjk.org.cn/gtzpbedlei.html

[U79] PHP：静态分析
来源：http://hz.dashuyun.cn/gteonstmqz.html

composer require --dev phpstan/phpstan
来源：http://hz.jqgfzy.top/gtqttlxlsp.html

[U80] PHP：代码规范修复
来源：http://hz.nanxinkj.top/gtdxsffjhj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.zdqjudy.top/gttgpbucgo.html

[U81] JS：初始化项目
来源：http://hz.cheryme.top/gtgzaqcezh.html

npm init -y;  npm i express
来源：http://hz.pycfn.com/gtreszbuom.html

[U82] JS：package.json 脚本
来源：http://hz.0kj1m.cn/gtdldrkqqs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ybcxt.top/gtgmkoykxw.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhaomingkeji.xyz/gtkhuqkqeu.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yongpay.top/gtaiiukges.html

[U84] JS：CommonJS 写法
来源：http://hz.hfpthk.cn/gtmnkdxtbe.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.mhx1999.top/gtkjbqlhku.html

[U85] JS：可选链
来源：http://hz.zdqjudy.top/gtwvbjnzie.html

a?.b?.c
来源：http://hz.dashuyun.cn/gttaxjbtes.html

[U86] JS：空值合并
来源：http://hz.yj20258.top/gtaizfxtgi.html

a ?? b
来源：http://hz.ybcxt.top/gturihqgjd.html

[U87] JS：解构默认值
来源：http://hz.gogol.net.cn/gttscydgfv.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shangyingyoupin.top/gtrpvloleg.html

[U88] JS：对象展开合并
来源：http://hz.zhiwuduotai.top/gtefbakczh.html

{ ...a, ...b }
来源：http://hz.tianlin.xyz/gtmduimsdc.html

[U89] JS：数组去重
来源：http://hz.snrcjt.cn/gtaeeooojm.html

[...new Set(arr)]
来源：http://hz.ehwqpu.com/gtkuhclqbp.html

[U90] JS：数字数组排序
来源：http://hz.chenjidiqi.icu/gthxegchrr.html

[...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtancltlda.html

[U91] JS：对象键值遍历
来源：http://hz.hammf.cn/gtzorayvph.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.gzhubu.top/gtnukitlhs.html

[U92] JS：深拷贝
来源：http://hz.yvedp.cn/gtuhqmpbah.html

structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtyizuazru.html

[U93] JS：模板字符串
来源：http://hz.pycfn.com/gtjavowkzk.html

`共 ${n} 条`
来源：http://hz.sxryk.cn/gtiszgrtzb.html

[U94] JS：箭头函数
来源：http://hz.hnqzz.top/gtpbevxhuu.html

const double = x => x * 2;
来源：http://hz.cdnleiting.top/gtdyfoaxyw.html

[U95] JS：Promise 包装
来源：http://hz.yuxming.cn/gtjdhcomss.html

new Promise((resolve, reject) => {})
来源：http://hz.yongpay.top/gtsypspkqe.html

[U96] JS：async/await 与异常
来源：http://hz.jqgfzy.top/gtvghfoxub.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.sysykeji.top/gttzoeqteu.html

[U97] JS：并发请求
来源：http://hz.ybcxt.top/gtkkbrntgi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtmjtcdxia.html

[U98] JS：fetch 带 JSON
来源：http://hz.yvedp.cn/gteadeeddj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.sweek.top/gtysyrsmga.html

[U99] JS：事件监听
来源：http://hz.yonumen.top/gthalhzywe.html

el.addEventListener("click", e => {})
来源：http://hz.shanyushiyangkeji.top/gtaaqinbif.html

[U100] JS：DOM 查询
来源：http://hz.jiagoushi.top/gtjrwgpbzf.html

document.querySelector(".item")
来源：http://hz.jinqigufen.top/gticovhxps.html

[U101] JS：classList 操作
来源：http://hz.zhengqikj.top/gthkqgrddh.html

el.classList.toggle("active")
来源：http://hz.zhengqikj.top/gtrdpmagzf.html

[U102] JS：本地存储
来源：http://hz.hywenlv.cn/gtjurhxtgc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.jiagoushi.top/gtqijwsyue.html

[U103] JS：定时器
来源：http://hz.fengsongda.top/gtkqcrgrmc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.ydzc1.top/gtqgjndtom.html

[U104] JS：防抖
来源：http://hz.chenzaomai.com/gtuudpvxhb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yuxming.cn/gtxfhqmjco.html

[U105] JS：节流
来源：http://hz.yvedp.cn/gthatcmrul.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.daxiang520.top/gtnvwbnrxt.html

[U106] JS：日期格式化
来源：http://hz.zhiwuduotai.top/gttkvuqalz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.guannengcc.top/gtiwmdxpit.html

[U107] JS：数字千分位
来源：http://hz.guowangkeji.top/gtaosfeiva.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.kuanghao11.cn/gticxztllw.html

[U108] JS：随机整数
来源：http://hz.pengpengdd.cyou/gtgrryqiog.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.daxiang520.top/gtjzzkpipo.html

[U109] JS：数组分组
来源：http://hz.fzhhl.top/gtupzgpeqz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangtech.top/gtshdaubak.html

[U110] JS：数组分块
来源：http://hz.yvedp.cn/gtfzqeuqhb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.cucudq.cn/gtdmrjkuhd.html

[U111] JS：对象转 Map
来源：http://hz.smart0.xyz/gtlaumclvh.html

new Map(Object.entries(obj))
来源：http://hz.yj202588.top/gttjuytjke.html

[U112] JS：字符串补位
来源：http://hz.sufxvd.cn/gtfgirdyxn.html

"7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtkxszabat.html

[U113] JS：正则替换全部
来源：http://hz.yangfankeji.com/gttjgmbhks.html

s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtiobfljrd.html

[U114] JS：JSON 深比较
来源：http://hz.gogol.net.cn/gtrktcrsnb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dashuyun.cn/gtrxuaxtwf.html

[U115] JS：生成 UUID
来源：http://hz.mhx1999.top/gtjaonnspv.html

crypto.randomUUID()
来源：http://hz.hongshengwenyu.top/gtetffkbaj.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.tianlin.xyz/gtwzfnhlzt.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yvedp.cn/gtvuervfvh.html

[U117] JS：单元测试
来源：http://hz.yuxming.cn/gtyjpqhrnz.html

npm i -D vitest;  npx vitest
来源：http://hz.yongpay.top/gtselwxbpv.html

[U118] JS：开发服务器
来源：http://hz.jiagoushi.top/gtnbvnmdqo.html

npm i -D vite;  npx vite
来源：http://hz.cheryme.top/gtbzgbmufl.html

[U119] JS：生产构建
来源：http://hz.jinqigufen.top/gtrpalhslf.html

npx vite build
来源：http://hz.chenlongwang.top/gtdkhbrkal.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xuetiantiany.cn/gtygzmpbmc.html

import.meta.env.VITE_API_URL
来源：http://hz.ivvv.top/gtbwtdrfdp.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtiheaxeix.html

统计汇总
来源：http://hz.gogol.net.cn/gtwcsjlskc.html

================================================================================
来源：http://hz.ivvv.top/gtszsawjqj.html

按语言统计（条）：
来源：http://hz.shanyushiyangtech.top/gtzsbtqckq.html

Python ......... 252
来源：http://hz.mhx1999.top/gtguzazloa.html

PHP ............ 252
来源：http://hz.316326.xyz/gtlrbdggnc.html

JavaScript ..... 252
来源：http://hz.ydzc1.top/gtbgxyptcs.html

TypeScript ..... 212
来源：http://hz.hongshengwenyu.top/gtaywschqs.html

Java ........... 212
来源：http://hz.cdnleiting.top/gtwqncvgun.html

Go ............. 212
来源：http://hz.tian-w.cn/gtggshfnku.html

Ruby ........... 212
来源：http://hz.aibaodan.cn/gttpggriwh.html

C# ............. 212
来源：http://hz.hnqzz.top/gtnrraevyg.html

C .............. 30
来源：http://hz.pengpengdd.cyou/gtiynfjntq.html

C++ ............ 30
来源：http://hz.chenjidiqi.icu/gtifxtecwq.html

SQL ............ 90
来源：http://hz.c1oappe.top/gtdpwwztgd.html

Bash ........... 80
来源：http://hz.bjfxy.top/gtevgbmupz.html

Kotlin ......... 15
来源：http://hz.gzhubu.top/gtoucpwmja.html

Swift .......... 15
来源：http://hz.yueranfly.top/gtcwbtpxwy.html

Lua ............ 10
来源：http://hz.gzhubu.top/gtkvblrrei.html

Perl ........... 10
来源：http://hz.cdnleiting.top/gtliprsqxt.html

Scala .......... 10
来源：http://hz.shanyushiyangkeji.top/gtlbwnyfvi.html

------------------------------------
来源：http://hz.ivvv.top/gtkactxbor.html

合计 ........... 2106 条
来源：http://hz.daria6918.cn/gtigvbkpvx.html

按章节统计：
来源：http://hz.shanyushiyangkeji.top/gtzkddovpg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.zhengqikj.top/gtnleyzwpb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gtabblfbbs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.9152youxi.cn/gtiusmmzrr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.jlsjyb.cn/gtzpvyyhpm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinyuanbaomall.cn/gtszpusfdq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.316326.xyz/gttcsolbmg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.zhaomingkeji.xyz/gtuoxkrsan.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.guannengcc.top/gtxqbcbkav.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtqnvnkhqt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cashguo.top/gtqzbexjze.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gttlcavumj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtdrohqzfd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.gotoacloud.top/gtedncjskj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.svipenyu.cn/gtxgokygdo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yonumen.top/gtmupfezps.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtnhnvqyfh.html

Q SQL 专题                              90
来源：http://hz.cucudq.cn/gtfrdzmsqv.html

R Bash 专题                             80
来源：http://hz.sweek.top/gtsxitseml.html

S C / C++ 专题                          60
来源：http://hz.xziqi.cn/gtlqbvxepf.html

T 其他语言补充                          60
来源：http://hz.52xcode.cn/gtyyqdibme.html

U 高频实用片段                         120
来源：http://hz.wangdashe.top/gtzsxnrbrh.html

------------------------------------
来源：http://hz.jiagoushi.top/gtmhbexnko.html

合计                                  2106 条
来源：http://hz.ehwqpu.com/gtzkxhxbwu.html

--------------------------------------------------------------------------------
来源：http://hz.jinghuilouyu.cn/gtratfksmd.html

使用提醒
来源：http://hz.tian-w.cn/gtxeclaopn.html

--------------------------------------------------------------------------------
来源：http://hz.birdmap.top/gtjfywyapn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.shanyushiyangkeji.top/gtlqogsqek.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.ydzc1.top/gtmjfgopfx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.guannengcc.top/gtacjtbska.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.cdnleiting.top/gtuuzyqzoq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cashguo.top/gtnsebqlps.html

—— 文件结束 ——
来源：http://hz.guannengcc.top/gtsidawumi.html

================================================================================
来源：http://hz.hnqzz.top/gtfeeneeuz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.jinyuanbaomall.cn/gtbgosdhmt.html

Common Programming Examples Cheat Book
来源：http://hz.smart0.xyz/gtljeuzugi.html

================================================================================
来源：http://hz.daria6918.cn/gtvpqdxifs.html

【收录内容】
来源：http://hz.cdnleiting.top/gtmelimxdg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.dianchejie.cn/gtoemgjbit.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.dianchejie.cn/gtznrckvwi.html

SQL · Bash · C · C++
来源：http://hz.gzhubu.top/gtojabyqyk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.fzhhl.top/gtidcwpnmr.html

【使用说明】
来源：http://hz.cheryme.top/gtvtkwxbay.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhoulong.xyz/gtjgqzakua.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.pycfn.com/gtogvdhxgm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.cucudq.cn/gtydrzecux.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jinyuanbaomall.cn/gtarzpxbaz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shanyushiyangkeji.top/gtyvuogyqb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.c1oappe.top/gttodcutjg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.wangdashe.top/gtazcowqvj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.fengsongda.top/gtzczdonjf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.kuanghao11.cn/gtkjqmzceh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.smart0.xyz/gtdspuvvyw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhijiandao.cn/gtynjcvhqd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xingfuxueyuan.xyz/gtbnurimtw.html

【文件统计】
来源：http://hz.gaohongyu789.top/gtfqjwnfmc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.smart0.xyz/gtqfwlklxp.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gtgbilhwwj.html

目  录
来源：http://hz.316326.xyz/gtjyqsjspg.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtkexdvkkc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhaomingkeji.xyz/gtqgyshfbu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.gogol.net.cn/gttzznuyag.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hysaishi.cn/gtxzeomgri.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.jlsjyb.cn/gtpcvwfnxf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.ehwqpu.com/gtbaeofmkj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.iojbl.cn/gtpysrsudw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jlsjyb.cn/gtuvqwuwdx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gtjtapjhju.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.cashguo.top/gtmeefihun.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.gzhubu.top/gtzwkdmzuo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yongpay.top/gtdvamcids.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.xuanzx.com/gtxzidhcon.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.daxiang520.top/gtrxzmkbgq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.hysaishi.cn/gtcqzqtkqe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhijiandao.cn/gtflabhgay.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zdqjudy.top/gthrhziuix.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.xziqi.cn/gteufebpxv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.pycfn.com/gtnwkwrnnv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.sufxvd.cn/gtswslgexp.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuxming.cn/gtesewaouu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.daria6918.cn/gtptzjidhn.html

================================================================================
来源：http://hz.aizwys.cn/gtqtdikuiw.html

A. 基础语法与类型
来源：http://hz.gotoacloud.top/gthizzbedp.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrjotfwkm.html

[A01] Hello World
来源：http://hz.xuanzx.com/gtclfgmpcs.html

Py:   print("Hello, World!")
来源：http://hz.hnqzz.top/gtyyfzbcsp.html

PHP:  echo "Hello, World!";
来源：http://hz.nanxuanxn.top/gtctmhodaz.html

JS:   console.log("Hello, World!");
来源：http://hz.chenzaomai.com/gtrgnrshfa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhaomingkeji.xyz/gtdqemkvqq.html

Java: System.out.println("Hello, World!");
来源：http://hz.yj20258.top/gtatpjqyla.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.hnxiangtu.top/gtgmrvavau.html

Ruby: puts "Hello, World!"
来源：http://hz.zycfv.cn/gtrdhxjany.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cqqwz.cn/gtwtnsbgfx.html

[A02] 变量声明与赋值
来源：http://hz.chenjidiqi.icu/gtehfoyqsx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yanxiufei.cn/gtlfnwkuvg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shangyingyoupin.top/gtyenrxack.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhiwuduotai.top/gtsliemvik.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xingfuxueyuan.xyz/gtwepkskud.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhengqikj.top/gtfspmonmj.html

Go:   name := "Alex"; age := 20
来源：http://hz.9152youxi.cn/gtpmcxgxju.html

Ruby: name = "Alex"; age = 20
来源：http://hz.nanxinkj.top/gtvcgnpoww.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.zdqjudy.top/gtybehfikz.html

[A03] 常量定义
来源：http://hz.redwolf501.top/gtgxqsvpuw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.gogol.net.cn/gttzetfhxd.html

PHP:  const PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtfgxynopi.html

JS:   const PI = 3.14159;
来源：http://hz.sufxvd.cn/gtpjcinviz.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhongyouzk.top/gtswtvmvrn.html

Java: static final double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtaopippbb.html

Go:   const PI = 3.14159
来源：http://hz.bjfxy.top/gtzrlntfvp.html

Ruby: PI = 3.14159
来源：http://hz.xinyue.icu/gtjqtdfahl.html

C#:   const double PI = 3.14159;
来源：http://hz.yanxiufei.cn/gtzkzsresf.html

[A04] 判断变量类型
来源：http://hz.ywan-chungtsiang.top/gtqzikpjql.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.xuetiantiany.cn/gtheklrtps.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.tanke756.top/gtvhuovhtn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.wangdashe.top/gtqtjopbip.html

TS:   typeof x; x instanceof Date
来源：http://hz.snrcjt.cn/gtpzstvusn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.cheryme.top/gterxugcpt.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jinyuanbaomall.cn/gtbmcrmgrc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.jiagoushi.top/gtsobhgqug.html

C#:   x.GetType().Name; x is int
来源：http://hz.daxiang520.top/gtsxbpeahd.html

[A05] 整数除法与取模
来源：http://hz.aizwys.cn/gtydieqccw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.sxryk.cn/gtspobsvwo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.wangshuangyany.cn/gthcqwardq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hnqzz.top/gtxgekruip.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.guannengcc.top/gtvgxcstno.html

Java: 7 / 2; 7 % 2
来源：http://hz.hywenlv.cn/gtdhkhpkad.html

Go:   7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gtydqdhtkd.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yueranfly.top/gtjpriykha.html

C#:   7 / 2; 7 % 2
来源：http://hz.yanxiufei.cn/gtcvqipnbo.html

[A06] 字符串转数字
来源：http://hz.snrcjt.cn/gtckoanazm.html

Py:   int("42"); float("3.14")
来源：http://hz.fzhhl.top/gtbedqutio.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xylfe.cn/gtecjpgbjf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.sweek.top/gtxlqbsslz.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yuanzhike.top/gtecbmdetq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.chenlongwang.top/gtjusdzaxl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.yonumen.top/gtrdhnadbj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ybcxt.top/gtpxqwriwb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.feifeiyinyue.top/gtuarlsotg.html

[A07] 数字转字符串
来源：http://hz.haohaochexian.top/gtvdkptmzh.html

Py:   str(42)
来源：http://hz.haohaochexian.top/gtqoagbpzx.html

PHP:  (string) 42; strval(42)
来源：http://hz.yanxiufei.cn/gtkuiiwanh.html

JS:   String(42); (42).toString()
来源：http://hz.daria6918.cn/gtvkborlzz.html

TS:   String(42)
来源：http://hz.zhijiandao.cn/gtuorlxsff.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.svipenyu.cn/gtnwkgbdye.html

Go:   strconv.Itoa(42)
来源：http://hz.cdnleiting.top/gtojwpahzt.html

Ruby: 42.to_s
来源：http://hz.daria6918.cn/gtgwrmtqxw.html

C#:   42.ToString()
来源：http://hz.shanyushiyangtech.top/gtxpmoovvt.html

[A08] 取整与四舍五入
来源：http://hz.chenzaomai.com/gtjssaijke.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jqgfzy.top/gtcpqelsyx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.kuanghao11.cn/gtdvqmkced.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.pengpengdd.cyou/gthmuvplyg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.iojbl.cn/gtpmkkrlsp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.c1oappe.top/gtnrpkxzbe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jyoumei.cn/gtbudvxrlf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.ydzc1.top/gthsvrfggd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.andypj.xyz/gtsznplnpp.html

[A09] 绝对值与最大最小值
来源：http://hz.dianchejie.cn/gtysyweshe.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xinyue.icu/gttoagqdtm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yj20258888.top/gtcmueayle.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.nanxuanxn.top/gtsepenooi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.hammf.cn/gtdcxnyzzv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.fengsongda.top/gtfgkwhnfq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.9152youxi.cn/gtcqoveljq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.ybcxt.top/gthsqkhxeb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yj202588.top/gthrbyrnhr.html

[A10] 生成随机数
来源：http://hz.yangfankeji.com/gttjnkqsnj.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hnqzz.top/gtenoqpaev.html

PHP:  random_int(1, 100);
来源：http://hz.52xcode.cn/gtlybserou.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hfpthk.cn/gtvmemjijh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhaomingkeji.xyz/gtxnnzztfg.html

Java: new Random().nextInt(100) + 1
来源：http://hz.0kj1m.cn/gtqolevpld.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.ehwqpu.com/gtxcvlcqkv.html

Ruby: rand(1..100)
来源：http://hz.tianlin.xyz/gtiswoymxv.html

C#:   new Random().Next(1, 101)
来源：http://hz.yanxiufei.cn/gtxszchjdx.html

[A11] 条件表达式（三元）
来源：http://hz.gzhubu.top/gtmjitncab.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.gogol.net.cn/gteiutvxuj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.ywan-chungtsiang.top/gteiiuwpek.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gtzuplhnsd.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zhengqikj.top/gtxhofhvva.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.ppjwa.cn/gtppcqjvku.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.52xcode.cn/gtfhxzgbkw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.ywan-chungtsiang.top/gtsfvdwykm.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.tian-w.cn/gtvhvqyyjo.html

[A12] 字符串插值 / 格式化
来源：http://hz.ivvv.top/gtvvrfmosu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.316326.xyz/gtgbhipxki.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.haohaochexian.top/gthnyhhena.html

JS:   `Hello, ${name}!`
来源：http://hz.aizwys.cn/gtnwnbvcii.html

TS:   `Hello, ${name}!`
来源：http://hz.gaohongyu789.top/gtxitavlev.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.yangfankeji.com/gtjqkbmtrk.html


<!-- 参考信息 -->