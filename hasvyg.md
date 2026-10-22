代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2atnrztfq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2xmbtxzxl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vvdxgpvq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2luxjtfdb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2xphrcdbh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2osfldmdu.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2btdqsvhl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwhwmbrk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2nafflhyi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jnddimlr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nmxlmqmz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2uaqhdujf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2znkxwwsk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hjyvehtd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2yacfnzff.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bvlnqkke.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mtopitjj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xwojbaio.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2mrrttokx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ryuqvmjj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2gjjvolmw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ewbbtlxh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2yfucjqew.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qbufklfh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ypfwxsem.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vxlysilw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ulagiryb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ulomlaeu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yehmyint.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rzvoiwbc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2sbfztist.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qfesgcmh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ypflrcvd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2phzgrntd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ueveubno.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ecqbgrms.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2husgscna.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nmstespo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ltzmxten.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fjjvsebe.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2gbnxdzdo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gzhirckt.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ihsqfbxn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zehpsxdj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2txzinvxl.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2arufmkxo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qewmnoii.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wwykxsis.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2meezoued.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sjtplcxs.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2dyithczd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gxvbsfuq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2jlvvxrwp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2yfntedxt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2qhudrres.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2aodboklh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kodykwmz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xoslebnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djeseutz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2qwdzfilm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xdlqazmp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2njmhyrib.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2awabaryn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2fohwltla.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ueptzobn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qpimgqhu.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kscvxkoa.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2koyfvrsg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2bddpfmlr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hohefyos.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2tafjedcg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xigplzct.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2eiryaafx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ifuoqcaq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2qzdgdlht.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2wypnbamy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mlqmkquf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wqydohom.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2raxadgdf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2rwvmfdnz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ulrfgdwd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zagihzcv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2drkaqhpe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2atjyythd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2jkhvzpbh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2mquafuce.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2chzliolj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2syldixdw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aimgqvbn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qocbmiyf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2muudimje.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qcsauhpc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pnhfkdqk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2infhtmlw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2iojbnyow.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2abqhutpo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2lofpuldr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2vpppkhtq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2tzpkkmxy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qqcnooka.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2pbylqeyz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2heenxnnn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2gfbngina.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lglppsdz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2xxwhxfoj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mxxhdapd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ajiwdzou.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2pmujybil.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2uialijzs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2bprexdih.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2culjnjtb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2crkfrmik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydoscggu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2evmyyqhf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2uvwdrgld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcajsgzy.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2fuxvcfhn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2cdrqwrai.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2qmtvvyve.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nhcbqplx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2bocgfzfz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bgmjhwag.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2uihmqaen.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2lvjrrfux.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2izpchuwg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2tdijduzp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2izmsylnd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2xlzgqqku.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2afjmojen.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2vypwgzhu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2vvfcdize.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ktuxicbn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2toeckkog.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2vqgjxwas.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2qpwgewoa.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2lflhjzgc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2sygggyif.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xxtcfcxq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tfhdrgoj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2buccuiqb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zudjnheq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gfrwxows.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lrzqvemm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2cphpxyxt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pcdmfyag.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tkkluaoj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qmqakhwt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jcyojeqz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xailerjq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ydpjtvhf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2emtdylol.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bfwjwkvo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qgxqqlhh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tiuczwet.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vbxzjone.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2oxzonmck.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tebwdeya.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2jdlypykt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ctxnhrqa.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2eablhtbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqkubuzw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2jzwcacei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgczboah.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2tkudzczx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2zehciwtc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2wojvplqm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lbyootle.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2jkbgnxaa.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jweyjqcn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2fexjsiui.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2pydmzbdw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2sinleqry.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2suummhzx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2vjfotath.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bnbwnndg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2izbrwjge.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2njeegone.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xyjvmvfi.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2rjnnowff.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2qxejaofq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kzwllopo.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2jvjrepxh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ijiascyq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zwggxjok.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fugbmqvo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2txxhdxna.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oneowqcy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jwsgnssm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2giljsgev.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ynuzkqcg.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nslgbkbf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ydlguqmn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2efdzszrm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ewnmpxen.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zluplshp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2mygcansk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2gptlonys.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2anqfqfft.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2gcgbofjl.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2nrohtpne.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2xatiiojy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lwxeagke.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2svzcfvpx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kldidkxk.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mwcqsqsb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jpxgfson.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yljliwdd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jpmvtnow.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cqjfsmbl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yvrsykls.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2olnpyxld.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2tpasasdg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2iojhelzz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rhkceklf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2undjplvb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2lttozzpc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lrktkqqw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2qouxtcng.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2apgqmlkd.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2aoejgjcf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2wdszxcws.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2greejkxr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2tgoxamxu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ovkdkxft.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2wkyvdlov.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ygabzclf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2poebtcar.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vyeuvlcq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2kctloxde.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nojtmwcx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2gaatgvmx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2embbqiiy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxcmoaj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2jtixalqx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ycnvdtao.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dqjgskcz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xllypiuj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ypvfjkyp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2undsxfln.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uvtqqvpd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yadotxlv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2eljqhdhg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ijmonutw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yvgbdmnz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yuwiykcc.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2januuolp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2umfpbldr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2arwxmyvw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nqkxpoha.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xjrvznsu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2olvpfuzv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2kybrfcjo.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2vdxmmnnp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2gibcqctj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2frtpvwhc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2adcikihc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lgkmwzzc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wtdeasve.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hmxcvyit.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2aqvwosra.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2csjgieyv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yhaiuhow.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2odfsrpsd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2qwsxaujg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2rmcvenyp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2cydhbqih.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vtqiczsy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2tjuthbnl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2joplpmws.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hwwbaeau.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xivnybxk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ztpbmlak.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pdfuwlgt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vobubtur.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2avdogwxr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wmftyxwc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ztubsbcj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dpzdjtok.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rqzwhpxd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zouvqmfi.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ldiskmjf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2idpxvjis.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bjjwnjhr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fsxzijvl.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cjtvibue.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2sxmlixtg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uaukdfqn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2rlysflnh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2amwkauxp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2spssbybm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vmxpoblm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gxkibuoa.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nmfyepzn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vtsddmqc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2etsxfrfp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qrgiowla.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2syboniub.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gicrlhqu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2rdjfexld.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vipzvjen.html


<!-- 参考信息 -->