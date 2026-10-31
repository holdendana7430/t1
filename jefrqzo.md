代发 wailian999

[U77] PHP：模板渲染
来源：http://gl.jianghongdianzi.cn

composer require twig/twig
来源：http://or.jctech888.com.cn

[U78] PHP：单元测试
来源：http://az.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://ep.yuexingan06.cn

[U79] PHP：静态分析
来源：http://cn.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://fx.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://wg.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pu.muxihuayi.cn

[U81] JS：初始化项目
来源：http://ph.szsharing.cn

npm init -y;  npm i express
来源：http://xa.newstarts.cn

[U82] JS：package.json 脚本
来源：http://pj.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bq.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://kq.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gb.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://tk.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hq.gzmigu.cn

[U85] JS：可选链
来源：http://zk.muxihuayi.cn

a?.b?.c
来源：http://fi.muxihuayi.cn

[U86] JS：空值合并
来源：http://ok.nicolike.cn

a ?? b
来源：http://gs.nicolike.cn

[U87] JS：解构默认值
来源：http://ke.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://hr.panjiajie.cn

[U88] JS：对象展开合并
来源：http://ac.wgjwhj.cn

{ ...a, ...b }
来源：http://ff.huixiangedu.cn

[U89] JS：数组去重
来源：http://zj.wgjwhj.cn

[...new Set(arr)]
来源：http://dm.hahajie.cn

[U90] JS：数字数组排序
来源：http://mr.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://zt.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://kl.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ny.9csxet.cn

[U92] JS：深拷贝
来源：http://gl.panjiajie.cn

structuredClone(obj)
来源：http://xa.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://li.nicolike.cn

`共 ${n} 条`
来源：http://it.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://yh.jctech888.com.cn

const double = x => x * 2;
来源：http://jh.gzmigu.cn

[U95] JS：Promise 包装
来源：http://kf.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://ga.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://ud.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rl.bjjhwx.cn

[U97] JS：并发请求
来源：http://ql.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ax.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://xw.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mp.jctech888.com.cn

[U99] JS：事件监听
来源：http://fe.huanxung.cn

el.addEventListener("click", e => {})
来源：http://yc.521024.cn

[U100] JS：DOM 查询
来源：http://ym.bookmarksfly.cn

document.querySelector(".item")
来源：http://ue.gzmigu.cn

[U101] JS：classList 操作
来源：http://nb.asd995.cn

el.classList.toggle("active")
来源：http://pl.521024.cn

[U102] JS：本地存储
来源：http://ts.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ky.yuexingan06.cn

[U103] JS：定时器
来源：http://fr.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://no.bookmarksfly.cn

[U104] JS：防抖
来源：http://gi.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bb.hnjuh.cn

[U105] JS：节流
来源：http://om.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xn.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://fl.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://op.shxzukj.cn

[U107] JS：数字千分位
来源：http://qw.szsharing.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yp.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://ua.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lv.jctech888.com.cn

[U109] JS：数组分组
来源：http://pb.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://yg.gzmigu.cn

[U110] JS：数组分块
来源：http://xd.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gh.shxzukj.cn

[U111] JS：对象转 Map
来源：http://lz.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://xf.colortex.cn

[U112] JS：字符串补位
来源：http://rd.huixiangedu.cn

"7".padStart(3, "0")
来源：http://hz.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://cd.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://pg.newstarts.cn

[U114] JS：JSON 深比较
来源：http://qh.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://du.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://fr.shtwfgs.cn

crypto.randomUUID()
来源：http://se.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://wa.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://kb.nszjky.cn

[U117] JS：单元测试
来源：http://ou.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://fn.shtwfgs.cn

[U118] JS：开发服务器
来源：http://nd.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://gt.nicolike.cn

[U119] JS：生产构建
来源：http://ay.shxzskj.cn

npx vite build
来源：http://rc.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ci.asd995.cn

import.meta.env.VITE_API_URL
来源：http://in.shxzskj.cn

================================================================================
来源：http://fs.huanxung.cn

统计汇总
来源：http://ke.shxzukj.cn

================================================================================
来源：http://jv.gzmigu.cn

按语言统计（条）：
来源：http://jk.nicolike.cn

Python ......... 252
来源：http://ca.jctech888.com.cn

PHP ............ 252
来源：http://dc.9csxet.cn

JavaScript ..... 252
来源：http://sp.shtwfgs.cn

TypeScript ..... 212
来源：http://kr.colortex.cn

Java ........... 212
来源：http://tq.szxytkj.cn

Go ............. 212
来源：http://gy.gzmigu.cn

Ruby ........... 212
来源：http://hl.bjjhwx.cn

C# ............. 212
来源：http://ez.nicolike.cn

C .............. 30
来源：http://gj.yuexingan06.cn

C++ ............ 30
来源：http://wj.hnjuh.cn

SQL ............ 90
来源：http://qm.shtwfgs.cn

Bash ........... 80
来源：http://ef.hahajie.cn

Kotlin ......... 15
来源：http://ga.huanxung.cn

Swift .......... 15
来源：http://pp.shtwfgs.cn

Lua ............ 10
来源：http://jk.haigaiapp.cn

Perl ........... 10
来源：http://oh.nicolike.cn

Scala .......... 10
来源：http://xw.panjiajie.cn

------------------------------------
来源：http://jw.szsharing.cn

合计 ........... 2106 条
来源：http://ym.szsharing.cn

按章节统计：
来源：http://jq.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rr.szxytkj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rx.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hg.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eq.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ty.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ku.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rl.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ym.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ej.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ow.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ch.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wf.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://os.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mx.szsharing.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nm.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vc.newstarts.cn

Q SQL 专题                              90
来源：http://kt.nszjky.cn

R Bash 专题                             80
来源：http://yb.colortex.cn

S C / C++ 专题                          60
来源：http://zj.szsharing.cn

T 其他语言补充                          60
来源：http://ct.nicolike.cn

U 高频实用片段                         120
来源：http://aq.szxytkj.cn

------------------------------------
来源：http://gn.hnjuh.cn

合计                                  2106 条
来源：http://ws.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://jh.bookmarksfly.cn

使用提醒
来源：http://bt.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://vq.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qg.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pi.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ds.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://re.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://un.nszjky.cn

—— 文件结束 ——
来源：http://mx.9csxet.cn

================================================================================
来源：http://ma.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://vt.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://no.hnjuh.cn

================================================================================
来源：http://jg.yuntaijiaju.cn

【收录内容】
来源：http://me.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oq.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vi.newstarts.cn

SQL · Bash · C · C++
来源：http://kz.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qu.panjiajie.cn

【使用说明】
来源：http://jk.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ot.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vv.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tu.lnxyls.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yz.yuntaijiaju.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yv.yuexingan06.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xy.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yw.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://eu.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kc.szxytkj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sl.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ue.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yd.panjiajie.cn

【文件统计】
来源：http://qj.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xi.szsharing.cn

--------------------------------------------------------------------------------
来源：http://id.bjjhwx.cn

目  录
来源：http://yz.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://gw.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iy.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ge.szsharing.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ec.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xn.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ol.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fb.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://df.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lk.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sb.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ch.shtwfgs.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lo.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yv.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kh.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ij.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iw.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fh.bjjhwx.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rk.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oe.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://co.521024.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hm.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mp.9csxet.cn

================================================================================
来源：http://si.yuntaijiaju.cn

A. 基础语法与类型
来源：http://hu.gzmigu.cn

================================================================================
来源：http://ca.newstarts.cn

[A01] Hello World
来源：http://hb.shxzskj.cn

Py:   print("Hello, World!")
来源：http://eg.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://jt.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://fz.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rw.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://zf.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://zh.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://oy.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xo.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://tb.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ff.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://to.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ru.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xp.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://mc.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://pu.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://lt.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ei.9csxet.cn

[A03] 常量定义
来源：http://kj.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://em.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://uj.521024.cn

JS:   const PI = 3.14159;
来源：http://gn.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://bc.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://tk.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://yd.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://ap.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://ng.bjjhwx.cn

[A04] 判断变量类型
来源：http://za.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fr.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qs.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rd.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://aq.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dc.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ht.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zl.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://mk.muxihuayi.cn

[A05] 整数除法与取模
来源：http://qu.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tb.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://on.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eg.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bo.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://tk.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://hl.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://yl.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://pn.9csxet.cn

[A06] 字符串转数字
来源：http://kd.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://sj.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yl.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kp.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tb.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ni.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eg.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wd.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://er.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://lv.asd995.cn

Py:   str(42)
来源：http://oy.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://au.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://tr.muxihuayi.cn

TS:   String(42)
来源：http://ij.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bg.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://mv.shtwfgs.cn

Ruby: 42.to_s
来源：http://ff.chemitech.net.cn

C#:   42.ToString()
来源：http://xp.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://og.chemitech.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vz.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ue.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jk.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ro.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hx.szxytkj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xz.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://re.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://aa.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://rp.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tv.yuexingan06.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ef.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rm.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pl.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lv.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pw.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://in.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jq.hnjuh.cn

[A10] 生成随机数
来源：http://fy.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://xg.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://ws.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://om.asd995.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dj.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://me.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vp.nszjky.cn

Ruby: rand(1..100)
来源：http://vx.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://za.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://mt.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://tw.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yz.shxzskj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://im.521024.cn

TS:   x > 0 ? "yes" : "no"
来源：http://id.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://zy.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cs.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ps.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zz.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://au.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ug.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zm.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://nd.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://xa.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://ew.lnxyls.cn


<!-- 参考信息 -->