代发 wailian999

[U95] JS：Promise 包装
来源：http://wi.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://aq.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://ra.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yt.panjiajie.cn

[U97] JS：并发请求
来源：http://ym.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dj.521024.cn

[U98] JS：fetch 带 JSON
来源：http://hz.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yd.lnxyls.cn

[U99] JS：事件监听
来源：http://qa.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://qt.gzmigu.cn

[U100] JS：DOM 查询
来源：http://bg.bjjhwx.cn

document.querySelector(".item")
来源：http://yr.szxytkj.cn

[U101] JS：classList 操作
来源：http://te.yuexingan06.cn

el.classList.toggle("active")
来源：http://wc.nicolike.cn

[U102] JS：本地存储
来源：http://wy.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jn.newstarts.cn

[U103] JS：定时器
来源：http://hd.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yu.yuntaijiaju.cn

[U104] JS：防抖
来源：http://ui.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zp.yuntaijiaju.cn

[U105] JS：节流
来源：http://uu.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zi.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://vu.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lb.panjiajie.cn

[U107] JS：数字千分位
来源：http://gx.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jm.lnxyls.cn

[U108] JS：随机整数
来源：http://gl.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iv.shtwfgs.cn

[U109] JS：数组分组
来源：http://mf.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://fi.shtwfgs.cn

[U110] JS：数组分块
来源：http://bj.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zv.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://rh.shxzskj.cn

new Map(Object.entries(obj))
来源：http://mc.muxihuayi.cn

[U112] JS：字符串补位
来源：http://eo.jctech888.com.cn

"7".padStart(3, "0")
来源：http://uq.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://xu.huanxung.cn

s.replaceAll("a", "b")
来源：http://ce.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://qd.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cq.shxzukj.cn

[U115] JS：生成 UUID
来源：http://uf.shtwfgs.cn

crypto.randomUUID()
来源：http://zh.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://eq.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://qq.hnjuh.cn

[U117] JS：单元测试
来源：http://fh.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://ea.szsharing.cn

[U118] JS：开发服务器
来源：http://ek.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://fn.panjiajie.cn

[U119] JS：生产构建
来源：http://bi.lnxyls.cn

npx vite build
来源：http://sg.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://tl.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://wp.asd995.cn

================================================================================
来源：http://cu.panjiajie.cn

统计汇总
来源：http://tg.nszjky.cn

================================================================================
来源：http://xl.shtwfgs.cn

按语言统计（条）：
来源：http://aa.jctech888.com.cn

Python ......... 252
来源：http://vz.521024.cn

PHP ............ 252
来源：http://yj.hahajie.cn

JavaScript ..... 252
来源：http://dk.hahajie.cn

TypeScript ..... 212
来源：http://cw.yuexingan06.cn

Java ........... 212
来源：http://da.szxytkj.cn

Go ............. 212
来源：http://cc.szsharing.cn

Ruby ........... 212
来源：http://eq.bjjhwx.cn

C# ............. 212
来源：http://zf.haigaiapp.cn

C .............. 30
来源：http://sc.newstarts.cn

C++ ............ 30
来源：http://vu.huixinmuqiang.cn

SQL ............ 90
来源：http://ks.yuexingan06.cn

Bash ........... 80
来源：http://it.szsharing.cn

Kotlin ......... 15
来源：http://lc.colortex.cn

Swift .......... 15
来源：http://vg.shxzukj.cn

Lua ............ 10
来源：http://zf.jctech888.com.cn

Perl ........... 10
来源：http://xw.shtwfgs.cn

Scala .......... 10
来源：http://ur.gzmigu.cn

------------------------------------
来源：http://xb.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://bj.yuntaijiaju.cn

按章节统计：
来源：http://xh.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xw.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qo.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xs.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hs.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rh.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nx.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ee.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ea.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xf.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ss.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zv.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ou.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sd.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dq.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wz.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nv.gzmigu.cn

Q SQL 专题                              90
来源：http://ec.haigaiapp.cn

R Bash 专题                             80
来源：http://nw.nszjky.cn

S C / C++ 专题                          60
来源：http://ii.521024.cn

T 其他语言补充                          60
来源：http://uh.shxzskj.cn

U 高频实用片段                         120
来源：http://ey.hahajie.cn

------------------------------------
来源：http://nr.panjiajie.cn

合计                                  2106 条
来源：http://hr.nszjky.cn

--------------------------------------------------------------------------------
来源：http://wa.panjiajie.cn

使用提醒
来源：http://zs.9csxet.cn

--------------------------------------------------------------------------------
来源：http://uz.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nw.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bn.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qb.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uy.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aa.shxzukj.cn

—— 文件结束 ——
来源：http://gs.shxzskj.cn

================================================================================
来源：http://ig.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://yk.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://lv.shtwfgs.cn

================================================================================
来源：http://br.shtwfgs.cn

【收录内容】
来源：http://gv.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dq.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yx.jctech888.com.cn

SQL · Bash · C · C++
来源：http://hk.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ba.asd995.cn

【使用说明】
来源：http://wo.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cl.shtwfgs.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mk.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://my.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zb.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ii.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://he.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gi.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dl.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://df.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tz.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://no.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wj.muxihuayi.cn

【文件统计】
来源：http://cl.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://aa.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://uy.huanxung.cn

目  录
来源：http://sg.9csxet.cn

--------------------------------------------------------------------------------
来源：http://gc.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mp.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://md.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://md.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pq.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ig.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zj.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ll.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ni.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dc.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qk.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xr.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bd.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lw.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bk.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ri.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zh.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mj.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ju.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ht.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bx.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fv.jctech888.com.cn

================================================================================
来源：http://jt.nicolike.cn

A. 基础语法与类型
来源：http://xk.haigaiapp.cn

================================================================================
来源：http://ry.colortex.cn

[A01] Hello World
来源：http://je.asd995.cn

Py:   print("Hello, World!")
来源：http://rh.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://un.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://hg.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wc.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://ot.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://gz.521024.cn

Ruby: puts "Hello, World!"
来源：http://ru.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dw.shxzskj.cn

[A02] 变量声明与赋值
来源：http://kf.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nn.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ti.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://uj.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jd.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://lg.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://dq.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://rh.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wr.hnjuh.cn

[A03] 常量定义
来源：http://lu.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://da.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://jy.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://tc.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://wf.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://xh.shxzskj.cn

Go:   const PI = 3.14159
来源：http://xj.521024.cn

Ruby: PI = 3.14159
来源：http://in.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://ei.huixiangedu.cn

[A04] 判断变量类型
来源：http://vj.yuntaijiaju.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ob.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mp.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ro.yuexingan06.cn

TS:   typeof x; x instanceof Date
来源：http://la.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qs.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ic.panjiajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pu.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://xa.colortex.cn

[A05] 整数除法与取模
来源：http://ug.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://py.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ln.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ee.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://as.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://hw.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://eb.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://uq.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://fc.newstarts.cn

[A06] 字符串转数字
来源：http://cy.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://vf.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ct.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://em.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fr.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://be.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eu.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ug.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xp.nszjky.cn

[A07] 数字转字符串
来源：http://ki.nicolike.cn

Py:   str(42)
来源：http://ir.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://os.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://dx.lnxyls.cn

TS:   String(42)
来源：http://ih.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ob.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://jb.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://cx.asd995.cn

C#:   42.ToString()
来源：http://ni.newstarts.cn

[A08] 取整与四舍五入
来源：http://xw.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pt.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://et.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://px.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ja.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mn.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fb.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ns.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://aa.521024.cn

[A09] 绝对值与最大最小值
来源：http://mx.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hy.9csxet.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vv.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hf.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yj.hnjuh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vy.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uh.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vi.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qw.521024.cn

[A10] 生成随机数
来源：http://zg.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://qp.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://tu.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bc.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ck.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://yg.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ho.9csxet.cn

Ruby: rand(1..100)
来源：http://qk.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://mn.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://od.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://na.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qj.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sb.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rs.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://pi.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tb.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cw.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qr.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://vv.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xc.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://al.521024.cn

JS:   `Hello, ${name}!`
来源：http://wz.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://yo.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://gw.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ty.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://jc.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://oa.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qx.szsharing.cn

Py:   "第一行\n第二行"
来源：http://ez.bookmarksfly.cn

PHP:  "第一行\n第二行"
来源：http://gh.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://pp.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://zt.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://ip.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://hd.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://rn.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://fi.9csxet.cn

[A14] 注释写法
来源：http://lt.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nr.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pu.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://jv.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://va.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ld.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://wf.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nw.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://vp.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://kz.yuexingan06.cn

Py:   value = data or "默认值"
来源：http://vj.lnxyls.cn

PHP:  $value = $data ?? "默认值";
来源：http://yb.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://fb.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://rw.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://in.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://ct.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://uu.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://az.asd995.cn

[A16] 真假值判断规则
来源：http://bp.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pk.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://or.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dj.huixiangedu.cn

TS:   if (!x) {}
来源：http://ca.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kf.9csxet.cn


<!-- 参考信息 -->