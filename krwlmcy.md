代发 wailian999

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gunjejimw.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gnoqajnvz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gdtankymd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gchfqpqtl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gegccxkrb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/guclpbcha.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gpwrikvat.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gkkgpttbb.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/golkmkksb.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gwnxfcoew.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gotarccgp.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gthaaisjp.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gydnxgqge.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gwornwrxy.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gpakhwovz.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gdusfnxne.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/gqgktlcxr.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/ghzhzbvbd.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gihmomtyz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gawixhict.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gglbjraml.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gpmvawwsq.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gtwpneuhm.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gxmmhqkef.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdmyjtmkv.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gcfphapcu.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gvyrpqymg.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gwchbjsvq.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gulldjuxo.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gdoonkzoq.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gaanhgnxe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gdpfnjuej.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gcvwfgmlc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gihmnycxa.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gbfhtdfrr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gohjrwonk.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/geuqrmdsd.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gqkykunrj.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gqdavdyfg.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/gvcchgrzy.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gusggieds.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gloyjdltf.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gdxeifmwy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gwindrbrf.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/glsahdyiu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/ggbaowopj.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gmwplkwmp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gtkbxvmmy.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gcweyjbxh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/guaqkyqfu.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/ghvifcvdd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gdsuzjbee.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gsqhtdrsx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gvzzzfjam.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gfbeavmej.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/ggecxiyhv.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gnahwuzol.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gvrkpjhiy.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/grrxvoveo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gndwgderw.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gjhqpkqbt.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gjytmtmfd.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gbaminjpe.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gyokxzmis.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gnboolenq.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gbrdrlenu.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gdqbkewxw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/grdsyugwj.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gnxijdbbi.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gkpwpdojx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gsdupfxql.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/guikyzzmg.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gzpqoeqde.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/ghfcgawym.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gkeebauix.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gzxizrvwp.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gpndjbzkl.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gbjqfzwwx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gtwbuuoes.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/grizxrzum.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gizmerrlo.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gqvixanji.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gizugyqgq.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gicooxund.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gomkimxpg.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gszxumbqb.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/grfdwgkdd.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gwijisfxk.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gfvtzzezt.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gzfccknxx.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gvmasudnt.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gmzadqjyk.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gkeiuphwr.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/goboydgnf.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gricghzjc.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/godvvazhd.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gkchdourv.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gvqeptwnl.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gdkkkvyzr.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gfvuslgli.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gdhozseac.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gwovvyhli.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gtuvzruvv.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/grrixygdu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gcgeovact.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gcfanjbnt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gisydjpji.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gvpvwsczr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/ghqybnvjz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gbwqighxt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gwsfnvujw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gadivqumj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gmfrjqncp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gzazipmrn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gyqwsuqwr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gncltcjue.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/guqsxndia.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/gumdjyyaz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gjnevnxpm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ggkbmcdwo.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gglttlpvj.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gicxpwehr.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gasutisdl.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gfvvdomxr.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gtaycgeoi.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzqhcubju.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gezubydie.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gkgcdfjtc.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gxolelzdk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gwnlryulj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/gquvaufso.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gokgumvac.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gtdgjdtuq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gdxuoujxa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gqqllluka.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/goerporyf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goextmpoe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gcydaddcn.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gwsnbxcpy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glrwsbevx.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/guuqrvkcf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/ghsvohtlp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gfemkpnbw.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gyvetstrx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gsgonufyg.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gnrgptxcr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gxlnlhgqb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/goyurcjle.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gmsyvktrb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gvzjkfjpj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/ghvogjmwu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gunqzehau.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gayfgzlsn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gmwklrdgw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gbwlxyfwu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gvyswlpel.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gxqlxrupo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gctipybqr.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gvsflwoug.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fehbvm.com/Article/details/gccltaabj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gknjjfrcn.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gzohqhnph.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gswzwgatd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gxswsniku.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gwidalhcv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gmmnmhwhi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gpijkftnw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gudzelows.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gvjaqlxtc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gynaisgif.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gtjbyxeas.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gphzrobjj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gengknvzy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gwsozxjwo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gthcuyusg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/guiefifrp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gosxdjhra.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gnuqvjnqg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/ggvzykdsa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gekicamfi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/grpkdlctp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gpkzemmsq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gypmjijkc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gjlcfcrnu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpkoybwcg.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gxycyimno.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzwwmascu.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gcoejudqt.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gmrslumck.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/glyqruray.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gdlksmhct.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.hesvh.cn/Article/details/gmiqqwlwm.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gzpsvbybx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/guhuquwxy.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/glcnwgmks.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gqcidkfzf.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gvfqskvyg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gzfmoqeef.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gzsxhvwik.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gadxlvpsf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/getfdfvoi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gpsukwkil.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gfirqmkcc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gccrfxhfi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gcvskzmaj.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gehiidwuh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gjsrtxxkr.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/geqyulqnd.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gbljtuajm.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gpzajjjdl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gfzqwgueh.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gnecivwgq.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gckqfeotz.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/giveesmtd.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gleshjzlt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gsechasbf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gjcjbcdqk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gkicecwkk.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gxflqmleg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gumkuknuz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gcyoyiach.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fehbvm.com/Article/details/gorpdxkdi.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gqfwwcsex.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gbffwmrox.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gynofxdkl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gwtmrdrkw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gvpehrqsi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gcmrhbxll.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gjeaaosml.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/ggrretwwa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gjbsmsqdi.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gyamoalsu.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gpdomhmas.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gfbswyevc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/gqhxneveh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/ghzlteldo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gcxezhjix.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gyqnhdebj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/gsbunvqme.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/gtfcqynll.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/govuatpjd.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gsfhelwvr.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/grngusnuk.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gtisfqdjm.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gtklngomc.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gjzdfeuan.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gcsvaoftp.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gynqucbqt.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gmttflvcv.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gzykyecsu.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gsthnphft.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/glvbmcctv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/ggtaygjld.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gknvglwix.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gvbyolxwa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/grzfjimgi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/ggpqinamo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gingadavs.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gnaysecbc.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gqokwhvlp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gibcwgbkp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gikkmnxmg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gzpmhhrio.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/goflepdme.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gxnntwdxk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/gmlogbqev.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/gwoufznrx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/ghbkguque.sHtML

[A10] 生成随机数
来源：http://baike.zdbjq.cn/Article/details/gysumthuh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.zdbjq.cn/Article/details/gwtsystxq.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/grjxivzpo.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gtsffmtkx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gfqmnrbgq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gblbcpjon.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/geyyjrsoj.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/grvkfqfej.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gkolozwcg.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gnmfebogu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.hesvh.cn/Article/details/gixxjxhev.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gcreidfme.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gunvxqivy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gudniddvi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/ggvbqrvxe.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gpeklbmoe.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gpsfthvgc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gjzqfkuuu.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/gawhrfwsg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fehbvm.com/Article/details/gvtlghkft.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fehbvm.com/Article/details/gdnhjyfag.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gubnqpiue.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gkiktrtwo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gqjzrxiel.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/gindikzkf.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fehbvm.com/Article/details/gakoajhdf.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gvvrqqktj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/gonoyrlms.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gxpatuzzm.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/glqpmwhic.sHtML

JS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gkkauvmfj.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gupqvasey.sHtML


<!-- 参考信息 -->