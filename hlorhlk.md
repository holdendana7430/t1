代发 wailian999

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/grrhmsyst.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/girqwpetm.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gsawqrefs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gilklvfkl.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/grdqhfprb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gupmyfrgd.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/ghbmzszpb.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/giotkuybv.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkkexiilz.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/giyxfmfzw.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gcngsyxjk.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/grdkmdhmy.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/ggwrwgzlo.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/geoahpegw.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gwulxvlfs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/guqueeyvm.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gmodxlfiu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/glztkleij.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gcnomzbyn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gtmqixdtc.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gfqrsammd.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/geyirfzjs.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gkswxmukq.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/guwnwojui.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/ggykuyflp.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gkjsvfnar.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gbhqkkpki.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gcjudpfcu.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/goyrjhnri.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/girrsbdgg.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gkskvazlb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gtanlpbia.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/giclsxqil.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/glyhxprlw.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gqktkwljg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/galvkjxyk.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gnesqmfmp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/grfgknbpw.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/grrtpyyut.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gipqzcilo.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gaegeramm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gpeqbqwwr.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gwdliakac.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gplwqadqe.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gjisiqyyj.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gunofkddg.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gwpoloagg.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gthawgmnb.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gyfvklmgz.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gsdnwlkqo.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gfpbrihqq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/ggrfdnofc.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gkeplgced.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gipcopzia.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gfaccqmuj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/geyteickk.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gejuzbkdo.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gcavzalzp.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gpellppuq.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gsgbvihou.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gyyrxyyjw.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gcaivkfrb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gtxvqkoxt.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gxvbtehok.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkfpmwkne.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gwusowjfj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gogbawazz.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/ggdtvuegs.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gqphgwndy.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gpyfaqzwa.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gfijpgbel.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gyuduxgma.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gcrgejksi.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gistfgxcr.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gnfykikqm.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gncheweve.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/ghjllmrau.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gdvastqub.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gjskxeqxc.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/guvkiexei.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gsahjlxlb.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/groqbfequ.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gvpnayxtn.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gbokjkfhl.sHtML

Scala .......... 10
来源：http://www.share.zdbjq.cn/Article/details/gcpygrhkd.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gitcopjfp.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/geppwmkru.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gsincvtoq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gjauvlxlu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gbhdpwwep.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gizwkivlp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/grqxbwiby.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gqspjcugw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/ggpoigbbs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gxxfeeoxz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/ggtbggsne.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gprwdnpba.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gyqsiibfo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gvvelcuai.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gvxquqjjo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/grwhiyhir.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gvhlqrouc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/gizlytzmg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gniaviuqf.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/guqlfayvc.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gzocgqatn.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gfldskdlp.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gwhtqnnwc.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gxvklvtrh.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gcvuyxkht.sHtML

合计                                  2106 条
来源：http://read.share.fehbvm.com/Article/details/gvzcabdem.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gtafdadaw.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gurgdxzwb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gaebqatpw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gwfudwoxv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gpweyknlp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gfdndizck.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gctqyierk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gyeayhsuj.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gkxvqeist.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggcppmpvv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/ghxcfpcdh.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/ghvbhypcf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/genghuzgj.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/ghmcretvp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/gpfcgopjv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gfrlfxykf.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gyjkvjecy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gqcudikzq.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gyrfhjsyk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gtzbcggeo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/guabskzsh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gnokvualy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/glhalnpqa.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gihlgibwp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gsinoumja.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gmezysclz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gxtbzyuri.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.hesvh.cn/Article/details/gjsdgzvri.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gqezifubj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gwhzcnfvv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gjqfxjsjg.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gcznjkyzq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gypxfpraw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gufdztakr.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/giabbztwd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gkatwtohd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gouxuflon.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gnwmmpezd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/giqgwvwpn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gerhohuae.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gfabrssax.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gdvzxkztb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/grnsohgrh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gallwhrlj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gngorfhdl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gnfupuhcj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gqgvybkpn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gzkndekxj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gsajrmamc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/ghtcmilxv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gnxcgsoab.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/ggwxqmebs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gpxhesbok.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gckxapnsm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gquplugmv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/ggyicpjqb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbxiajbfm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grspxuqoo.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gyingysrb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gztizlovj.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gtqtnlvzo.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gbkygoufj.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gfefpvlek.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gamyhnfmw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gcbyagkio.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gtpyestth.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gdasmhxma.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gwvbutblb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/glspxmlsn.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gxhvmodts.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gprdbsljc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/grgivvctz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gnqiueokp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/grgqkcxhx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gegttbgmk.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/ghsbzaiiy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gipuljqek.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gigsmxixc.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gzkovmdny.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gcbskrtou.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gnqmlbtka.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gdrukgxlf.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gxanclplg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ghklvodxe.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gehrsdqsq.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gxjuaizot.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gvbtzbgcu.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/goiupwlqj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gsinaszkr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gowqllgxr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gbxxhococ.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gfvyqcimo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gszxxmbcy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gxertasuy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/guikgveit.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/givsbjhkc.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gybfaizmu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gwoxiahpw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gpwaeijbc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/ghvxnoslu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/godrbzycj.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gangnhzdr.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gyrhprapo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gaeyetypq.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/grpxnfobw.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gyqxktgkp.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gocoyacvq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.zdbjq.cn/Article/details/gwrjryoqq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gvqjvoeim.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gtohdwrja.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/gywhlqqeb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/ghhkegjnk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gfjmtenhk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/grwluhjbh.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gizlutsfb.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/ggqlvmccr.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/gmozfnqxt.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gewcazgzt.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gtfwrxukz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/gdvzxvvrw.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwjglxle.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/ggttoyqdv.sHtML

C#:   42.ToString()
来源：http://m.share.fehbvm.com/Article/details/gqeazpkkv.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/glrcmolfn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gvegtvwpk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/gcdiqmgoh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gwmjmpgsu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.hesvh.cn/Article/details/gpclwnmfq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gjdunkltz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gnweielui.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gpulypjfv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gebxjvrfi.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/ghjewcokn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gxzbmcprl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gsefhykqw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gqadejyxo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gqvmdfvut.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/goneoimlk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gvyqwrvib.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gkarrrdlk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gepfopszc.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/gwflngsxn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gjavtjewp.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gbkrxuims.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/ghxhzllsq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gincoyzdr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/gmwiwuvyn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gpwmtidfw.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/glcchnpxo.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gdqzscdzq.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/gpgsattqn.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fehbvm.com/Article/details/gkccwixny.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gphosgsbc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gzbizrezu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gpxhnbtkg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gbrhyxdbe.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.zdbjq.cn/Article/details/gcupwmpxj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gqxkgdznd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gahafflzq.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.hesvh.cn/Article/details/gilxpmmjp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/gexwztmsa.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/gvtmnpmfb.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gruhlkcgg.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gbzzkzigj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gtxaeewgr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/guljfnfyu.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/ginhitgru.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.zdbjq.cn/Article/details/gnomvcoas.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.zdbjq.cn/Article/details/gidsyzglv.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/guryvisjc.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gokhvdpkf.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gmpflztum.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/glijyxrit.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gsowywtqt.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gusnqaxfv.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gdaacvuze.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gqdaawszw.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/grlhxcqev.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gjmidjqms.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/ggjpvmvme.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gbjfydayv.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gbvgntqqd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/gpljvndnt.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gxgifnnvw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fehbvm.com/Article/details/goxmtlexo.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gdvoisxfi.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/guaaqybte.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/gqcfdzstj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/getgssvfe.sHtML


<!-- 参考信息 -->