代发 wailian999

[U79] PHP：静态分析
来源：http://sl.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://fy.nicolike.cn

[U80] PHP：代码规范修复
来源：http://dw.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://np.haigaiapp.cn

[U81] JS：初始化项目
来源：http://qv.szxytkj.cn

npm init -y;  npm i express
来源：http://lr.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://cq.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oc.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://bf.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://io.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://my.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ds.shxzukj.cn

[U85] JS：可选链
来源：http://kc.hahajie.cn

a?.b?.c
来源：http://hr.hnjuh.cn

[U86] JS：空值合并
来源：http://tw.nszjky.cn

a ?? b
来源：http://rg.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://py.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://ni.szsharing.cn

[U88] JS：对象展开合并
来源：http://af.chemitech.net.cn

{ ...a, ...b }
来源：http://jj.521024.cn

[U89] JS：数组去重
来源：http://nf.panjiajie.cn

[...new Set(arr)]
来源：http://kj.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://yl.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://rt.nszjky.cn

[U91] JS：对象键值遍历
来源：http://qz.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://im.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://pd.huixiangedu.cn

structuredClone(obj)
来源：http://by.huixiangedu.cn

[U93] JS：模板字符串
来源：http://ad.shtwfgs.cn

`共 ${n} 条`
来源：http://ch.shxzukj.cn

[U94] JS：箭头函数
来源：http://fn.jianghongdianzi.cn

const double = x => x * 2;
来源：http://ik.szxytkj.cn

[U95] JS：Promise 包装
来源：http://ig.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://tb.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://my.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xf.nicolike.cn

[U97] JS：并发请求
来源：http://ox.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zf.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://ho.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://te.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://jh.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://kj.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://uw.jianghongdianzi.cn

document.querySelector(".item")
来源：http://qz.yuexingan06.cn

[U101] JS：classList 操作
来源：http://cj.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://oe.szsharing.cn

[U102] JS：本地存储
来源：http://oq.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bz.hnjuh.cn

[U103] JS：定时器
来源：http://ht.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ye.hnjuh.cn

[U104] JS：防抖
来源：http://th.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kz.huixinmuqiang.cn

[U105] JS：节流
来源：http://qf.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kr.gzmigu.cn

[U106] JS：日期格式化
来源：http://ih.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zw.hnjuh.cn

[U107] JS：数字千分位
来源：http://fc.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xe.bookmarksfly.cn

[U108] JS：随机整数
来源：http://js.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ae.bookmarksfly.cn

[U109] JS：数组分组
来源：http://ln.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://yv.jctech888.com.cn

[U110] JS：数组分块
来源：http://tv.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tv.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://vk.newstarts.cn

new Map(Object.entries(obj))
来源：http://bo.shxzukj.cn

[U112] JS：字符串补位
来源：http://ky.szsharing.cn

"7".padStart(3, "0")
来源：http://ik.9csxet.cn

[U113] JS：正则替换全部
来源：http://qg.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://pv.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://xx.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wl.lnxyls.cn

[U115] JS：生成 UUID
来源：http://eu.shxzskj.cn

crypto.randomUUID()
来源：http://gc.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://pw.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://lw.bookmarksfly.cn

[U117] JS：单元测试
来源：http://mz.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://cm.hnjuh.cn

[U118] JS：开发服务器
来源：http://hx.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://ly.shxzukj.cn

[U119] JS：生产构建
来源：http://ry.nicolike.cn

npx vite build
来源：http://vn.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://bz.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://ws.gzmigu.cn

================================================================================
来源：http://at.huixiangedu.cn

统计汇总
来源：http://st.chemitech.net.cn

================================================================================
来源：http://kz.huixiangedu.cn

按语言统计（条）：
来源：http://hq.colortex.cn

Python ......... 252
来源：http://ep.haigaiapp.cn

PHP ............ 252
来源：http://qu.nszjky.cn

JavaScript ..... 252
来源：http://cr.wgjwhj.cn

TypeScript ..... 212
来源：http://ff.nszjky.cn

Java ........... 212
来源：http://zy.newstarts.cn

Go ............. 212
来源：http://ce.szxytkj.cn

Ruby ........... 212
来源：http://di.szsharing.cn

C# ............. 212
来源：http://va.bjjhwx.cn

C .............. 30
来源：http://ut.bookmarksfly.cn

C++ ............ 30
来源：http://jf.bjjhwx.cn

SQL ............ 90
来源：http://dz.newstarts.cn

Bash ........... 80
来源：http://iy.shtwfgs.cn

Kotlin ......... 15
来源：http://bd.chemitech.net.cn

Swift .......... 15
来源：http://gy.nicolike.cn

Lua ............ 10
来源：http://ck.bookmarksfly.cn

Perl ........... 10
来源：http://qy.yuexingan06.cn

Scala .......... 10
来源：http://wt.haigaiapp.cn

------------------------------------
来源：http://zv.bjjhwx.cn

合计 ........... 2106 条
来源：http://ys.szxytkj.cn

按章节统计：
来源：http://de.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ej.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://me.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hm.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ks.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ou.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xv.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ux.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nt.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tc.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mu.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tk.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fk.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rl.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rd.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fi.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ww.newstarts.cn

Q SQL 专题                              90
来源：http://mt.chemitech.net.cn

R Bash 专题                             80
来源：http://eu.szxytkj.cn

S C / C++ 专题                          60
来源：http://nj.hnjuh.cn

T 其他语言补充                          60
来源：http://sb.hnjuh.cn

U 高频实用片段                         120
来源：http://jz.jctech888.com.cn

------------------------------------
来源：http://cf.panjiajie.cn

合计                                  2106 条
来源：http://nl.colortex.cn

--------------------------------------------------------------------------------
来源：http://tu.hnjuh.cn

使用提醒
来源：http://ku.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://db.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://su.jctech888.com.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mq.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lb.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sl.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ri.asd995.cn

—— 文件结束 ——
来源：http://vk.bookmarksfly.cn

================================================================================
来源：http://tx.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://is.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://ar.szxytkj.cn

================================================================================
来源：http://lb.jianghongdianzi.cn

【收录内容】
来源：http://et.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gb.wgjwhj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fx.asd995.cn

SQL · Bash · C · C++
来源：http://jn.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oc.hnjuh.cn

【使用说明】
来源：http://he.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ev.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vt.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dz.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zg.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lk.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ua.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ls.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://os.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cw.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qd.nszjky.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uk.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mw.muxihuayi.cn

【文件统计】
来源：http://os.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dj.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://cj.521024.cn

目  录
来源：http://ny.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ph.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://az.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rv.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vv.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rg.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rj.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pv.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xj.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nm.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ja.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dl.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wd.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ij.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xy.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ex.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hf.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qi.panjiajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lv.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hu.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wo.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bf.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ew.szsharing.cn

================================================================================
来源：http://jo.asd995.cn

A. 基础语法与类型
来源：http://gu.asd995.cn

================================================================================
来源：http://fa.shxzskj.cn

[A01] Hello World
来源：http://oc.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://cu.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://qa.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://ax.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pi.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://hy.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://vu.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://tt.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xm.lnxyls.cn

[A02] 变量声明与赋值
来源：http://ew.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://re.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ll.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cp.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ff.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://la.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://vy.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://xk.wgjwhj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cr.bookmarksfly.cn

[A03] 常量定义
来源：http://eq.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sw.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://ka.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://id.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://kr.colortex.cn

Java: static final double PI = 3.14159;
来源：http://up.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://gh.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://em.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://uh.9csxet.cn

[A04] 判断变量类型
来源：http://ll.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qk.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lc.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lz.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://xh.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://is.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ns.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dm.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://zs.9csxet.cn

[A05] 整数除法与取模
来源：http://yg.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://aw.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tw.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fu.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nq.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://ok.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://wn.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://yl.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://ww.hahajie.cn

[A06] 字符串转数字
来源：http://fs.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://te.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vw.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kt.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xw.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nl.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rw.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wa.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://su.huanxung.cn

[A07] 数字转字符串
来源：http://rx.jctech888.com.cn

Py:   str(42)
来源：http://fn.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://gr.hahajie.cn

JS:   String(42); (42).toString()
来源：http://ua.bookmarksfly.cn

TS:   String(42)
来源：http://zo.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ix.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://kv.szsharing.cn

Ruby: 42.to_s
来源：http://lq.nszjky.cn

C#:   42.ToString()
来源：http://en.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://gv.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ii.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cy.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bj.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gj.lnxyls.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gs.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vm.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sw.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wn.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://mc.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://of.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dv.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jc.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kh.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sh.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jp.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://po.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mz.haigaiapp.cn

[A10] 生成随机数
来源：http://pq.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://fg.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://za.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fg.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nu.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://lf.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sa.gzmigu.cn

Ruby: rand(1..100)
来源：http://ek.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://ca.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://gj.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://cg.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bk.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lt.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ol.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://lu.nicolike.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://co.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gr.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yf.szsharing.cn

[A12] 字符串插值 / 格式化
来源：http://uh.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kf.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sj.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://dn.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://yh.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://ik.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dh.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://gf.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://aj.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bd.nicolike.cn


<!-- 参考信息 -->