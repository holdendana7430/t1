代发 wailian999

[U75] PHP：依赖注入
来源：http://hp.jianghongdianzi.cn

composer require psr/container
来源：http://vq.shtwfgs.cn

[U76] PHP：简单路由
来源：http://yu.yuntaijiaju.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zl.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://ok.colortex.cn

composer require twig/twig
来源：http://in.lnxyls.cn

[U78] PHP：单元测试
来源：http://yh.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://ye.huanxung.cn

[U79] PHP：静态分析
来源：http://eo.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://ia.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://eq.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://da.yuexingan06.cn

[U81] JS：初始化项目
来源：http://li.muxihuayi.cn

npm init -y;  npm i express
来源：http://qj.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://em.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://af.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://zk.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zw.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://bt.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yb.szsharing.cn

[U85] JS：可选链
来源：http://wo.bookmarksfly.cn

a?.b?.c
来源：http://lq.9csxet.cn

[U86] JS：空值合并
来源：http://pa.szxytkj.cn

a ?? b
来源：http://bd.bjjhwx.cn

[U87] JS：解构默认值
来源：http://rr.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://tn.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://av.wgjwhj.cn

{ ...a, ...b }
来源：http://jg.szxytkj.cn

[U89] JS：数组去重
来源：http://cw.hahajie.cn

[...new Set(arr)]
来源：http://jj.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://nm.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://xy.colortex.cn

[U91] JS：对象键值遍历
来源：http://zk.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bc.gzmigu.cn

[U92] JS：深拷贝
来源：http://zw.colortex.cn

structuredClone(obj)
来源：http://iw.huixiangedu.cn

[U93] JS：模板字符串
来源：http://zg.bookmarksfly.cn

`共 ${n} 条`
来源：http://dy.shxzskj.cn

[U94] JS：箭头函数
来源：http://ei.shxzukj.cn

const double = x => x * 2;
来源：http://vy.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://qy.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://cj.colortex.cn

[U96] JS：async/await 与异常
来源：http://fr.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ws.huixiangedu.cn

[U97] JS：并发请求
来源：http://tv.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vz.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://vo.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ab.szxytkj.cn

[U99] JS：事件监听
来源：http://jf.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://ex.szxytkj.cn

[U100] JS：DOM 查询
来源：http://tm.shtwfgs.cn

document.querySelector(".item")
来源：http://fm.huanxung.cn

[U101] JS：classList 操作
来源：http://fb.hnjuh.cn

el.classList.toggle("active")
来源：http://ze.yuexingan06.cn

[U102] JS：本地存储
来源：http://nm.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ya.haigaiapp.cn

[U103] JS：定时器
来源：http://ig.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nb.shxzskj.cn

[U104] JS：防抖
来源：http://vb.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rn.huanxung.cn

[U105] JS：节流
来源：http://fs.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xc.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://ku.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mk.wgjwhj.cn

[U107] JS：数字千分位
来源：http://xl.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sz.jctech888.com.cn

[U108] JS：随机整数
来源：http://vl.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qo.yuexingan06.cn

[U109] JS：数组分组
来源：http://kv.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://ox.shxzukj.cn

[U110] JS：数组分块
来源：http://pf.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mn.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://ra.9csxet.cn

new Map(Object.entries(obj))
来源：http://ba.colortex.cn

[U112] JS：字符串补位
来源：http://si.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://md.panjiajie.cn

[U113] JS：正则替换全部
来源：http://kq.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://yq.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://gz.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ff.521024.cn

[U115] JS：生成 UUID
来源：http://nu.yuntaijiaju.cn

crypto.randomUUID()
来源：http://qv.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://gm.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://an.szxytkj.cn

[U117] JS：单元测试
来源：http://ov.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://cm.colortex.cn

[U118] JS：开发服务器
来源：http://yo.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://ii.nicolike.cn

[U119] JS：生产构建
来源：http://fr.shtwfgs.cn

npx vite build
来源：http://zr.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://as.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://is.nszjky.cn

================================================================================
来源：http://cz.bjjhwx.cn

统计汇总
来源：http://pb.panjiajie.cn

================================================================================
来源：http://wg.szsharing.cn

按语言统计（条）：
来源：http://jp.shtwfgs.cn

Python ......... 252
来源：http://ph.jianghongdianzi.cn

PHP ............ 252
来源：http://vk.szsharing.cn

JavaScript ..... 252
来源：http://mg.wgjwhj.cn

TypeScript ..... 212
来源：http://jh.jianghongdianzi.cn

Java ........... 212
来源：http://pf.asd995.cn

Go ............. 212
来源：http://ny.hnjuh.cn

Ruby ........... 212
来源：http://jh.szxytkj.cn

C# ............. 212
来源：http://cz.muxihuayi.cn

C .............. 30
来源：http://jw.asd995.cn

C++ ............ 30
来源：http://ia.gzmigu.cn

SQL ............ 90
来源：http://xm.newstarts.cn

Bash ........... 80
来源：http://uc.haigaiapp.cn

Kotlin ......... 15
来源：http://yp.lnxyls.cn

Swift .......... 15
来源：http://iv.521024.cn

Lua ............ 10
来源：http://nq.521024.cn

Perl ........... 10
来源：http://ec.bookmarksfly.cn

Scala .......... 10
来源：http://it.nszjky.cn

------------------------------------
来源：http://pq.huixiangedu.cn

合计 ........... 2106 条
来源：http://qg.jctech888.com.cn

按章节统计：
来源：http://hx.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ur.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dg.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xq.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qm.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lz.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zl.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vh.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jk.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ip.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fg.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oc.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bp.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xq.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eh.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bo.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eh.szsharing.cn

Q SQL 专题                              90
来源：http://ue.muxihuayi.cn

R Bash 专题                             80
来源：http://td.colortex.cn

S C / C++ 专题                          60
来源：http://zc.shxzskj.cn

T 其他语言补充                          60
来源：http://my.szxytkj.cn

U 高频实用片段                         120
来源：http://pb.nszjky.cn

------------------------------------
来源：http://rf.shxzukj.cn

合计                                  2106 条
来源：http://gy.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://hq.hahajie.cn

使用提醒
来源：http://ba.nicolike.cn

--------------------------------------------------------------------------------
来源：http://mi.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://my.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cz.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yo.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gr.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vj.lnxyls.cn

—— 文件结束 ——
来源：http://qh.nicolike.cn

================================================================================
来源：http://as.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://lu.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://bs.yuntaijiaju.cn

================================================================================
来源：http://yz.shxzskj.cn

【收录内容】
来源：http://xm.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bt.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ar.newstarts.cn

SQL · Bash · C · C++
来源：http://nt.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vo.asd995.cn

【使用说明】
来源：http://ql.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wd.hahajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sa.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sn.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sk.yuntaijiaju.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gr.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mv.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cr.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ja.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sm.szxytkj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fr.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ld.bjjhwx.cn

【文件统计】
来源：http://as.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xi.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://hi.szsharing.cn

目  录
来源：http://fb.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://kb.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ef.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ov.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oc.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oe.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://af.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vc.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ae.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eu.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bl.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vu.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gm.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kq.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://da.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bw.hnjuh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ye.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oe.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nu.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pc.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jo.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zo.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bj.wgjwhj.cn

================================================================================
来源：http://mq.jianghongdianzi.cn

A. 基础语法与类型
来源：http://gn.haigaiapp.cn

================================================================================
来源：http://pm.shtwfgs.cn

[A01] Hello World
来源：http://ws.huanxung.cn

Py:   print("Hello, World!")
来源：http://jf.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://pw.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://ur.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://mp.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://vq.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://gf.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://oj.panjiajie.cn

[A02] 变量声明与赋值
来源：http://ea.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ds.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qo.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jf.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lb.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://wj.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://dm.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://wy.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ej.gzmigu.cn

[A03] 常量定义
来源：http://sw.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qh.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://ve.asd995.cn

JS:   const PI = 3.14159;
来源：http://st.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://yg.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://ny.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://cm.panjiajie.cn

Ruby: PI = 3.14159
来源：http://oe.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://td.chemitech.net.cn

[A04] 判断变量类型
来源：http://zg.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nm.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://my.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sw.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://wc.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cn.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zc.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://il.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://mi.huixiangedu.cn

[A05] 整数除法与取模
来源：http://wt.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ok.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ld.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jp.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sv.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://yx.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://ek.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://oo.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://hn.muxihuayi.cn

[A06] 字符串转数字
来源：http://tj.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://uv.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kv.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ce.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lk.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xh.yuntaijiaju.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vg.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ob.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ua.chemitech.net.cn

[A07] 数字转字符串
来源：http://om.szxytkj.cn

Py:   str(42)
来源：http://hh.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://jh.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://sv.huixiangedu.cn

TS:   String(42)
来源：http://ph.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yq.521024.cn

Go:   strconv.Itoa(42)
来源：http://bz.huanxung.cn

Ruby: 42.to_s
来源：http://eu.jianghongdianzi.cn

C#:   42.ToString()
来源：http://yt.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://sk.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://du.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xe.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mw.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kz.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cq.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eb.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kp.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://td.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://hy.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wb.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yl.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yg.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fw.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://um.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ty.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ee.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zr.521024.cn

[A10] 生成随机数
来源：http://sg.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://ab.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://ha.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://se.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://he.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://io.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ho.asd995.cn

Ruby: rand(1..100)
来源：http://sh.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://la.newstarts.cn

[A11] 条件表达式（三元）
来源：http://mp.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://ne.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mw.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fh.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cz.nszjky.cn

Java: x > 0 ? "yes" : "no"
来源：http://xl.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://og.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vb.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zm.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://it.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jm.yuntaijiaju.cn


<!-- 参考信息 -->