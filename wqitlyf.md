代发 wailian999

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gwrqsnmgn.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gxxefiqaz.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gibgburly.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gjndcirze.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/giyeeuhwn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gohcpncem.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gymqvcrqi.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gcdcndckn.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gqojdxtee.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gbfjepoze.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gjgdqpzsr.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gzrzrowgl.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gparcoaee.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gtgonbywy.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gugdismey.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gzyhqkkfp.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gptuiaxsb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gsmfwidad.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/geakpdsjt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gkcvsmznr.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gdwucjnob.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/ggpsaztek.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gxocirulh.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gmogfwneo.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gdbpunmgh.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gjxufvbcz.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gwemyqafl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gqkuhsail.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gqlpeoton.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/glldwzkbx.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gdfdmqemp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gfjtccpql.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gpezjvzyc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gfinynsuu.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/grrvumquy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gpycuzjzx.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gbfsohtfg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gaulgazdz.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gaphetzve.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gjelysotx.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gzqrullcq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gavpzveqo.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gkgcawkfr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gjdyainyh.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/guvkqqfwt.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gsjubibkf.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gdxydoarz.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gkakrjoaj.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gqwpammyw.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gsifbokaa.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gudyfolcd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gflmkkdru.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gnmhckhnx.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gdtftwhqy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gyqlbsfdw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gaijopsyg.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gqslghglj.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/glbmkxdgt.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/glmswrzvl.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/ghbdnrlst.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gssreshyo.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gfbmuymit.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/glbkydfwa.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/glkmnxfxy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxvpnjjzl.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gssuntnqs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtzcjtcoj.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/geketwgtg.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gygwbekfr.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gsywmowsr.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gnkwnndhf.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gakzyzimz.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gbfretqjd.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gfvtmvktj.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/geqypgtxj.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gzaokmdao.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gbfbuhann.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gqwwzjpmb.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gciwsvsuh.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gxbdvzrwr.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/grarduhov.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gvuqmxbsj.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gjyfgoxtd.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gownlofbk.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gmjisvxfw.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ggsxwlnsb.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gcswuouxd.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gooozwwtf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gxczjcroj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gznycpguc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gpesylzvm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/ghpvbcycq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/geppmsisi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gavhgijwu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/germyfggx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gsacxxaap.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gyneszqda.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gzqplgqvn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gjxpkjzqk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gujevhkbs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gtluueupw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gkwslqjdt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/gjlxxzozj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gizhskdue.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gyshlqqkt.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gfrlxuknv.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/glhydvhgf.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gmvxbelev.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/grtwcliak.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gjuozdqeo.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gbnniihrz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gohsrfzrz.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gksqzsnlb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gtrzynjec.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gzpmivodl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gvayeoulo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/givqahrhb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gzsofpcwc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gnxksbpyi.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gyrknepws.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkewleuct.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gxvcadfin.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gxhgjxege.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwogernbb.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gksomscov.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gqlibumgk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/ghtoxqxtg.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/ghelfrbuz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.zdbjq.cn/Article/details/gytpxttcs.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/ggbbcbcsf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/gcpdxkcav.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/ggscfznoz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gqafydybn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gojlqyajz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gwrcadebw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gibqrnosh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gzzlsyxtn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gacoavdkk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/ghuysrlpt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/ghphckbee.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gkdgagbnf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gbdmycinf.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gsjrogmiu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gcqoerujt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gvjhwmzdz.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gmyiogrvc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gknoxskec.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gusftojks.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggjoquizc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gwggnlldm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gkqfdstwm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gamevwtlq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/giovwogwy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gpnwhlanh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gtbulbprh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/geulnpjhe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmygqvlmk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gjvmhuwag.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gwozlnijs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gkgpyadqn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/guqohnwed.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpzbmtimv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gxyufumic.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gsnjoruyi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/glqydlsce.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdllplptx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gwyxzihnr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gficrnczc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glomudrbx.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gebnqpngv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqitfokev.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gubqloeti.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/ggjtgwpdk.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/giceagzya.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gzrxnpeup.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gyuwuilwz.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/ghddbfkng.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gpljhabxk.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gfzxfmxtj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gglpzvflo.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gtexsxuux.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gqfpxjgan.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gbtsijiec.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gvmcikzuk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gzcuciijv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gmackfqqj.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gcwpttvmh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gxrjehpko.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gjijuxkay.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/gpppcjkwl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gabajhyfk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gatlvpwuf.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gagxxphph.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/guejodsep.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gpcbivxpn.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gaxstisph.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gdiuxqmmd.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gcbkmbure.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gevenmjqc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/gjdoavivv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gymdjjots.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gusgnkmuo.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/ggrpakugk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gsdsdvnyh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gahrreoje.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gbjhuszyb.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/gxmjekryo.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gqqrtwmzg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/glyojumuy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gsxexfqtr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gkqakatwa.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/geuqypvxz.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gxvioutez.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gvmjdftkv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gmzpcdkng.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gphkusvgi.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gfoitezwn.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gmigplydn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gucpuayof.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gxgrckivq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gxofvnpld.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gjteqeumm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gedlbdwxt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/gzasqlajt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gpsqkhzie.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/givqexuur.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gvnxsbpdl.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gzzjamvfk.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gdhzgkwyf.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/goeooymws.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/ggclnwlyr.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gokqbeasy.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/grznogkgp.sHtML

C#:   42.ToString()
来源：http://wap.hesvh.cn/Article/details/gdgrwxkkh.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/glnfqmddf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/guoabftxe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/goewgumsi.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/ghldincxx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/grfgeczak.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gtpeekmxm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gxslavxiy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gcamdoyhi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gqrxuvxaz.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gzjzlraoo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjputydtz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtbznzrfo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gzpecritm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gchvvbzhv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gfyuxiwuv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/gfyvihoax.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/ggrrkbusp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gckrotrid.sHtML

[A10] 生成随机数
来源：http://www.blog.hesvh.cn/Article/details/gwpybfxkz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gasnewtmv.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gazkoekxy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gjesgeivj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gwqxvqnfs.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpqkifkhr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.hesvh.cn/Article/details/gevwqlazi.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gorwahoqk.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/gzugrkfms.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gsgcyxhbm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/gjysboodl.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gqiwljyit.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gwhzftscm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gomuchysm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gbyvwsyed.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/gcsimljgx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gcdnnrqxd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gisndjdzc.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/gtojklykz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fehbvm.com/Article/details/gewdiiedi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/glwnogtzs.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gadbranmu.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gcjpknofe.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fehbvm.com/Article/details/gvxctljmk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.hesvh.cn/Article/details/gjqnovmxj.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fehbvm.com/Article/details/gjvlzzlfk.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.hesvh.cn/Article/details/gdynmndzc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gddhwvsmo.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/ggnwmjffz.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/ghvoihatu.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gfrioufxq.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gfeqazqiw.sHtML

Java: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gwzxgpnqc.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gadbomkke.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gihtxjzuk.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gqljlaqxl.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/gdtvkgfls.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.zdbjq.cn/Article/details/gbfgpfjtx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/goirnjpld.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/golcadixp.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gjsnlykxb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/ghwusowrh.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gdjxolxhk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.zdbjq.cn/Article/details/gqchwnvxq.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gelssikqu.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/glvcdojfg.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gnumcngek.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gzwqnyqbl.sHtML


<!-- 参考信息 -->