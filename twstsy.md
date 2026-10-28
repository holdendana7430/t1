代发 wailian999

[U81] JS：初始化项目
来源：http://hz.tian-w.cn/gtdvsowxzn.html

npm init -y;  npm i express
来源：http://hz.sufxvd.cn/gthwcnqzux.html

[U82] JS：package.json 脚本
来源：http://hz.xziqi.cn/gtpkjmdgsf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.bjfxy.top/gtqwvtyxyg.html

[U83] JS：ES Module 导入导出
来源：http://hz.cheryme.top/gtrrgpiwds.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.9152youxi.cn/gtysdgzxga.html

[U84] JS：CommonJS 写法
来源：http://hz.jianghu66.top/gtclcaspwa.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.aibaodan.cn/gtmqlstqcl.html

[U85] JS：可选链
来源：http://hz.sxryk.cn/gtdshkvvnz.html

a?.b?.c
来源：http://hz.ehwqpu.com/gtlvcdxtao.html

[U86] JS：空值合并
来源：http://hz.nwbrower.top/gtjoagnbnp.html

a ?? b
来源：http://hz.zhixingplan.top/gtqcjjkkvp.html

[U87] JS：解构默认值
来源：http://hz.ppjwa.cn/gtzlhytopa.html

const { a = 1, b = 2 } = obj;
来源：http://hz.tanke756.top/gtsvdszpei.html

[U88] JS：对象展开合并
来源：http://hz.vqdsnc.cn/gtwzmdypiy.html

{ ...a, ...b }
来源：http://hz.fzhhl.top/gtqajrlgsy.html

[U89] JS：数组去重
来源：http://hz.guowangkeji.top/gtyjmzrumf.html

[...new Set(arr)]
来源：http://hz.mhx1999.top/gtofitvlqy.html

[U90] JS：数字数组排序
来源：http://hz.fzhhl.top/gtaptnwtqx.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtegdrsgbz.html

[U91] JS：对象键值遍历
来源：http://hz.shanyushiyangtech.top/gtcrovoyzh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.gaohongyu789.top/gtwxjsxiyd.html

[U92] JS：深拷贝
来源：http://hz.52xcode.cn/gtrjwndnti.html

structuredClone(obj)
来源：http://hz.dashuyun.cn/gtaumjkxmx.html

[U93] JS：模板字符串
来源：http://hz.shuidangran.top/gthlnpjmik.html

`共 ${n} 条`
来源：http://hz.gaohongyu789.top/gtjhsuyazk.html

[U94] JS：箭头函数
来源：http://hz.zhengqikj.top/gtbekgxlla.html

const double = x => x * 2;
来源：http://hz.aizwys.cn/gtttfchgfi.html

[U95] JS：Promise 包装
来源：http://hz.hnxiangtu.top/gtavnvggrf.html

new Promise((resolve, reject) => {})
来源：http://hz.tian-w.cn/gtmntefois.html

[U96] JS：async/await 与异常
来源：http://hz.nwbrower.top/gtzndwtzhs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtbpgcvjhq.html

[U97] JS：并发请求
来源：http://hz.daxiang520.top/gtsgvdaypo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jiagoushi.top/gtuajfajsl.html

[U98] JS：fetch 带 JSON
来源：http://hz.cashguo.top/gtkxoxfdov.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.svipenyu.cn/gtteaxbgnr.html

[U99] JS：事件监听
来源：http://hz.pengpengdd.cyou/gtlgclhnvo.html

el.addEventListener("click", e => {})
来源：http://hz.shuidangran.top/gtnvdyqxar.html

[U100] JS：DOM 查询
来源：http://hz.hysaishi.cn/gtnesvnaib.html

document.querySelector(".item")
来源：http://hz.52xcode.cn/gtzurpnmfu.html

[U101] JS：classList 操作
来源：http://hz.cashguo.top/gtvxafzhdp.html

el.classList.toggle("active")
来源：http://hz.jinqigfzy.top/gtsternrjl.html

[U102] JS：本地存储
来源：http://hz.sxryk.cn/gtmvedshrg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.daxiang520.top/gtxrubpcrx.html

[U103] JS：定时器
来源：http://hz.hnqzz.top/gtswoknydg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zdqjudy.top/gtyuktliyw.html

[U104] JS：防抖
来源：http://hz.52xcode.cn/gtoyxvobdp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shanyushiyangkeji.top/gthnhpzufa.html

[U105] JS：节流
来源：http://hz.andypj.xyz/gtmldyveae.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.9152youxi.cn/gtiaieejps.html

[U106] JS：日期格式化
来源：http://hz.hywenlv.cn/gtuvisddma.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.fengsongda.top/gtptsrlevm.html

[U107] JS：数字千分位
来源：http://hz.zhaomingkeji.xyz/gtxdvjrujg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.zhijiandao.cn/gtdkpssuav.html

[U108] JS：随机整数
来源：http://hz.hammf.cn/gtzbjichgr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jianghu66.top/gtxyyrsgsb.html

[U109] JS：数组分组
来源：http://hz.cdnleiting.top/gtsrsjflgq.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xuanzx.com/gthqfihfsj.html

[U110] JS：数组分块
来源：http://hz.jinyuanbaomall.cn/gtxgkfpjet.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jianghu66.top/gtmelwdlrl.html

[U111] JS：对象转 Map
来源：http://hz.shanyushiyangkeji.top/gtotsaaptn.html

new Map(Object.entries(obj))
来源：http://hz.meibo888.top/gtmpaselrx.html

[U112] JS：字符串补位
来源：http://hz.shanyushiyangkeji.top/gtqyvumzwi.html

"7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtyulpqzuf.html

[U113] JS：正则替换全部
来源：http://hz.daria6918.cn/gtdeykyaeg.html

s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtdyopbncw.html

[U114] JS：JSON 深比较
来源：http://hz.52xcode.cn/gtrgtgrkif.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hfpthk.cn/gtbwyqovmm.html

[U115] JS：生成 UUID
来源：http://hz.gzhubu.top/gtdhzxzgao.html

crypto.randomUUID()
来源：http://hz.shanyushiyangtech.top/gtrgdrvcbl.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.pengpengdd.cyou/gtzrtrwhmw.html

/** @param {string} name */ function f(name) {}
来源：http://hz.cheryme.top/gtvofkzowi.html

[U117] JS：单元测试
来源：http://hz.havefunace.top/gtmnywpmrw.html

npm i -D vitest;  npx vitest
来源：http://hz.zhaomingkeji.xyz/gtmipbdkyn.html

[U118] JS：开发服务器
来源：http://hz.pycfn.com/gtxwlqpetz.html

npm i -D vite;  npx vite
来源：http://hz.ybcxt.top/gtidvrbfwa.html

[U119] JS：生产构建
来源：http://hz.wangdashe.top/gtjxyjtekz.html

npx vite build
来源：http://hz.jyoumei.cn/gthtlatzxk.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hfpthk.cn/gtaiochvxe.html

import.meta.env.VITE_API_URL
来源：http://hz.yuanzhike.top/gtnjkdlhpx.html

================================================================================
来源：http://hz.fengsongda.top/gticanaaip.html

统计汇总
来源：http://hz.ydzc1.top/gtuliajwvk.html

================================================================================
来源：http://hz.9152youxi.cn/gtrqbcaasr.html

按语言统计（条）：
来源：http://hz.sysykeji.top/gtrxamrhng.html

Python ......... 252
来源：http://hz.jinghuilouyu.cn/gtefakpppg.html

PHP ............ 252
来源：http://hz.guannengcc.top/gtiafuulgz.html

JavaScript ..... 252
来源：http://hz.xinyue.icu/gtmscbkjce.html

TypeScript ..... 212
来源：http://hz.sweek.top/gtxwlynjti.html

Java ........... 212
来源：http://hz.dianchejie.cn/gtzmmozsxf.html

Go ............. 212
来源：http://hz.zhijiandao.cn/gtsigmzcbt.html

Ruby ........... 212
来源：http://hz.hfpthk.cn/gtgfkfzull.html

C# ............. 212
来源：http://hz.gaohongyu789.top/gtqoeblkku.html

C .............. 30
来源：http://hz.sxryk.cn/gtjegzxleh.html

C++ ............ 30
来源：http://hz.xziqi.cn/gtfhtsmdiy.html

SQL ............ 90
来源：http://hz.hysaishi.cn/gtgsdjclfd.html

Bash ........... 80
来源：http://hz.ybcxt.top/gtpjcrhray.html

Kotlin ......... 15
来源：http://hz.daxiang520.top/gtexalaioi.html

Swift .......... 15
来源：http://hz.cucudq.cn/gtztijveew.html

Lua ............ 10
来源：http://hz.yangfankeji.com/gtxbsnmzdp.html

Perl ........... 10
来源：http://hz.cucudq.cn/gtewylklmg.html

Scala .......... 10
来源：http://hz.0kj1m.cn/gtgtrgdigj.html

------------------------------------
来源：http://hz.ybcxt.top/gtqkeflouj.html

合计 ........... 2106 条
来源：http://hz.daria6918.cn/gtwpvoplaw.html

按章节统计：
来源：http://hz.xuanzx.com/gtbnmdpdmt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.gotoacloud.top/gtpzhzlxcc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.daria6918.cn/gtonigmktc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gtrgsnogrv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.kuanghao11.cn/gtdmjtcxpl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.sysykeji.top/gtueovcczi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.cucudq.cn/gtweqsaesn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.yvedp.cn/gtnibcqmtw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nwbrower.top/gteshvlvrf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.guowangkeji.top/gtfviqdrhp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.tianlin.xyz/gtmrnoakwk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtterevehy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.9152youxi.cn/gtjwkegthd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.jyoumei.cn/gtzjibqpbv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jyoumei.cn/gtwyvbpgps.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yj20258888.top/gtqochosit.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.gogol.net.cn/gtavkotakx.html

Q SQL 专题                              90
来源：http://hz.shanyushiyangtech.top/gteozmkyse.html

R Bash 专题                             80
来源：http://hz.zhixingplan.top/gtxodxwqwz.html

S C / C++ 专题                          60
来源：http://hz.wangshuangyany.cn/gtkzttcxcn.html

T 其他语言补充                          60
来源：http://hz.havefunace.top/gtgfefozzp.html

U 高频实用片段                         120
来源：http://hz.vqdsnc.cn/gtkzqdujeq.html

------------------------------------
来源：http://hz.zhongyouzk.top/gtfbheuzoi.html

合计                                  2106 条
来源：http://hz.aibaodan.cn/gtrtqtfhmw.html

--------------------------------------------------------------------------------
来源：http://hz.jianghu66.top/gtulgwwlqn.html

使用提醒
来源：http://hz.cucudq.cn/gtaciqhcpj.html

--------------------------------------------------------------------------------
来源：http://hz.hammf.cn/gteamggghk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.gzhubu.top/gtfoyrkkmt.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.guannengcc.top/gtecwtbusm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yangfankeji.com/gtsffcziwp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.jianghu66.top/gtjychzmeu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zdqjudy.top/gtefdpditq.html

—— 文件结束 ——
来源：http://hz.sweek.top/gtgyxictoe.html

================================================================================
来源：http://hz.aizwys.cn/gtwebyawak.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.quarkkingdee.top/gtqnpptqoc.html

Common Programming Examples Cheat Book
来源：http://hz.gzhubu.top/gtwwhruchf.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrtmllmqt.html

【收录内容】
来源：http://hz.aizwys.cn/gtswjqbpby.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yanxiufei.cn/gtfmrfujqu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.zhixingplan.top/gtrphjopgi.html

SQL · Bash · C · C++
来源：http://hz.zycfv.cn/gtluzaopfv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.c1oappe.top/gtxmvmsjrb.html

【使用说明】
来源：http://hz.jinqigufen.top/gttzlaskcb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.pycfn.com/gtnbjjfcwz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhijiandao.cn/gtzorjqait.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.hnxiangtu.top/gtlkjejtnx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.jianghu66.top/gttzrrcklm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jinqigfzy.top/gtjlyxsbmc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.gaohongyu789.top/gtfnvobdlw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.mhx1999.top/gtrqqvsemt.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.yangfankeji.com/gtcazrybqw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.yonumen.top/gtcdjzqrxp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shuidangran.top/gtftxudlrh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.nanxuanxn.top/gtiedvsilm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xuetiantiany.cn/gtfhoexutx.html

【文件统计】
来源：http://hz.hnxiangtu.top/gtlxlxomca.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.guannengcc.top/gtyabimmju.html

--------------------------------------------------------------------------------
来源：http://hz.yj202588.top/gtlptxsvhb.html

目  录
来源：http://hz.andypj.xyz/gtyrnxxhjw.html

--------------------------------------------------------------------------------
来源：http://hz.nanxinkj.top/gtjhuyjtej.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.cqqwz.cn/gtcsyoagtj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.shanyushiyangtech.top/gtsqzpxhcr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gtmhxcfhrd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.ywan-chungtsiang.top/gtqfbbutmr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.tanke756.top/gtozlyrmpn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yanxiufei.cn/gtydilsguo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.cucudq.cn/gtdgtzcima.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.xuanzx.com/gtzeexqptw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yangfankeji.com/gtabzijtlr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.tian-w.cn/gtxqpcanlf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.shanyushiyangkeji.top/gtvfirsyrj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yvedp.cn/gtwiacvwio.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.aibaodan.cn/gtzccgujxj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yangfankeji.com/gtqidtrjje.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.smart0.xyz/gtccgieqtm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gtzspsqxom.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.shuidangran.top/gtoznyscum.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.guowangkeji.top/gtqzrjfyqf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hfpthk.cn/gtoooqesbm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xingfuxueyuan.xyz/gttgdmgskw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gthnqhdtis.html

================================================================================
来源：http://hz.daria6918.cn/gtglgylmcw.html

A. 基础语法与类型
来源：http://hz.yj20258888.top/gtaokcoifi.html

================================================================================
来源：http://hz.vqdsnc.cn/gtacmpigqb.html

[A01] Hello World
来源：http://hz.jqgfzy.top/gtvptoazjx.html

Py:   print("Hello, World!")
来源：http://hz.hnqzz.top/gtdligyezd.html

PHP:  echo "Hello, World!";
来源：http://hz.52xcode.cn/gtdpzbojoo.html

JS:   console.log("Hello, World!");
来源：http://hz.jiagoushi.top/gtdrxguwiq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.316326.xyz/gtwlatecef.html

Java: System.out.println("Hello, World!");
来源：http://hz.dianchejie.cn/gtttawxtjx.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.feifeiyinyue.top/gtndxsepqq.html

Ruby: puts "Hello, World!"
来源：http://hz.nwbrower.top/gteonrafwc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.yuanzhike.top/gtktpoewod.html

[A02] 变量声明与赋值
来源：http://hz.hnqzz.top/gtbgvslepm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.sufxvd.cn/gtqmzknsql.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.cashguo.top/gtghfhsgfy.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.yanxiufei.cn/gtoeckymgn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ehwqpu.com/gtasfazgxj.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.cqqwz.cn/gtpbctdnok.html

Go:   name := "Alex"; age := 20
来源：http://hz.sysykeji.top/gtlssoerne.html

Ruby: name = "Alex"; age = 20
来源：http://hz.zhoulong.xyz/gttwilmojj.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ivvv.top/gtlpagoizb.html

[A03] 常量定义
来源：http://hz.shanyushiyangkeji.top/gteyvqnkoa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.guowangkeji.top/gtyreiljsj.html

PHP:  const PI = 3.14159;
来源：http://hz.zhengqikj.top/gtgynmsenn.html

JS:   const PI = 3.14159;
来源：http://hz.shzxlz.cn/gtembdavva.html

TS:   const PI: number = 3.14159;
来源：http://hz.0kj1m.cn/gtfxtsspvx.html

Java: static final double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtavgdbvmd.html

Go:   const PI = 3.14159
来源：http://hz.hnqzz.top/gtxewxrhxt.html

Ruby: PI = 3.14159
来源：http://hz.cqqwz.cn/gtmzymyllv.html

C#:   const double PI = 3.14159;
来源：http://hz.xylfe.cn/gtzydeyxto.html

[A04] 判断变量类型
来源：http://hz.jqgufenzy.top/gtcjndkqvw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.sufxvd.cn/gtuxkszjmh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.ybcxt.top/gtseupekov.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.0kj1m.cn/gtwhagmxzb.html

TS:   typeof x; x instanceof Date
来源：http://hz.tanke756.top/gtmtrjceko.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ehwqpu.com/gtjqyokept.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.pengpengdd.cyou/gtirkwyemr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.gzhubu.top/gtfrafpwgi.html

C#:   x.GetType().Name; x is int
来源：http://hz.xylfe.cn/gtucpkkzao.html

[A05] 整数除法与取模
来源：http://hz.yongpay.top/gtistdfyjm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.xziqi.cn/gtzdjbkpvn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.hywenlv.cn/gtzxqslolw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.meibo888.top/gtgszlfurj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.haohaochexian.top/gteyffliwz.html

Java: 7 / 2; 7 % 2
来源：http://hz.jqgufenzy.top/gtozhxltvz.html

Go:   7 / 2; 7 % 2
来源：http://hz.316326.xyz/gthdeqrcbe.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.yueranfly.top/gtrcfbggrx.html

C#:   7 / 2; 7 % 2
来源：http://hz.daria6918.cn/gtimwobbae.html

[A06] 字符串转数字
来源：http://hz.dianchejie.cn/gtalndvpgm.html

Py:   int("42"); float("3.14")
来源：http://hz.bjfxy.top/gtjepdlxar.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zycfv.cn/gtjfcmpcfd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.xingfuxueyuan.xyz/gtftwfvggt.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.c1oappe.top/gtuyjvosxu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.dianchejie.cn/gtaifjxcck.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.zhijiandao.cn/gtkxfiytak.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jiagoushi.top/gtrjsnsvus.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.birdmap.top/gttjrzilxk.html

[A07] 数字转字符串
来源：http://hz.xinyue.icu/gtqohwkydk.html

Py:   str(42)
来源：http://hz.cqqwz.cn/gtvhfghrlv.html

PHP:  (string) 42; strval(42)
来源：http://hz.wangshuangyany.cn/gtdgjvlyrv.html

JS:   String(42); (42).toString()
来源：http://hz.kuanghao11.cn/gtdvjrnmjp.html

TS:   String(42)
来源：http://hz.9152youxi.cn/gtsxnooyzv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hammf.cn/gtylsnyrvj.html

Go:   strconv.Itoa(42)
来源：http://hz.fzhhl.top/gtuwavjcgl.html

Ruby: 42.to_s
来源：http://hz.zhengqikj.top/gtbzfhvhsw.html

C#:   42.ToString()
来源：http://hz.jqgfzy.top/gtadnqbhwv.html

[A08] 取整与四舍五入
来源：http://hz.yuanzhike.top/gtpwyobyms.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.svipenyu.cn/gtpvhrbfnd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zycfv.cn/gthnrwhmxz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhiwuduotai.top/gtzofnswyb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.gaohongyu789.top/gtkuphjzeg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.ybcxt.top/gtvagsrhpe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.snrcjt.cn/gtqtwjejlm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.pengpengdd.cyou/gtyfuohhii.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.nwbrower.top/gttdbvbbqq.html

[A09] 绝对值与最大最小值
来源：http://hz.shanyushiyangkeji.top/gtzbrftaky.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zdqjudy.top/gtffrxnqca.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.nanxuanxn.top/gtcvmdipxo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.jiagoushi.top/gtxrdokdud.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhengqikj.top/gtxqvrwrgu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.andypj.xyz/gtusjcmkhv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jinqigufen.top/gtgfvcvbqm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.hysaishi.cn/gtbmuvxrcu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.meibo888.top/gtcyacnzsr.html

[A10] 生成随机数
来源：http://hz.sweek.top/gteczwbszx.html

Py:   import random; random.randint(1, 100)
来源：http://hz.dashuyun.cn/gtlqwlzqfc.html

PHP:  random_int(1, 100);
来源：http://hz.daria6918.cn/gtunflzolg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yongpay.top/gtmgjofarf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.52xcode.cn/gtwejxytsf.html

Java: new Random().nextInt(100) + 1
来源：http://hz.tianlin.xyz/gtjjtkqsdt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zhengqikj.top/gtzolbjuju.html

Ruby: rand(1..100)
来源：http://hz.52xcode.cn/gtxyeiyfpy.html

C#:   new Random().Next(1, 101)
来源：http://hz.316326.xyz/gtyddldosu.html

[A11] 条件表达式（三元）
来源：http://hz.c1oappe.top/gtgdyusjda.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.pycfn.com/gtxmbzsnsp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.yonumen.top/gthhuxvveh.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangkeji.top/gthjvbauzd.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jinqigufen.top/gtmlxlwftb.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.gogol.net.cn/gtyfbiaygv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.havefunace.top/gtzdmhlnsn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.smart0.xyz/gtvvcdopev.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.xingfuxueyuan.xyz/gtmbvsrdqv.html

[A12] 字符串插值 / 格式化
来源：http://hz.daria6918.cn/gtizvlgbme.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.gaohongyu789.top/gtcgunxwgz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.ehwqpu.com/gtbifhxdwf.html

JS:   `Hello, ${name}!`
来源：http://hz.0kj1m.cn/gtjzkaemsn.html

TS:   `Hello, ${name}!`
来源：http://hz.pycfn.com/gtitoaddco.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.ehwqpu.com/gtzdxnoczn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.iojbl.cn/gtgjhgkwsq.html

Ruby: "Hello, #{name}!"
来源：http://hz.nwbrower.top/gtqnyxjvfu.html

C#:   $"Hello, {name}!"
来源：http://hz.hammf.cn/gtkiljuntq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.c1oappe.top/gtphydonav.html

Py:   "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtjrsnkxxt.html

PHP:  "第一行\n第二行"
来源：http://hz.cheryme.top/gtxaejkhsd.html

JS:   "第一行\n第二行"
来源：http://hz.jqgfzy.top/gtilpqnlhg.html

TS:   "第一行\n第二行"
来源：http://hz.shanyushiyangkeji.top/gtwbqrmayx.html


<!-- 参考信息 -->