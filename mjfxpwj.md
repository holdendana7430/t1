代发 wailian999

[U77] PHP：模板渲染
来源：http://gg.huixiangedu.cn

composer require twig/twig
来源：http://mf.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://an.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://or.hnjuh.cn

[U79] PHP：静态分析
来源：http://or.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://fb.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://oh.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kx.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://ii.bjjhwx.cn

npm init -y;  npm i express
来源：http://qp.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://su.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ga.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://al.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://td.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://hu.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xh.jianghongdianzi.cn

[U85] JS：可选链
来源：http://zr.bjjhwx.cn

a?.b?.c
来源：http://pi.haigaiapp.cn

[U86] JS：空值合并
来源：http://fq.huanxung.cn

a ?? b
来源：http://dp.nicolike.cn

[U87] JS：解构默认值
来源：http://vw.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ou.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://zt.hnjuh.cn

{ ...a, ...b }
来源：http://mu.nicolike.cn

[U89] JS：数组去重
来源：http://xx.lnxyls.cn

[...new Set(arr)]
来源：http://jf.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://bg.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://jb.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://np.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ct.gzmigu.cn

[U92] JS：深拷贝
来源：http://an.nicolike.cn

structuredClone(obj)
来源：http://he.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://ay.panjiajie.cn

`共 ${n} 条`
来源：http://zh.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://zl.shxzukj.cn

const double = x => x * 2;
来源：http://xb.nszjky.cn

[U95] JS：Promise 包装
来源：http://tw.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://do.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://gt.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cm.hahajie.cn

[U97] JS：并发请求
来源：http://da.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vs.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://uc.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wx.shxzskj.cn

[U99] JS：事件监听
来源：http://kb.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://hp.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://rm.yuntaijiaju.cn

document.querySelector(".item")
来源：http://qn.lnxyls.cn

[U101] JS：classList 操作
来源：http://lm.asd995.cn

el.classList.toggle("active")
来源：http://pu.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://qn.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://af.chemitech.net.cn

[U103] JS：定时器
来源：http://tg.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zd.lnxyls.cn

[U104] JS：防抖
来源：http://zk.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qr.muxihuayi.cn

[U105] JS：节流
来源：http://mn.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uq.szsharing.cn

[U106] JS：日期格式化
来源：http://ga.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dn.lnxyls.cn

[U107] JS：数字千分位
来源：http://ye.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bq.nszjky.cn

[U108] JS：随机整数
来源：http://pq.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fd.asd995.cn

[U109] JS：数组分组
来源：http://zi.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://rg.jctech888.com.cn

[U110] JS：数组分块
来源：http://ub.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nk.colortex.cn

[U111] JS：对象转 Map
来源：http://rn.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://at.huixiangedu.cn

[U112] JS：字符串补位
来源：http://ju.wgjwhj.cn

"7".padStart(3, "0")
来源：http://hb.shxzukj.cn

[U113] JS：正则替换全部
来源：http://zq.asd995.cn

s.replaceAll("a", "b")
来源：http://iz.nszjky.cn

[U114] JS：JSON 深比较
来源：http://sn.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ka.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://sn.huanxung.cn

crypto.randomUUID()
来源：http://tj.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://jo.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://ru.huanxung.cn

[U117] JS：单元测试
来源：http://xc.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://fl.asd995.cn

[U118] JS：开发服务器
来源：http://dm.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://wi.yuexingan06.cn

[U119] JS：生产构建
来源：http://ko.jianghongdianzi.cn

npx vite build
来源：http://zh.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://ty.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://wk.shxzskj.cn

================================================================================
来源：http://jt.nszjky.cn

统计汇总
来源：http://ai.colortex.cn

================================================================================
来源：http://rk.jctech888.com.cn

按语言统计（条）：
来源：http://ul.muxihuayi.cn

Python ......... 252
来源：http://yo.haigaiapp.cn

PHP ............ 252
来源：http://uq.jctech888.com.cn

JavaScript ..... 252
来源：http://su.huanxung.cn

TypeScript ..... 212
来源：http://ts.shxzukj.cn

Java ........... 212
来源：http://rg.haigaiapp.cn

Go ............. 212
来源：http://yo.shtwfgs.cn

Ruby ........... 212
来源：http://ml.shxzskj.cn

C# ............. 212
来源：http://ye.huixiangedu.cn

C .............. 30
来源：http://of.shtwfgs.cn

C++ ............ 30
来源：http://yq.hahajie.cn

SQL ............ 90
来源：http://is.yuexingan06.cn

Bash ........... 80
来源：http://cu.chemitech.net.cn

Kotlin ......... 15
来源：http://nf.jianghongdianzi.cn

Swift .......... 15
来源：http://qu.lnxyls.cn

Lua ............ 10
来源：http://si.muxihuayi.cn

Perl ........... 10
来源：http://dm.jianghongdianzi.cn

Scala .......... 10
来源：http://xz.huanxung.cn

------------------------------------
来源：http://ve.muxihuayi.cn

合计 ........... 2106 条
来源：http://kh.hnjuh.cn

按章节统计：
来源：http://qb.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ev.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://va.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pa.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ln.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zc.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dc.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kg.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lg.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qq.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xm.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ms.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://io.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://de.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://km.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gq.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cy.521024.cn

Q SQL 专题                              90
来源：http://ud.wgjwhj.cn

R Bash 专题                             80
来源：http://bj.panjiajie.cn

S C / C++ 专题                          60
来源：http://ff.shxzskj.cn

T 其他语言补充                          60
来源：http://st.colortex.cn

U 高频实用片段                         120
来源：http://jk.521024.cn

------------------------------------
来源：http://rh.521024.cn

合计                                  2106 条
来源：http://ng.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://nt.asd995.cn

使用提醒
来源：http://xq.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://pc.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://si.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zn.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xw.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zn.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kp.bjjhwx.cn

—— 文件结束 ——
来源：http://pc.nszjky.cn

================================================================================
来源：http://co.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://zi.asd995.cn

Common Programming Examples Cheat Book
来源：http://sl.muxihuayi.cn

================================================================================
来源：http://bx.chemitech.net.cn

【收录内容】
来源：http://rz.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://it.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ov.newstarts.cn

SQL · Bash · C · C++
来源：http://bo.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kz.asd995.cn

【使用说明】
来源：http://kq.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ab.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://en.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xr.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vr.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mc.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ng.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qw.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ob.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lj.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xm.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://es.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hb.nicolike.cn

【文件统计】
来源：http://ux.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://an.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://mt.bjjhwx.cn

目  录
来源：http://cm.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://kq.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://te.shtwfgs.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://km.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mr.9csxet.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sg.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rf.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://as.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yl.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ig.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vf.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oq.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://de.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kp.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tj.521024.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hg.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ax.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iu.bjjhwx.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iq.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fn.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tu.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ws.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ar.shtwfgs.cn

================================================================================
来源：http://bj.yuntaijiaju.cn

A. 基础语法与类型
来源：http://sz.newstarts.cn

================================================================================
来源：http://gz.yuntaijiaju.cn

[A01] Hello World
来源：http://mv.hnjuh.cn

Py:   print("Hello, World!")
来源：http://ld.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://zw.colortex.cn

JS:   console.log("Hello, World!");
来源：http://ps.asd995.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://he.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://xw.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://rs.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://rd.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jn.gzmigu.cn

[A02] 变量声明与赋值
来源：http://qb.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zx.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ty.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://id.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xr.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://po.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://na.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://cd.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fv.shtwfgs.cn

[A03] 常量定义
来源：http://ro.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fw.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://la.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://ty.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://mt.asd995.cn

Java: static final double PI = 3.14159;
来源：http://lw.shxzskj.cn

Go:   const PI = 3.14159
来源：http://vo.nicolike.cn

Ruby: PI = 3.14159
来源：http://kr.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://ss.wgjwhj.cn

[A04] 判断变量类型
来源：http://km.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ct.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tw.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wq.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://ia.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xw.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://du.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zn.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://cy.chemitech.net.cn

[A05] 整数除法与取模
来源：http://wt.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fo.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qr.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ou.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lz.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://rg.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://qk.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://an.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://jr.shxzskj.cn

[A06] 字符串转数字
来源：http://sx.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://tk.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gq.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gb.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ak.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hi.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rw.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ed.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ad.szsharing.cn

[A07] 数字转字符串
来源：http://kf.jianghongdianzi.cn

Py:   str(42)
来源：http://tw.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://ai.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://mn.chemitech.net.cn

TS:   String(42)
来源：http://ay.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wq.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://ih.9csxet.cn

Ruby: 42.to_s
来源：http://td.szxytkj.cn

C#:   42.ToString()
来源：http://oi.shxzukj.cn

[A08] 取整与四舍五入
来源：http://hg.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rv.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://us.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uq.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ml.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hs.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ca.jctech888.com.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qr.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jq.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://ud.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cr.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cs.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zp.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://st.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lx.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://si.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zu.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ma.jianghongdianzi.cn

[A10] 生成随机数
来源：http://lj.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://ey.colortex.cn

PHP:  random_int(1, 100);
来源：http://yf.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qh.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ko.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://cb.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fv.521024.cn

Ruby: rand(1..100)
来源：http://pc.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://sz.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://uf.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://oo.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://du.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lb.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vr.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://nw.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://il.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://df.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yt.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://tf.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ct.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wm.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://ep.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://uo.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://dk.521024.cn


<!-- 参考信息 -->