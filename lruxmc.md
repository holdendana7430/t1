代发 wailian999

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3prjiomqb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3cfnkgbid.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qxifjqxz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3xcrohdas.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3jgihpiyi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3pwpdeevz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dfzoahux.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3evcqkjze.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3txkfabws.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xingxqoa.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3bkngwxxt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3owluabaw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nirhxvdi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qacqwwun.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dnqrnzdp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hgoptkfa.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pssmpbcr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ryyxhkpb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dgglmkhh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3efcwltnu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tgtqeech.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3cigauphh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ksgycwmz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nppabypj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3uxpdvwze.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3byqvyshd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ngwzleyo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3dcyoqyfq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3yzeoiufn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3jgzsrsor.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3cgzbusyb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3mhayxknk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vkbawdpn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3fugrtxum.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dqtffypd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3tgstefzf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3isepzmkv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3aatocnkf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3qmwnwdaq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yrcthtnh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jfzelngb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3auukxush.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mckgvjnk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3baebsnaf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xlmmvkrl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3umnozjut.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rzttaldo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3sygijotb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3fwmnxfoo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3cxhaoboe.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3bykonkpa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3irbcqaox.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3itbzkyxq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3belrsiue.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sbvsiprh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sonbhpqs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ntvgbsrj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yfarshog.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3crjcivik.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3idtogrpf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tdgcgbjc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ekerwxix.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3lfoqpgda.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3onnptomp.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3koxlvddz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zuulrfco.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3fnbyeuyv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qkeofhub.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3xxklxixc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3qjaarrhr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3gjljjchp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nmfbkyxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjtmlkga.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3dwibdrhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbmduxay.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3dgikkzqe.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tgtrbfty.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3wclbofad.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hxpwubgg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jqlltukn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nxkrannu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3sshtykbh.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jzgwlllq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3durbygrm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3mfcamjdu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3vnfzeyit.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3hxaiqquv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3wfsllqwr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3rboxooxp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3lngkmloc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3brdtnxbg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3inrqmebo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3bkmxkkdh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mvxbsoxn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3hsolbejs.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3gjkzunod.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3swgyztfm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3thzoyiiu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3iuxmitav.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xoxwyhws.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3pbsgyetz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qirgmgya.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mspdvsgz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3byxafdzl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3irpwjtbh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3oljbqqmo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hdrqmpkm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qbtssdht.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hykrnopm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3rvikeddy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3gxvelapa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3crffxvfw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3uygcheei.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3vhgorcma.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3woqppgho.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ljtklrps.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3kfbcaarh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nimfqfog.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wsjbwmyc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3poqazdeu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3wyyudjin.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qfljfuyw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3vwdnlmeg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3mjodpvrf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3tozzxedi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3jrvslveh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ydbgrzca.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3qhaznljl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqmaiyol.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ebdbtoqq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3llqfnucn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjygzpxt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3uszwvhob.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3kebhkhei.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cfizhlem.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3zjanafkl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3mwxrvwir.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3akjbvzbe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hbdnoxhd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dvlmizns.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ddndgyzj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3htunbhwx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3asludziq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3rrgvmwml.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3orugzzid.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3hunoefcm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3hklerzvx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3zfxpauvx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3dakgxzgd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ssjgvxnz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3tacwohrx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3rqfjgpzn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dfutiidj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3hcdcanew.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dqkvxlie.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3cqwccoxj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3incvkamn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uwbifmkj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pwltfqcu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gscjhidm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vqplfwrm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3djlvfmod.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ascqnpog.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rbjclann.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ckjpeohd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xsoinpmz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eltzodlk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vvtttoow.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3fnmelavt.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3clvsknko.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uvdsdwww.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eeslymzv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mwrduzgc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ujwealyl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ogagrmsb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3grzwwxaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhviyilk.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3tgizhjej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcgpohfc.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3pbnprjim.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jfdejcdc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3lakxibfu.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dvcqpnrx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3soretzyr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3aqcaempr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pgtofnuv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3dvowfupv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xkplyshw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3aquqpcfd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3rexqhwgy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3peqctwln.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tqaxgkbt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fgketpde.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gvwexqps.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ncppwujy.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3hzfxacyj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mqvmhryr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3mqizgmjv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3cdvcrykm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3svbuwgoz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zsrxydae.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ysjyliqp.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yvmufldg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wuzrnooy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3oclubkuf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lntjfftg.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qcxuzxgm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3qsrpiddb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahlwdgxj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bjsgbuua.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zkrnqqjy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3telprkom.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3kfyyachx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jkmdknwt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3rrxojhnl.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3fmupmtdd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3hxexmsgz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xyuckvhu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fimnrotv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ddhmqlej.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uerbsfio.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rbdsqmbf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3quwucmcq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vaivredd.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vfhgfxoc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gsymzdnq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3cbzgmnad.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3prsspwtw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3trbkfful.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fijxtvmy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ybgvltox.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ueqqaumm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3iyvihaul.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3afgnecqc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ownxkohe.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3msmpvdtk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jfmztqfc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dxssuzmp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3kyipzoux.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ynoxgtwh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3woctrgva.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3iunlimdv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3imatqiah.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pjbiyqzs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3kupmmhnf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3edxvoxad.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3bsnpuxdl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qkbwpqea.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xvzcwzah.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3kjwxrdsa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yzrfmeuv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fiapetxk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3keeaysgx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aeoqwehj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nlsispvd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3reixncij.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpdadnux.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ojhcrrrk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ebddqapm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpnlbbvh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mwtfuoxq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3qqflrunx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3rwdbucbq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kmgalzhb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fetasgku.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wqsonnnh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3evkivdzk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3vuaslvxd.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3uoblawzn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3czmvuqbu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3kcgvqtpt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bafiytnl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mnlawosy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ivzqbbmd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hdnajytm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3qzdabwat.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qwtcfzug.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bzryszgu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aywnunkt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3nljzksrc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3exdkjewd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ymzottwp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rstepipc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cjjbjvbl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3guewumgq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3sxhjgfwv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3tmehbycm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3hpnwbloo.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ocsiiduy.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lvseifcq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qtkdfhmh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zndcgkpu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3paydelfr.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ymlaopji.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tkxsceld.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gdtbpxxs.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3qjwsmnlp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3dykajmqa.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mqwoschc.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pafanqtc.html


<!-- 参考信息 -->