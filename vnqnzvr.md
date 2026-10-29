代发 wailian999

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/gcvjhgyyu.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gprdhgwmw.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gguorcbel.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gbfvuqttz.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gntpxrbes.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gnsgxjhhr.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gzbuoizrg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gxbvmdgks.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/ghigtlqic.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gicnpoefh.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gzeuvaxek.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gcogbbeif.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gcfokhhlk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gsqgukecg.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/ghfbyehtx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gohibjama.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gzhytjvkh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gnbpiemln.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gpoxgoolu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gxramtvjv.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/ghklssofi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gsthugoyw.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gcdbmrudx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gbykoehgl.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/grlsoqqxz.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gvxjybcdg.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gdgearkhe.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gtwxcurcn.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/ggttlbuhe.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/goxdlwywu.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gsvgdkkyl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/ghdgbbetg.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gbzhfpqqg.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/grlgjiero.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gtuheymve.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gzsvknzxm.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/ggjdcpqrn.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gmcarutib.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gleqatdqc.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gfxdafdxl.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gfbbgmios.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gqvjqnobv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gkotcngzv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gvqirmuts.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxrcckqfj.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gggjegewr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaisoweiz.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gvmwyyont.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gumwtgfwc.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gtevygron.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gscxtflrx.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gdleboswo.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gbxxfefrj.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gxyuxtqyx.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gnwbvviun.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gvgmnhnyf.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gdqryvrih.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gszbihodh.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gkprxgrus.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gladoende.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gbeysbjci.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gxzbbfvbt.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/glwygdxar.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/ghnakmcor.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/ggoujfchm.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gperntnfn.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/grqowtsuu.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gcnmglxjr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/giqmbacbu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/giwbludjn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gqeqfftmm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gcscrqtal.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gcqosfwjr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gtiahwnyx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gflcieqrw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gyhzlbdgq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ghmrcxycm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gmicxlegi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gxhbdhdlm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gdaimubau.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gcmothfal.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gppqvnyxr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gpxqjyuvk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gqwjwcxoi.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gfwfxqjgh.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gtqbwlzyv.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gayuudknk.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/ggkgmcvka.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gizvggiiv.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/glzjjasmv.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/grcemuvay.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gpqkuuypv.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gpnqzbmtz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gtcppvmuo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gbubynwky.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gfflwmgdi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gjinwpbjn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gxhquvdxv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/glzxruzxh.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/ghqwtirqs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsujsszjf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gkgphijkl.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gepjewosz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gihpjydcb.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gvwdlalmn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gwclfjncb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gyuzfpdqi.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/ghaklewkr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/goslafwjc.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gywvusvcj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/glhirctjy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gyndmbqym.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gqqpthtxl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/guoyiqdun.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/geurffmpu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gybhfjenp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gqlapayfa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gdzlczjdr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gtzzvklpv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gnziithzo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gzjjestph.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gbfysdode.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gwdzwsqgi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/gzmaanbia.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gacrsiepm.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gobykrgzl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gwkdxsntt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gnsrohtxx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/glrnewzja.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gdlxhdisp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/guwyaogvb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/guqbssjjq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gvtvxvnov.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gsxvhpucx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gtxgijsiy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ghiuptaer.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gcbercekj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/grzkxtmgu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/grwksgdvz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gjckolych.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gouozxkzl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/gffvqcpsg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gzociwrbl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gpbmvxabd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/gszfjwsdh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gezipdxdo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gqgfjmbmy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gnjemdvkq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grsgitaeh.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/giyaqvxpc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsbnvrzdn.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gdddcmzkv.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/ggolhnvgw.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gvmkcvjux.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gajgkuehs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gteeanlzu.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/ghqbeyuvx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gmbehmygg.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/ghhhtuypu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwdgxiq.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gblyxzmuo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gwiwsyrzr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/gqxaxcdae.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gruayvgum.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/gbmqnlris.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/geuzjtdep.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gqlyxmvok.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/grhjbscqw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/ghyxpkgmk.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/gptljznmb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/getorijuz.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ghssoidji.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gxvlonota.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gopkafahb.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gpcvctcjj.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gukcrwdts.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gqqnmpdfy.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gpsfbhays.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gkrhkaegx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gxcvtildq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gdbyzblis.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gdfdcgyka.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gdbdgjxrm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/gkfgfabjc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gunxszydm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/ghtwmcgsn.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/gijzidsok.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/gmwjjyjbg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gynczjbui.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/ghkoodwzp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gyryorhvw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gbwnkbyys.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/goinzzkvl.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gsiesddvd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gjbowagpw.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gknxxksvw.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gkclegreb.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.hesvh.cn/Article/details/giugwxhen.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/girvtdcch.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/goqicclst.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gkzfgbgrh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gblccpakq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gubfeqwgd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/gmuozrnyg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gceqiyzym.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/gxnrieqht.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/ghracfqoo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/guypybuct.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.hesvh.cn/Article/details/gppwekzfp.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/guqakooxr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gbwdzhves.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/gwwavpddp.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/gwjggocel.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/ghkbesqex.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/ghpmgjdse.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gxnpgbwjf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gqkkzqlpm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gfwszocbh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gujstzwpp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gbuzevmft.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gjmiqzpax.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/gcaquaedy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gmmmypool.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/gxbyfbndl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gffhkdwqd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/giuwjceil.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gdvtmxumj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gxcoymhyt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gmwtluftm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gwjirhicg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.zdbjq.cn/Article/details/gzsqttewc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gedtxuiyv.sHtML

[A10] 生成随机数
来源：http://read.share.hesvh.cn/Article/details/glmrkjach.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gefykemnr.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.hesvh.cn/Article/details/gwgpqtzcc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gfjunbrzm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/ginodihej.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gnnacnxxw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gpsgomxhf.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/glxrcbvas.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/gcsfsipmu.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fehbvm.com/Article/details/gplzcftkh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/gxajiebwg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/ggsqsuxuo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gveiiiysu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gjfoshsgl.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/ggcpgbzrb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.hesvh.cn/Article/details/gmhlytfdk.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gpvyktgkd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/ggeooxwoc.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/gjnxlqdyj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/grizqbitz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/gqjgguprt.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gdzmgbgwb.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gyowwlqsv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fehbvm.com/Article/details/ghqvvgwxz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/gkswemhnt.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/gprpmtdqv.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gtwiaqrlv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gcakirxos.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gcfwudjag.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gzfnkzxzb.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gglyjpapx.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gflbclyry.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gannzwbff.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gdeecrqdf.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gmgzsxwyh.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gsqybumhs.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gvlkdzlwf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gnuymefhv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gwezidiub.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/ggppqgmei.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/ghwqafpzl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fehbvm.com/Article/details/gatyidemf.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gmldtjcyt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gbgmfhhaz.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gkypfdbke.sHtML

[A15] 空值判断与默认值
来源：http://read.share.hesvh.cn/Article/details/gpptvoghx.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/gvxvljuvt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gdyaoyfnf.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gykubumzv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/ghpggyupg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/gbbrwjcrq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.zdbjq.cn/Article/details/gslnshawg.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gpsuodfex.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/ghzrdqpqf.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/gfxlemjix.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fehbvm.com/Article/details/gmnzgvxoz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.zdbjq.cn/Article/details/gnwulvuyh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.hesvh.cn/Article/details/gfvhdxxop.sHtML

TS:   if (!x) {}
来源：http://mobile.fehbvm.com/Article/details/gnhwlwizw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxkzcsprh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/glhpdxsgw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.zdbjq.cn/Article/details/gzcppmwed.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.zdbjq.cn/Article/details/gczsysctx.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/gdhprwlju.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gnmbayviv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/gljmocjzd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gmsvrmhnp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gosjxwzge.sHtML


<!-- 参考信息 -->