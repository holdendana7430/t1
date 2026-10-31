代发 wailian999

[U95] JS：Promise 包装
来源：http://tj.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://qi.huanxung.cn

[U96] JS：async/await 与异常
来源：http://ww.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ot.haigaiapp.cn

[U97] JS：并发请求
来源：http://ga.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ar.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://ev.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ay.yuexingan06.cn

[U99] JS：事件监听
来源：http://mv.nicolike.cn

el.addEventListener("click", e => {})
来源：http://vd.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://ta.yuntaijiaju.cn

document.querySelector(".item")
来源：http://zr.lnxyls.cn

[U101] JS：classList 操作
来源：http://nv.shxzskj.cn

el.classList.toggle("active")
来源：http://ul.lnxyls.cn

[U102] JS：本地存储
来源：http://js.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ry.jctech888.com.cn

[U103] JS：定时器
来源：http://yk.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sa.bjjhwx.cn

[U104] JS：防抖
来源：http://fp.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hf.jctech888.com.cn

[U105] JS：节流
来源：http://hr.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ak.wgjwhj.cn

[U106] JS：日期格式化
来源：http://lp.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ff.521024.cn

[U107] JS：数字千分位
来源：http://bq.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eq.jctech888.com.cn

[U108] JS：随机整数
来源：http://vm.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pt.nszjky.cn

[U109] JS：数组分组
来源：http://uf.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://jb.nszjky.cn

[U110] JS：数组分块
来源：http://yu.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nn.lnxyls.cn

[U111] JS：对象转 Map
来源：http://js.521024.cn

new Map(Object.entries(obj))
来源：http://hl.muxihuayi.cn

[U112] JS：字符串补位
来源：http://zn.bjjhwx.cn

"7".padStart(3, "0")
来源：http://ms.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://el.shxzukj.cn

s.replaceAll("a", "b")
来源：http://rn.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://zi.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cr.nicolike.cn

[U115] JS：生成 UUID
来源：http://wm.lnxyls.cn

crypto.randomUUID()
来源：http://wz.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://vj.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://og.9csxet.cn

[U117] JS：单元测试
来源：http://id.asd995.cn

npm i -D vitest;  npx vitest
来源：http://yv.wgjwhj.cn

[U118] JS：开发服务器
来源：http://rt.huanxung.cn

npm i -D vite;  npx vite
来源：http://cw.yuexingan06.cn

[U119] JS：生产构建
来源：http://xx.colortex.cn

npx vite build
来源：http://cq.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://ws.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://my.hnjuh.cn

================================================================================
来源：http://sc.nicolike.cn

统计汇总
来源：http://mb.nszjky.cn

================================================================================
来源：http://vx.muxihuayi.cn

按语言统计（条）：
来源：http://vl.521024.cn

Python ......... 252
来源：http://dt.shtwfgs.cn

PHP ............ 252
来源：http://td.hahajie.cn

JavaScript ..... 252
来源：http://nk.yuntaijiaju.cn

TypeScript ..... 212
来源：http://gp.gzmigu.cn

Java ........... 212
来源：http://jz.lnxyls.cn

Go ............. 212
来源：http://ji.haigaiapp.cn

Ruby ........... 212
来源：http://ei.9csxet.cn

C# ............. 212
来源：http://kj.yuntaijiaju.cn

C .............. 30
来源：http://bw.szsharing.cn

C++ ............ 30
来源：http://dn.hnjuh.cn

SQL ............ 90
来源：http://ja.jctech888.com.cn

Bash ........... 80
来源：http://or.shxzskj.cn

Kotlin ......... 15
来源：http://nu.szxytkj.cn

Swift .......... 15
来源：http://pf.haigaiapp.cn

Lua ............ 10
来源：http://sa.yuntaijiaju.cn

Perl ........... 10
来源：http://gb.shxzskj.cn

Scala .......... 10
来源：http://zb.colortex.cn

------------------------------------
来源：http://yw.chemitech.net.cn

合计 ........... 2106 条
来源：http://bh.shtwfgs.cn

按章节统计：
来源：http://fn.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://md.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hr.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nd.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://te.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oj.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dl.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ik.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zy.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yw.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kd.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vr.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://af.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rg.jianghongdianzi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cu.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yj.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://de.shxzukj.cn

Q SQL 专题                              90
来源：http://am.yuntaijiaju.cn

R Bash 专题                             80
来源：http://gr.shxzukj.cn

S C / C++ 专题                          60
来源：http://uo.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://aj.bookmarksfly.cn

U 高频实用片段                         120
来源：http://hu.hnjuh.cn

------------------------------------
来源：http://yj.hahajie.cn

合计                                  2106 条
来源：http://gt.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://sy.chemitech.net.cn

使用提醒
来源：http://xz.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://rv.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ub.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kf.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lg.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qu.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eo.newstarts.cn

—— 文件结束 ——
来源：http://ii.yuntaijiaju.cn

================================================================================
来源：http://pu.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://ze.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://hf.lnxyls.cn

================================================================================
来源：http://tu.shtwfgs.cn

【收录内容】
来源：http://ga.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://si.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uj.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://eb.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cr.huixinmuqiang.cn

【使用说明】
来源：http://xu.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nq.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://br.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ke.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://le.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mf.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vr.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gl.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kl.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pj.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zz.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sw.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mu.muxihuayi.cn

【文件统计】
来源：http://rw.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vf.9csxet.cn

--------------------------------------------------------------------------------
来源：http://oj.colortex.cn

目  录
来源：http://da.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ko.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cu.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bm.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uc.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qa.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://au.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ce.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qs.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sl.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zs.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://af.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ov.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zi.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zv.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cq.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fe.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ft.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xx.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iq.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yh.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rk.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fn.nicolike.cn

================================================================================
来源：http://mv.wgjwhj.cn

A. 基础语法与类型
来源：http://gf.chemitech.net.cn

================================================================================
来源：http://sp.lnxyls.cn

[A01] Hello World
来源：http://do.shxzukj.cn

Py:   print("Hello, World!")
来源：http://jp.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://cy.asd995.cn

JS:   console.log("Hello, World!");
来源：http://sq.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ju.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://vn.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ny.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://wv.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sl.shxzskj.cn

[A02] 变量声明与赋值
来源：http://yw.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ft.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gc.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://te.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ym.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://el.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://nt.shxzukj.cn

Ruby: name = "Alex"; age = 20
来源：http://qa.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wt.bookmarksfly.cn

[A03] 常量定义
来源：http://hr.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vj.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://aw.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://ld.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://ze.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://pm.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://mu.szsharing.cn

Ruby: PI = 3.14159
来源：http://ag.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://mr.haigaiapp.cn

[A04] 判断变量类型
来源：http://rg.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://it.colortex.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hp.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dh.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://lp.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dm.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://og.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xp.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://nz.gzmigu.cn

[A05] 整数除法与取模
来源：http://tc.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xo.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kz.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mj.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ss.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://mb.521024.cn

Go:   7 / 2; 7 % 2
来源：http://ik.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://wy.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://mq.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://bj.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://hi.yuexingan06.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gc.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bg.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ki.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://db.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fy.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://un.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ht.hnjuh.cn

[A07] 数字转字符串
来源：http://vg.panjiajie.cn

Py:   str(42)
来源：http://nr.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://jo.9csxet.cn

JS:   String(42); (42).toString()
来源：http://hk.lnxyls.cn

TS:   String(42)
来源：http://iy.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jq.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://nf.hnjuh.cn

Ruby: 42.to_s
来源：http://ac.shtwfgs.cn

C#:   42.ToString()
来源：http://mi.nszjky.cn

[A08] 取整与四舍五入
来源：http://yn.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bw.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fj.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qf.panjiajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://di.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yj.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ty.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tx.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pa.9csxet.cn

[A09] 绝对值与最大最小值
来源：http://pv.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dw.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yt.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ef.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://no.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ir.bookmarksfly.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ik.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://am.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sg.huanxung.cn

[A10] 生成随机数
来源：http://bs.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://gz.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://qz.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qo.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rt.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://bl.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yl.hahajie.cn

Ruby: rand(1..100)
来源：http://kt.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://dw.nicolike.cn

[A11] 条件表达式（三元）
来源：http://wm.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://qv.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rh.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yo.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://di.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://sw.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ux.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ma.huanxung.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gl.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://hk.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bj.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ct.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://hb.521024.cn

TS:   `Hello, ${name}!`
来源：http://ke.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://cb.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://py.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://zv.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://zn.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://up.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://sh.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://xh.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://bf.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://cj.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://va.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://zk.521024.cn

Ruby: "第一行\n第二行"
来源：http://qz.nicolike.cn

C#:   "第一行\n第二行"
来源：http://fj.huanxung.cn

[A14] 注释写法
来源：http://zl.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wd.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uu.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://pt.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://et.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ux.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://dh.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ei.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://mc.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://cl.gzmigu.cn

Py:   value = data or "默认值"
来源：http://hz.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://zv.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://qe.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://ac.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vp.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://by.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://sx.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://vq.colortex.cn

[A16] 真假值判断规则
来源：http://wb.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://al.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uj.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dd.bookmarksfly.cn

TS:   if (!x) {}
来源：http://cp.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ya.huixiangedu.cn


<!-- 参考信息 -->