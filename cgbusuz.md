代发 wailian999

[U77] PHP：模板渲染
来源：http://ed.colortex.cn

composer require twig/twig
来源：http://am.shtwfgs.cn

[U78] PHP：单元测试
来源：http://bq.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://ak.haigaiapp.cn

[U79] PHP：静态分析
来源：http://ho.colortex.cn

composer require --dev phpstan/phpstan
来源：http://dl.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://gx.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://al.wgjwhj.cn

[U81] JS：初始化项目
来源：http://al.shxzskj.cn

npm init -y;  npm i express
来源：http://py.521024.cn

[U82] JS：package.json 脚本
来源：http://ko.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xl.panjiajie.cn

[U83] JS：ES Module 导入导出
来源：http://tv.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lj.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://pr.newstarts.cn

module.exports = { a };  const { a } = require("./m");
来源：http://et.gzmigu.cn

[U85] JS：可选链
来源：http://io.gzmigu.cn

a?.b?.c
来源：http://iy.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://xs.asd995.cn

a ?? b
来源：http://vv.newstarts.cn

[U87] JS：解构默认值
来源：http://zb.muxihuayi.cn

const { a = 1, b = 2 } = obj;
来源：http://su.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://kd.gzmigu.cn

{ ...a, ...b }
来源：http://ku.shxzukj.cn

[U89] JS：数组去重
来源：http://to.huanxung.cn

[...new Set(arr)]
来源：http://jr.hahajie.cn

[U90] JS：数字数组排序
来源：http://tf.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://kc.huanxung.cn

[U91] JS：对象键值遍历
来源：http://db.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://si.521024.cn

[U92] JS：深拷贝
来源：http://za.bookmarksfly.cn

structuredClone(obj)
来源：http://pv.lnxyls.cn

[U93] JS：模板字符串
来源：http://bo.haigaiapp.cn

`共 ${n} 条`
来源：http://qw.szxytkj.cn

[U94] JS：箭头函数
来源：http://xp.newstarts.cn

const double = x => x * 2;
来源：http://hs.newstarts.cn

[U95] JS：Promise 包装
来源：http://nf.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://yi.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://eg.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hv.szxytkj.cn

[U97] JS：并发请求
来源：http://qi.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zz.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://fu.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://px.colortex.cn

[U99] JS：事件监听
来源：http://qw.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://yd.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://fm.shxzskj.cn

document.querySelector(".item")
来源：http://wg.muxihuayi.cn

[U101] JS：classList 操作
来源：http://ok.shxzukj.cn

el.classList.toggle("active")
来源：http://ym.lnxyls.cn

[U102] JS：本地存储
来源：http://ep.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rj.szsharing.cn

[U103] JS：定时器
来源：http://sf.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rk.yuntaijiaju.cn

[U104] JS：防抖
来源：http://qg.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://is.jctech888.com.cn

[U105] JS：节流
来源：http://ix.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mw.shtwfgs.cn

[U106] JS：日期格式化
来源：http://rw.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ga.hnjuh.cn

[U107] JS：数字千分位
来源：http://lq.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://we.yuexingan06.cn

[U108] JS：随机整数
来源：http://sj.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ft.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://qa.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://ov.panjiajie.cn

[U110] JS：数组分块
来源：http://eb.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://af.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://au.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://mr.hahajie.cn

[U112] JS：字符串补位
来源：http://bu.newstarts.cn

"7".padStart(3, "0")
来源：http://zi.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://kh.shxzskj.cn

s.replaceAll("a", "b")
来源：http://wm.hahajie.cn

[U114] JS：JSON 深比较
来源：http://zr.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nu.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://qc.huixiangedu.cn

crypto.randomUUID()
来源：http://wz.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://gh.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://le.newstarts.cn

[U117] JS：单元测试
来源：http://et.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://wb.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://eb.shxzukj.cn

npm i -D vite;  npx vite
来源：http://dk.szsharing.cn

[U119] JS：生产构建
来源：http://ui.9csxet.cn

npx vite build
来源：http://yw.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://wc.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://ct.bjjhwx.cn

================================================================================
来源：http://dq.bjjhwx.cn

统计汇总
来源：http://kb.gzmigu.cn

================================================================================
来源：http://ry.chemitech.net.cn

按语言统计（条）：
来源：http://qo.colortex.cn

Python ......... 252
来源：http://to.panjiajie.cn

PHP ............ 252
来源：http://yc.lnxyls.cn

JavaScript ..... 252
来源：http://pj.asd995.cn

TypeScript ..... 212
来源：http://ks.szxytkj.cn

Java ........... 212
来源：http://ag.nicolike.cn

Go ............. 212
来源：http://rx.huanxung.cn

Ruby ........... 212
来源：http://pl.yuexingan06.cn

C# ............. 212
来源：http://al.yuexingan06.cn

C .............. 30
来源：http://zg.huixiangedu.cn

C++ ............ 30
来源：http://pn.nicolike.cn

SQL ............ 90
来源：http://ae.hahajie.cn

Bash ........... 80
来源：http://vb.9csxet.cn

Kotlin ......... 15
来源：http://il.huixiangedu.cn

Swift .......... 15
来源：http://ud.szsharing.cn

Lua ............ 10
来源：http://fo.9csxet.cn

Perl ........... 10
来源：http://iu.shtwfgs.cn

Scala .......... 10
来源：http://pc.asd995.cn

------------------------------------
来源：http://li.szxytkj.cn

合计 ........... 2106 条
来源：http://sx.shxzskj.cn

按章节统计：
来源：http://qe.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lp.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gr.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ph.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dc.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gn.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tz.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gg.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uw.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hu.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dj.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kn.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uf.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xc.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kd.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kw.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ai.shtwfgs.cn

Q SQL 专题                              90
来源：http://zm.szsharing.cn

R Bash 专题                             80
来源：http://ja.jctech888.com.cn

S C / C++ 专题                          60
来源：http://wq.9csxet.cn

T 其他语言补充                          60
来源：http://gl.shxzskj.cn

U 高频实用片段                         120
来源：http://be.colortex.cn

------------------------------------
来源：http://mb.asd995.cn

合计                                  2106 条
来源：http://an.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://xr.yuntaijiaju.cn

使用提醒
来源：http://au.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://li.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xh.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tm.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tw.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sj.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oh.shtwfgs.cn

—— 文件结束 ——
来源：http://jy.huanxung.cn

================================================================================
来源：http://hx.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://ny.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://sh.szsharing.cn

================================================================================
来源：http://eu.huixinmuqiang.cn

【收录内容】
来源：http://ex.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://li.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://od.huixiangedu.cn

SQL · Bash · C · C++
来源：http://yw.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://et.nszjky.cn

【使用说明】
来源：http://xd.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nj.yuntaijiaju.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oi.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ph.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mr.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ud.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fy.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yf.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xn.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ks.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ca.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gy.bookmarksfly.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mn.hahajie.cn

【文件统计】
来源：http://om.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fd.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://wo.newstarts.cn

目  录
来源：http://za.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://cv.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mu.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hy.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://li.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wu.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sz.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lk.nszjky.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oe.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cw.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bx.szsharing.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nf.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ky.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ca.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oz.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xu.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nd.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zp.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vj.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ft.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fw.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uk.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://al.jctech888.com.cn

================================================================================
来源：http://tp.szsharing.cn

A. 基础语法与类型
来源：http://vy.huixinmuqiang.cn

================================================================================
来源：http://ud.shxzukj.cn

[A01] Hello World
来源：http://hj.hnjuh.cn

Py:   print("Hello, World!")
来源：http://ra.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://os.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://nl.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sj.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://wg.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://xj.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://tq.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cs.szxytkj.cn

[A02] 变量声明与赋值
来源：http://iy.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qm.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vm.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ez.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ek.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://dj.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://vt.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://um.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ub.nicolike.cn

[A03] 常量定义
来源：http://kj.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zk.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://tt.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://oc.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://hx.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://je.9csxet.cn

Go:   const PI = 3.14159
来源：http://by.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://kv.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://mu.hnjuh.cn

[A04] 判断变量类型
来源：http://mm.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://td.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rv.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ir.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://ai.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lu.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kq.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lg.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://wx.nszjky.cn

[A05] 整数除法与取模
来源：http://tb.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ke.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://is.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ii.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oq.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://ji.521024.cn

Go:   7 / 2; 7 % 2
来源：http://vt.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://fv.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://gj.nszjky.cn

[A06] 字符串转数字
来源：http://xi.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://wl.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ti.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://aa.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cl.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iz.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://en.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ur.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kx.nicolike.cn

[A07] 数字转字符串
来源：http://et.lnxyls.cn

Py:   str(42)
来源：http://es.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://fp.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://as.newstarts.cn

TS:   String(42)
来源：http://ye.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sr.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://pm.521024.cn

Ruby: 42.to_s
来源：http://rl.hnjuh.cn

C#:   42.ToString()
来源：http://ek.nicolike.cn

[A08] 取整与四舍五入
来源：http://qe.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qb.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nq.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wm.haigaiapp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yy.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ct.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ka.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://io.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pf.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://hp.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zh.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nh.lnxyls.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bq.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://am.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ff.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gx.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cy.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cd.lnxyls.cn

[A10] 生成随机数
来源：http://ej.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://ql.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://qa.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jf.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://iq.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://tv.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oy.muxihuayi.cn

Ruby: rand(1..100)
来源：http://yj.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://tt.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://so.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://fq.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ma.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ko.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ii.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://pd.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ou.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jq.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lu.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://bb.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ck.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fp.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://fr.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://ub.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://so.bookmarksfly.cn


<!-- 参考信息 -->