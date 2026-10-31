代发 wailian999

[U75] PHP：依赖注入
来源：http://cn.wgjwhj.cn

composer require psr/container
来源：http://mj.hahajie.cn

[U76] PHP：简单路由
来源：http://nq.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ip.panjiajie.cn

[U77] PHP：模板渲染
来源：http://ts.wgjwhj.cn

composer require twig/twig
来源：http://qx.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://rk.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://ha.shxzskj.cn

[U79] PHP：静态分析
来源：http://ov.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://xg.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://tq.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lb.asd995.cn

[U81] JS：初始化项目
来源：http://ia.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://xd.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://ja.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ly.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://dq.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hr.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://sh.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ek.521024.cn

[U85] JS：可选链
来源：http://wq.jctech888.com.cn

a?.b?.c
来源：http://nf.newstarts.cn

[U86] JS：空值合并
来源：http://et.chemitech.net.cn

a ?? b
来源：http://ma.hahajie.cn

[U87] JS：解构默认值
来源：http://ba.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://ox.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://yy.muxihuayi.cn

{ ...a, ...b }
来源：http://mh.wgjwhj.cn

[U89] JS：数组去重
来源：http://tu.szsharing.cn

[...new Set(arr)]
来源：http://gw.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://ft.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://cs.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://wk.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qp.gzmigu.cn

[U92] JS：深拷贝
来源：http://gj.lnxyls.cn

structuredClone(obj)
来源：http://xg.colortex.cn

[U93] JS：模板字符串
来源：http://vv.shtwfgs.cn

`共 ${n} 条`
来源：http://lg.shxzskj.cn

[U94] JS：箭头函数
来源：http://tl.asd995.cn

const double = x => x * 2;
来源：http://wg.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://rm.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://yr.szsharing.cn

[U96] JS：async/await 与异常
来源：http://bx.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uw.yuexingan06.cn

[U97] JS：并发请求
来源：http://rp.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lj.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://en.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cy.hnjuh.cn

[U99] JS：事件监听
来源：http://cn.szsharing.cn

el.addEventListener("click", e => {})
来源：http://or.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://fk.bookmarksfly.cn

document.querySelector(".item")
来源：http://ko.haigaiapp.cn

[U101] JS：classList 操作
来源：http://cb.shxzskj.cn

el.classList.toggle("active")
来源：http://gs.wgjwhj.cn

[U102] JS：本地存储
来源：http://bv.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mf.muxihuayi.cn

[U103] JS：定时器
来源：http://id.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ne.newstarts.cn

[U104] JS：防抖
来源：http://zx.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zc.szxytkj.cn

[U105] JS：节流
来源：http://dl.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vr.nszjky.cn

[U106] JS：日期格式化
来源：http://td.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bl.panjiajie.cn

[U107] JS：数字千分位
来源：http://mh.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zf.hahajie.cn

[U108] JS：随机整数
来源：http://yl.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lw.hnjuh.cn

[U109] JS：数组分组
来源：http://wv.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://jh.szsharing.cn

[U110] JS：数组分块
来源：http://oy.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gl.gzmigu.cn

[U111] JS：对象转 Map
来源：http://at.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://sx.yuexingan06.cn

[U112] JS：字符串补位
来源：http://dp.nszjky.cn

"7".padStart(3, "0")
来源：http://nb.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://zu.panjiajie.cn

s.replaceAll("a", "b")
来源：http://lx.colortex.cn

[U114] JS：JSON 深比较
来源：http://tu.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gc.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://ts.bjjhwx.cn

crypto.randomUUID()
来源：http://hf.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://tb.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://zs.lnxyls.cn

[U117] JS：单元测试
来源：http://qh.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://ff.szsharing.cn

[U118] JS：开发服务器
来源：http://vq.hahajie.cn

npm i -D vite;  npx vite
来源：http://pk.newstarts.cn

[U119] JS：生产构建
来源：http://ay.nszjky.cn

npx vite build
来源：http://gy.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://nc.colortex.cn

import.meta.env.VITE_API_URL
来源：http://tp.szsharing.cn

================================================================================
来源：http://wr.huanxung.cn

统计汇总
来源：http://nb.huixiangedu.cn

================================================================================
来源：http://mk.lnxyls.cn

按语言统计（条）：
来源：http://ku.521024.cn

Python ......... 252
来源：http://wh.huixinmuqiang.cn

PHP ............ 252
来源：http://wq.haigaiapp.cn

JavaScript ..... 252
来源：http://jn.nszjky.cn

TypeScript ..... 212
来源：http://uq.gzmigu.cn

Java ........... 212
来源：http://ci.nicolike.cn

Go ............. 212
来源：http://uk.bookmarksfly.cn

Ruby ........... 212
来源：http://wg.newstarts.cn

C# ............. 212
来源：http://kj.jianghongdianzi.cn

C .............. 30
来源：http://hi.shxzskj.cn

C++ ............ 30
来源：http://sb.szsharing.cn

SQL ............ 90
来源：http://at.jctech888.com.cn

Bash ........... 80
来源：http://xc.gzmigu.cn

Kotlin ......... 15
来源：http://mk.bjjhwx.cn

Swift .......... 15
来源：http://co.shtwfgs.cn

Lua ............ 10
来源：http://dy.jianghongdianzi.cn

Perl ........... 10
来源：http://tu.huixinmuqiang.cn

Scala .......... 10
来源：http://jf.newstarts.cn

------------------------------------
来源：http://li.lnxyls.cn

合计 ........... 2106 条
来源：http://ih.chemitech.net.cn

按章节统计：
来源：http://ij.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gf.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cq.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mo.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xu.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sr.nszjky.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cx.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lo.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://va.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nv.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://km.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://me.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zc.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uv.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ia.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rb.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://du.huanxung.cn

Q SQL 专题                              90
来源：http://bo.bjjhwx.cn

R Bash 专题                             80
来源：http://xj.gzmigu.cn

S C / C++ 专题                          60
来源：http://fn.bjjhwx.cn

T 其他语言补充                          60
来源：http://gn.yuexingan06.cn

U 高频实用片段                         120
来源：http://fy.huixinmuqiang.cn

------------------------------------
来源：http://lf.panjiajie.cn

合计                                  2106 条
来源：http://qc.szsharing.cn

--------------------------------------------------------------------------------
来源：http://au.colortex.cn

使用提醒
来源：http://qs.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://vz.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xy.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nf.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bv.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wz.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qf.asd995.cn

—— 文件结束 ——
来源：http://rq.jctech888.com.cn

================================================================================
来源：http://np.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://gk.colortex.cn

Common Programming Examples Cheat Book
来源：http://to.szxytkj.cn

================================================================================
来源：http://vg.huixiangedu.cn

【收录内容】
来源：http://qm.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://py.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tj.chemitech.net.cn

SQL · Bash · C · C++
来源：http://dw.nicolike.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://on.hnjuh.cn

【使用说明】
来源：http://pv.nicolike.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ie.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vb.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pw.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yo.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xi.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bt.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lz.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qa.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cf.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jt.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pt.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eg.newstarts.cn

【文件统计】
来源：http://pi.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hd.huanxung.cn

--------------------------------------------------------------------------------
来源：http://tn.hnjuh.cn

目  录
来源：http://so.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://yr.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ek.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yd.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ln.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xm.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wl.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tv.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nr.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mn.wgjwhj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wg.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uk.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cb.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cr.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vc.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ri.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zk.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xh.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zw.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cd.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ut.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vr.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zu.bjjhwx.cn

================================================================================
来源：http://qv.shxzukj.cn

A. 基础语法与类型
来源：http://xz.huixinmuqiang.cn

================================================================================
来源：http://xg.huanxung.cn

[A01] Hello World
来源：http://du.shxzukj.cn

Py:   print("Hello, World!")
来源：http://fv.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://tk.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://rz.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zi.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://lj.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://gr.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://gt.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qo.521024.cn

[A02] 变量声明与赋值
来源：http://hd.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xo.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rd.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xn.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yv.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://ac.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://qq.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://xe.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ep.newstarts.cn

[A03] 常量定义
来源：http://lc.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sg.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://me.nicolike.cn

JS:   const PI = 3.14159;
来源：http://xd.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://iq.colortex.cn

Java: static final double PI = 3.14159;
来源：http://lm.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://jw.521024.cn

Ruby: PI = 3.14159
来源：http://zm.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://em.huixiangedu.cn

[A04] 判断变量类型
来源：http://ue.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://eg.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ne.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nc.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://sd.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vp.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zs.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xp.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://xj.colortex.cn

[A05] 整数除法与取模
来源：http://vn.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ac.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rk.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vv.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://en.521024.cn

Java: 7 / 2; 7 % 2
来源：http://wl.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://yz.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://zm.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://fy.bjjhwx.cn

[A06] 字符串转数字
来源：http://xz.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://ob.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iu.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://er.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wo.yuntaijiaju.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xt.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ik.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sc.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cf.jctech888.com.cn

[A07] 数字转字符串
来源：http://bp.shxzukj.cn

Py:   str(42)
来源：http://io.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://lf.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://wc.wgjwhj.cn

TS:   String(42)
来源：http://hk.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qs.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://wa.hahajie.cn

Ruby: 42.to_s
来源：http://pw.hahajie.cn

C#:   42.ToString()
来源：http://pc.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://ij.hnjuh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uy.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sz.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lw.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qs.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rp.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kg.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uo.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ro.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://cy.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pg.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yk.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gm.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ch.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lf.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kn.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nh.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gp.shxzukj.cn

[A10] 生成随机数
来源：http://cg.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://ck.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://ck.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://in.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dk.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://fg.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ru.colortex.cn

Ruby: rand(1..100)
来源：http://me.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://mu.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://vk.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://bv.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hj.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fu.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tu.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://ux.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://os.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fp.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hi.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://kb.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rd.hahajie.cn


<!-- 参考信息 -->