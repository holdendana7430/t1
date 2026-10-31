代发 wailian999

[U89] JS：数组去重
来源：http://nc.huixinmuqiang.cn

[...new Set(arr)]
来源：http://it.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://et.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://yb.9csxet.cn

[U91] JS：对象键值遍历
来源：http://qt.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yx.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://gx.huixinmuqiang.cn

structuredClone(obj)
来源：http://hm.jctech888.com.cn

[U93] JS：模板字符串
来源：http://yv.szxytkj.cn

`共 ${n} 条`
来源：http://uo.wgjwhj.cn

[U94] JS：箭头函数
来源：http://uz.hahajie.cn

const double = x => x * 2;
来源：http://hb.shxzskj.cn

[U95] JS：Promise 包装
来源：http://xt.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://ow.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://rl.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wq.nicolike.cn

[U97] JS：并发请求
来源：http://wr.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qe.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://pt.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sy.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://tp.nszjky.cn

el.addEventListener("click", e => {})
来源：http://di.nszjky.cn

[U100] JS：DOM 查询
来源：http://vf.colortex.cn

document.querySelector(".item")
来源：http://yg.gzmigu.cn

[U101] JS：classList 操作
来源：http://gt.hnjuh.cn

el.classList.toggle("active")
来源：http://sw.nicolike.cn

[U102] JS：本地存储
来源：http://qa.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ms.chemitech.net.cn

[U103] JS：定时器
来源：http://sp.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bz.colortex.cn

[U104] JS：防抖
来源：http://il.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mr.jctech888.com.cn

[U105] JS：节流
来源：http://hp.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dm.huixiangedu.cn

[U106] JS：日期格式化
来源：http://vg.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://df.panjiajie.cn

[U107] JS：数字千分位
来源：http://eb.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://el.nszjky.cn

[U108] JS：随机整数
来源：http://tw.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sg.gzmigu.cn

[U109] JS：数组分组
来源：http://pw.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://ki.chemitech.net.cn

[U110] JS：数组分块
来源：http://ou.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ib.huanxung.cn

[U111] JS：对象转 Map
来源：http://mu.9csxet.cn

new Map(Object.entries(obj))
来源：http://ye.lnxyls.cn

[U112] JS：字符串补位
来源：http://vp.shxzskj.cn

"7".padStart(3, "0")
来源：http://bh.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://qk.shxzukj.cn

s.replaceAll("a", "b")
来源：http://jo.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://mq.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sm.panjiajie.cn

[U115] JS：生成 UUID
来源：http://yx.shtwfgs.cn

crypto.randomUUID()
来源：http://qe.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://hc.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://ko.gzmigu.cn

[U117] JS：单元测试
来源：http://he.521024.cn

npm i -D vitest;  npx vitest
来源：http://uz.shxzskj.cn

[U118] JS：开发服务器
来源：http://iy.9csxet.cn

npm i -D vite;  npx vite
来源：http://ey.huanxung.cn

[U119] JS：生产构建
来源：http://if.nszjky.cn

npx vite build
来源：http://mr.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://xw.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://mo.jctech888.com.cn

================================================================================
来源：http://yw.colortex.cn

统计汇总
来源：http://ms.asd995.cn

================================================================================
来源：http://mz.huanxung.cn

按语言统计（条）：
来源：http://nf.chemitech.net.cn

Python ......... 252
来源：http://ph.shxzukj.cn

PHP ............ 252
来源：http://yl.jianghongdianzi.cn

JavaScript ..... 252
来源：http://og.hahajie.cn

TypeScript ..... 212
来源：http://mf.gzmigu.cn

Java ........... 212
来源：http://wc.wgjwhj.cn

Go ............. 212
来源：http://jo.gzmigu.cn

Ruby ........... 212
来源：http://xd.jctech888.com.cn

C# ............. 212
来源：http://qv.bjjhwx.cn

C .............. 30
来源：http://bt.shtwfgs.cn

C++ ............ 30
来源：http://xk.chemitech.net.cn

SQL ............ 90
来源：http://wp.bookmarksfly.cn

Bash ........... 80
来源：http://ls.shtwfgs.cn

Kotlin ......... 15
来源：http://up.huanxung.cn

Swift .......... 15
来源：http://qx.huanxung.cn

Lua ............ 10
来源：http://fn.nicolike.cn

Perl ........... 10
来源：http://ox.bookmarksfly.cn

Scala .......... 10
来源：http://lt.bookmarksfly.cn

------------------------------------
来源：http://sb.huanxung.cn

合计 ........... 2106 条
来源：http://ns.huixinmuqiang.cn

按章节统计：
来源：http://jt.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xx.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hp.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hw.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fq.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://om.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lj.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gl.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kh.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sz.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cp.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cl.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cu.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://go.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iz.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qk.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kh.bjjhwx.cn

Q SQL 专题                              90
来源：http://kv.asd995.cn

R Bash 专题                             80
来源：http://ew.wgjwhj.cn

S C / C++ 专题                          60
来源：http://bj.haigaiapp.cn

T 其他语言补充                          60
来源：http://ji.bookmarksfly.cn

U 高频实用片段                         120
来源：http://cv.huanxung.cn

------------------------------------
来源：http://ch.muxihuayi.cn

合计                                  2106 条
来源：http://ct.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://ul.yuexingan06.cn

使用提醒
来源：http://kr.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://vx.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fu.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nr.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://we.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tc.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jj.colortex.cn

—— 文件结束 ——
来源：http://rd.521024.cn

================================================================================
来源：http://ap.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://af.nszjky.cn

Common Programming Examples Cheat Book
来源：http://te.panjiajie.cn

================================================================================
来源：http://mv.9csxet.cn

【收录内容】
来源：http://mq.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qu.panjiajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qt.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://kc.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jw.huixinmuqiang.cn

【使用说明】
来源：http://eb.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ep.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yn.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ii.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pm.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qf.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hd.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lu.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ui.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wq.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tn.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fa.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yy.jctech888.com.cn

【文件统计】
来源：http://rm.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ra.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://eo.chemitech.net.cn

目  录
来源：http://gd.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://uy.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zg.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://is.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ck.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xh.colortex.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oy.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ni.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qg.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sv.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://md.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ws.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fi.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rz.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://du.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cj.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pa.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rw.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nj.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://er.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://od.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bs.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pg.bookmarksfly.cn

================================================================================
来源：http://gn.yuntaijiaju.cn

A. 基础语法与类型
来源：http://zc.shxzukj.cn

================================================================================
来源：http://nz.szsharing.cn

[A01] Hello World
来源：http://ep.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://tm.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://um.521024.cn

JS:   console.log("Hello, World!");
来源：http://wj.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://no.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://sm.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://qw.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://jm.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cq.colortex.cn

[A02] 变量声明与赋值
来源：http://ss.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zz.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dm.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xw.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wt.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://ct.521024.cn

Go:   name := "Alex"; age := 20
来源：http://zs.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://hh.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jw.colortex.cn

[A03] 常量定义
来源：http://qf.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ot.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://fk.asd995.cn

JS:   const PI = 3.14159;
来源：http://pz.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://nl.asd995.cn

Java: static final double PI = 3.14159;
来源：http://jl.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://ig.nszjky.cn

Ruby: PI = 3.14159
来源：http://vq.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://sv.huanxung.cn

[A04] 判断变量类型
来源：http://rq.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ji.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vx.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wn.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://jm.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hl.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hm.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bj.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://rg.hahajie.cn

[A05] 整数除法与取模
来源：http://cp.szxytkj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lf.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tj.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://to.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vo.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://xj.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://lu.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://ul.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://tm.haigaiapp.cn

[A06] 字符串转数字
来源：http://wg.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://eh.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jz.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jv.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ol.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ib.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mv.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fb.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uc.hahajie.cn

[A07] 数字转字符串
来源：http://az.huanxung.cn

Py:   str(42)
来源：http://mj.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://wm.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://wi.521024.cn

TS:   String(42)
来源：http://iq.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tt.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://at.asd995.cn

Ruby: 42.to_s
来源：http://py.yuexingan06.cn

C#:   42.ToString()
来源：http://aj.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://wq.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wj.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rf.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jz.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cf.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dm.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fo.haigaiapp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bo.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uj.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://bw.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tv.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cf.lnxyls.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mx.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hx.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vs.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ok.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yg.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ay.colortex.cn

[A10] 生成随机数
来源：http://lx.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://bx.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://it.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ak.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nf.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://ex.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mq.asd995.cn

Ruby: rand(1..100)
来源：http://qp.521024.cn

C#:   new Random().Next(1, 101)
来源：http://iy.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://xx.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://iy.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ld.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://js.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dr.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://zw.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ib.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ma.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://aw.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://nm.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ws.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://od.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://vd.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://qe.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://el.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tc.521024.cn

Ruby: "Hello, #{name}!"
来源：http://oc.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://dw.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zt.huanxung.cn

Py:   "第一行\n第二行"
来源：http://jy.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://vg.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://qy.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://md.colortex.cn

Java: "第一行\n第二行"
来源：http://yz.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://nk.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://it.9csxet.cn

C#:   "第一行\n第二行"
来源：http://pu.hahajie.cn

[A14] 注释写法
来源：http://wn.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pw.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ao.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://wg.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://uw.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xf.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://ti.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fu.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://xr.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://cv.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://ro.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://fk.bjjhwx.cn


<!-- 参考信息 -->