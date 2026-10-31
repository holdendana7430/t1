代发 wailian999

[U93] JS：模板字符串
来源：http://tt.gzmigu.cn

`共 ${n} 条`
来源：http://nt.muxihuayi.cn

[U94] JS：箭头函数
来源：http://za.haigaiapp.cn

const double = x => x * 2;
来源：http://mj.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://iv.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://jw.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://sg.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ms.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://jz.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yb.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://hc.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://om.bjjhwx.cn

[U99] JS：事件监听
来源：http://sl.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://jx.huanxung.cn

[U100] JS：DOM 查询
来源：http://fm.bjjhwx.cn

document.querySelector(".item")
来源：http://ds.521024.cn

[U101] JS：classList 操作
来源：http://co.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://kb.muxihuayi.cn

[U102] JS：本地存储
来源：http://ob.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qj.hnjuh.cn

[U103] JS：定时器
来源：http://su.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uy.hahajie.cn

[U104] JS：防抖
来源：http://yi.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dx.nicolike.cn

[U105] JS：节流
来源：http://we.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qo.newstarts.cn

[U106] JS：日期格式化
来源：http://tc.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xi.szsharing.cn

[U107] JS：数字千分位
来源：http://lz.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ol.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://bz.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://os.asd995.cn

[U109] JS：数组分组
来源：http://yp.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://ic.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://mu.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sy.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://bj.shxzukj.cn

new Map(Object.entries(obj))
来源：http://uq.wgjwhj.cn

[U112] JS：字符串补位
来源：http://vh.shtwfgs.cn

"7".padStart(3, "0")
来源：http://ap.panjiajie.cn

[U113] JS：正则替换全部
来源：http://cy.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://pv.nszjky.cn

[U114] JS：JSON 深比较
来源：http://zn.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jd.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://ky.shxzukj.cn

crypto.randomUUID()
来源：http://mq.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://dp.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://aa.gzmigu.cn

[U117] JS：单元测试
来源：http://cv.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://wo.szxytkj.cn

[U118] JS：开发服务器
来源：http://zm.shxzukj.cn

npm i -D vite;  npx vite
来源：http://hw.colortex.cn

[U119] JS：生产构建
来源：http://ud.jctech888.com.cn

npx vite build
来源：http://ji.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://ko.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://sm.huanxung.cn

================================================================================
来源：http://ou.szsharing.cn

统计汇总
来源：http://mx.haigaiapp.cn

================================================================================
来源：http://qz.shxzukj.cn

按语言统计（条）：
来源：http://fs.bjjhwx.cn

Python ......... 252
来源：http://lp.hahajie.cn

PHP ............ 252
来源：http://qb.szxytkj.cn

JavaScript ..... 252
来源：http://fz.shtwfgs.cn

TypeScript ..... 212
来源：http://fd.hnjuh.cn

Java ........... 212
来源：http://cs.huanxung.cn

Go ............. 212
来源：http://to.asd995.cn

Ruby ........... 212
来源：http://ny.szsharing.cn

C# ............. 212
来源：http://rv.gzmigu.cn

C .............. 30
来源：http://fv.lnxyls.cn

C++ ............ 30
来源：http://jv.huixiangedu.cn

SQL ............ 90
来源：http://lp.hahajie.cn

Bash ........... 80
来源：http://al.bookmarksfly.cn

Kotlin ......... 15
来源：http://al.lnxyls.cn

Swift .......... 15
来源：http://xp.hahajie.cn

Lua ............ 10
来源：http://ew.bookmarksfly.cn

Perl ........... 10
来源：http://fq.gzmigu.cn

Scala .......... 10
来源：http://to.jianghongdianzi.cn

------------------------------------
来源：http://nz.panjiajie.cn

合计 ........... 2106 条
来源：http://oj.hnjuh.cn

按章节统计：
来源：http://dr.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ib.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qy.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nw.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xx.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yr.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lo.huanxung.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mi.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ez.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qi.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bf.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fo.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kx.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ld.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vl.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xu.shtwfgs.cn

Q SQL 专题                              90
来源：http://yq.newstarts.cn

R Bash 专题                             80
来源：http://tg.chemitech.net.cn

S C / C++ 专题                          60
来源：http://lk.nszjky.cn

T 其他语言补充                          60
来源：http://ka.hnjuh.cn

U 高频实用片段                         120
来源：http://pg.bjjhwx.cn

------------------------------------
来源：http://rz.szsharing.cn

合计                                  2106 条
来源：http://tn.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ed.bookmarksfly.cn

使用提醒
来源：http://vm.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://dc.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vj.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://po.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bc.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cj.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hq.huanxung.cn

—— 文件结束 ——
来源：http://po.bookmarksfly.cn

================================================================================
来源：http://yt.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://xi.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://jl.jianghongdianzi.cn

================================================================================
来源：http://xv.jianghongdianzi.cn

【收录内容】
来源：http://pr.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kb.9csxet.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://az.szsharing.cn

SQL · Bash · C · C++
来源：http://vt.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gm.jctech888.com.cn

【使用说明】
来源：http://tj.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zd.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://th.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wm.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kx.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uu.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ch.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cm.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zh.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://um.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oe.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uj.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jh.nicolike.cn

【文件统计】
来源：http://hj.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yn.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://tp.haigaiapp.cn

目  录
来源：http://fy.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://fp.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ia.shtwfgs.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tq.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xu.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uc.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tq.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vq.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yf.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xk.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bc.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mz.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tf.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cp.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mp.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yj.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qi.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://op.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vo.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ch.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gj.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cc.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ua.bookmarksfly.cn

================================================================================
来源：http://ue.yuntaijiaju.cn

A. 基础语法与类型
来源：http://hp.huixinmuqiang.cn

================================================================================
来源：http://fh.hahajie.cn

[A01] Hello World
来源：http://go.szsharing.cn

Py:   print("Hello, World!")
来源：http://it.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://of.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://yc.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bj.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://lb.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://me.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://og.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xg.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://er.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ij.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lv.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gw.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://df.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://yu.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://cc.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://zx.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mo.asd995.cn

[A03] 常量定义
来源：http://wv.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hs.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://mg.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://af.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://ll.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://xw.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://pn.521024.cn

Ruby: PI = 3.14159
来源：http://eu.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://vw.nszjky.cn

[A04] 判断变量类型
来源：http://yl.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oh.wgjwhj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hu.yuntaijiaju.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wj.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://fz.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cd.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gy.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gh.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://jv.lnxyls.cn

[A05] 整数除法与取模
来源：http://gd.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ao.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tm.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oi.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rd.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://ly.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://vb.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://rw.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://rh.szxytkj.cn

[A06] 字符串转数字
来源：http://tx.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://hm.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ca.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hd.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://iv.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oj.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pd.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wb.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xk.jctech888.com.cn

[A07] 数字转字符串
来源：http://qb.bjjhwx.cn

Py:   str(42)
来源：http://fw.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://oj.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://tk.lnxyls.cn

TS:   String(42)
来源：http://wt.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://on.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://zx.colortex.cn

Ruby: 42.to_s
来源：http://es.521024.cn

C#:   42.ToString()
来源：http://na.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://yo.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zx.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qr.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ud.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gk.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sd.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xu.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cu.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rn.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://dy.haigaiapp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fe.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vs.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rz.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sp.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ff.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jx.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hj.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://de.newstarts.cn

[A10] 生成随机数
来源：http://rr.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://hd.colortex.cn

PHP:  random_int(1, 100);
来源：http://mb.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fx.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tk.huanxung.cn

Java: new Random().nextInt(100) + 1
来源：http://ok.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://se.jctech888.com.cn

Ruby: rand(1..100)
来源：http://hs.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://qu.newstarts.cn

[A11] 条件表达式（三元）
来源：http://ku.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://wq.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hc.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xu.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zy.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://zi.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ix.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cg.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ya.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://hd.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sa.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ky.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://im.asd995.cn

TS:   `Hello, ${name}!`
来源：http://os.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://ed.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xj.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://km.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://ww.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://od.521024.cn

Py:   "第一行\n第二行"
来源：http://ul.asd995.cn

PHP:  "第一行\n第二行"
来源：http://bq.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://we.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://kv.asd995.cn

Java: "第一行\n第二行"
来源：http://ba.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://ha.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://my.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://iv.gzmigu.cn

[A14] 注释写法
来源：http://fg.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vv.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://od.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://no.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://jv.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yi.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://zy.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ly.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://kt.shxzskj.cn

[A15] 空值判断与默认值
来源：http://re.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://gy.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://vb.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://ty.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://xq.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jq.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://ty.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://rt.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://tn.lnxyls.cn

[A16] 真假值判断规则
来源：http://ve.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rz.huanxung.cn


<!-- 参考信息 -->