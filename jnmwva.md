代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ciomedov.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2uhaqgbcw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2meobgrlo.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2omdcsqrs.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ipwubmxi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2lafjimux.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2olqxawsb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ckardujt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dqcjobte.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jrpermrh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ojzgpril.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nffchkzf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2caeagqyd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rfmjtssw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jipcnalu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wvhbbebb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2qudmopny.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mixevklj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dkjgwggt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vrelkjhm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2nncnyudz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2nacpigbd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qshdvvgl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsdjvgoj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2rdxhntrt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ufbbrsxz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2akicrmda.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2jkfijnbh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2xcpozwgk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2axvgitpy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jgfosddt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cydtrufg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2iptobmrb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2hanjtdru.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2umohhnpq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2joxetqed.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2pbxiizxh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wpvvjizx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2thntwkij.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ygxdmgyd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zwlwcccw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nfabmyav.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zlpspkek.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2kbbwgrcx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ylvlopzn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fihbwign.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2psujxofm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vowsfvpy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2jneeuqjx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2auptbxvl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ucanrksa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2aihlbgmx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xmffhwds.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2geixvqod.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2trkpevuj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hvmpzgit.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2gxovtjan.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ydtbzhnj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2zgkkpxxg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mmgqrdhj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kgatfrmn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jstocukh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2baggwqcd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2hbyxavqz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hlwaufrc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2bwwzdkav.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xjazcxhw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ywmbitjp.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2eajqmayz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2qkyidtzp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2roatxrlh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2jhexbkbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxutdmot.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tszjhqbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndpzpfap.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2yhhxindx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xutlhpdf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2izxzrqlr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2wjvooyyk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ijxxpgnq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wwloguom.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wqxxnwgg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tnuqgcvw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zncculij.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2wyjubzkc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2isbceieh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2scivfoec.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ldauuabd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2vcietmur.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2eodtzicn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ijejwyvo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cjhmvthq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mozhpjhk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fkthhwfn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2woobkmkg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lwycojio.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dkteltfa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ppqfbpfz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pygezijn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xvvizmdc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2eawlhqiq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xskskwfx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2roqlszdu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2weohfzxl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lozfmmia.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2iqkhezcl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2evyrmksh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hzdlqtyy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2unsnriql.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lrbcosvc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2jciwhqtm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dqgumefk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2hsdkvrgs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2yjvlnspa.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2vsenpysj.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2wdpizsqj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2blbvwbwr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uudztavn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2tbxsyfjq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vkkreccl.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2nxttmdkx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nywhcjko.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2igdgnfkc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2mpyhtjfj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2zhbcwqoc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2oyonvnky.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2hivyzlyp.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2hwkrxwfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrgllvti.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2qzldkeaw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2rlidedqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whyoohzo.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2cjpxxukr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2czjwalzq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2synwtepw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2riqwyvcs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2enlglvcx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hxiysmgz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2gfxxmahu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2mfntjpro.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2dutqwkap.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rcbmtemv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2lbnvrvax.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2mwlmiqzs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2calrkhoa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2lxzurtru.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ketflkxf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2lazkbvbk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2mceeobri.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2vqpcmgvc.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2vbkuzjfh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xwtolofb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fgoxaxxs.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2adhvizyz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tokevtkk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xjsyrdqg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hfaydcyb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uvfahzpa.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lydngobq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pcvrgdgp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2vrqpbrcp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ocqamhap.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ucyoffcq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ddvaswsp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uzsbfbtv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mkoicjdq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lgrjrsor.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eyyvohqk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cyjmadim.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2efopgenb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cworxodc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2yqrewopo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fqytdwez.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2dcwfgquw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dqlxkxjw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uzqfdrli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iuqamexp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2kljufewi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfrneszm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qkzkutfv.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2odwbqzdz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2wyddotch.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bjhniblv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2moejwxjy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xiisyhob.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2eldhzjpl.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wfjqqxiz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vxbyppfu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ybnimeuw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2tkfebplq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zvdhpabs.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2powtbjui.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2flskmvpf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mmhozdvd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2qlbblvtf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2isiodfkb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2btemznhz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2gthseobx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2urocqttc.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2irgnbfza.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mqmzjtio.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ohjfdjiq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2djhctgpm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2nxmxtvfv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2nwyutzag.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hizcifgw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2uodrmjwk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ldmldjuh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2mpfreiqu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2zmwtblsh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2onfmsqyv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2tfxoalyy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2rkruvxoz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2rcfvdnrx.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rnfvmqme.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2vodlcquw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ddudjhek.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xskorpok.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ikomuqrm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gzybdxxt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hrgdpdmc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ecokcicc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eiydqrqj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rtorgocl.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kwmgjayi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mokegkmg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2newiqbpy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xxzjhknz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rvdndimq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2defbitay.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2aahvxblj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2lvhwcbrm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hljbzagr.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2crjwqxim.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2sfhjkeoo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2esrbeaqe.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ymukxbzp.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2rwphpjcx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ipbhmwvh.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xzmzbfzc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2lakeuftn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mopgruhk.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2icvnvjnc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wjryqvpg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2lfxozlfq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ephyysqh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2vyfuftnu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dfomgmfn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gpvteycv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2msgkoejt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ttnwueke.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vgsktijb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ukvzozsx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvarwxfi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bnzupgpz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpcoynzl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgrmujw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2airfxbdj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zrbaoory.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tpzawywo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2susebsbh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2oqnblvma.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2meemxfbx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2iutbjuqc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ueddzeco.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eliwsovk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2sabfagkd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2nqneesxy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2xtryltni.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2fucqryad.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2lzphvupv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ronbiyuz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pdqsxcgz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fkarfqut.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uxiwkfgm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2waxcfuor.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2neyhzdfd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2diczaluo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2xldgbsyk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2fsadpuog.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2qctzpebw.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2idpdpvtq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qhycxono.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2pkdhopjh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ejhqpmuw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2usybbwgf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2byzlvxpq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2dyaogtie.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bcprwrgp.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iczonbwo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2llwqompw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2edhogkel.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rcwsznhg.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ccxlsoqk.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wjhgiluv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qghkwpfx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2vzuxzoje.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2yvvamhtf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xtubfwbm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lswqphcv.html


<!-- 参考信息 -->