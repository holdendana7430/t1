代发 wailian999

[U97] JS：并发请求
来源：http://xf.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ni.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://fr.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sf.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://um.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://tx.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://lf.szxytkj.cn

document.querySelector(".item")
来源：http://zr.yuexingan06.cn

[U101] JS：classList 操作
来源：http://dy.shxzukj.cn

el.classList.toggle("active")
来源：http://yx.bjjhwx.cn

[U102] JS：本地存储
来源：http://lk.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dn.asd995.cn

[U103] JS：定时器
来源：http://jg.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wr.haigaiapp.cn

[U104] JS：防抖
来源：http://vc.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://an.chemitech.net.cn

[U105] JS：节流
来源：http://jk.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yu.colortex.cn

[U106] JS：日期格式化
来源：http://mz.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gn.bjjhwx.cn

[U107] JS：数字千分位
来源：http://dy.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hs.bookmarksfly.cn

[U108] JS：随机整数
来源：http://fn.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tp.muxihuayi.cn

[U109] JS：数组分组
来源：http://xi.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://lq.huixiangedu.cn

[U110] JS：数组分块
来源：http://xg.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ug.panjiajie.cn

[U111] JS：对象转 Map
来源：http://fa.panjiajie.cn

new Map(Object.entries(obj))
来源：http://ey.chemitech.net.cn

[U112] JS：字符串补位
来源：http://gc.shxzukj.cn

"7".padStart(3, "0")
来源：http://tw.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://jf.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://co.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://cq.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gs.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://oh.huanxung.cn

crypto.randomUUID()
来源：http://dy.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://dj.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://xn.gzmigu.cn

[U117] JS：单元测试
来源：http://cc.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://ad.huanxung.cn

[U118] JS：开发服务器
来源：http://dj.panjiajie.cn

npm i -D vite;  npx vite
来源：http://pq.shtwfgs.cn

[U119] JS：生产构建
来源：http://ms.colortex.cn

npx vite build
来源：http://es.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://kj.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://gk.9csxet.cn

================================================================================
来源：http://fk.haigaiapp.cn

统计汇总
来源：http://bm.shxzskj.cn

================================================================================
来源：http://wc.wgjwhj.cn

按语言统计（条）：
来源：http://cl.521024.cn

Python ......... 252
来源：http://ml.hahajie.cn

PHP ............ 252
来源：http://ra.chemitech.net.cn

JavaScript ..... 252
来源：http://nq.szsharing.cn

TypeScript ..... 212
来源：http://us.9csxet.cn

Java ........... 212
来源：http://ch.shtwfgs.cn

Go ............. 212
来源：http://no.shxzukj.cn

Ruby ........... 212
来源：http://ww.nicolike.cn

C# ............. 212
来源：http://ev.szsharing.cn

C .............. 30
来源：http://fv.newstarts.cn

C++ ............ 30
来源：http://wv.haigaiapp.cn

SQL ............ 90
来源：http://dh.huixiangedu.cn

Bash ........... 80
来源：http://gm.huixinmuqiang.cn

Kotlin ......... 15
来源：http://ct.gzmigu.cn

Swift .......... 15
来源：http://em.nszjky.cn

Lua ............ 10
来源：http://xo.hahajie.cn

Perl ........... 10
来源：http://wy.hnjuh.cn

Scala .......... 10
来源：http://aq.szsharing.cn

------------------------------------
来源：http://hb.colortex.cn

合计 ........... 2106 条
来源：http://vs.yuexingan06.cn

按章节统计：
来源：http://fq.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ma.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ji.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://am.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ea.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ic.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cz.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xf.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yo.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pw.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sp.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rl.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lg.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pg.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xq.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wp.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vm.szsharing.cn

Q SQL 专题                              90
来源：http://li.bookmarksfly.cn

R Bash 专题                             80
来源：http://vz.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://zv.nszjky.cn

T 其他语言补充                          60
来源：http://tk.nszjky.cn

U 高频实用片段                         120
来源：http://kd.bjjhwx.cn

------------------------------------
来源：http://tf.shxzskj.cn

合计                                  2106 条
来源：http://ht.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://yz.hnjuh.cn

使用提醒
来源：http://hb.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://fx.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sg.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bk.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dm.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ab.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://de.wgjwhj.cn

—— 文件结束 ——
来源：http://zl.gzmigu.cn

================================================================================
来源：http://vg.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://eh.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://sn.asd995.cn

================================================================================
来源：http://an.huixinmuqiang.cn

【收录内容】
来源：http://dq.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pk.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xq.9csxet.cn

SQL · Bash · C · C++
来源：http://wz.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lk.newstarts.cn

【使用说明】
来源：http://gh.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://go.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ip.nicolike.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://er.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ub.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ef.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vz.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sp.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vw.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kp.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fs.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cy.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xj.shtwfgs.cn

【文件统计】
来源：http://vs.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ff.asd995.cn

--------------------------------------------------------------------------------
来源：http://sb.colortex.cn

目  录
来源：http://uo.huanxung.cn

--------------------------------------------------------------------------------
来源：http://oy.gzmigu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://am.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ky.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://av.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rj.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qp.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ne.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gk.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://br.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ms.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dp.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nw.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ia.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dh.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ak.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dc.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dy.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jc.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eh.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ro.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ez.szsharing.cn

================================================================================
来源：http://nc.yuexingan06.cn

A. 基础语法与类型
来源：http://qk.nszjky.cn

================================================================================
来源：http://ww.nszjky.cn

[A01] Hello World
来源：http://hs.colortex.cn

Py:   print("Hello, World!")
来源：http://re.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://rs.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://cu.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wg.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://dk.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://fp.bookmarksfly.cn

Ruby: puts "Hello, World!"
来源：http://yv.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ln.panjiajie.cn

[A02] 变量声明与赋值
来源：http://bh.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tj.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qk.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vi.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dp.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://ft.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://hg.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://fj.szxytkj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dx.521024.cn

[A03] 常量定义
来源：http://wb.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tx.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://rm.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://su.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://vx.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://ty.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://lm.panjiajie.cn

Ruby: PI = 3.14159
来源：http://wh.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://sw.shxzukj.cn

[A04] 判断变量类型
来源：http://qm.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vg.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ft.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xm.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://bv.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rw.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nf.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zy.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://ae.521024.cn

[A05] 整数除法与取模
来源：http://wd.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jr.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fk.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vk.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nz.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://ny.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://um.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://zz.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://kk.9csxet.cn

[A06] 字符串转数字
来源：http://rh.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://vp.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oe.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vx.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xh.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ui.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ko.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rs.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vd.bjjhwx.cn

[A07] 数字转字符串
来源：http://yh.newstarts.cn

Py:   str(42)
来源：http://nr.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://io.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://fc.yuexingan06.cn

TS:   String(42)
来源：http://wm.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xg.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://ff.jctech888.com.cn

Ruby: 42.to_s
来源：http://pr.szxytkj.cn

C#:   42.ToString()
来源：http://er.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://vo.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ml.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vv.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ah.lnxyls.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pm.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yo.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nq.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zg.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ee.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://qe.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yv.colortex.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lt.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xg.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uz.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qz.hnjuh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ps.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rx.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cd.muxihuayi.cn

[A10] 生成随机数
来源：http://jm.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://ys.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://qh.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gu.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://no.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://rx.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cb.bjjhwx.cn

Ruby: rand(1..100)
来源：http://fc.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://ae.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://bw.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://vu.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jk.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xh.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ji.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://kw.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wv.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dv.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jc.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://gu.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ir.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yb.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://ca.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://at.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://dc.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zg.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://gw.521024.cn

C#:   $"Hello, {name}!"
来源：http://da.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vf.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://ur.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://pj.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://mw.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://rq.szsharing.cn

Java: "第一行\n第二行"
来源：http://ro.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://gm.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://mn.newstarts.cn

C#:   "第一行\n第二行"
来源：http://kx.haigaiapp.cn

[A14] 注释写法
来源：http://ad.newstarts.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ci.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hw.521024.cn

JS:   // 单行；/* 多行 */
来源：http://yx.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://xt.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aq.wgjwhj.cn

Go:   // 单行；/* 多行 */
来源：http://ug.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dl.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://sc.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://wj.asd995.cn

Py:   value = data or "默认值"
来源：http://lk.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://jy.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://dg.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://jm.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qx.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://gx.nszjky.cn

Ruby: value = data || "默认值"
来源：http://mn.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://ew.huixiangedu.cn

[A16] 真假值判断规则
来源：http://ku.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vg.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eh.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qi.shtwfgs.cn

TS:   if (!x) {}
来源：http://ch.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://at.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ds.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hy.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ui.newstarts.cn

[A17] 位运算
来源：http://sm.szsharing.cn


<!-- 参考信息 -->