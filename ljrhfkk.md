代发 wailian999

[U93] JS：模板字符串
来源：http://ri.9csxet.cn

`共 ${n} 条`
来源：http://pl.panjiajie.cn

[U94] JS：箭头函数
来源：http://dg.bookmarksfly.cn

const double = x => x * 2;
来源：http://wd.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://by.colortex.cn

new Promise((resolve, reject) => {})
来源：http://rp.huanxung.cn

[U96] JS：async/await 与异常
来源：http://nx.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oo.shxzukj.cn

[U97] JS：并发请求
来源：http://gk.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yn.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://fc.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hr.nszjky.cn

[U99] JS：事件监听
来源：http://vt.newstarts.cn

el.addEventListener("click", e => {})
来源：http://su.panjiajie.cn

[U100] JS：DOM 查询
来源：http://lo.huixiangedu.cn

document.querySelector(".item")
来源：http://zq.lnxyls.cn

[U101] JS：classList 操作
来源：http://rf.shxzukj.cn

el.classList.toggle("active")
来源：http://fp.lnxyls.cn

[U102] JS：本地存储
来源：http://ws.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ca.jctech888.com.cn

[U103] JS：定时器
来源：http://vp.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yx.szxytkj.cn

[U104] JS：防抖
来源：http://cv.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lj.colortex.cn

[U105] JS：节流
来源：http://fc.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oe.521024.cn

[U106] JS：日期格式化
来源：http://ue.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cw.hahajie.cn

[U107] JS：数字千分位
来源：http://az.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eb.shxzskj.cn

[U108] JS：随机整数
来源：http://be.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bd.haigaiapp.cn

[U109] JS：数组分组
来源：http://qj.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://kk.shtwfgs.cn

[U110] JS：数组分块
来源：http://ii.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jt.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://ef.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://ek.szsharing.cn

[U112] JS：字符串补位
来源：http://fh.shtwfgs.cn

"7".padStart(3, "0")
来源：http://nf.shxzskj.cn

[U113] JS：正则替换全部
来源：http://jq.9csxet.cn

s.replaceAll("a", "b")
来源：http://ss.nicolike.cn

[U114] JS：JSON 深比较
来源：http://ik.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wu.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://kc.jianghongdianzi.cn

crypto.randomUUID()
来源：http://wc.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://op.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://xx.szxytkj.cn

[U117] JS：单元测试
来源：http://tk.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://uw.nszjky.cn

[U118] JS：开发服务器
来源：http://wl.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://el.lnxyls.cn

[U119] JS：生产构建
来源：http://zh.huixinmuqiang.cn

npx vite build
来源：http://gg.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ek.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://ji.hnjuh.cn

================================================================================
来源：http://ul.haigaiapp.cn

统计汇总
来源：http://vt.huanxung.cn

================================================================================
来源：http://gj.newstarts.cn

按语言统计（条）：
来源：http://qg.panjiajie.cn

Python ......... 252
来源：http://xm.asd995.cn

PHP ............ 252
来源：http://re.panjiajie.cn

JavaScript ..... 252
来源：http://lu.wgjwhj.cn

TypeScript ..... 212
来源：http://cm.521024.cn

Java ........... 212
来源：http://jo.wgjwhj.cn

Go ............. 212
来源：http://vw.colortex.cn

Ruby ........... 212
来源：http://sz.nicolike.cn

C# ............. 212
来源：http://up.huanxung.cn

C .............. 30
来源：http://tz.jctech888.com.cn

C++ ............ 30
来源：http://df.bookmarksfly.cn

SQL ............ 90
来源：http://rv.wgjwhj.cn

Bash ........... 80
来源：http://ef.gzmigu.cn

Kotlin ......... 15
来源：http://cy.wgjwhj.cn

Swift .......... 15
来源：http://gh.9csxet.cn

Lua ............ 10
来源：http://if.szxytkj.cn

Perl ........... 10
来源：http://mj.shtwfgs.cn

Scala .......... 10
来源：http://be.bjjhwx.cn

------------------------------------
来源：http://ol.colortex.cn

合计 ........... 2106 条
来源：http://xx.szsharing.cn

按章节统计：
来源：http://cp.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fq.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sb.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bf.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ra.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ru.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ef.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ga.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yb.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ti.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uh.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vp.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://za.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sv.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://km.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ax.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gb.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://wz.chemitech.net.cn

R Bash 专题                             80
来源：http://hc.asd995.cn

S C / C++ 专题                          60
来源：http://xf.lnxyls.cn

T 其他语言补充                          60
来源：http://db.szsharing.cn

U 高频实用片段                         120
来源：http://wv.bjjhwx.cn

------------------------------------
来源：http://gj.gzmigu.cn

合计                                  2106 条
来源：http://jb.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://xe.shxzukj.cn

使用提醒
来源：http://gj.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://yi.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qj.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ph.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xi.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ef.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://po.jianghongdianzi.cn

—— 文件结束 ——
来源：http://nl.shxzskj.cn

================================================================================
来源：http://db.szsharing.cn

程序语言常见例子速查手册（2024 版）
来源：http://ug.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://xp.colortex.cn

================================================================================
来源：http://rp.asd995.cn

【收录内容】
来源：http://vf.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oa.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nk.newstarts.cn

SQL · Bash · C · C++
来源：http://fy.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vh.asd995.cn

【使用说明】
来源：http://mi.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zr.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fb.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qw.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ut.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sh.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ro.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xh.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://we.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://je.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uu.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cv.huixinmuqiang.cn

【文件统计】
来源：http://vv.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dp.521024.cn

--------------------------------------------------------------------------------
来源：http://yy.521024.cn

目  录
来源：http://ge.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://vv.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lu.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qo.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mq.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cw.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cz.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://au.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://th.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qc.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jn.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fh.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fg.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vp.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gq.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gd.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tv.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hw.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rr.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qt.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ds.yuexingan06.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sk.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://br.muxihuayi.cn

================================================================================
来源：http://zw.huixiangedu.cn

A. 基础语法与类型
来源：http://wh.9csxet.cn

================================================================================
来源：http://xa.muxihuayi.cn

[A01] Hello World
来源：http://la.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://je.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://rd.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://ns.bookmarksfly.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hs.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://kw.shxzukj.cn

Go:   fmt.Println("Hello, World!")
来源：http://ub.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://xu.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qs.9csxet.cn

[A02] 变量声明与赋值
来源：http://ep.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ia.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fq.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ok.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yh.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://tk.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://xd.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://ip.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ix.nszjky.cn

[A03] 常量定义
来源：http://bx.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sm.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://jp.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://yz.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://dx.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://le.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://kj.hahajie.cn

Ruby: PI = 3.14159
来源：http://ba.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://pv.521024.cn

[A04] 判断变量类型
来源：http://nl.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://aj.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nw.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zf.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://xa.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eb.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hq.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qn.521024.cn

C#:   x.GetType().Name; x is int
来源：http://mm.colortex.cn

[A05] 整数除法与取模
来源：http://od.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dd.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sz.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fi.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zr.nszjky.cn

Java: 7 / 2; 7 % 2
来源：http://yg.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://zo.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://qj.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://uz.bjjhwx.cn

[A06] 字符串转数字
来源：http://km.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://qw.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vi.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rq.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qq.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ui.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fz.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ez.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oo.9csxet.cn

[A07] 数字转字符串
来源：http://py.haigaiapp.cn

Py:   str(42)
来源：http://pv.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://tp.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://pq.haigaiapp.cn

TS:   String(42)
来源：http://hv.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://me.521024.cn

Go:   strconv.Itoa(42)
来源：http://ix.szxytkj.cn

Ruby: 42.to_s
来源：http://sy.shxzukj.cn

C#:   42.ToString()
来源：http://nq.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://qe.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vt.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dv.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yn.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ak.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xk.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jz.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ns.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://km.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://up.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ge.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qr.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hb.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ec.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ih.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qu.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rg.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fh.nicolike.cn

[A10] 生成随机数
来源：http://vx.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://ep.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://fp.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zb.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ea.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://fz.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nz.newstarts.cn

Ruby: rand(1..100)
来源：http://bj.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://ne.hahajie.cn

[A11] 条件表达式（三元）
来源：http://xz.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://vf.jianghongdianzi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fk.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sc.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ll.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://ev.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://fz.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sl.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iv.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://fz.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ly.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vx.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://ex.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://xc.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://ed.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bc.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://rp.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://bf.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cx.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://oc.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://do.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://du.9csxet.cn

TS:   "第一行\n第二行"
来源：http://io.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://js.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://fl.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://yc.newstarts.cn

C#:   "第一行\n第二行"
来源：http://wq.colortex.cn

[A14] 注释写法
来源：http://zr.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yx.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ox.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://yn.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://ok.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fm.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://uo.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tu.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://zv.shxzukj.cn

[A15] 空值判断与默认值
来源：http://av.shxzukj.cn

Py:   value = data or "默认值"
来源：http://xu.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://ku.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://eq.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://pv.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uc.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://zv.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://pj.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://mw.lnxyls.cn

[A16] 真假值判断规则
来源：http://us.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ii.hnjuh.cn


<!-- 参考信息 -->