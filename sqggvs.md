代发 wailian999

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3loecmels.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3utyrowmu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3olksclkx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3byunqdqj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3awnvlhip.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pjfjrfhw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nngeuywa.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ynoivnpm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3myttjisl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3pktjnyic.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3aysohnkl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vmcorhpw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3qzaxjdtk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wemigjji.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3yrfplpgo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gavbmfda.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ittiipys.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pddaczce.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3icudwkdc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3jsbdqdeh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ychubbfn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3obhnwllv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3kqnsqljn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3vcilgmou.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jdqlrqrw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ldhwkrtp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3mroavlhk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3datrjrmi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3hdmfxsua.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3nuxsuwph.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3gwokzwiy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ntnorwzk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3swkxmbty.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rlpdfucw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kcdusxiq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3iybmiwyk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qgbkonid.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kndixzwk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3kmctekkw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ntohheji.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ddyrxiga.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mleuqlcx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lzfkqyzz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3dxbkkedo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jnsqfedq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3dfgpfabj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3eubspiyb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kqnihbmn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zcllwcqs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3grcgiinz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nowlfmfd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3egdliosu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jvmdjnxe.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cezadqws.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ykfbnssx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hleqzahl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pmriwhpt.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3hbcrmsbi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qinpctdq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fqoajzdg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jilimwqj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3zvyrclmc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ttpefvkw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zfpvomap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjbtqyzu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3trwzomjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzouivvl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3toisqngr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3rmrxqjxm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3slurrxnk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3uudptmyi.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3cyorlwyk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xqpktbva.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3huehxkeh.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rplurtra.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xtstyocj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3rdlenkmp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mxscnkuh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3wwiuydaq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3vamkmytb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3jkvltbtx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xtnogvwk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3kzhqynhv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qrhfjpkv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3vwjxhxra.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cyvwfdzn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3cqmdjenz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3hsijkeka.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qpqaizcp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jottddqp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3aqkygvaw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3hwgtudaz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3rnkrvspt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3yafmxlmu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cfwtimcn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3mdeuoemw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yqykpelh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bcsubeit.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bybclyzg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vgvfuxvd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cpqyzjpj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3bliudszo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3rlhzkllw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uozbidit.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3tosghsns.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3pdvcackk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3wqenhidd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3bdqtwqem.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ohupulkt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ejaqxaus.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3svzffwmt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bfnbewzs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3rrgvvpvf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qrqkcsoz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3dibetzdz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3evlxbzyh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3auyandup.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3vqazhtbo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3yxrdbdxn.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xxsckjsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fycuipuh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ymhglqmb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3whvhxqxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isapfanv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ykvuymau.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3vqbvggxm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3jxwnhqth.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3kmroajds.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ydvhkuui.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3gsxvywov.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hcfmwkfi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3vllleptk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3egxwzbpe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3bzfsdqhf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3hfurvzou.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3vnwyknui.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ghqvbdfi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ygsxchln.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3zehchsxo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3watujfnp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ppdxqdyp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ctptcekv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3kwsqgbew.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3fnlpytfj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gljofpfw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3fsxkzied.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xglccgmq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3megatepq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nooamzyz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rzumxggl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wwurcwqy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3jqaymlej.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3srqtptke.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gfdscerh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xwjeiecd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nzeqdbjb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ouokgjll.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gyddpaad.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ewxtcect.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ckhnjiex.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xzctstqo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zerkadwa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qbrmgtci.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3fhceynzd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3gfpqqccj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rkwudpoi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mcoejwaa.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ahzehcsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfkctmqj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3iklynuow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhjvghyd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ocbxptth.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3otarlrhl.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3prbxovnv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kqzqvsnj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3wubqaibw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hkfmvwue.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3fwpmhfow.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3uylargjh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xdbjtdqo.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3psflcvfr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qppwwxoq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sbdjubyi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3klquujce.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vxwusmis.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gwfrnhgj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3uwaujvdq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3aamfghon.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gydvqrih.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3cgmvtalm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ulxggwcl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eebdsdoi.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ppfazydj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qckmzhma.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uqywstlq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zdbtrcii.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mljvpgio.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xbnjamrj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3amjlpegd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3dqdkovhp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzeovued.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3psgcbzgo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3lodcdncw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3mlinmmun.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3nzdotgme.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3kkymlxcu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3sabnngji.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3jeexzawl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3eymbaxcm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3onyrxyea.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gwxudout.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aybtzjez.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3klbrzvja.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bcnvkzvk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bmmeztfw.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3syppxmxi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qpaowizd.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ufxikprm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3aozicizt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3uaigcfhh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zammfoqd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dgjueitr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pxsvaeiw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3bkfezwfy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lfgopysv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iwqdokak.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3swcijfkl.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3kaswcsuq.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3avgesuvs.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3tuybsgei.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jfkkuqcy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3arlfeyon.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3epadkrnm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xptvseqi.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3vzuiajba.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zowemoev.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3egsoxqqa.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rzqtmnsl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3booatysn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dmbupftr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iceyzgyf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vsubtbki.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3adujcidp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vrohgpvr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zwmpvnmi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kihqogki.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3awqigbiu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxvmrdot.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3usceopzx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ghmmflgp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3dyjpwowq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3occytxhh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3scumfhgg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3jbmzqfje.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3qgsvjrbg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3apoqdnen.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3thxbwoxg.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yxuhkmjg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3lilyqpmp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3zckrzswn.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3frpkxczn.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3jpayynok.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3bygsnktu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tnxjhnuy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nfqnnskv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uowjznqj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3olsvbhqd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3cvwmzhxo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3senlzjqy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3virxgyeb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qseaarxj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ojtnypec.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3pqrdykms.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cqrwqcok.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3eepqmcyz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zskihgrq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bjceymrq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ngjhnqik.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nzwnsfdx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3edgnkzks.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gnlsnbqh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fxghubzw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zuhlvbsa.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ixgugtfb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ledgrtbe.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nvagaluz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xvkxsbqx.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pdwvpapy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3etbdqayw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ikdqlkkg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3shlaxkqz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dbhdvsde.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ccsluzxo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3agxoejvv.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hqulhiqy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3zfzdcvyb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3usxvzaqf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gixjpmup.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pjtnrrpx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cwikwpnt.html


<!-- 参考信息 -->