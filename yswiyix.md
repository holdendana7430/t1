代发 wailian999

[U85] JS：可选链
来源：http://dv.panjiajie.cn

a?.b?.c
来源：http://fj.szsharing.cn

[U86] JS：空值合并
来源：http://fa.yuntaijiaju.cn

a ?? b
来源：http://qs.newstarts.cn

[U87] JS：解构默认值
来源：http://lt.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://hr.newstarts.cn

[U88] JS：对象展开合并
来源：http://uw.hahajie.cn

{ ...a, ...b }
来源：http://in.szxytkj.cn

[U89] JS：数组去重
来源：http://ds.haigaiapp.cn

[...new Set(arr)]
来源：http://bf.hnjuh.cn

[U90] JS：数字数组排序
来源：http://cy.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://is.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://qq.haigaiapp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ok.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://pd.panjiajie.cn

structuredClone(obj)
来源：http://co.colortex.cn

[U93] JS：模板字符串
来源：http://zn.bjjhwx.cn

`共 ${n} 条`
来源：http://fe.wgjwhj.cn

[U94] JS：箭头函数
来源：http://qx.newstarts.cn

const double = x => x * 2;
来源：http://jf.hnjuh.cn

[U95] JS：Promise 包装
来源：http://gq.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://sz.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://ey.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ae.newstarts.cn

[U97] JS：并发请求
来源：http://xe.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ju.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://wi.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bg.colortex.cn

[U99] JS：事件监听
来源：http://qs.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://qf.colortex.cn

[U100] JS：DOM 查询
来源：http://hy.huixinmuqiang.cn

document.querySelector(".item")
来源：http://aa.shtwfgs.cn

[U101] JS：classList 操作
来源：http://mb.hnjuh.cn

el.classList.toggle("active")
来源：http://ig.nicolike.cn

[U102] JS：本地存储
来源：http://gd.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wk.nszjky.cn

[U103] JS：定时器
来源：http://pi.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ln.haigaiapp.cn

[U104] JS：防抖
来源：http://og.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xt.asd995.cn

[U105] JS：节流
来源：http://xo.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://we.jctech888.com.cn

[U106] JS：日期格式化
来源：http://pj.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sz.shxzukj.cn

[U107] JS：数字千分位
来源：http://oo.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://of.lnxyls.cn

[U108] JS：随机整数
来源：http://pz.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://de.bookmarksfly.cn

[U109] JS：数组分组
来源：http://mw.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://ek.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://rb.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eu.asd995.cn

[U111] JS：对象转 Map
来源：http://uz.lnxyls.cn

new Map(Object.entries(obj))
来源：http://ef.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://mu.szsharing.cn

"7".padStart(3, "0")
来源：http://rw.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://np.panjiajie.cn

s.replaceAll("a", "b")
来源：http://bn.szsharing.cn

[U114] JS：JSON 深比较
来源：http://zf.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mc.szsharing.cn

[U115] JS：生成 UUID
来源：http://wu.huixiangedu.cn

crypto.randomUUID()
来源：http://di.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://rs.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://tt.haigaiapp.cn

[U117] JS：单元测试
来源：http://dq.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://zu.haigaiapp.cn

[U118] JS：开发服务器
来源：http://au.521024.cn

npm i -D vite;  npx vite
来源：http://iv.muxihuayi.cn

[U119] JS：生产构建
来源：http://tt.hahajie.cn

npx vite build
来源：http://ez.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://xd.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://zy.yuexingan06.cn

================================================================================
来源：http://xd.haigaiapp.cn

统计汇总
来源：http://jm.hahajie.cn

================================================================================
来源：http://da.chemitech.net.cn

按语言统计（条）：
来源：http://kn.shtwfgs.cn

Python ......... 252
来源：http://je.asd995.cn

PHP ............ 252
来源：http://up.lnxyls.cn

JavaScript ..... 252
来源：http://sy.521024.cn

TypeScript ..... 212
来源：http://dy.jctech888.com.cn

Java ........... 212
来源：http://wv.hahajie.cn

Go ............. 212
来源：http://iz.shxzukj.cn

Ruby ........... 212
来源：http://wr.shtwfgs.cn

C# ............. 212
来源：http://gd.bjjhwx.cn

C .............. 30
来源：http://eg.jianghongdianzi.cn

C++ ............ 30
来源：http://vz.chemitech.net.cn

SQL ............ 90
来源：http://ip.bjjhwx.cn

Bash ........... 80
来源：http://wz.colortex.cn

Kotlin ......... 15
来源：http://ga.yuntaijiaju.cn

Swift .......... 15
来源：http://ji.shxzukj.cn

Lua ............ 10
来源：http://sw.nszjky.cn

Perl ........... 10
来源：http://eu.shxzskj.cn

Scala .......... 10
来源：http://jp.huanxung.cn

------------------------------------
来源：http://xq.nicolike.cn

合计 ........... 2106 条
来源：http://oe.hnjuh.cn

按章节统计：
来源：http://uj.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jj.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tj.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gr.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ne.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qd.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rs.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tk.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cs.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nl.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kd.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xg.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kb.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://we.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vm.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hh.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vh.9csxet.cn

Q SQL 专题                              90
来源：http://il.521024.cn

R Bash 专题                             80
来源：http://gx.shxzskj.cn

S C / C++ 专题                          60
来源：http://xs.huanxung.cn

T 其他语言补充                          60
来源：http://lg.colortex.cn

U 高频实用片段                         120
来源：http://gi.haigaiapp.cn

------------------------------------
来源：http://qe.hnjuh.cn

合计                                  2106 条
来源：http://zs.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://xr.nszjky.cn

使用提醒
来源：http://pe.9csxet.cn

--------------------------------------------------------------------------------
来源：http://gh.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jy.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://no.haigaiapp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qz.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ha.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wp.panjiajie.cn

—— 文件结束 ——
来源：http://yh.hnjuh.cn

================================================================================
来源：http://qg.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://xh.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://vz.newstarts.cn

================================================================================
来源：http://rk.hnjuh.cn

【收录内容】
来源：http://mm.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://at.haigaiapp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pi.jctech888.com.cn

SQL · Bash · C · C++
来源：http://eu.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ft.szxytkj.cn

【使用说明】
来源：http://vz.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cl.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fz.huixinmuqiang.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rh.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oo.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gj.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vx.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jm.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yx.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zg.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bo.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ia.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yq.yuntaijiaju.cn

【文件统计】
来源：http://yt.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://re.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://hp.9csxet.cn

目  录
来源：http://gn.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://mo.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ix.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yo.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://to.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ed.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lz.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://no.nszjky.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qe.yuexingan06.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rj.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ew.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://km.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vi.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lu.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://at.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tz.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lh.521024.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mt.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ja.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fy.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sf.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fy.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fi.colortex.cn

================================================================================
来源：http://jk.jianghongdianzi.cn

A. 基础语法与类型
来源：http://np.hahajie.cn

================================================================================
来源：http://xc.muxihuayi.cn

[A01] Hello World
来源：http://wv.jianghongdianzi.cn

Py:   print("Hello, World!")
来源：http://fe.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://la.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://bh.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vm.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://il.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://wz.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://km.hahajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jx.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://as.muxihuayi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ec.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mc.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mt.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yn.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://ur.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://sy.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://dw.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cv.lnxyls.cn

[A03] 常量定义
来源：http://pj.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sy.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://zt.newstarts.cn

JS:   const PI = 3.14159;
来源：http://fv.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://dn.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://cr.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://qu.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://ty.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://po.jctech888.com.cn

[A04] 判断变量类型
来源：http://ux.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://km.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bz.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sv.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://ja.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hg.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ub.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tl.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://lz.shtwfgs.cn

[A05] 整数除法与取模
来源：http://fd.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kj.wgjwhj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wg.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dt.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sy.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://ji.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://nq.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://ff.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://ko.haigaiapp.cn

[A06] 字符串转数字
来源：http://qi.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://cd.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yn.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wr.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qi.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ff.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jb.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bw.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hm.asd995.cn

[A07] 数字转字符串
来源：http://ic.shxzskj.cn

Py:   str(42)
来源：http://yz.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://cz.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://og.yuntaijiaju.cn

TS:   String(42)
来源：http://ei.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hf.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://ic.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://ao.lnxyls.cn

C#:   42.ToString()
来源：http://qy.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://ln.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yh.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://so.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cf.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kk.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jq.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ns.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gq.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fv.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://fk.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://js.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ke.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vi.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hb.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ad.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dn.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vm.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uz.huixiangedu.cn

[A10] 生成随机数
来源：http://ck.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://wd.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://jn.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rg.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mq.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://vp.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://co.shtwfgs.cn

Ruby: rand(1..100)
来源：http://iu.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://oq.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://td.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://pt.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gx.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bj.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kh.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://jd.yuexingan06.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yb.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://np.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://su.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://ni.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fh.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://va.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://mb.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://sg.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://yf.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ss.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://vq.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://yd.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yo.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://kh.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://pa.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://ki.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://tj.hnjuh.cn

Java: "第一行\n第二行"
来源：http://ry.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://wm.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://cf.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://yr.panjiajie.cn

[A14] 注释写法
来源：http://qa.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ri.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vh.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://je.newstarts.cn


<!-- 参考信息 -->