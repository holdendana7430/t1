代发 wailian999

[U79] PHP：静态分析
来源：http://hz.jlsjyb.cn/gtqaudvaja.html

composer require --dev phpstan/phpstan
来源：http://hz.hysaishi.cn/gtpcqvsvpi.html

[U80] PHP：代码规范修复
来源：http://hz.vqdsnc.cn/gtxtoxwmyp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hfpthk.cn/gttvjwjdqi.html

[U81] JS：初始化项目
来源：http://hz.shzxlz.cn/gtbeorgame.html

npm init -y;  npm i express
来源：http://hz.snrcjt.cn/gtwzueocqy.html

[U82] JS：package.json 脚本
来源：http://hz.tianlin.xyz/gtgnmlvowl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.sysykeji.top/gtzpbnotwg.html

[U83] JS：ES Module 导入导出
来源：http://hz.andypj.xyz/gtmfuxcdnf.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hongshengwenyu.top/gtotgpdpyf.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangkeji.top/gtdtycbgsw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.gzhubu.top/gtycgcowmv.html

[U85] JS：可选链
来源：http://hz.cucudq.cn/gtdgtxbqod.html

a?.b?.c
来源：http://hz.sysykeji.top/gtwyyobjfb.html

[U86] JS：空值合并
来源：http://hz.hywenlv.cn/gtapohszdj.html

a ?? b
来源：http://hz.daria6918.cn/gtmozugqdh.html

[U87] JS：解构默认值
来源：http://hz.ydjk.org.cn/gthjqedpzy.html

const { a = 1, b = 2 } = obj;
来源：http://hz.aizwys.cn/gtuppwdpwv.html

[U88] JS：对象展开合并
来源：http://hz.xuanzx.com/gtrsvtamyz.html

{ ...a, ...b }
来源：http://hz.yuanzhike.top/gttdabimdw.html

[U89] JS：数组去重
来源：http://hz.zhiwuduotai.top/gtpmhpayqk.html

[...new Set(arr)]
来源：http://hz.tian-w.cn/gtylunqcgc.html

[U90] JS：数字数组排序
来源：http://hz.zycfv.cn/gtduzlambp.html

[...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtsordjjvq.html

[U91] JS：对象键值遍历
来源：http://hz.hammf.cn/gthoezewjt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xinyue.icu/gtsxxgswyq.html

[U92] JS：深拷贝
来源：http://hz.gzhubu.top/gthuoayddj.html

structuredClone(obj)
来源：http://hz.xuanzx.com/gtbqwnvtfr.html

[U93] JS：模板字符串
来源：http://hz.feifeiyinyue.top/gtkkgmifwb.html

`共 ${n} 条`
来源：http://hz.xylfe.cn/gtemexzobe.html

[U94] JS：箭头函数
来源：http://hz.jqgfzy.top/gtqccrzksq.html

const double = x => x * 2;
来源：http://hz.cqqwz.cn/gttezfuqll.html

[U95] JS：Promise 包装
来源：http://hz.yj20258.top/gtnqwydazy.html

new Promise((resolve, reject) => {})
来源：http://hz.yvedp.cn/gtccfiebhc.html

[U96] JS：async/await 与异常
来源：http://hz.316326.xyz/gtfkkcpnkp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258.top/gtredtgxha.html

[U97] JS：并发请求
来源：http://hz.guowangkeji.top/gtugaxmppt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtwygeiobb.html

[U98] JS：fetch 带 JSON
来源：http://hz.daria6918.cn/gtddbcolzu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.ehwqpu.com/gtzryitfkz.html

[U99] JS：事件监听
来源：http://hz.hysaishi.cn/gtxldyniuw.html

el.addEventListener("click", e => {})
来源：http://hz.chenlongwang.top/gtwpevydlv.html

[U100] JS：DOM 查询
来源：http://hz.xinyue.icu/gtkxfsvojy.html

document.querySelector(".item")
来源：http://hz.zhixingplan.top/gtatzxfucr.html

[U101] JS：classList 操作
来源：http://hz.hywenlv.cn/gtvtekpatl.html

el.classList.toggle("active")
来源：http://hz.shuidangran.top/gtmklatwee.html

[U102] JS：本地存储
来源：http://hz.hysaishi.cn/gtlnsjirek.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.quarkkingdee.top/gttnerkuxa.html

[U103] JS：定时器
来源：http://hz.316326.xyz/gtpotlvtdx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.52xcode.cn/gtmtogfhat.html

[U104] JS：防抖
来源：http://hz.tian-w.cn/gtrfvvelpi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.ybcxt.top/gtzwfymyue.html

[U105] JS：节流
来源：http://hz.pycfn.com/gtkgruztra.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hnxiangtu.top/gtuqvnxlxc.html

[U106] JS：日期格式化
来源：http://hz.yuanzhike.top/gtdgogjhbn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.0kj1m.cn/gtxhcnovzz.html

[U107] JS：数字千分位
来源：http://hz.wangshuangyany.cn/gtnlryfsvx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuxming.cn/gtxbwffsib.html

[U108] JS：随机整数
来源：http://hz.zhoulong.xyz/gtixkuojkx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.9152youxi.cn/gteqopwjug.html

[U109] JS：数组分组
来源：http://hz.havefunace.top/gtwhcnmccs.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hywenlv.cn/gtdmclbtej.html

[U110] JS：数组分块
来源：http://hz.haohaochexian.top/gttsziskdk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.havefunace.top/gtrrehwwjl.html

[U111] JS：对象转 Map
来源：http://hz.zdqjudy.top/gtcztxxunc.html

new Map(Object.entries(obj))
来源：http://hz.aizwys.cn/gtlkuxxvph.html

[U112] JS：字符串补位
来源：http://hz.aizwys.cn/gtpntrkdcj.html

"7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtxwgyuvju.html

[U113] JS：正则替换全部
来源：http://hz.dianchejie.cn/gtrkezqxva.html

s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtsxwbcnhu.html

[U114] JS：JSON 深比较
来源：http://hz.redwolf501.top/gtoqppwqoy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.dashuyun.cn/gtxrfvvoow.html

[U115] JS：生成 UUID
来源：http://hz.ywan-chungtsiang.top/gtvumonzen.html

crypto.randomUUID()
来源：http://hz.hysaishi.cn/gtguhydhfi.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.sxryk.cn/gtbtaonsdx.html

/** @param {string} name */ function f(name) {}
来源：http://hz.316326.xyz/gtjipmnynj.html

[U117] JS：单元测试
来源：http://hz.ppjwa.cn/gtubwyjpkd.html

npm i -D vitest;  npx vitest
来源：http://hz.yueranfly.top/gtglahnzzy.html

[U118] JS：开发服务器
来源：http://hz.xuetiantiany.cn/gtokvtppzb.html

npm i -D vite;  npx vite
来源：http://hz.yuanzhike.top/gtkcrhvtvp.html

[U119] JS：生产构建
来源：http://hz.shanyushiyangtech.top/gtemqegfew.html

npx vite build
来源：http://hz.xuanzx.com/gtpbjslmzl.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hywenlv.cn/gtrdqdleer.html

import.meta.env.VITE_API_URL
来源：http://hz.svipenyu.cn/gtwrmfcoud.html

================================================================================
来源：http://hz.gogol.net.cn/gtlawsjfkj.html

统计汇总
来源：http://hz.feifeiyinyue.top/gtmecwvrud.html

================================================================================
来源：http://hz.kuanghao11.cn/gtnhznqpli.html

按语言统计（条）：
来源：http://hz.tanke756.top/gtfyflbarq.html

Python ......... 252
来源：http://hz.sweek.top/gtcqnkzzyy.html

PHP ............ 252
来源：http://hz.meibo888.top/gtrdbqryqu.html

JavaScript ..... 252
来源：http://hz.mhx1999.top/gtaetwvtfj.html

TypeScript ..... 212
来源：http://hz.0kj1m.cn/gtmgsjzihd.html

Java ........... 212
来源：http://hz.zdqjudy.top/gtcxdtuipf.html

Go ............. 212
来源：http://hz.hywenlv.cn/gtzktnxioa.html

Ruby ........... 212
来源：http://hz.shanyushiyangkeji.top/gteciefbed.html

C# ............. 212
来源：http://hz.yuanzhike.top/gtjdycmcrs.html

C .............. 30
来源：http://hz.wangdashe.top/gtzbvrcyab.html

C++ ............ 30
来源：http://hz.andypj.xyz/gtscwomjjo.html

SQL ............ 90
来源：http://hz.hysaishi.cn/gtsimvsvxq.html

Bash ........... 80
来源：http://hz.zhiwuduotai.top/gtdeuepnfn.html

Kotlin ......... 15
来源：http://hz.birdmap.top/gtaebimsur.html

Swift .......... 15
来源：http://hz.ywan-chungtsiang.top/gtjabwplcw.html

Lua ............ 10
来源：http://hz.zhaomingkeji.xyz/gtewplecei.html

Perl ........... 10
来源：http://hz.jyoumei.cn/gtkfrzwfcm.html

Scala .......... 10
来源：http://hz.pycfn.com/gtnkrtglic.html

------------------------------------
来源：http://hz.chenlongwang.top/gtmmzazcvg.html

合计 ........... 2106 条
来源：http://hz.wangshuangyany.cn/gtbwyahiaa.html

按章节统计：
来源：http://hz.daxiang520.top/gtswzatbfl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.sufxvd.cn/gtbfqvlcxt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhiwuduotai.top/gtgghysabw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jyoumei.cn/gtwpuvuldn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.quarkkingdee.top/gtvozugwpb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.xinyue.icu/gtxnlhdoun.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.tianlin.xyz/gtoorfohgs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.svipenyu.cn/gtgryydhwj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yongpay.top/gtxgoxkzny.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtwrsipzkm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.wangdashe.top/gtmsfcpjwf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gtahxnpzjk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.shuidangran.top/gtjgluqlww.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.aizwys.cn/gtbdknqemd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.zhoulong.xyz/gtqyxnpeon.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yueranfly.top/gtliizgwfl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yvedp.cn/gtngythimd.html

Q SQL 专题                              90
来源：http://hz.tian-w.cn/gtkhjfeany.html

R Bash 专题                             80
来源：http://hz.xuanzx.com/gtupehybyv.html

S C / C++ 专题                          60
来源：http://hz.xylfe.cn/gtjgoamfij.html

T 其他语言补充                          60
来源：http://hz.ydzc1.top/gtrtluycvo.html

U 高频实用片段                         120
来源：http://hz.guowangkeji.top/gtquixmxxz.html

------------------------------------
来源：http://hz.redwolf501.top/gtovkohecs.html

合计                                  2106 条
来源：http://hz.yangfankeji.com/gtbylerhlc.html

--------------------------------------------------------------------------------
来源：http://hz.gzhubu.top/gtiqachlpx.html

使用提醒
来源：http://hz.gogol.net.cn/gtcffednkt.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gteqdsadqi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yueranfly.top/gtotjpgipl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.quarkkingdee.top/gteovnaekd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yangfankeji.com/gtvcqzpvoi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.9152youxi.cn/gtmdhpbfnq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.snrcjt.cn/gtinmmohmi.html

—— 文件结束 ——
来源：http://hz.hnqzz.top/gtkcazgizr.html

================================================================================
来源：http://hz.mhx1999.top/gtbbwttdjb.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.zhoulong.xyz/gtokemssqs.html

Common Programming Examples Cheat Book
来源：http://hz.yonumen.top/gtppdlkvxb.html

================================================================================
来源：http://hz.cqqwz.cn/gtbsxbnevi.html

【收录内容】
来源：http://hz.cucudq.cn/gtcjmluxln.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.0kj1m.cn/gtpqkxmpbn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.bjfxy.top/gtmaetdmxw.html

SQL · Bash · C · C++
来源：http://hz.wangshuangyany.cn/gtuwqheqhw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.nanxinkj.top/gtotaotyrc.html

【使用说明】
来源：http://hz.bjfxy.top/gtelphzadt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.jqgufenzy.top/gtdzfnzbrb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.fengsongda.top/gtwabwwznz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.cdnleiting.top/gtvadsxcjg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.gotoacloud.top/gtwtbjlwxa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.snrcjt.cn/gtstrglmse.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.xingfuxueyuan.xyz/gtfvgiibni.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.ybcxt.top/gtilhxezis.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.0kj1m.cn/gtroqaxeye.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.ivvv.top/gttwjtpwpj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xinyue.icu/gtvedfepzj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.kuanghao11.cn/gtmafcdjsb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.316326.xyz/gtkhpcunzd.html

【文件统计】
来源：http://hz.yuxming.cn/gtqpcnlvfg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.zdqjudy.top/gtiixfqgth.html

--------------------------------------------------------------------------------
来源：http://hz.nanxinkj.top/gteopyhned.html

目  录
来源：http://hz.cdnleiting.top/gtsrqckzle.html

--------------------------------------------------------------------------------
来源：http://hz.xinyue.icu/gtuymmlxxh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.snrcjt.cn/gtheslouuy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.0kj1m.cn/gtjdsupffn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.redwolf501.top/gtnkmebkxs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.nanxuanxn.top/gttlbvsvhg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.feifeiyinyue.top/gtsrjpbqgx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.jiagoushi.top/gtprylovcn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jinqigfzy.top/gtmbqphfvr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.iojbl.cn/gttixacnta.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.chenjidiqi.icu/gtkinutvln.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gtkngjkuwf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtbgpkflez.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.gaohongyu789.top/gtwghftokf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gtqoltazou.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.snrcjt.cn/gtxuirjcgb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.52xcode.cn/gtsltebcaz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.yuanzhike.top/gtmajwnjxj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.52xcode.cn/gtdeaunbfe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.gzhubu.top/gtrxwidxmq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.tanke756.top/gttgzttgvw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hfpthk.cn/gtwgoogqmk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.316326.xyz/gtjyrzrihg.html

================================================================================
来源：http://hz.guowangkeji.top/gtrhobedtw.html

A. 基础语法与类型
来源：http://hz.pengpengdd.cyou/gtmlabwbxa.html

================================================================================
来源：http://hz.gotoacloud.top/gtdlpzvohd.html

[A01] Hello World
来源：http://hz.yanxiufei.cn/gtffiqmidu.html

Py:   print("Hello, World!")
来源：http://hz.hammf.cn/gtdavofpus.html

PHP:  echo "Hello, World!";
来源：http://hz.gogol.net.cn/gtkwfkmiwp.html

JS:   console.log("Hello, World!");
来源：http://hz.chenlongwang.top/gtsxrojobf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.tianlin.xyz/gtdqhlsbom.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenjidiqi.icu/gtgdrtwxjo.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xingfuxueyuan.xyz/gtsxkuqotd.html

Ruby: puts "Hello, World!"
来源：http://hz.nanxuanxn.top/gtcjfrfzls.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ivvv.top/gtrywxruml.html

[A02] 变量声明与赋值
来源：http://hz.hnxiangtu.top/gtldoruekl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.kuanghao11.cn/gttgxaqzyi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.hnqzz.top/gtcutxmjjx.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.zhijiandao.cn/gtgxwboqbv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.ehwqpu.com/gteiagmifm.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhiwuduotai.top/gtlnjmmvdw.html

Go:   name := "Alex"; age := 20
来源：http://hz.gaohongyu789.top/gtyobvzqie.html

Ruby: name = "Alex"; age = 20
来源：http://hz.hysaishi.cn/gtildnyunv.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.ydjk.org.cn/gtfwvwjvfs.html

[A03] 常量定义
来源：http://hz.havefunace.top/gtbyqeyhps.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.shuidangran.top/gtjkbuiwev.html

PHP:  const PI = 3.14159;
来源：http://hz.ehwqpu.com/gtpelibchy.html

JS:   const PI = 3.14159;
来源：http://hz.zdqjudy.top/gtbhsljqob.html

TS:   const PI: number = 3.14159;
来源：http://hz.tanke756.top/gtodmsifja.html

Java: static final double PI = 3.14159;
来源：http://hz.fzhhl.top/gtbivelbbf.html

Go:   const PI = 3.14159
来源：http://hz.jqgufenzy.top/gtozidbqmm.html

Ruby: PI = 3.14159
来源：http://hz.gaohongyu789.top/gthiroreif.html

C#:   const double PI = 3.14159;
来源：http://hz.jqgufenzy.top/gtufvtgkdt.html

[A04] 判断变量类型
来源：http://hz.cheryme.top/gtojxpfeoz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.zhixingplan.top/gtoowfbpcn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.daxiang520.top/gtdahqfpoc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.daxiang520.top/gtpgixxxaj.html

TS:   typeof x; x instanceof Date
来源：http://hz.wangshuangyany.cn/gtegzjcyte.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhengqikj.top/gthlvshzes.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.quarkkingdee.top/gtbexoicgu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.hywenlv.cn/gtuqqpbzcy.html

C#:   x.GetType().Name; x is int
来源：http://hz.guannengcc.top/gtcmudaciv.html

[A05] 整数除法与取模
来源：http://hz.shuidangran.top/gtcuhkmryh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jiagoushi.top/gtqranemjx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.ydjk.org.cn/gtshlaldth.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.aibaodan.cn/gtgzykanpr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.zhijiandao.cn/gtekqajvsu.html

Java: 7 / 2; 7 % 2
来源：http://hz.cqqwz.cn/gtixcyacnh.html

Go:   7 / 2; 7 % 2
来源：http://hz.0kj1m.cn/gtneuvgbvf.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.jlsjyb.cn/gtmpjnbnmc.html

C#:   7 / 2; 7 % 2
来源：http://hz.smart0.xyz/gtravbwtzd.html

[A06] 字符串转数字
来源：http://hz.zdqjudy.top/gtfcqvasaq.html

Py:   int("42"); float("3.14")
来源：http://hz.vqdsnc.cn/gtjrokgbaa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zhongyouzk.top/gtvieijlco.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.zhaomingkeji.xyz/gtpeaagvdy.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yonumen.top/gtbjzdcxjt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.kuanghao11.cn/gtzlvcjksc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.0kj1m.cn/gtyfshjwwx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.cucudq.cn/gtticwtrii.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jinghuilouyu.cn/gtxgiamnpw.html

[A07] 数字转字符串
来源：http://hz.gaohongyu789.top/gtazkyppjs.html

Py:   str(42)
来源：http://hz.wangdashe.top/gtknwdrxdz.html

PHP:  (string) 42; strval(42)
来源：http://hz.xingfuxueyuan.xyz/gtbqappfsw.html

JS:   String(42); (42).toString()
来源：http://hz.sysykeji.top/gtxpbebyqo.html

TS:   String(42)
来源：http://hz.hysaishi.cn/gtmhejnpyg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.cheryme.top/gtmdocwtpz.html

Go:   strconv.Itoa(42)
来源：http://hz.zhiwuduotai.top/gtvtqoytwx.html

Ruby: 42.to_s
来源：http://hz.tian-w.cn/gtfuwhvjxs.html

C#:   42.ToString()
来源：http://hz.cucudq.cn/gttslzkbgn.html

[A08] 取整与四舍五入
来源：http://hz.fengsongda.top/gtaoqvzfzc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.hysaishi.cn/gtdanbaguf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.chenlongwang.top/gtlrgmujzt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hysaishi.cn/gtafvaqira.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jinyuanbaomall.cn/gtajrnntkp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.guannengcc.top/gtdayypjdy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.nwbrower.top/gtthpqcsbf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jlsjyb.cn/gtauimruvp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.redwolf501.top/gtuhvqaldn.html

[A09] 绝对值与最大最小值
来源：http://hz.tianlin.xyz/gtsgabrqlf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shangyingyoupin.top/gtmcbpldwa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.sxryk.cn/gtpqqwejkd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.haohaochexian.top/gtdkrdaenu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.zhiwuduotai.top/gtifarijhp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.pengpengdd.cyou/gtriymhqeo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jlsjyb.cn/gtrmnnqtyn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.birdmap.top/gtftowwitl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.smart0.xyz/gtdhvbduds.html

[A10] 生成随机数
来源：http://hz.sweek.top/gtrhkjyxhr.html

Py:   import random; random.randint(1, 100)
来源：http://hz.tian-w.cn/gtwxllbhis.html

PHP:  random_int(1, 100);
来源：http://hz.xylfe.cn/gtckmbbfqg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.andypj.xyz/gtswdbbsut.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.snrcjt.cn/gttrbgfobo.html

Java: new Random().nextInt(100) + 1
来源：http://hz.andypj.xyz/gtskzqbyeu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.cashguo.top/gtblwfggax.html

Ruby: rand(1..100)
来源：http://hz.jinyuanbaomall.cn/gtrsaljjbn.html

C#:   new Random().Next(1, 101)
来源：http://hz.hfpthk.cn/gtkjucfwgx.html

[A11] 条件表达式（三元）
来源：http://hz.tian-w.cn/gtrahvbaku.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.yongpay.top/gthrtxbdmy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.zhongyouzk.top/gttspvqbdr.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.zhiwuduotai.top/gtvxgvcdau.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.kuanghao11.cn/gtaflocnef.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.havefunace.top/gtavxyqtnl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.pengpengdd.cyou/gtscfwrmeu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.yj20258.top/gtmvhysckf.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.sxryk.cn/gtmsfveyfl.html

[A12] 字符串插值 / 格式化
来源：http://hz.guowangkeji.top/gtdwwzardp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.0kj1m.cn/gtsybhxrbd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.redwolf501.top/gtgxbfztiq.html

JS:   `Hello, ${name}!`
来源：http://hz.wangshuangyany.cn/gtkihovejo.html

TS:   `Hello, ${name}!`
来源：http://hz.hywenlv.cn/gtowgidxck.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.pengpengdd.cyou/gtjjdwuyfo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.fengsongda.top/gtfeeorofz.html

Ruby: "Hello, #{name}!"
来源：http://hz.nanxuanxn.top/gtawdpvdir.html

C#:   $"Hello, {name}!"
来源：http://hz.pycfn.com/gtazffudai.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jqgfzy.top/gtjgrjfvjc.html


<!-- 参考信息 -->