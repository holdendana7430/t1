代发 wailian999

[U81] JS：初始化项目
来源：http://tm.nicolike.cn

npm init -y;  npm i express
来源：http://je.521024.cn

[U82] JS：package.json 脚本
来源：http://gg.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://po.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://hx.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ht.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://nf.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lh.521024.cn

[U85] JS：可选链
来源：http://jf.szsharing.cn

a?.b?.c
来源：http://xu.hnjuh.cn

[U86] JS：空值合并
来源：http://xf.lnxyls.cn

a ?? b
来源：http://pn.chemitech.net.cn

[U87] JS：解构默认值
来源：http://kv.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://sn.hahajie.cn

[U88] JS：对象展开合并
来源：http://ny.yuexingan06.cn

{ ...a, ...b }
来源：http://tn.newstarts.cn

[U89] JS：数组去重
来源：http://gw.shtwfgs.cn

[...new Set(arr)]
来源：http://aj.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://kl.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://to.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://ot.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ym.asd995.cn

[U92] JS：深拷贝
来源：http://su.newstarts.cn

structuredClone(obj)
来源：http://ye.lnxyls.cn

[U93] JS：模板字符串
来源：http://de.nszjky.cn

`共 ${n} 条`
来源：http://oc.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://di.bjjhwx.cn

const double = x => x * 2;
来源：http://vv.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://bt.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://hk.nszjky.cn

[U96] JS：async/await 与异常
来源：http://jj.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sl.szxytkj.cn

[U97] JS：并发请求
来源：http://lk.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lx.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://ih.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lc.panjiajie.cn

[U99] JS：事件监听
来源：http://gq.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://mk.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://aa.colortex.cn

document.querySelector(".item")
来源：http://cx.haigaiapp.cn

[U101] JS：classList 操作
来源：http://jt.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://dx.szsharing.cn

[U102] JS：本地存储
来源：http://al.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://np.shxzukj.cn

[U103] JS：定时器
来源：http://nr.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kf.nicolike.cn

[U104] JS：防抖
来源：http://st.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fr.jctech888.com.cn

[U105] JS：节流
来源：http://yj.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jq.wgjwhj.cn

[U106] JS：日期格式化
来源：http://mp.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uj.asd995.cn

[U107] JS：数字千分位
来源：http://gt.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ej.szsharing.cn

[U108] JS：随机整数
来源：http://xt.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jb.521024.cn

[U109] JS：数组分组
来源：http://ks.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://eb.bjjhwx.cn

[U110] JS：数组分块
来源：http://tw.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ue.lnxyls.cn

[U111] JS：对象转 Map
来源：http://az.shxzukj.cn

new Map(Object.entries(obj))
来源：http://jx.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://vh.jctech888.com.cn

"7".padStart(3, "0")
来源：http://sv.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://xk.nszjky.cn

s.replaceAll("a", "b")
来源：http://et.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://rz.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://po.panjiajie.cn

[U115] JS：生成 UUID
来源：http://vj.asd995.cn

crypto.randomUUID()
来源：http://dr.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://be.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://vd.nszjky.cn

[U117] JS：单元测试
来源：http://hd.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://cs.gzmigu.cn

[U118] JS：开发服务器
来源：http://hv.hnjuh.cn

npm i -D vite;  npx vite
来源：http://lm.szsharing.cn

[U119] JS：生产构建
来源：http://ne.huixinmuqiang.cn

npx vite build
来源：http://jz.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://uo.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://rx.jctech888.com.cn

================================================================================
来源：http://kf.muxihuayi.cn

统计汇总
来源：http://nv.shxzukj.cn

================================================================================
来源：http://gm.hnjuh.cn

按语言统计（条）：
来源：http://rv.shtwfgs.cn

Python ......... 252
来源：http://dl.nicolike.cn

PHP ............ 252
来源：http://lc.wgjwhj.cn

JavaScript ..... 252
来源：http://ny.wgjwhj.cn

TypeScript ..... 212
来源：http://no.jianghongdianzi.cn

Java ........... 212
来源：http://kn.huixinmuqiang.cn

Go ............. 212
来源：http://qk.9csxet.cn

Ruby ........... 212
来源：http://jx.haigaiapp.cn

C# ............. 212
来源：http://vm.wgjwhj.cn

C .............. 30
来源：http://ys.shxzskj.cn

C++ ............ 30
来源：http://dg.nszjky.cn

SQL ............ 90
来源：http://hu.hahajie.cn

Bash ........... 80
来源：http://xa.colortex.cn

Kotlin ......... 15
来源：http://lf.gzmigu.cn

Swift .......... 15
来源：http://ro.lnxyls.cn

Lua ............ 10
来源：http://vd.jianghongdianzi.cn

Perl ........... 10
来源：http://lt.521024.cn

Scala .......... 10
来源：http://vu.521024.cn

------------------------------------
来源：http://rz.nicolike.cn

合计 ........... 2106 条
来源：http://jx.muxihuayi.cn

按章节统计：
来源：http://ho.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jd.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://au.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xo.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lx.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ac.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ig.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uc.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fi.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://se.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://if.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ky.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mx.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uz.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xu.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ei.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://si.wgjwhj.cn

Q SQL 专题                              90
来源：http://hm.wgjwhj.cn

R Bash 专题                             80
来源：http://ef.colortex.cn

S C / C++ 专题                          60
来源：http://bt.colortex.cn

T 其他语言补充                          60
来源：http://kd.nicolike.cn

U 高频实用片段                         120
来源：http://sb.hahajie.cn

------------------------------------
来源：http://lp.muxihuayi.cn

合计                                  2106 条
来源：http://zx.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ek.shxzukj.cn

使用提醒
来源：http://va.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://sy.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hv.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ud.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vk.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fa.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pm.haigaiapp.cn

—— 文件结束 ——
来源：http://as.muxihuayi.cn

================================================================================
来源：http://jg.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://tg.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://ul.hahajie.cn

================================================================================
来源：http://kg.yuntaijiaju.cn

【收录内容】
来源：http://bk.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bq.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ip.shxzskj.cn

SQL · Bash · C · C++
来源：http://xc.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ck.szxytkj.cn

【使用说明】
来源：http://na.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yn.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jy.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xr.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gk.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sd.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://si.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pi.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lk.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://el.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://te.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ir.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qi.huixinmuqiang.cn

【文件统计】
来源：http://fc.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://av.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://ee.asd995.cn

目  录
来源：http://dh.szsharing.cn

--------------------------------------------------------------------------------
来源：http://es.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nb.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xl.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://al.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wg.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tn.huanxung.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xg.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tb.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lr.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ob.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jf.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fy.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cg.yuntaijiaju.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wq.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hb.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fa.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://do.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gk.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qu.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dy.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ov.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ox.nszjky.cn

================================================================================
来源：http://kf.huanxung.cn

A. 基础语法与类型
来源：http://bf.yuntaijiaju.cn

================================================================================
来源：http://dc.huixinmuqiang.cn

[A01] Hello World
来源：http://pz.521024.cn

Py:   print("Hello, World!")
来源：http://ex.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://fy.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://le.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bl.521024.cn

Java: System.out.println("Hello, World!");
来源：http://ix.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://mo.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://gk.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xs.asd995.cn

[A02] 变量声明与赋值
来源：http://he.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tx.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mb.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ai.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pj.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://iz.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://ip.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://uf.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yw.asd995.cn

[A03] 常量定义
来源：http://az.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uh.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://fc.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://jv.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://tn.521024.cn

Java: static final double PI = 3.14159;
来源：http://sq.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://hr.newstarts.cn

Ruby: PI = 3.14159
来源：http://js.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://az.nszjky.cn

[A04] 判断变量类型
来源：http://wc.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hw.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://um.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ie.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://uj.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bz.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fs.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://io.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://pt.chemitech.net.cn

[A05] 整数除法与取模
来源：http://bl.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pn.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qn.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ub.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nw.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://qy.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://zr.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://ul.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://ov.bjjhwx.cn

[A06] 字符串转数字
来源：http://oy.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://xh.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fs.panjiajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://km.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pi.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ka.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bw.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hi.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gj.panjiajie.cn

[A07] 数字转字符串
来源：http://vo.huixiangedu.cn

Py:   str(42)
来源：http://wt.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://bl.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://ie.521024.cn

TS:   String(42)
来源：http://jr.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ax.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://sf.panjiajie.cn

Ruby: 42.to_s
来源：http://cp.gzmigu.cn

C#:   42.ToString()
来源：http://vs.hahajie.cn

[A08] 取整与四舍五入
来源：http://pn.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hv.hnjuh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qi.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xc.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zv.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ay.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tt.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fz.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://an.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://mj.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jc.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zk.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qq.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ck.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://il.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://im.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nt.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cr.wgjwhj.cn

[A10] 生成随机数
来源：http://zo.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://ba.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://st.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jv.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ss.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://iv.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wr.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://qn.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://de.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://qd.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://lo.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mf.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://am.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kh.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://yf.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jh.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nt.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fc.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://mo.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ch.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nd.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://oq.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://ky.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://ia.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://if.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://cx.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://mq.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jh.asd995.cn

Py:   "第一行\n第二行"
来源：http://tb.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://tf.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://tx.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://sw.haigaiapp.cn


<!-- 参考信息 -->