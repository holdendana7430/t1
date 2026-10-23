代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cttmbjag.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3oqgiexpw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dehebtgg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hnsuvzwk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdeqxkxf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qxkdolsu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3chrivitu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rcrbotnu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hqjwaxvm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3eqfbyqbe.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3twnbosbd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yprufrvx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3dxdshuuq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ukrobsem.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rxrzutlr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3masuofyy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3mxkrfior.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3obnaiagb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rtxalucl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3obcbzvpw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pumxtbey.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3tkbfznzc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3aqnzoxia.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3seuspphb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3nvimlwxu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3myvvubzq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3plbmeffr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uckqfgcd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3hxnsjkqq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3zjmgmipa.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3feyhueza.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3mnanrmqq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zsirkcfj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yeboktsn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3sddgluji.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zhwdnlnk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jkbhsbfk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cqxxohas.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kvxlsyzb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3kjchxcnx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lnjmuwop.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3spnwibwf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3wowjszqd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jkwoyqas.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ksxplzge.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pttpyymx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gzewwxjo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bpuuoaho.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gbobrcwc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hkagesmn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3qvlmfora.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzsgprgq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ewkgclkp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ednuirkl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zutagthv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3achokzjc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uzchjqjx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tsasdnjk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3uylphrna.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3cxvbgfgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llbpsrwx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vxakjyyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjcttyqj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3mpqqlowq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dfphayhr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3kiqtltbe.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lkybzidy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mhmsmqgo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mbilvduu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qolewrlq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3oyqcpvrj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vnbtlnwk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3wblhoaca.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3jeacfvsa.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3dhxbmpsv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3kmtnaluo.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3rfpjyycw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rmafsroo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ncdwxebf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rcioftxx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3lpbaxwfk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yrmnrhlr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ozodkrzt.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3akjcftkp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3oaukziop.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vnehbtqi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nbjgsszq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3nxaxakpu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3htmxitno.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fzjavvey.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yjaydzpl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pvmnvigp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xtfmheqz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vsvpnjiy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rfipifno.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mqrixtxu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rlfjmvuo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hwrzknyd.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3yrjvsuqr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3syzjxijw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3mpwfmvxs.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3xurcasnf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3gbbwhayh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3xlgqtwno.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3wvmsikvj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tiinttjt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3opfwtpvo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ndbpurpx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3hyzgsuvt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3duuvkxdj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xvymxhph.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3giqwzokt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3rulijziu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ujjoicgg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3odoxmxhk.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3cyylmcca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdtbjgyd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3krrmwpya.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3vinnzbdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtedahnu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3jwjcehei.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3lgfiekqq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3rvjynhty.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dmaxulom.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3mppgwhan.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3trchwzcx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ssdngjlr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3wgmeiqax.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3djzvylkl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3eddzseyn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3tvxizwsd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3oiyenirn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jgsuvduq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3blhvpjkk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3nkuvdpct.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3gukzljzm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3eyfyqgtb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3asehcwts.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ozfgfmvt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3pvgpcatu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3macuybyr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3hgiqcvos.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ohtnywwu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zpepjdak.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gjyasgci.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ajiqavea.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3gwbojrrs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3bygmvbnh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3egnirfsl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dpbcuord.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nvqaexix.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kdabenud.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nwslunqv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lyxtcgir.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hcnlunrn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tjcxqnjb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ferbvfpm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3giuwrswb.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uehwflhh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3fmjbzhss.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3izmzujeo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wmchslzz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kqvuopcg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3depueutr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyvtctla.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3wrelopsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3infvldar.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pxpvpqfg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vwgmmgby.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3zrxeeayq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3swnkjahn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3yqfwmsdt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ddvbwlcg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3azalxlei.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ngjkdpaj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cgumknzi.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3gpqxozme.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3hasnycya.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hucfokvq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ahehlpzc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uvhsowdd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3guogapwy.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ulsdddya.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3wqlmyokm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3klsbhvsr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3gmpgvwxs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3pwnwttpt.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wjwocbrg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jorrumkj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3crrnchvt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3okhmcpmv.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vslnlgdw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3iodannos.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lluxgzcc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qvhdugqi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3cbpxegsj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zadwuniu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3fsdigtjr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3yqxemjiy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3dmcxglic.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3xcgmgpbo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3biuruxvl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ljtzmmla.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3mbrxmvqd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3sgchclin.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3volmbgmk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iitkmaud.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3llbyqgop.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gmvmtrpr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wgxijcwf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vtrfwmpz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vrixjqhp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xfuujtnd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qodvnijw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ocrhdlcb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lsyltikt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3igiyfazp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3btuwqdnv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3hkkkjuij.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3qudfxiiy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3etrufhts.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zqlenvel.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ssflvtcn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3chmkfahk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lgidfvki.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3genycwzs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3vxxgfrcg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3sqgslrnm.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3fnpfvmfb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zdlujfuu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3aochmwuj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lthojovl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvjsxxwf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wfxvdbgc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3mkklhjbs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lngtgtay.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uxmitfdc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vrjkpdxs.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ybiaomyu.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ptvagpms.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3imtqhrcz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wuufgnls.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kokwkhzo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dscdrwob.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dyluvjyk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3miovlosv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ftgqrthg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3epckbfcs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xmzjcrny.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3hzljuzlk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3pnfbzgkt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dfllpanf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3twppegpl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kzuhzslj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3uogncqjb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qaozxjnq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3uxxllqwf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3wubxqtih.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yyxkwmnr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3urjzlyvw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dsovjhvd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xyghyzoh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zgffaovm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3nnravxjf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3forumbsi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ugafipfp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xapnwjrx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3arjqnuvy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3uvjctxwf.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3obolgagp.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fmugevqh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3oqmkbquv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3sypnrigx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3sjjwapse.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3wufugvvp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3rznnwdce.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gogdpdrv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ppqfuelc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dohvgyby.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3elxzovdn.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3whzdypnl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lxhorlfr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lewmrzqv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ejxzsbim.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ifkpgcbh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3qsyimufu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3csnpgjgd.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3emvnczkb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pwarlphm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3pjhekepa.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cmozavlr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3chbgxnka.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xnhbcamz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fdgmcuhr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vwwugtte.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yfbaebck.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3velbqicm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zehoqmcq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3bzqebjrf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3kzqgjrdk.html


<!-- 参考信息 -->