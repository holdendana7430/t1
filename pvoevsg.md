代发 wailian999

[U91] JS：对象键值遍历
来源：http://ki.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qp.hahajie.cn

[U92] JS：深拷贝
来源：http://cy.521024.cn

structuredClone(obj)
来源：http://yj.asd995.cn

[U93] JS：模板字符串
来源：http://yn.gzmigu.cn

`共 ${n} 条`
来源：http://rs.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://zd.shxzukj.cn

const double = x => x * 2;
来源：http://ob.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://wx.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://pc.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://cx.szxytkj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ob.hahajie.cn

[U97] JS：并发请求
来源：http://hy.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wm.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://st.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dj.szsharing.cn

[U99] JS：事件监听
来源：http://qb.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://eb.lnxyls.cn

[U100] JS：DOM 查询
来源：http://cl.gzmigu.cn

document.querySelector(".item")
来源：http://sb.yuntaijiaju.cn

[U101] JS：classList 操作
来源：http://qy.chemitech.net.cn

el.classList.toggle("active")
来源：http://ac.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://jh.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gc.bookmarksfly.cn

[U103] JS：定时器
来源：http://vn.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ly.jctech888.com.cn

[U104] JS：防抖
来源：http://pc.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ju.gzmigu.cn

[U105] JS：节流
来源：http://tt.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qk.hahajie.cn

[U106] JS：日期格式化
来源：http://ju.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://km.muxihuayi.cn

[U107] JS：数字千分位
来源：http://qh.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uv.yuexingan06.cn

[U108] JS：随机整数
来源：http://uh.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kv.shxzukj.cn

[U109] JS：数组分组
来源：http://rd.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://iy.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://dq.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lu.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://jb.colortex.cn

new Map(Object.entries(obj))
来源：http://wv.huixiangedu.cn

[U112] JS：字符串补位
来源：http://hv.shtwfgs.cn

"7".padStart(3, "0")
来源：http://nd.huanxung.cn

[U113] JS：正则替换全部
来源：http://dm.panjiajie.cn

s.replaceAll("a", "b")
来源：http://ag.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://tu.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://re.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://fa.jctech888.com.cn

crypto.randomUUID()
来源：http://kv.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://yt.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://jk.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://yu.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://aj.hnjuh.cn

[U118] JS：开发服务器
来源：http://cg.hnjuh.cn

npm i -D vite;  npx vite
来源：http://sh.newstarts.cn

[U119] JS：生产构建
来源：http://or.muxihuayi.cn

npx vite build
来源：http://se.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://qt.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://lq.nszjky.cn

================================================================================
来源：http://hs.jianghongdianzi.cn

统计汇总
来源：http://bx.9csxet.cn

================================================================================
来源：http://eb.szsharing.cn

按语言统计（条）：
来源：http://lc.huixinmuqiang.cn

Python ......... 252
来源：http://gk.gzmigu.cn

PHP ............ 252
来源：http://ix.shtwfgs.cn

JavaScript ..... 252
来源：http://kk.huixiangedu.cn

TypeScript ..... 212
来源：http://wc.gzmigu.cn

Java ........... 212
来源：http://zl.asd995.cn

Go ............. 212
来源：http://wu.bjjhwx.cn

Ruby ........... 212
来源：http://ye.jianghongdianzi.cn

C# ............. 212
来源：http://vu.szsharing.cn

C .............. 30
来源：http://cg.jianghongdianzi.cn

C++ ............ 30
来源：http://zr.nszjky.cn

SQL ............ 90
来源：http://wz.yuexingan06.cn

Bash ........... 80
来源：http://xt.asd995.cn

Kotlin ......... 15
来源：http://ku.colortex.cn

Swift .......... 15
来源：http://uk.shxzskj.cn

Lua ............ 10
来源：http://st.9csxet.cn

Perl ........... 10
来源：http://ca.jctech888.com.cn

Scala .......... 10
来源：http://xn.asd995.cn

------------------------------------
来源：http://ds.newstarts.cn

合计 ........... 2106 条
来源：http://jf.jianghongdianzi.cn

按章节统计：
来源：http://ap.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oh.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mh.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dr.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://df.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cv.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://th.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fp.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lw.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dj.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gr.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qw.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kb.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kn.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gf.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zp.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cl.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://uz.bjjhwx.cn

R Bash 专题                             80
来源：http://co.nszjky.cn

S C / C++ 专题                          60
来源：http://bv.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://yx.lnxyls.cn

U 高频实用片段                         120
来源：http://wi.newstarts.cn

------------------------------------
来源：http://au.panjiajie.cn

合计                                  2106 条
来源：http://wf.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://aj.szxytkj.cn

使用提醒
来源：http://zi.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://rb.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://he.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hn.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qn.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fw.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ea.huixinmuqiang.cn

—— 文件结束 ——
来源：http://lq.huanxung.cn

================================================================================
来源：http://jz.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://al.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://th.asd995.cn

================================================================================
来源：http://ia.asd995.cn

【收录内容】
来源：http://le.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rg.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://al.yuexingan06.cn

SQL · Bash · C · C++
来源：http://ht.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zp.panjiajie.cn

【使用说明】
来源：http://os.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://br.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rb.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nl.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ct.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bp.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xc.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yb.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://or.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ka.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jq.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ey.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mj.jianghongdianzi.cn

【文件统计】
来源：http://jb.hahajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://to.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://tr.yuexingan06.cn

目  录
来源：http://ys.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://zp.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mv.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://of.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ze.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://be.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wc.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ee.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://th.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://it.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bc.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://re.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ae.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://id.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://da.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ux.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mp.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sg.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gv.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://no.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yy.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yo.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://aj.szxytkj.cn

================================================================================
来源：http://sc.nszjky.cn

A. 基础语法与类型
来源：http://qp.nicolike.cn

================================================================================
来源：http://an.shtwfgs.cn

[A01] Hello World
来源：http://hj.newstarts.cn

Py:   print("Hello, World!")
来源：http://ts.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://ev.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://yy.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kj.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://lc.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://yt.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://ko.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fg.lnxyls.cn

[A02] 变量声明与赋值
来源：http://wh.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://az.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fj.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ua.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jg.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://ra.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://ol.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://uc.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ru.nszjky.cn

[A03] 常量定义
来源：http://oe.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wc.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://pm.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://rh.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://ch.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://zz.szxytkj.cn

Go:   const PI = 3.14159
来源：http://kd.9csxet.cn

Ruby: PI = 3.14159
来源：http://yh.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://sl.shtwfgs.cn

[A04] 判断变量类型
来源：http://xb.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dn.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sc.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ip.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://cx.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://va.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ky.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zi.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://kv.yuexingan06.cn

[A05] 整数除法与取模
来源：http://kz.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uk.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bh.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hi.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lj.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://pt.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://tt.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://yo.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://um.panjiajie.cn

[A06] 字符串转数字
来源：http://bn.shxzskj.cn

Py:   int("42"); float("3.14")
来源：http://gi.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vt.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ef.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uk.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bu.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pp.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vv.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bb.shxzukj.cn

[A07] 数字转字符串
来源：http://sz.newstarts.cn

Py:   str(42)
来源：http://qn.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://ub.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://zz.bookmarksfly.cn

TS:   String(42)
来源：http://rp.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gm.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://qp.colortex.cn

Ruby: 42.to_s
来源：http://yx.shxzukj.cn

C#:   42.ToString()
来源：http://hl.hnjuh.cn

[A08] 取整与四舍五入
来源：http://vd.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jm.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://he.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ez.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ft.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vg.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zc.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fm.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://id.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://cr.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pc.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qd.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fi.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ku.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hj.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qr.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ia.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fa.521024.cn

[A10] 生成随机数
来源：http://kg.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://qb.asd995.cn

PHP:  random_int(1, 100);
来源：http://ue.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://go.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xb.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://su.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qh.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://wb.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://ug.newstarts.cn

[A11] 条件表达式（三元）
来源：http://ui.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://gl.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dh.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dj.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gn.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://bg.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xr.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pd.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tx.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://zo.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ht.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://og.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://gp.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://dy.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://dg.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gi.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://fn.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://lw.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://la.hahajie.cn

Py:   "第一行\n第二行"
来源：http://ue.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://pp.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://xm.huanxung.cn

TS:   "第一行\n第二行"
来源：http://uy.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://zo.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://oc.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://cn.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://go.muxihuayi.cn

[A14] 注释写法
来源：http://ct.hnjuh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qh.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ly.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://cf.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://ar.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hh.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://gt.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ep.521024.cn

C#:   // 单行；/* 多行 */
来源：http://pt.shxzukj.cn

[A15] 空值判断与默认值
来源：http://ba.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://au.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://tp.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://bp.shtwfgs.cn

TS:   const value = data ?? "默认值";
来源：http://on.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cw.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://wn.panjiajie.cn


<!-- 参考信息 -->