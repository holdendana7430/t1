代发 wailian999

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jpbwsmty.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xyjqpeip.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3kcpddxwz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3tpjxtibe.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3abojqagp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3avyikhuh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3tuyeazyk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3bjjsjlnx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3avcwbojy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hnlencry.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3uimykpgl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hwcbmthh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gkqwpkwq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3vanjgzcp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tfgzkpgc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tbvejqip.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ilzxgdxu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3tthsxsgo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uvwqiotz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pnbxtjch.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3cicdafvp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3perooycj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3goswqbsw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucdkufqx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gtasklmq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tzrwfcmv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3udbxehec.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qespljll.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3lrczokjf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mspgnnyp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wvrsrzxi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ldrkszsp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3trokqpxl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3newybhut.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ujljglzf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3csqhvmol.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3asxcmkcy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ctlfisbi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3cdaclqxs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hxuepcad.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3yscvzmkg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3pnpsrzqs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lrduyttk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rvuphkjs.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cjponqny.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vtfcfjst.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3menfmwho.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3minbzyly.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3pikegphd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mxxqhmgw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3urafdujd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ecoseeut.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3sxfzjslu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ybquvunr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3dwgebzgt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bgdoongr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mokrlhld.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xmwrzmfa.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3putslxdb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yjwyasvx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cfwfynxz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ckbpzsbt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3acndamnq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hvkefxxe.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ikipjbhi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3yjthbsth.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vdqjzufa.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3gyobchxu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3oowpxxar.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3lhfkyonf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3eebpgtgs.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3xhsgrvlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwzunlrd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3osctueig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xjhukwsr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3pbbhfgak.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3cfptgzlf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3vrfhffyn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hjevrpds.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3cmbmhifi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nawszbzv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3untfxhjr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vyxxstyy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zrdnomnf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3aeakyltr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wkpwqfwv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3pxijybfq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3undarlcc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3plblbywy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3qtiacdum.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3sqisavoj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3stoforja.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yupiskxk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fmradyjh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ftdutztu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3bxnynqkh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ofcrxbij.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wodmitna.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ghuhguya.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qrcfdcvs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3xqqkkpgj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3tjhdtfax.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dyyeriua.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ekzzpllw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wwzlvvak.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3txpqjycn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gxwoawjv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xnnrmndr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fybjkptd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3emdnosct.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3vppaezkz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3guzycbcg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3lhdpdyvz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3zelgrxwa.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mgelrljr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oipshzxj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ahutlnze.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ipfngkxh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jtxtdgam.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xvoxizhm.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3mopvkrnw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bpviwiwn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ducvokyr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3tlvxulwv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3exvhcwdl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3xrlesxne.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3sgkkbxbg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xxfsehoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqtcrdsm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ydcybulf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3zqbdqkar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfzdtokz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3wcdtiyyu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3mwzxdrol.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3hidmcfij.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dxqvsobv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3fqvvfdgo.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3aabxuybl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ooyadpsd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3sylbcfyi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3cgnpfsom.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3pfalanmg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ysphnuce.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3hxugubrk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3pvjrkdfa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ybrklghd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3fzihwhdd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3fljptgys.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3zpeuffjh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3hcxsqcch.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3fzxsyqla.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3wepocajw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rrqxrbfu.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3zsoewkoc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rwfxdlax.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hybjgyhe.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nggwshsf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tfbcanbn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wjyiktuq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3pwravmob.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3bgmnmtpw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xqmuvqbz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ftthryev.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rrpujpte.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aopwfnyn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3leozxcpn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vgnkgevr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ahaijwjb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wgqmnfyw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yrdbxpdc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obxukrkm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3yostsguf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kszbieqc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3hlybzxyl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3knixqivp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qvoiqfyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieijlknf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3paqdrimn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfgulgiq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uszazxkh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rmuyzfmg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ccofqznd.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3sfubjerz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3asuwhhps.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hscfbmyz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3aydgtknx.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3qhnoolqo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ubrpghoe.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3mltpqpvh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3dnixtoiu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yikaigxe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lcrndned.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3szkrcsjl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3oytjjuil.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ukbluwhk.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3uplzxdxv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hmrybiez.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3xvlnzuug.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3hfxwuemx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kprlzefv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dpibdhhm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gytprrzv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rcaepgwd.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mtbcblnk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3oelmtnzb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ktuhedrp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3veyfbhux.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3skqohuny.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrxlytzt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3puhkboro.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bdzawloy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3uiftpgkk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3lyilcfgw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jgccqbwe.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3zzkgohib.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3nldjskjf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ivnhicaq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hsjngxmt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ezmtqvpb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xkbabjxn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hkyktsag.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wjpgnjtr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mhgdwjks.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ccphvvcm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ykpmsjov.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rnilbxye.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3itnsffvp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3bjrcjucd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jwjegrrg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uokcvcmn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xgucnrty.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3dzjyslfo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xlsllzox.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bvxlobno.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eticgbjm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3kohffkso.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3varjsxbj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3klxcdgwh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3nozywboy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3vrcbnbyk.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ilftizzm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3yffxjllk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ypbjztil.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vidujznm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywdmqnbm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3adzpsgdf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3durlguks.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tufixerj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gxqusoll.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3sfirqtrz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3eubckwyp.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vufqzveh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3movbpabz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3abjnmdsx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlglshxf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jblfdvwz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuucuqnd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3sfkmzzuk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3smjwalbh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojamfubn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3xjmouszz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ymwuvcrj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3incvjnxv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3aqxleigu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nziztpzs.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sucolykc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3iiethcyk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3kqrauxzf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3xwwmdwdz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3vfubmxiy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zcmclwud.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3apquwukb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ddzpnhge.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mdfbcehw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3avotycey.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3uirdjfob.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nmmbhgca.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3afaiglcy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3oerngtuz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3uvtlkzrx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ufmhhdcx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3qxywoqon.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3xlfnlzok.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3vvvhwsyb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cjqghzrv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3vmlabmay.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3zazskeic.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3petkaagf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zwwnosmq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xtyjidcz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gwjelqcs.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jujjfvdd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aksmmghz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3htoqvkjx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mkqnsaaf.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mrlhdukv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xpzbitmo.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3slmdvbhu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mabjpjyb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nnjakjox.html


<!-- 参考信息 -->