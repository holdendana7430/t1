代发 wailian999

[U79] PHP：静态分析
来源：http://ro.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://vi.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://ud.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mj.szxytkj.cn

[U81] JS：初始化项目
来源：http://pz.haigaiapp.cn

npm init -y;  npm i express
来源：http://dy.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://vq.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qn.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://pl.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tn.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://xy.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pu.asd995.cn

[U85] JS：可选链
来源：http://py.muxihuayi.cn

a?.b?.c
来源：http://uq.panjiajie.cn

[U86] JS：空值合并
来源：http://ud.shxzukj.cn

a ?? b
来源：http://io.muxihuayi.cn

[U87] JS：解构默认值
来源：http://nl.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://qt.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://dy.nicolike.cn

{ ...a, ...b }
来源：http://iq.hnjuh.cn

[U89] JS：数组去重
来源：http://qp.asd995.cn

[...new Set(arr)]
来源：http://gh.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://xz.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://dv.9csxet.cn

[U91] JS：对象键值遍历
来源：http://de.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ot.hahajie.cn

[U92] JS：深拷贝
来源：http://vz.colortex.cn

structuredClone(obj)
来源：http://de.yuexingan06.cn

[U93] JS：模板字符串
来源：http://nf.nszjky.cn

`共 ${n} 条`
来源：http://yz.bjjhwx.cn

[U94] JS：箭头函数
来源：http://rm.gzmigu.cn

const double = x => x * 2;
来源：http://ve.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://sm.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://pl.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://sr.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wd.gzmigu.cn

[U97] JS：并发请求
来源：http://wz.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wx.9csxet.cn

[U98] JS：fetch 带 JSON
来源：http://em.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://km.asd995.cn

[U99] JS：事件监听
来源：http://tp.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://up.szxytkj.cn

[U100] JS：DOM 查询
来源：http://ec.shxzukj.cn

document.querySelector(".item")
来源：http://zq.bjjhwx.cn

[U101] JS：classList 操作
来源：http://jo.hahajie.cn

el.classList.toggle("active")
来源：http://mb.lnxyls.cn

[U102] JS：本地存储
来源：http://qd.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rj.jctech888.com.cn

[U103] JS：定时器
来源：http://er.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nq.szsharing.cn

[U104] JS：防抖
来源：http://lg.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vt.huanxung.cn

[U105] JS：节流
来源：http://sz.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://du.panjiajie.cn

[U106] JS：日期格式化
来源：http://hy.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cw.shtwfgs.cn

[U107] JS：数字千分位
来源：http://wa.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mj.521024.cn

[U108] JS：随机整数
来源：http://mv.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eu.shtwfgs.cn

[U109] JS：数组分组
来源：http://xp.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://qg.521024.cn

[U110] JS：数组分块
来源：http://cg.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rw.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://kh.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://rc.szxytkj.cn

[U112] JS：字符串补位
来源：http://vb.shxzukj.cn

"7".padStart(3, "0")
来源：http://qk.hahajie.cn

[U113] JS：正则替换全部
来源：http://az.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://dg.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://uy.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hs.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://zt.huixiangedu.cn

crypto.randomUUID()
来源：http://mc.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://dc.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://ps.bjjhwx.cn

[U117] JS：单元测试
来源：http://cy.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://rp.szxytkj.cn

[U118] JS：开发服务器
来源：http://pm.huixinmuqiang.cn

npm i -D vite;  npx vite
来源：http://ql.haigaiapp.cn

[U119] JS：生产构建
来源：http://wz.521024.cn

npx vite build
来源：http://va.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://yf.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://wz.bookmarksfly.cn

================================================================================
来源：http://ft.szsharing.cn

统计汇总
来源：http://kf.wgjwhj.cn

================================================================================
来源：http://vq.lnxyls.cn

按语言统计（条）：
来源：http://jy.bookmarksfly.cn

Python ......... 252
来源：http://xk.jctech888.com.cn

PHP ............ 252
来源：http://jb.gzmigu.cn

JavaScript ..... 252
来源：http://hu.haigaiapp.cn

TypeScript ..... 212
来源：http://wu.huanxung.cn

Java ........... 212
来源：http://zz.shxzukj.cn

Go ............. 212
来源：http://ry.nicolike.cn

Ruby ........... 212
来源：http://cz.hahajie.cn

C# ............. 212
来源：http://wx.bookmarksfly.cn

C .............. 30
来源：http://jm.yuntaijiaju.cn

C++ ............ 30
来源：http://md.hahajie.cn

SQL ............ 90
来源：http://qi.newstarts.cn

Bash ........... 80
来源：http://ty.huanxung.cn

Kotlin ......... 15
来源：http://wx.shxzukj.cn

Swift .......... 15
来源：http://rs.jianghongdianzi.cn

Lua ............ 10
来源：http://vf.hnjuh.cn

Perl ........... 10
来源：http://vu.huixiangedu.cn

Scala .......... 10
来源：http://ni.bjjhwx.cn

------------------------------------
来源：http://yx.gzmigu.cn

合计 ........... 2106 条
来源：http://jo.huanxung.cn

按章节统计：
来源：http://yn.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dc.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://or.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ic.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sg.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tv.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://un.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qn.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cr.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uw.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wy.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bg.nicolike.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hc.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sc.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lz.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ce.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pc.bookmarksfly.cn

Q SQL 专题                              90
来源：http://pw.nszjky.cn

R Bash 专题                             80
来源：http://nv.newstarts.cn

S C / C++ 专题                          60
来源：http://bi.huixiangedu.cn

T 其他语言补充                          60
来源：http://kl.chemitech.net.cn

U 高频实用片段                         120
来源：http://sq.haigaiapp.cn

------------------------------------
来源：http://te.huixiangedu.cn

合计                                  2106 条
来源：http://oc.asd995.cn

--------------------------------------------------------------------------------
来源：http://zr.shtwfgs.cn

使用提醒
来源：http://yi.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://ed.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cl.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mi.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tu.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ty.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bj.shxzskj.cn

—— 文件结束 ——
来源：http://hl.muxihuayi.cn

================================================================================
来源：http://pc.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://uj.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://bl.huanxung.cn

================================================================================
来源：http://bw.bjjhwx.cn

【收录内容】
来源：http://nz.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vn.wgjwhj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dq.521024.cn

SQL · Bash · C · C++
来源：http://go.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gm.szsharing.cn

【使用说明】
来源：http://wu.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xc.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zj.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qe.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lu.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ye.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dg.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cq.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vh.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fw.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vr.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nj.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yv.nszjky.cn

【文件统计】
来源：http://li.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ni.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://wm.huanxung.cn

目  录
来源：http://gn.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ly.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sp.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://to.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://su.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ck.asd995.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ku.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rs.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://up.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dj.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ok.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hh.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ip.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ds.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mo.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mx.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yf.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vc.bjjhwx.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yb.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pj.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://op.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qp.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.asd995.cn

================================================================================
来源：http://ym.521024.cn

A. 基础语法与类型
来源：http://tr.szxytkj.cn

================================================================================
来源：http://ye.9csxet.cn

[A01] Hello World
来源：http://kk.gzmigu.cn

Py:   print("Hello, World!")
来源：http://gl.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://np.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://ph.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gz.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://gs.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://yk.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://xn.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ln.nicolike.cn

[A02] 变量声明与赋值
来源：http://hh.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gp.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cl.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bn.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ul.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://so.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://ts.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://dq.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hx.lnxyls.cn

[A03] 常量定义
来源：http://ha.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ct.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://tv.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://ck.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://ov.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://kc.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://fo.jctech888.com.cn

Ruby: PI = 3.14159
来源：http://im.asd995.cn

C#:   const double PI = 3.14159;
来源：http://jm.huixiangedu.cn

[A04] 判断变量类型
来源：http://zj.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mx.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jo.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yc.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://sc.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://of.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jv.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qs.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://yw.9csxet.cn

[A05] 整数除法与取模
来源：http://mm.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bt.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vn.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ah.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ff.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://fz.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://kh.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://vx.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://xb.bookmarksfly.cn

[A06] 字符串转数字
来源：http://wb.521024.cn

Py:   int("42"); float("3.14")
来源：http://te.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zp.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cw.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bm.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dy.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ym.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yf.jianghongdianzi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yx.jctech888.com.cn

[A07] 数字转字符串
来源：http://xg.chemitech.net.cn

Py:   str(42)
来源：http://ak.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://wi.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://le.huixinmuqiang.cn

TS:   String(42)
来源：http://vx.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fw.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://qy.wgjwhj.cn

Ruby: 42.to_s
来源：http://xe.jianghongdianzi.cn

C#:   42.ToString()
来源：http://qb.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://if.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mx.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qx.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ik.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xv.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zx.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://er.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xi.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ui.asd995.cn

[A09] 绝对值与最大最小值
来源：http://zr.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pa.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nj.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tg.haigaiapp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zy.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cf.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kj.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ns.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qz.shxzskj.cn

[A10] 生成随机数
来源：http://tv.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://hq.asd995.cn

PHP:  random_int(1, 100);
来源：http://bu.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mt.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wn.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://fs.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uy.haigaiapp.cn

Ruby: rand(1..100)
来源：http://eq.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://nt.asd995.cn

[A11] 条件表达式（三元）
来源：http://ib.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://ek.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yx.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hw.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fx.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://pw.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rv.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ir.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://aq.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://gk.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sl.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cd.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://te.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://ka.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://ao.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ph.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://wh.colortex.cn

C#:   $"Hello, {name}!"
来源：http://gg.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mu.szxytkj.cn


<!-- 参考信息 -->