代发 wailian999

[U77] PHP：模板渲染
来源：http://pc.szsharing.cn

composer require twig/twig
来源：http://hd.9csxet.cn

[U78] PHP：单元测试
来源：http://rp.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://vb.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://xs.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://qf.nicolike.cn

[U80] PHP：代码规范修复
来源：http://ls.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tg.bjjhwx.cn

[U81] JS：初始化项目
来源：http://pf.gzmigu.cn

npm init -y;  npm i express
来源：http://dg.hahajie.cn

[U82] JS：package.json 脚本
来源：http://vq.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uo.asd995.cn

[U83] JS：ES Module 导入导出
来源：http://jx.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://as.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://gl.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://il.yuntaijiaju.cn

[U85] JS：可选链
来源：http://tz.huanxung.cn

a?.b?.c
来源：http://pc.gzmigu.cn

[U86] JS：空值合并
来源：http://fy.shxzukj.cn

a ?? b
来源：http://at.huanxung.cn

[U87] JS：解构默认值
来源：http://io.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://gq.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://fk.szxytkj.cn

{ ...a, ...b }
来源：http://kc.bookmarksfly.cn

[U89] JS：数组去重
来源：http://pf.jianghongdianzi.cn

[...new Set(arr)]
来源：http://rb.nicolike.cn

[U90] JS：数字数组排序
来源：http://nb.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://fu.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://fn.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xq.asd995.cn

[U92] JS：深拷贝
来源：http://cy.jianghongdianzi.cn

structuredClone(obj)
来源：http://gq.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://cf.colortex.cn

`共 ${n} 条`
来源：http://lm.colortex.cn

[U94] JS：箭头函数
来源：http://yl.huixinmuqiang.cn

const double = x => x * 2;
来源：http://cu.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://wa.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://hd.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://ex.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jp.szxytkj.cn

[U97] JS：并发请求
来源：http://su.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oy.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://iv.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qj.shxzskj.cn

[U99] JS：事件监听
来源：http://tz.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://qq.panjiajie.cn

[U100] JS：DOM 查询
来源：http://oj.bookmarksfly.cn

document.querySelector(".item")
来源：http://vg.nicolike.cn

[U101] JS：classList 操作
来源：http://gf.jctech888.com.cn

el.classList.toggle("active")
来源：http://fu.nszjky.cn

[U102] JS：本地存储
来源：http://ey.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sa.szxytkj.cn

[U103] JS：定时器
来源：http://ue.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lz.jianghongdianzi.cn

[U104] JS：防抖
来源：http://nn.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xv.wgjwhj.cn

[U105] JS：节流
来源：http://kd.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wz.yuexingan06.cn

[U106] JS：日期格式化
来源：http://ka.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ug.hnjuh.cn

[U107] JS：数字千分位
来源：http://bn.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jq.lnxyls.cn

[U108] JS：随机整数
来源：http://ra.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://in.panjiajie.cn

[U109] JS：数组分组
来源：http://mg.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://os.hahajie.cn

[U110] JS：数组分块
来源：http://ap.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xg.lnxyls.cn

[U111] JS：对象转 Map
来源：http://ts.shxzskj.cn

new Map(Object.entries(obj))
来源：http://vl.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://mw.shxzskj.cn

"7".padStart(3, "0")
来源：http://lg.nszjky.cn

[U113] JS：正则替换全部
来源：http://jt.szsharing.cn

s.replaceAll("a", "b")
来源：http://io.asd995.cn

[U114] JS：JSON 深比较
来源：http://lb.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gl.nszjky.cn

[U115] JS：生成 UUID
来源：http://ez.jctech888.com.cn

crypto.randomUUID()
来源：http://dv.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://pw.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://ja.9csxet.cn

[U117] JS：单元测试
来源：http://rg.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://ay.nicolike.cn

[U118] JS：开发服务器
来源：http://gg.hahajie.cn

npm i -D vite;  npx vite
来源：http://zu.shtwfgs.cn

[U119] JS：生产构建
来源：http://rw.shxzskj.cn

npx vite build
来源：http://pk.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://oz.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://bd.shtwfgs.cn

================================================================================
来源：http://iu.hnjuh.cn

统计汇总
来源：http://wn.bjjhwx.cn

================================================================================
来源：http://uv.nicolike.cn

按语言统计（条）：
来源：http://df.muxihuayi.cn

Python ......... 252
来源：http://kw.yuexingan06.cn

PHP ............ 252
来源：http://ii.yuexingan06.cn

JavaScript ..... 252
来源：http://wq.chemitech.net.cn

TypeScript ..... 212
来源：http://rj.szsharing.cn

Java ........... 212
来源：http://zl.jctech888.com.cn

Go ............. 212
来源：http://nh.szsharing.cn

Ruby ........... 212
来源：http://dd.asd995.cn

C# ............. 212
来源：http://kb.chemitech.net.cn

C .............. 30
来源：http://fo.szxytkj.cn

C++ ............ 30
来源：http://mw.huixiangedu.cn

SQL ............ 90
来源：http://pp.lnxyls.cn

Bash ........... 80
来源：http://kf.chemitech.net.cn

Kotlin ......... 15
来源：http://hj.asd995.cn

Swift .......... 15
来源：http://nh.lnxyls.cn

Lua ............ 10
来源：http://ak.haigaiapp.cn

Perl ........... 10
来源：http://kq.bookmarksfly.cn

Scala .......... 10
来源：http://ho.colortex.cn

------------------------------------
来源：http://kt.huixiangedu.cn

合计 ........... 2106 条
来源：http://il.huixinmuqiang.cn

按章节统计：
来源：http://dt.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mf.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://av.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sr.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qf.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wd.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ur.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ep.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fh.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ux.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oy.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ud.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mu.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qj.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wo.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jo.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wn.colortex.cn

Q SQL 专题                              90
来源：http://mw.szxytkj.cn

R Bash 专题                             80
来源：http://rx.shtwfgs.cn

S C / C++ 专题                          60
来源：http://yf.newstarts.cn

T 其他语言补充                          60
来源：http://yp.asd995.cn

U 高频实用片段                         120
来源：http://ob.9csxet.cn

------------------------------------
来源：http://gn.shtwfgs.cn

合计                                  2106 条
来源：http://tr.nicolike.cn

--------------------------------------------------------------------------------
来源：http://mz.hahajie.cn

使用提醒
来源：http://xo.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ca.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jz.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xn.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hx.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tw.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wo.chemitech.net.cn

—— 文件结束 ——
来源：http://ez.szsharing.cn

================================================================================
来源：http://tu.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://wc.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://rn.chemitech.net.cn

================================================================================
来源：http://fp.wgjwhj.cn

【收录内容】
来源：http://my.huixiangedu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tj.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jg.yuexingan06.cn

SQL · Bash · C · C++
来源：http://fq.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bt.hahajie.cn

【使用说明】
来源：http://zr.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gb.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://os.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lu.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zo.asd995.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pj.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lb.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wa.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wn.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sj.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fk.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zk.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uy.panjiajie.cn

【文件统计】
来源：http://tm.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ct.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://mh.wgjwhj.cn

目  录
来源：http://lc.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://rt.shtwfgs.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zw.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ki.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lf.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qv.jctech888.com.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hw.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bp.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vz.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ho.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ln.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gu.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://id.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zi.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hv.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qg.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ya.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zi.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jj.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ry.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ue.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yl.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kr.yuntaijiaju.cn

================================================================================
来源：http://ce.shtwfgs.cn

A. 基础语法与类型
来源：http://tx.jianghongdianzi.cn

================================================================================
来源：http://hh.hnjuh.cn

[A01] Hello World
来源：http://st.szsharing.cn

Py:   print("Hello, World!")
来源：http://xa.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://jd.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://yv.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sx.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://es.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://sw.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://if.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pl.szxytkj.cn

[A02] 变量声明与赋值
来源：http://zz.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tj.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vn.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yb.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fb.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://zk.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://fq.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://ms.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kb.chemitech.net.cn

[A03] 常量定义
来源：http://mr.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wi.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://bh.nicolike.cn

JS:   const PI = 3.14159;
来源：http://qh.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://zb.colortex.cn

Java: static final double PI = 3.14159;
来源：http://af.shxzukj.cn

Go:   const PI = 3.14159
来源：http://vj.lnxyls.cn

Ruby: PI = 3.14159
来源：http://ai.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://gt.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://gn.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pu.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ez.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xb.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://bj.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oz.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://an.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ff.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://ys.panjiajie.cn

[A05] 整数除法与取模
来源：http://wr.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cp.wgjwhj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gf.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wn.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://az.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://ch.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://ag.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://hj.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://de.shxzukj.cn

[A06] 字符串转数字
来源：http://bl.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://tl.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ri.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cs.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bc.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dh.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rm.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ko.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kv.szxytkj.cn

[A07] 数字转字符串
来源：http://wk.gzmigu.cn

Py:   str(42)
来源：http://jh.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://by.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://eu.bookmarksfly.cn

TS:   String(42)
来源：http://os.huanxung.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rf.colortex.cn

Go:   strconv.Itoa(42)
来源：http://xc.shxzskj.cn

Ruby: 42.to_s
来源：http://xl.521024.cn

C#:   42.ToString()
来源：http://ch.lnxyls.cn

[A08] 取整与四舍五入
来源：http://ql.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wg.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xq.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gg.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ug.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ny.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dg.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qc.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pm.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://qz.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tf.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qt.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qg.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ef.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ji.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dn.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sa.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cj.colortex.cn

[A10] 生成随机数
来源：http://rt.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://fw.szxytkj.cn

PHP:  random_int(1, 100);
来源：http://gq.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wl.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ii.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://uz.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sa.colortex.cn

Ruby: rand(1..100)
来源：http://hm.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://gt.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://nl.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://lg.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ca.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qb.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ej.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://xh.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hg.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nc.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qi.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://bk.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zf.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qd.521024.cn

JS:   `Hello, ${name}!`
来源：http://wx.asd995.cn

TS:   `Hello, ${name}!`
来源：http://sx.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://vf.bookmarksfly.cn


<!-- 参考信息 -->