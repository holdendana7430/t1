代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ytoxowxc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3dfiqqybk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ijetjbwt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rseteqvj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3uvkgjsug.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3msmtjfdj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ghwlgvea.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3pwrsaoiq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ymhhvdld.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lwdxdaxx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3mvpnopck.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xyacpxnc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mmgjjsqf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3bkmozdnq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ardwegys.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3itrfjczh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hwbljnnc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3uwrmkpob.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lfbuogxo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3saimcllu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3imnjwpht.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bdhxoeca.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3impicidr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bulixnst.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ouazvzbf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zdlcyiud.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fvroblds.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3fhlzxwqt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tuonzjhb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ahcpujzm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3oebttnsp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3prjmszhg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dyirtufq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3blenzwhp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3hsbtclwj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xduecyta.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3mcjzgueg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3knjumkve.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ctghzzvl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xnmatgnj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vmluasvm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3krckjdee.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ysrdfrus.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3yfweiqph.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lziuuzmo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jatuaucn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3picdgpol.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3miuqaiaj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3aikbkxnt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3udqsvkkb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3flzuobqf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nqavysxc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3kydjosuh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3muqldkxk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3tccvfpul.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tcwzusra.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3woyjryre.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vdgyqvdo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nhnihrjj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wynzwjds.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ocfnurku.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cdgupeju.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tsmuvqin.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulosqtun.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bjscwttm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3zbhfwytw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3papmewjm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wzvtfpoh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3adpwelbg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3waupzffw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bzhauvqu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ohsslwpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znuoqkxc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kkpeshzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktouwrtn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3gtehwjdf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3iylzvwfg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3bdzitzjm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3eldxzsqk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ypxtxfxc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mswtpxzl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jdohdefu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pfusfzby.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mbzhgasc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3clgeclpj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3djyndgnb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ljahmrjq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3giualmcz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3sbpoesqp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3edfrzlxn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nfwbijjj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3dcgcsbpj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zcdaznxn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qqtipyws.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3plqrlzge.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3eocvgxht.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nwkrweur.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3evanllsy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3chuvbqdb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rhpjzxer.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jvcnoyqa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3coacsyfk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gzfmpfrx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3memvgkab.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xwbqfwas.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wewmmpvx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rtqydzok.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fndeckmd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xxbnwgdx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mazulxsr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3qgdgkrgo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3alkhhazk.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3szoovqch.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3wxqcwmse.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3nqjubwbf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3inecoqqp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3jhmuiiht.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ukkoxnrd.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fdtwozxu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cxputvkt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ajdifyco.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lzyvcarq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3rnbislgl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3rcjwxygt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3azqqcfzi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qgrhmbrh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3tromrahm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3hrpbraux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jctopabc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ihbynrvp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ygcvjpfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhjphiqb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3smimjycl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3kdpehlhh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3bxiwoxwr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3mdwlhbth.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3qwbeonrt.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3nzpkprhn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3iyodjrqg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3biykvanl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3xdfhwdhj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3qqybcsmp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3uaarrnkm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3opiqksci.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3xogbwnzl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3isfisdhz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3cfzmvqoh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3wsamiexw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3fvuqwbxk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3znafwzks.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3qjjlaxvc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3icjjbfft.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dxipeylg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3lxdhmjcc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xtxooxuv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3jnwdlunx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3iruekfyh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pzvxsblq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ekoclrgk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3kkbpwyxj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3pyesrfno.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zqdlrwsf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ondmzibx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3blkohxuo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dnjxfzmw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pttisizl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ngechuaj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jhpvazis.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3azibrcob.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3unvgbvfw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hfdhuonh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vpqvwjdz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xyjgldkj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ydznbfmm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jcumpmro.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ysgueama.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzfrkgkh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3wsmhmqhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azqucbfk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rjqvmxmu.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lishxlgu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3uyzieejn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zzswfuxf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3qhocfriv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xwjmqwly.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3futvvaks.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3rrjaecbh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vstrvzdm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ualurlbf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ffqdpowe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3eutezmus.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wegirxtz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zukkhmsh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yhtzpqaw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3eeqwhyio.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3sudpzsoy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hwjeswed.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3jwaozsjs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3rjxzypho.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wybfvoxq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hentwxqc.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fuxvjxdg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gtikekoa.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wyfzvenh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fpthbvyr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ftfibrjc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3kgfynlze.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3pwzeatos.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kyvesiig.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nevfoepr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rklrtaeh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3bhbmxgyi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3eglsbexq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3sagieobj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3yahjilhs.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3szwnifwr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3vrrmhcuw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qqcsbfxs.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aeddpavo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mdehpgav.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ttkrpjoh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xbuzwatr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3modmffnj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zagwaknw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lnsmguvr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gixtubpt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3takxruof.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wtbrmasj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3obfpssjf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qnrsskvs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wvuujcqa.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ycbmudol.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mtdqtaye.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwjvgdva.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3zkrpcioz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3hirpcuak.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3fbieyxoj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3phsmezog.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3xjyhyktm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3rucatywv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3nhuvtzkx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tkqubbiz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3jykcddaf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3grehkysl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3odsbcdjp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3savhhrup.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3mekhznjp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3suiwaicz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3niwrmkbv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ohailmzv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3deaqhlcq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dxkegkrk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3blhacgem.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvfwtbeg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vtuexujw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gsdrkpda.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3igqhqdwf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ilepiyma.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3evwemsgr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3euqrmebk.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3bjgvrlmd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3hbatpphw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3cpplpzrd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bsknyhuu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3admtidto.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ykebbsui.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3hcgseuuu.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3xejmtvvj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3icvqlhuz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3yqvjldso.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3fawcdozi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bguknexa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hnwcuufw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rwwfzogo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ngdndnyr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3mchaxmro.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ukabquqy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pglgubsx.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3rhaebpdj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3tkhyqzrn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3tlfjzqmz.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3xbbaofrc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3tnzwduns.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3tjuytujw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ufxbuiht.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vgqvjwwl.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3dnwzkhqp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3leysvbdy.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3etaowqof.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yithpuoh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jbyazqlu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jzqxjjpw.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gootjobb.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3susekxqf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jizbsuyl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rjrjlsvm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3mfechxni.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3uesvaqsz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pkkotjjh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3prsokbjb.html


<!-- 参考信息 -->