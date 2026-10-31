代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://df.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://al.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://tq.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ek.szxytkj.cn

[U85] JS：可选链
来源：http://oc.hnjuh.cn

a?.b?.c
来源：http://ru.nszjky.cn

[U86] JS：空值合并
来源：http://pz.szsharing.cn

a ?? b
来源：http://wy.bjjhwx.cn

[U87] JS：解构默认值
来源：http://pk.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://at.panjiajie.cn

[U88] JS：对象展开合并
来源：http://dl.newstarts.cn

{ ...a, ...b }
来源：http://oi.bjjhwx.cn

[U89] JS：数组去重
来源：http://ma.huanxung.cn

[...new Set(arr)]
来源：http://xz.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://rc.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://kt.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://oh.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yq.asd995.cn

[U92] JS：深拷贝
来源：http://fr.szxytkj.cn

structuredClone(obj)
来源：http://ie.chemitech.net.cn

[U93] JS：模板字符串
来源：http://xt.521024.cn

`共 ${n} 条`
来源：http://sq.hnjuh.cn

[U94] JS：箭头函数
来源：http://sv.asd995.cn

const double = x => x * 2;
来源：http://ei.lnxyls.cn

[U95] JS：Promise 包装
来源：http://pz.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://fg.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://qe.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oj.huixiangedu.cn

[U97] JS：并发请求
来源：http://pa.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vx.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://re.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yb.lnxyls.cn

[U99] JS：事件监听
来源：http://fu.colortex.cn

el.addEventListener("click", e => {})
来源：http://xc.newstarts.cn

[U100] JS：DOM 查询
来源：http://rn.nszjky.cn

document.querySelector(".item")
来源：http://ma.lnxyls.cn

[U101] JS：classList 操作
来源：http://rf.asd995.cn

el.classList.toggle("active")
来源：http://mo.haigaiapp.cn

[U102] JS：本地存储
来源：http://qb.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://iy.haigaiapp.cn

[U103] JS：定时器
来源：http://ih.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vi.lnxyls.cn

[U104] JS：防抖
来源：http://zq.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ji.wgjwhj.cn

[U105] JS：节流
来源：http://qb.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mj.9csxet.cn

[U106] JS：日期格式化
来源：http://cn.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ow.shxzukj.cn

[U107] JS：数字千分位
来源：http://tz.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tv.huixiangedu.cn

[U108] JS：随机整数
来源：http://tk.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tc.colortex.cn

[U109] JS：数组分组
来源：http://ft.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://qo.gzmigu.cn

[U110] JS：数组分块
来源：http://no.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rc.lnxyls.cn

[U111] JS：对象转 Map
来源：http://vn.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://tv.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://hw.chemitech.net.cn

"7".padStart(3, "0")
来源：http://gy.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://cu.gzmigu.cn

s.replaceAll("a", "b")
来源：http://kv.hahajie.cn

[U114] JS：JSON 深比较
来源：http://xd.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nk.huanxung.cn

[U115] JS：生成 UUID
来源：http://my.huixiangedu.cn

crypto.randomUUID()
来源：http://bn.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://os.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://vh.jctech888.com.cn

[U117] JS：单元测试
来源：http://yp.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://vb.hahajie.cn

[U118] JS：开发服务器
来源：http://uo.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://kh.lnxyls.cn

[U119] JS：生产构建
来源：http://ud.yuntaijiaju.cn

npx vite build
来源：http://ze.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://bn.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://ci.9csxet.cn

================================================================================
来源：http://hm.bookmarksfly.cn

统计汇总
来源：http://ey.jctech888.com.cn

================================================================================
来源：http://pc.yuexingan06.cn

按语言统计（条）：
来源：http://ye.nicolike.cn

Python ......... 252
来源：http://sz.chemitech.net.cn

PHP ............ 252
来源：http://cw.szxytkj.cn

JavaScript ..... 252
来源：http://nt.yuexingan06.cn

TypeScript ..... 212
来源：http://to.gzmigu.cn

Java ........... 212
来源：http://ip.shxzskj.cn

Go ............. 212
来源：http://vo.bookmarksfly.cn

Ruby ........... 212
来源：http://gt.jianghongdianzi.cn

C# ............. 212
来源：http://lq.panjiajie.cn

C .............. 30
来源：http://ha.haigaiapp.cn

C++ ............ 30
来源：http://wh.hahajie.cn

SQL ............ 90
来源：http://vb.huixinmuqiang.cn

Bash ........... 80
来源：http://uw.nicolike.cn

Kotlin ......... 15
来源：http://cj.shxzskj.cn

Swift .......... 15
来源：http://te.haigaiapp.cn

Lua ............ 10
来源：http://yj.huixiangedu.cn

Perl ........... 10
来源：http://pp.hnjuh.cn

Scala .......... 10
来源：http://zx.haigaiapp.cn

------------------------------------
来源：http://py.panjiajie.cn

合计 ........... 2106 条
来源：http://fl.521024.cn

按章节统计：
来源：http://tt.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://at.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nh.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eb.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yp.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dd.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lp.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oh.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ha.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mh.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qg.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://po.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bn.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://me.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aj.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://es.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ss.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://cl.shxzukj.cn

R Bash 专题                             80
来源：http://ct.muxihuayi.cn

S C / C++ 专题                          60
来源：http://jk.lnxyls.cn

T 其他语言补充                          60
来源：http://zz.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://yg.jctech888.com.cn

------------------------------------
来源：http://ad.nszjky.cn

合计                                  2106 条
来源：http://rl.asd995.cn

--------------------------------------------------------------------------------
来源：http://en.asd995.cn

使用提醒
来源：http://be.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://ac.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://il.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xu.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hh.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zb.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hc.asd995.cn

—— 文件结束 ——
来源：http://gl.hahajie.cn

================================================================================
来源：http://rh.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://qt.colortex.cn

Common Programming Examples Cheat Book
来源：http://an.shtwfgs.cn

================================================================================
来源：http://jx.gzmigu.cn

【收录内容】
来源：http://td.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mf.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://up.gzmigu.cn

SQL · Bash · C · C++
来源：http://tv.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tb.asd995.cn

【使用说明】
来源：http://qo.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rb.bookmarksfly.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tp.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rl.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rk.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qf.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bm.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yo.jianghongdianzi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zj.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://em.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qt.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qb.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nt.yuntaijiaju.cn

【文件统计】
来源：http://ad.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xz.colortex.cn

--------------------------------------------------------------------------------
来源：http://sd.yuexingan06.cn

目  录
来源：http://ib.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://wn.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ah.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gz.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ay.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://js.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://st.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gj.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eq.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rr.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wa.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yh.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ds.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sd.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ny.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gv.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wi.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pc.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://us.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uq.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bq.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pf.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uk.muxihuayi.cn

================================================================================
来源：http://pe.panjiajie.cn

A. 基础语法与类型
来源：http://gw.newstarts.cn

================================================================================
来源：http://bq.jctech888.com.cn

[A01] Hello World
来源：http://jx.asd995.cn

Py:   print("Hello, World!")
来源：http://vp.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://oc.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://ra.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nw.521024.cn

Java: System.out.println("Hello, World!");
来源：http://jj.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://on.asd995.cn

Ruby: puts "Hello, World!"
来源：http://sl.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wo.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://cw.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qo.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rr.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cl.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zw.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://hi.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://qf.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://vv.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yw.szxytkj.cn

[A03] 常量定义
来源：http://pc.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bj.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://pw.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://ct.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://cb.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://vw.szxytkj.cn

Go:   const PI = 3.14159
来源：http://mv.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://mq.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://ja.nszjky.cn

[A04] 判断变量类型
来源：http://vl.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ui.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ak.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mf.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://ta.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bs.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gi.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yk.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://ck.9csxet.cn

[A05] 整数除法与取模
来源：http://fa.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rv.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ja.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bg.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ko.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://zv.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://ll.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://zu.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://po.szsharing.cn

[A06] 字符串转数字
来源：http://if.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://rc.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uy.chemitech.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ew.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zl.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ca.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://da.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jj.szxytkj.cn

[A07] 数字转字符串
来源：http://sz.shxzukj.cn

Py:   str(42)
来源：http://as.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://fy.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://bj.szxytkj.cn

TS:   String(42)
来源：http://xg.huanxung.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xw.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://vp.bookmarksfly.cn

Ruby: 42.to_s
来源：http://pw.asd995.cn

C#:   42.ToString()
来源：http://pi.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://qm.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zx.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ri.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dg.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vt.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lr.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bp.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://db.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zt.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://uf.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lu.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bh.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mh.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fn.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://va.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pg.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ls.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ys.hnjuh.cn

[A10] 生成随机数
来源：http://qa.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://vk.hahajie.cn

PHP:  random_int(1, 100);
来源：http://iy.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jp.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kw.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://uh.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ec.colortex.cn

Ruby: rand(1..100)
来源：http://iy.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://xz.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://yw.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://tf.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rn.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wm.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nl.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://lg.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ru.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ol.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pa.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://nz.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vy.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bv.521024.cn

JS:   `Hello, ${name}!`
来源：http://lk.wgjwhj.cn

TS:   `Hello, ${name}!`
来源：http://hp.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://od.nszjky.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pt.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://oh.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://ce.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hm.521024.cn

Py:   "第一行\n第二行"
来源：http://zr.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://fl.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://nz.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://kt.colortex.cn

Java: "第一行\n第二行"
来源：http://mh.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://xd.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://dn.colortex.cn

C#:   "第一行\n第二行"
来源：http://qu.jianghongdianzi.cn


<!-- 参考信息 -->