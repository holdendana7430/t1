代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://ii.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dx.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://dq.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cu.huixinmuqiang.cn

[U85] JS：可选链
来源：http://vt.shtwfgs.cn

a?.b?.c
来源：http://tx.nicolike.cn

[U86] JS：空值合并
来源：http://rg.jianghongdianzi.cn

a ?? b
来源：http://sf.huixiangedu.cn

[U87] JS：解构默认值
来源：http://wy.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://rd.9csxet.cn

[U88] JS：对象展开合并
来源：http://jy.chemitech.net.cn

{ ...a, ...b }
来源：http://ki.huanxung.cn

[U89] JS：数组去重
来源：http://bi.nszjky.cn

[...new Set(arr)]
来源：http://mh.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://oo.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://fv.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://by.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tj.nicolike.cn

[U92] JS：深拷贝
来源：http://cn.nicolike.cn

structuredClone(obj)
来源：http://yz.asd995.cn

[U93] JS：模板字符串
来源：http://ps.chemitech.net.cn

`共 ${n} 条`
来源：http://ri.szsharing.cn

[U94] JS：箭头函数
来源：http://zb.panjiajie.cn

const double = x => x * 2;
来源：http://tf.gzmigu.cn

[U95] JS：Promise 包装
来源：http://by.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://tx.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://mi.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gf.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://ll.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bu.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://xm.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zf.shxzukj.cn

[U99] JS：事件监听
来源：http://qf.newstarts.cn

el.addEventListener("click", e => {})
来源：http://vk.nszjky.cn

[U100] JS：DOM 查询
来源：http://dx.521024.cn

document.querySelector(".item")
来源：http://dn.521024.cn

[U101] JS：classList 操作
来源：http://wm.chemitech.net.cn

el.classList.toggle("active")
来源：http://qy.bjjhwx.cn

[U102] JS：本地存储
来源：http://nt.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ub.chemitech.net.cn

[U103] JS：定时器
来源：http://hd.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ut.wgjwhj.cn

[U104] JS：防抖
来源：http://br.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ig.yuntaijiaju.cn

[U105] JS：节流
来源：http://ut.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fx.huanxung.cn

[U106] JS：日期格式化
来源：http://cz.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pn.9csxet.cn

[U107] JS：数字千分位
来源：http://ro.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oa.asd995.cn

[U108] JS：随机整数
来源：http://kr.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fn.nszjky.cn

[U109] JS：数组分组
来源：http://bz.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://ur.szxytkj.cn

[U110] JS：数组分块
来源：http://dz.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ll.lnxyls.cn

[U111] JS：对象转 Map
来源：http://fr.shxzskj.cn

new Map(Object.entries(obj))
来源：http://rg.panjiajie.cn

[U112] JS：字符串补位
来源：http://nk.asd995.cn

"7".padStart(3, "0")
来源：http://gd.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://kg.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://wa.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://na.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://iw.nicolike.cn

[U115] JS：生成 UUID
来源：http://lh.szxytkj.cn

crypto.randomUUID()
来源：http://ol.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://xj.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://hg.jctech888.com.cn

[U117] JS：单元测试
来源：http://zb.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://ww.muxihuayi.cn

[U118] JS：开发服务器
来源：http://kw.szxytkj.cn

npm i -D vite;  npx vite
来源：http://um.muxihuayi.cn

[U119] JS：生产构建
来源：http://hd.bookmarksfly.cn

npx vite build
来源：http://zu.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://pc.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://mu.hnjuh.cn

================================================================================
来源：http://gy.nszjky.cn

统计汇总
来源：http://lp.gzmigu.cn

================================================================================
来源：http://gp.jctech888.com.cn

按语言统计（条）：
来源：http://za.yuexingan06.cn

Python ......... 252
来源：http://ka.shxzukj.cn

PHP ............ 252
来源：http://de.hnjuh.cn

JavaScript ..... 252
来源：http://bl.szsharing.cn

TypeScript ..... 212
来源：http://rm.bookmarksfly.cn

Java ........... 212
来源：http://nx.nszjky.cn

Go ............. 212
来源：http://vo.yuntaijiaju.cn

Ruby ........... 212
来源：http://yj.hahajie.cn

C# ............. 212
来源：http://oo.521024.cn

C .............. 30
来源：http://wp.nicolike.cn

C++ ............ 30
来源：http://fd.wgjwhj.cn

SQL ............ 90
来源：http://by.huanxung.cn

Bash ........... 80
来源：http://fy.huixiangedu.cn

Kotlin ......... 15
来源：http://xt.yuntaijiaju.cn

Swift .......... 15
来源：http://yq.bookmarksfly.cn

Lua ............ 10
来源：http://ez.shxzukj.cn

Perl ........... 10
来源：http://vt.hnjuh.cn

Scala .......... 10
来源：http://hl.bjjhwx.cn

------------------------------------
来源：http://qu.huixiangedu.cn

合计 ........... 2106 条
来源：http://ye.yuntaijiaju.cn

按章节统计：
来源：http://ca.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uz.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://il.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fg.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wb.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tt.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qt.9csxet.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wt.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zn.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ze.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pn.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zk.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ep.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ce.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ml.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vu.shxzskj.cn

Q SQL 专题                              90
来源：http://lt.521024.cn

R Bash 专题                             80
来源：http://br.newstarts.cn

S C / C++ 专题                          60
来源：http://co.nicolike.cn

T 其他语言补充                          60
来源：http://oa.shxzukj.cn

U 高频实用片段                         120
来源：http://do.jctech888.com.cn

------------------------------------
来源：http://xd.hnjuh.cn

合计                                  2106 条
来源：http://ct.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://gj.shxzukj.cn

使用提醒
来源：http://pw.9csxet.cn

--------------------------------------------------------------------------------
来源：http://nb.shxzukj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nm.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hi.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dd.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ci.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rm.bjjhwx.cn

—— 文件结束 ——
来源：http://kv.shtwfgs.cn

================================================================================
来源：http://eq.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://dh.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://lf.huixinmuqiang.cn

================================================================================
来源：http://ol.colortex.cn

【收录内容】
来源：http://yo.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cz.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://he.muxihuayi.cn

SQL · Bash · C · C++
来源：http://bm.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cz.asd995.cn

【使用说明】
来源：http://pn.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vt.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yb.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ef.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://et.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jc.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dy.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fo.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tb.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uf.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xn.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wd.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jb.9csxet.cn

【文件统计】
来源：http://cp.hahajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zu.colortex.cn

--------------------------------------------------------------------------------
来源：http://qm.gzmigu.cn

目  录
来源：http://js.huanxung.cn

--------------------------------------------------------------------------------
来源：http://eo.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nq.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sq.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mf.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iq.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sd.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yz.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://os.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uj.yuexingan06.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tu.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xk.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ge.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zd.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lt.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eq.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xi.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fu.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://by.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dz.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://au.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zq.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ok.chemitech.net.cn

================================================================================
来源：http://pt.panjiajie.cn

A. 基础语法与类型
来源：http://ir.hnjuh.cn

================================================================================
来源：http://tn.521024.cn

[A01] Hello World
来源：http://lz.panjiajie.cn

Py:   print("Hello, World!")
来源：http://dg.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://vr.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://yj.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zc.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://ex.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://mt.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://vm.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://oi.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://lo.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cz.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pd.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fg.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jx.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://tq.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://uf.szsharing.cn

Ruby: name = "Alex"; age = 20
来源：http://fc.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://es.haigaiapp.cn

[A03] 常量定义
来源：http://ug.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nr.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://ra.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://ne.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://uw.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://om.hnjuh.cn

Go:   const PI = 3.14159
来源：http://wz.nszjky.cn

Ruby: PI = 3.14159
来源：http://kx.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://ga.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://ap.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yi.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://av.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://tf.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ol.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gi.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://ie.shtwfgs.cn

[A05] 整数除法与取模
来源：http://ps.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qa.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ul.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qn.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pi.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://gu.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://uw.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://ws.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://kv.szxytkj.cn

[A06] 字符串转数字
来源：http://pq.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://qt.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dd.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cl.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ko.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://it.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qy.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://da.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mj.newstarts.cn

[A07] 数字转字符串
来源：http://vg.huixinmuqiang.cn

Py:   str(42)
来源：http://dk.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://lh.hahajie.cn

JS:   String(42); (42).toString()
来源：http://qu.szsharing.cn

TS:   String(42)
来源：http://am.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kl.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://ap.panjiajie.cn

Ruby: 42.to_s
来源：http://yw.jianghongdianzi.cn

C#:   42.ToString()
来源：http://if.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://kx.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://re.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ex.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qx.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://db.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dy.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qe.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ni.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pg.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://af.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cy.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tu.nszjky.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xq.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nj.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nc.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lj.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://an.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cf.9csxet.cn

[A10] 生成随机数
来源：http://fq.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://ld.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://te.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lr.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kh.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://cg.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hf.shtwfgs.cn

Ruby: rand(1..100)
来源：http://ff.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://ow.asd995.cn

[A11] 条件表达式（三元）
来源：http://lt.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://to.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ji.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ts.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ie.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://pn.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jb.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pq.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gk.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://bz.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sn.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bg.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://ar.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://ix.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://ip.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ad.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://ql.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://rw.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fq.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://ww.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://to.asd995.cn

JS:   "第一行\n第二行"
来源：http://xb.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://tl.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://ax.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://ia.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://hz.521024.cn

C#:   "第一行\n第二行"
来源：http://lg.yuexingan06.cn


<!-- 参考信息 -->