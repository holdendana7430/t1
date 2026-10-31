代发 wailian999

[U75] PHP：依赖注入
来源：http://yc.bjjhwx.cn

composer require psr/container
来源：http://ve.szxytkj.cn

[U76] PHP：简单路由
来源：http://hd.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jv.shxzskj.cn

[U77] PHP：模板渲染
来源：http://tg.szsharing.cn

composer require twig/twig
来源：http://vc.lnxyls.cn

[U78] PHP：单元测试
来源：http://en.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://xb.muxihuayi.cn

[U79] PHP：静态分析
来源：http://de.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://zy.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://es.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kt.colortex.cn

[U81] JS：初始化项目
来源：http://ng.lnxyls.cn

npm init -y;  npm i express
来源：http://qn.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://bz.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bq.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://st.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ta.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://vp.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tu.haigaiapp.cn

[U85] JS：可选链
来源：http://yd.asd995.cn

a?.b?.c
来源：http://kj.huixiangedu.cn

[U86] JS：空值合并
来源：http://xl.newstarts.cn

a ?? b
来源：http://fw.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://rp.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://rh.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://ge.9csxet.cn

{ ...a, ...b }
来源：http://wa.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://we.colortex.cn

[...new Set(arr)]
来源：http://lm.521024.cn

[U90] JS：数字数组排序
来源：http://zd.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://ff.huanxung.cn

[U91] JS：对象键值遍历
来源：http://df.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ho.wgjwhj.cn

[U92] JS：深拷贝
来源：http://su.hnjuh.cn

structuredClone(obj)
来源：http://zz.wgjwhj.cn

[U93] JS：模板字符串
来源：http://bt.asd995.cn

`共 ${n} 条`
来源：http://zd.nicolike.cn

[U94] JS：箭头函数
来源：http://ik.huixiangedu.cn

const double = x => x * 2;
来源：http://bi.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://xp.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://ai.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://wx.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dd.hahajie.cn

[U97] JS：并发请求
来源：http://hr.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ky.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://gx.shtwfgs.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dv.huanxung.cn

[U99] JS：事件监听
来源：http://lm.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://ig.panjiajie.cn

[U100] JS：DOM 查询
来源：http://ki.bjjhwx.cn

document.querySelector(".item")
来源：http://mc.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://mt.colortex.cn

el.classList.toggle("active")
来源：http://pi.shxzskj.cn

[U102] JS：本地存储
来源：http://jd.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tz.huixinmuqiang.cn

[U103] JS：定时器
来源：http://cy.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tp.szsharing.cn

[U104] JS：防抖
来源：http://wh.asd995.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sz.wgjwhj.cn

[U105] JS：节流
来源：http://vk.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dv.wgjwhj.cn

[U106] JS：日期格式化
来源：http://yx.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bo.panjiajie.cn

[U107] JS：数字千分位
来源：http://yl.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tk.yuexingan06.cn

[U108] JS：随机整数
来源：http://hu.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pj.hahajie.cn

[U109] JS：数组分组
来源：http://ro.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://gk.521024.cn

[U110] JS：数组分块
来源：http://pn.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sa.shxzskj.cn

[U111] JS：对象转 Map
来源：http://vl.panjiajie.cn

new Map(Object.entries(obj))
来源：http://tr.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://nz.haigaiapp.cn

"7".padStart(3, "0")
来源：http://tp.shxzskj.cn

[U113] JS：正则替换全部
来源：http://vu.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://sm.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://sq.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zv.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://qu.bookmarksfly.cn

crypto.randomUUID()
来源：http://ap.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ho.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://fo.huixiangedu.cn

[U117] JS：单元测试
来源：http://qt.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://mo.huanxung.cn

[U118] JS：开发服务器
来源：http://hg.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://bg.jctech888.com.cn

[U119] JS：生产构建
来源：http://xs.jianghongdianzi.cn

npx vite build
来源：http://jf.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ij.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://qc.asd995.cn

================================================================================
来源：http://ie.gzmigu.cn

统计汇总
来源：http://li.bjjhwx.cn

================================================================================
来源：http://fv.szsharing.cn

按语言统计（条）：
来源：http://vh.bjjhwx.cn

Python ......... 252
来源：http://qh.521024.cn

PHP ............ 252
来源：http://il.szsharing.cn

JavaScript ..... 252
来源：http://bs.yuntaijiaju.cn

TypeScript ..... 212
来源：http://jk.colortex.cn

Java ........... 212
来源：http://ni.haigaiapp.cn

Go ............. 212
来源：http://ax.huanxung.cn

Ruby ........... 212
来源：http://kf.szsharing.cn

C# ............. 212
来源：http://tf.muxihuayi.cn

C .............. 30
来源：http://mo.gzmigu.cn

C++ ............ 30
来源：http://si.asd995.cn

SQL ............ 90
来源：http://vf.muxihuayi.cn

Bash ........... 80
来源：http://ee.chemitech.net.cn

Kotlin ......... 15
来源：http://tx.muxihuayi.cn

Swift .......... 15
来源：http://vd.bookmarksfly.cn

Lua ............ 10
来源：http://zp.yuntaijiaju.cn

Perl ........... 10
来源：http://vl.hnjuh.cn

Scala .......... 10
来源：http://yz.huanxung.cn

------------------------------------
来源：http://te.haigaiapp.cn

合计 ........... 2106 条
来源：http://hv.wgjwhj.cn

按章节统计：
来源：http://db.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qx.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qe.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rk.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gj.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cq.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://al.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yj.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ne.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ej.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jt.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ge.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mu.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rn.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pn.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kk.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xo.panjiajie.cn

Q SQL 专题                              90
来源：http://qn.chemitech.net.cn

R Bash 专题                             80
来源：http://bw.huixiangedu.cn

S C / C++ 专题                          60
来源：http://cf.colortex.cn

T 其他语言补充                          60
来源：http://yi.muxihuayi.cn

U 高频实用片段                         120
来源：http://yg.9csxet.cn

------------------------------------
来源：http://em.9csxet.cn

合计                                  2106 条
来源：http://vn.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://qe.huixinmuqiang.cn

使用提醒
来源：http://xq.newstarts.cn

--------------------------------------------------------------------------------
来源：http://zb.chemitech.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://si.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cr.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xg.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wo.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dy.muxihuayi.cn

—— 文件结束 ——
来源：http://mo.muxihuayi.cn

================================================================================
来源：http://ny.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://yj.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://oz.gzmigu.cn

================================================================================
来源：http://cq.bookmarksfly.cn

【收录内容】
来源：http://po.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gt.huixiangedu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ri.bjjhwx.cn

SQL · Bash · C · C++
来源：http://aa.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://he.newstarts.cn

【使用说明】
来源：http://dq.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xv.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lo.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iu.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sm.shtwfgs.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ot.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vv.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rd.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lr.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zk.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xi.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ou.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ji.521024.cn

【文件统计】
来源：http://gn.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dw.521024.cn

--------------------------------------------------------------------------------
来源：http://qr.panjiajie.cn

目  录
来源：http://ar.nicolike.cn

--------------------------------------------------------------------------------
来源：http://gd.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oq.shxzskj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pe.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lh.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ae.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://je.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vc.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bf.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oq.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ee.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hf.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uq.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sy.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ez.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iq.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vz.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vf.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pf.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pf.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uq.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sq.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zb.newstarts.cn

================================================================================
来源：http://in.huixinmuqiang.cn

A. 基础语法与类型
来源：http://vr.asd995.cn

================================================================================
来源：http://fm.huanxung.cn

[A01] Hello World
来源：http://np.huanxung.cn

Py:   print("Hello, World!")
来源：http://lr.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://ys.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://qc.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ul.lnxyls.cn

Java: System.out.println("Hello, World!");
来源：http://zb.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://cz.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://cb.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vg.huixinmuqiang.cn

[A02] 变量声明与赋值
来源：http://qn.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ru.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cb.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wz.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gm.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://nd.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://zd.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://am.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ew.shxzukj.cn

[A03] 常量定义
来源：http://jp.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fj.colortex.cn

PHP:  const PI = 3.14159;
来源：http://fc.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://zb.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://uv.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://vx.hahajie.cn

Go:   const PI = 3.14159
来源：http://jp.muxihuayi.cn

Ruby: PI = 3.14159
来源：http://ff.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://hu.colortex.cn

[A04] 判断变量类型
来源：http://js.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hk.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jg.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://di.yuexingan06.cn

TS:   typeof x; x instanceof Date
来源：http://cs.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pd.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yw.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://eu.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://fo.colortex.cn

[A05] 整数除法与取模
来源：http://sp.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ir.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qt.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ks.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wf.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://tk.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://jo.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://pj.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://iz.gzmigu.cn

[A06] 字符串转数字
来源：http://lh.colortex.cn

Py:   int("42"); float("3.14")
来源：http://dy.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://va.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://en.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fl.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lr.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://az.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yl.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://na.shxzukj.cn

[A07] 数字转字符串
来源：http://fn.huixinmuqiang.cn

Py:   str(42)
来源：http://mv.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://of.nicolike.cn

JS:   String(42); (42).toString()
来源：http://hn.huixiangedu.cn

TS:   String(42)
来源：http://pm.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rz.521024.cn

Go:   strconv.Itoa(42)
来源：http://km.nicolike.cn

Ruby: 42.to_s
来源：http://qu.shxzukj.cn

C#:   42.ToString()
来源：http://jf.panjiajie.cn

[A08] 取整与四舍五入
来源：http://kl.521024.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ml.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nc.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rp.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eo.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mu.huixiangedu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hl.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://op.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rf.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://rl.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mc.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://st.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tu.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gr.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vt.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://if.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ph.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ju.panjiajie.cn

[A10] 生成随机数
来源：http://cm.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://tt.nicolike.cn

PHP:  random_int(1, 100);
来源：http://ml.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sy.colortex.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ma.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://xn.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gn.huanxung.cn

Ruby: rand(1..100)
来源：http://ue.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://oe.nszjky.cn

[A11] 条件表达式（三元）
来源：http://fx.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://ic.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ai.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fe.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pi.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://ks.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ph.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ya.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sa.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://rt.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xx.9csxet.cn


<!-- 参考信息 -->