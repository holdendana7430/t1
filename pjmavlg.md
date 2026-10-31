代发 wailian999

[U97] JS：并发请求
来源：http://io.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sr.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://uy.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hk.9csxet.cn

[U99] JS：事件监听
来源：http://bf.nicolike.cn

el.addEventListener("click", e => {})
来源：http://xq.9csxet.cn

[U100] JS：DOM 查询
来源：http://ae.newstarts.cn

document.querySelector(".item")
来源：http://dm.shxzskj.cn

[U101] JS：classList 操作
来源：http://nm.chemitech.net.cn

el.classList.toggle("active")
来源：http://nd.shxzukj.cn

[U102] JS：本地存储
来源：http://ql.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ow.huixiangedu.cn

[U103] JS：定时器
来源：http://rc.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ql.lnxyls.cn

[U104] JS：防抖
来源：http://tp.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jl.huixinmuqiang.cn

[U105] JS：节流
来源：http://bc.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sd.jctech888.com.cn

[U106] JS：日期格式化
来源：http://cy.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dj.huixiangedu.cn

[U107] JS：数字千分位
来源：http://sg.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://et.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://rr.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://td.nicolike.cn

[U109] JS：数组分组
来源：http://lm.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://ki.haigaiapp.cn

[U110] JS：数组分块
来源：http://db.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ts.nszjky.cn

[U111] JS：对象转 Map
来源：http://un.nszjky.cn

new Map(Object.entries(obj))
来源：http://jc.huanxung.cn

[U112] JS：字符串补位
来源：http://mk.szsharing.cn

"7".padStart(3, "0")
来源：http://cn.nszjky.cn

[U113] JS：正则替换全部
来源：http://di.521024.cn

s.replaceAll("a", "b")
来源：http://rr.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://rb.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xj.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://eh.hnjuh.cn

crypto.randomUUID()
来源：http://cw.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://nw.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://cy.huixiangedu.cn

[U117] JS：单元测试
来源：http://py.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://iv.colortex.cn

[U118] JS：开发服务器
来源：http://uu.nicolike.cn

npm i -D vite;  npx vite
来源：http://ph.colortex.cn

[U119] JS：生产构建
来源：http://rj.hnjuh.cn

npx vite build
来源：http://xy.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://ne.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://ng.9csxet.cn

================================================================================
来源：http://sc.bjjhwx.cn

统计汇总
来源：http://fs.wgjwhj.cn

================================================================================
来源：http://ra.huanxung.cn

按语言统计（条）：
来源：http://rz.hahajie.cn

Python ......... 252
来源：http://ox.shxzukj.cn

PHP ............ 252
来源：http://vk.shxzskj.cn

JavaScript ..... 252
来源：http://wg.bjjhwx.cn

TypeScript ..... 212
来源：http://ii.chemitech.net.cn

Java ........... 212
来源：http://ok.huixinmuqiang.cn

Go ............. 212
来源：http://bh.yuntaijiaju.cn

Ruby ........... 212
来源：http://ch.huanxung.cn

C# ............. 212
来源：http://ab.lnxyls.cn

C .............. 30
来源：http://op.wgjwhj.cn

C++ ............ 30
来源：http://zs.521024.cn

SQL ............ 90
来源：http://zl.hahajie.cn

Bash ........... 80
来源：http://ec.chemitech.net.cn

Kotlin ......... 15
来源：http://qo.gzmigu.cn

Swift .......... 15
来源：http://gf.asd995.cn

Lua ............ 10
来源：http://yr.jctech888.com.cn

Perl ........... 10
来源：http://dv.shxzskj.cn

Scala .......... 10
来源：http://zi.jianghongdianzi.cn

------------------------------------
来源：http://ht.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://px.huixinmuqiang.cn

按章节统计：
来源：http://ci.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://os.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wk.huixiangedu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://om.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xr.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nf.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vw.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jl.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xi.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ha.lnxyls.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jh.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ru.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kj.jianghongdianzi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cb.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://et.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vu.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tc.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://lv.hahajie.cn

R Bash 专题                             80
来源：http://qe.huanxung.cn

S C / C++ 专题                          60
来源：http://ow.chemitech.net.cn

T 其他语言补充                          60
来源：http://pi.muxihuayi.cn

U 高频实用片段                         120
来源：http://hi.9csxet.cn

------------------------------------
来源：http://zr.9csxet.cn

合计                                  2106 条
来源：http://js.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://pk.huixinmuqiang.cn

使用提醒
来源：http://zk.521024.cn

--------------------------------------------------------------------------------
来源：http://rr.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dy.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fw.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ap.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jq.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://os.panjiajie.cn

—— 文件结束 ——
来源：http://np.haigaiapp.cn

================================================================================
来源：http://mw.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://hx.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://cn.shxzukj.cn

================================================================================
来源：http://jz.bjjhwx.cn

【收录内容】
来源：http://vk.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ci.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vp.jctech888.com.cn

SQL · Bash · C · C++
来源：http://ze.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://aa.hnjuh.cn

【使用说明】
来源：http://bi.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qr.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mh.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ml.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sq.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lb.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fy.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vr.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://po.521024.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jo.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lo.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lb.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://do.shtwfgs.cn

【文件统计】
来源：http://pa.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bq.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://yq.panjiajie.cn

目  录
来源：http://ev.colortex.cn

--------------------------------------------------------------------------------
来源：http://vq.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ss.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wc.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://iz.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jq.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yh.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qg.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nf.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sj.nicolike.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uc.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wm.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lc.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xl.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://al.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jy.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zk.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bu.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ad.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ar.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://to.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ha.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oz.colortex.cn

================================================================================
来源：http://uf.huanxung.cn

A. 基础语法与类型
来源：http://va.muxihuayi.cn

================================================================================
来源：http://xk.newstarts.cn

[A01] Hello World
来源：http://nu.szsharing.cn

Py:   print("Hello, World!")
来源：http://ue.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://qz.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://wd.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yh.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://bt.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://mo.521024.cn

Ruby: puts "Hello, World!"
来源：http://jz.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wa.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://yx.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cl.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wx.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gx.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bb.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://ud.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://pr.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://bb.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://eu.521024.cn

[A03] 常量定义
来源：http://oj.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xv.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://go.521024.cn

JS:   const PI = 3.14159;
来源：http://ow.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://li.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://sj.shxzukj.cn

Go:   const PI = 3.14159
来源：http://ks.panjiajie.cn

Ruby: PI = 3.14159
来源：http://oi.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://cy.yuexingan06.cn

[A04] 判断变量类型
来源：http://hj.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tk.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://au.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pz.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://yq.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ez.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hn.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kz.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://qe.asd995.cn

[A05] 整数除法与取模
来源：http://ak.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vn.hahajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://om.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vp.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bp.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://xq.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://jl.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://yy.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://og.bjjhwx.cn

[A06] 字符串转数字
来源：http://hs.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://iq.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ri.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gl.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kj.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bi.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://or.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hs.haigaiapp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uq.panjiajie.cn

[A07] 数字转字符串
来源：http://kg.shxzskj.cn

Py:   str(42)
来源：http://mo.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://uo.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://wc.szsharing.cn

TS:   String(42)
来源：http://em.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qn.521024.cn

Go:   strconv.Itoa(42)
来源：http://mx.szsharing.cn

Ruby: 42.to_s
来源：http://ry.521024.cn

C#:   42.ToString()
来源：http://sv.huanxung.cn

[A08] 取整与四舍五入
来源：http://hd.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ak.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ae.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wy.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uq.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nl.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hb.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hc.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xi.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://ac.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cp.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yx.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gs.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jv.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://up.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zs.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tq.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ze.hnjuh.cn

[A10] 生成随机数
来源：http://rt.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://uk.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://qj.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oz.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vj.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://su.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ei.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://pe.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://dl.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://sf.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://as.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qo.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://op.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ub.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://cq.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ks.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ej.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uc.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://pf.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cu.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://it.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://xa.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://ch.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://cz.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ca.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://sq.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://jp.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gh.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://fp.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://ka.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://ee.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://kx.huanxung.cn

Java: "第一行\n第二行"
来源：http://cw.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://rs.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://fz.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://wq.nicolike.cn

[A14] 注释写法
来源：http://lg.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fc.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jr.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://cs.521024.cn

TS:   // 单行；/* 多行 */
来源：http://ao.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lc.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://jo.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xc.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://xa.newstarts.cn

[A15] 空值判断与默认值
来源：http://ro.szsharing.cn

Py:   value = data or "默认值"
来源：http://nk.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://ss.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://un.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://ue.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jy.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://kv.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://zc.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://ml.panjiajie.cn

[A16] 真假值判断规则
来源：http://du.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ve.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lh.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cf.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://vk.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fk.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ti.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ks.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tp.huixinmuqiang.cn

[A17] 位运算
来源：http://bp.szxytkj.cn


<!-- 参考信息 -->