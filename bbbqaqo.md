代发 wailian999

[U91] JS：对象键值遍历
来源：http://cb.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lf.muxihuayi.cn

[U92] JS：深拷贝
来源：http://se.nszjky.cn

structuredClone(obj)
来源：http://vf.shtwfgs.cn

[U93] JS：模板字符串
来源：http://kf.asd995.cn

`共 ${n} 条`
来源：http://nm.szxytkj.cn

[U94] JS：箭头函数
来源：http://lq.shxzukj.cn

const double = x => x * 2;
来源：http://sj.shxzskj.cn

[U95] JS：Promise 包装
来源：http://af.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://fo.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://gj.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gb.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://bx.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xo.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://oa.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eg.haigaiapp.cn

[U99] JS：事件监听
来源：http://mr.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://xu.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://dq.szsharing.cn

document.querySelector(".item")
来源：http://qd.hahajie.cn

[U101] JS：classList 操作
来源：http://fm.bjjhwx.cn

el.classList.toggle("active")
来源：http://fv.shxzskj.cn

[U102] JS：本地存储
来源：http://cz.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tr.szxytkj.cn

[U103] JS：定时器
来源：http://pm.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ly.huixiangedu.cn

[U104] JS：防抖
来源：http://ix.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://my.bookmarksfly.cn

[U105] JS：节流
来源：http://cl.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cj.bjjhwx.cn

[U106] JS：日期格式化
来源：http://wd.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ba.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://fq.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://la.shtwfgs.cn

[U108] JS：随机整数
来源：http://ml.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qd.hnjuh.cn

[U109] JS：数组分组
来源：http://el.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://hn.bookmarksfly.cn

[U110] JS：数组分块
来源：http://ex.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tt.9csxet.cn

[U111] JS：对象转 Map
来源：http://gu.hahajie.cn

new Map(Object.entries(obj))
来源：http://wl.wgjwhj.cn

[U112] JS：字符串补位
来源：http://wq.nicolike.cn

"7".padStart(3, "0")
来源：http://gd.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://kg.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://rh.9csxet.cn

[U114] JS：JSON 深比较
来源：http://ll.shxzukj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jr.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://sk.wgjwhj.cn

crypto.randomUUID()
来源：http://qo.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://yj.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://ng.chemitech.net.cn

[U117] JS：单元测试
来源：http://sm.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://mu.hnjuh.cn

[U118] JS：开发服务器
来源：http://fc.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://zi.bjjhwx.cn

[U119] JS：生产构建
来源：http://jn.521024.cn

npx vite build
来源：http://gt.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://ff.colortex.cn

import.meta.env.VITE_API_URL
来源：http://te.nszjky.cn

================================================================================
来源：http://fo.nszjky.cn

统计汇总
来源：http://np.asd995.cn

================================================================================
来源：http://qs.haigaiapp.cn

按语言统计（条）：
来源：http://xn.521024.cn

Python ......... 252
来源：http://wp.yuntaijiaju.cn

PHP ............ 252
来源：http://eq.bjjhwx.cn

JavaScript ..... 252
来源：http://nv.jctech888.com.cn

TypeScript ..... 212
来源：http://hf.asd995.cn

Java ........... 212
来源：http://rh.asd995.cn

Go ............. 212
来源：http://gc.huixiangedu.cn

Ruby ........... 212
来源：http://dz.bookmarksfly.cn

C# ............. 212
来源：http://zr.gzmigu.cn

C .............. 30
来源：http://zj.nszjky.cn

C++ ............ 30
来源：http://ld.newstarts.cn

SQL ............ 90
来源：http://ud.yuexingan06.cn

Bash ........... 80
来源：http://fv.wgjwhj.cn

Kotlin ......... 15
来源：http://cp.panjiajie.cn

Swift .......... 15
来源：http://wi.hnjuh.cn

Lua ............ 10
来源：http://un.muxihuayi.cn

Perl ........... 10
来源：http://ae.huanxung.cn

Scala .......... 10
来源：http://jz.muxihuayi.cn

------------------------------------
来源：http://ip.wgjwhj.cn

合计 ........... 2106 条
来源：http://vy.bookmarksfly.cn

按章节统计：
来源：http://wi.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ec.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sj.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://om.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vw.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qa.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uu.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xw.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ff.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uo.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sk.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bl.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://da.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xt.shxzukj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ah.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yb.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ks.szxytkj.cn

Q SQL 专题                              90
来源：http://cc.jctech888.com.cn

R Bash 专题                             80
来源：http://ey.lnxyls.cn

S C / C++ 专题                          60
来源：http://ke.chemitech.net.cn

T 其他语言补充                          60
来源：http://ip.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://pb.szxytkj.cn

------------------------------------
来源：http://qh.shxzukj.cn

合计                                  2106 条
来源：http://yf.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://iz.panjiajie.cn

使用提醒
来源：http://ej.huanxung.cn

--------------------------------------------------------------------------------
来源：http://gy.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gq.shxzskj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cs.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nb.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://om.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tk.hahajie.cn

—— 文件结束 ——
来源：http://wf.shtwfgs.cn

================================================================================
来源：http://qu.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://zz.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://do.yuexingan06.cn

================================================================================
来源：http://wr.muxihuayi.cn

【收录内容】
来源：http://ia.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tg.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pg.shxzukj.cn

SQL · Bash · C · C++
来源：http://oh.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ra.panjiajie.cn

【使用说明】
来源：http://tu.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xu.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vr.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cb.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ts.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fc.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jh.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://de.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hv.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pz.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ln.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yz.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lu.hahajie.cn

【文件统计】
来源：http://ky.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cy.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ya.shxzskj.cn

目  录
来源：http://ft.newstarts.cn

--------------------------------------------------------------------------------
来源：http://jn.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oe.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ka.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rk.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bf.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tw.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ve.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bo.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fy.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sj.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dl.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nj.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yz.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nx.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tn.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uq.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xl.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sy.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mk.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://je.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jg.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sp.yuexingan06.cn

================================================================================
来源：http://uf.shxzukj.cn

A. 基础语法与类型
来源：http://ln.szxytkj.cn

================================================================================
来源：http://lz.huanxung.cn

[A01] Hello World
来源：http://hy.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://lc.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://ts.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://rp.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hu.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://ph.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://gh.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://px.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jo.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://dy.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ue.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mu.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yp.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zd.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://ac.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://ht.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://hi.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xz.nicolike.cn

[A03] 常量定义
来源：http://ra.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fq.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://in.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://zh.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://si.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://ml.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://uw.panjiajie.cn

Ruby: PI = 3.14159
来源：http://mf.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://da.szsharing.cn

[A04] 判断变量类型
来源：http://rh.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zg.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oe.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://by.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://bu.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yj.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cs.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kl.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://ye.hahajie.cn

[A05] 整数除法与取模
来源：http://zf.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bn.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kk.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://un.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ek.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://oy.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://jp.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://mz.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://iw.hahajie.cn

[A06] 字符串转数字
来源：http://eh.colortex.cn

Py:   int("42"); float("3.14")
来源：http://li.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fg.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ar.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tt.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jk.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://at.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ud.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aj.hnjuh.cn

[A07] 数字转字符串
来源：http://ym.szxytkj.cn

Py:   str(42)
来源：http://tp.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://bf.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://ld.jctech888.com.cn

TS:   String(42)
来源：http://vc.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ea.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://bm.huanxung.cn

Ruby: 42.to_s
来源：http://ev.gzmigu.cn

C#:   42.ToString()
来源：http://sw.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://az.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dm.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vi.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://no.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dd.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ir.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ul.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ee.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gd.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://az.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oz.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ur.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jr.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://di.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ud.huixiangedu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bj.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nh.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ft.521024.cn

[A10] 生成随机数
来源：http://qa.9csxet.cn

Py:   import random; random.randint(1, 100)
来源：http://la.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://gt.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bh.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ps.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://fd.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qw.haigaiapp.cn

Ruby: rand(1..100)
来源：http://ao.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://ie.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://oz.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://hm.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nm.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nu.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qp.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://sh.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eh.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://au.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nd.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://xq.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uv.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qi.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://wj.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://mx.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://ct.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ph.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://ab.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://vm.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ss.521024.cn

Py:   "第一行\n第二行"
来源：http://bc.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://kk.asd995.cn

JS:   "第一行\n第二行"
来源：http://ji.521024.cn

TS:   "第一行\n第二行"
来源：http://pn.hnjuh.cn

Java: "第一行\n第二行"
来源：http://ry.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://nx.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://gz.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://jf.bjjhwx.cn

[A14] 注释写法
来源：http://hy.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pv.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://aq.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://kx.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://rs.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ba.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://qc.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qv.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://ft.lnxyls.cn

[A15] 空值判断与默认值
来源：http://pk.panjiajie.cn

Py:   value = data or "默认值"
来源：http://xw.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://th.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://gf.9csxet.cn

TS:   const value = data ?? "默认值";
来源：http://pw.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jc.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://uu.521024.cn


<!-- 参考信息 -->