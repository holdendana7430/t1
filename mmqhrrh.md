代发 wailian999

[U69] PHP：PDO 预处理
来源：http://hf.shtwfgs.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mq.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://dw.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cv.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://ad.huanxung.cn

throw new RuntimeException("失败", 500);
来源：http://ho.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://sw.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://js.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://sa.szsharing.cn

parse_ini_file("config.ini", true)
来源：http://fn.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://tv.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://vq.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://wh.shxzskj.cn

composer require psr/container
来源：http://gy.nszjky.cn

[U76] PHP：简单路由
来源：http://ld.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tq.asd995.cn

[U77] PHP：模板渲染
来源：http://co.asd995.cn

composer require twig/twig
来源：http://wj.nicolike.cn

[U78] PHP：单元测试
来源：http://qi.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://vb.panjiajie.cn

[U79] PHP：静态分析
来源：http://ch.colortex.cn

composer require --dev phpstan/phpstan
来源：http://cv.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://qj.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://db.hnjuh.cn

[U81] JS：初始化项目
来源：http://db.newstarts.cn

npm init -y;  npm i express
来源：http://oj.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://hs.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sh.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://sg.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ed.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://sv.jianghongdianzi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ks.colortex.cn

[U85] JS：可选链
来源：http://qi.newstarts.cn

a?.b?.c
来源：http://ts.hnjuh.cn

[U86] JS：空值合并
来源：http://md.chemitech.net.cn

a ?? b
来源：http://sk.szxytkj.cn

[U87] JS：解构默认值
来源：http://bo.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://hp.521024.cn

[U88] JS：对象展开合并
来源：http://iw.shxzskj.cn

{ ...a, ...b }
来源：http://nn.huixiangedu.cn

[U89] JS：数组去重
来源：http://fq.newstarts.cn

[...new Set(arr)]
来源：http://xs.asd995.cn

[U90] JS：数字数组排序
来源：http://kw.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://bn.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://pv.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wb.hahajie.cn

[U92] JS：深拷贝
来源：http://kh.haigaiapp.cn

structuredClone(obj)
来源：http://iw.hahajie.cn

[U93] JS：模板字符串
来源：http://xp.huixinmuqiang.cn

`共 ${n} 条`
来源：http://jn.chemitech.net.cn

[U94] JS：箭头函数
来源：http://sr.asd995.cn

const double = x => x * 2;
来源：http://ns.szxytkj.cn

[U95] JS：Promise 包装
来源：http://yr.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://en.szsharing.cn

[U96] JS：async/await 与异常
来源：http://rk.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zu.szsharing.cn

[U97] JS：并发请求
来源：http://ub.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uo.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://yc.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ag.bookmarksfly.cn

[U99] JS：事件监听
来源：http://vj.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://rt.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://pa.hnjuh.cn

document.querySelector(".item")
来源：http://qu.panjiajie.cn

[U101] JS：classList 操作
来源：http://wm.nicolike.cn

el.classList.toggle("active")
来源：http://dy.szxytkj.cn

[U102] JS：本地存储
来源：http://ip.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ft.9csxet.cn

[U103] JS：定时器
来源：http://oy.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lc.nszjky.cn

[U104] JS：防抖
来源：http://xn.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://go.haigaiapp.cn

[U105] JS：节流
来源：http://kc.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://db.521024.cn

[U106] JS：日期格式化
来源：http://fg.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bu.szxytkj.cn

[U107] JS：数字千分位
来源：http://lw.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vt.lnxyls.cn

[U108] JS：随机整数
来源：http://dj.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qk.newstarts.cn

[U109] JS：数组分组
来源：http://gl.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://lw.asd995.cn

[U110] JS：数组分块
来源：http://it.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vf.hahajie.cn

[U111] JS：对象转 Map
来源：http://us.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://yw.wgjwhj.cn

[U112] JS：字符串补位
来源：http://hi.shtwfgs.cn

"7".padStart(3, "0")
来源：http://ax.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://st.colortex.cn

s.replaceAll("a", "b")
来源：http://hh.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://gn.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vu.gzmigu.cn

[U115] JS：生成 UUID
来源：http://ew.chemitech.net.cn

crypto.randomUUID()
来源：http://al.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://of.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://no.shtwfgs.cn

[U117] JS：单元测试
来源：http://fc.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://qh.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://eo.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://bx.bookmarksfly.cn

[U119] JS：生产构建
来源：http://fa.wgjwhj.cn

npx vite build
来源：http://bw.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://zo.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://of.bookmarksfly.cn

================================================================================
来源：http://og.521024.cn

统计汇总
来源：http://nl.muxihuayi.cn

================================================================================
来源：http://nm.huixiangedu.cn

按语言统计（条）：
来源：http://pe.hahajie.cn

Python ......... 252
来源：http://sn.nicolike.cn

PHP ............ 252
来源：http://zm.shtwfgs.cn

JavaScript ..... 252
来源：http://zz.yuexingan06.cn

TypeScript ..... 212
来源：http://bv.jctech888.com.cn

Java ........... 212
来源：http://qa.nszjky.cn

Go ............. 212
来源：http://uu.hnjuh.cn

Ruby ........... 212
来源：http://vb.huanxung.cn

C# ............. 212
来源：http://ng.shxzukj.cn

C .............. 30
来源：http://uu.wgjwhj.cn

C++ ............ 30
来源：http://zz.shtwfgs.cn

SQL ............ 90
来源：http://re.jctech888.com.cn

Bash ........... 80
来源：http://pr.muxihuayi.cn

Kotlin ......... 15
来源：http://tv.yuexingan06.cn

Swift .......... 15
来源：http://uj.yuntaijiaju.cn

Lua ............ 10
来源：http://nr.hnjuh.cn

Perl ........... 10
来源：http://is.huixiangedu.cn

Scala .......... 10
来源：http://wg.szxytkj.cn

------------------------------------
来源：http://su.haigaiapp.cn

合计 ........... 2106 条
来源：http://iy.chemitech.net.cn

按章节统计：
来源：http://pe.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xc.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cm.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ja.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ue.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ey.yuexingan06.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://om.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sc.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cx.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jr.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lq.521024.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uw.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ol.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wp.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uk.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://re.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qd.chemitech.net.cn

Q SQL 专题                              90
来源：http://ny.9csxet.cn

R Bash 专题                             80
来源：http://pc.yuexingan06.cn

S C / C++ 专题                          60
来源：http://tb.gzmigu.cn

T 其他语言补充                          60
来源：http://fc.szxytkj.cn

U 高频实用片段                         120
来源：http://gg.9csxet.cn

------------------------------------
来源：http://dh.huixiangedu.cn

合计                                  2106 条
来源：http://wu.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ak.haigaiapp.cn

使用提醒
来源：http://gb.colortex.cn

--------------------------------------------------------------------------------
来源：http://rr.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wm.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bg.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dw.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vn.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uv.szsharing.cn

—— 文件结束 ——
来源：http://aq.yuexingan06.cn

================================================================================
来源：http://ck.szsharing.cn

程序语言常见例子速查手册（2024 版）
来源：http://ln.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://hz.bjjhwx.cn

================================================================================
来源：http://pn.lnxyls.cn

【收录内容】
来源：http://ck.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ny.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gj.9csxet.cn

SQL · Bash · C · C++
来源：http://hg.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ld.jianghongdianzi.cn

【使用说明】
来源：http://ps.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gl.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kk.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bw.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://se.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://in.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ys.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fb.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vl.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bu.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iq.huixinmuqiang.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oo.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oq.shxzskj.cn

【文件统计】
来源：http://ku.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ji.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://bk.hnjuh.cn

目  录
来源：http://qp.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://fx.shtwfgs.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xq.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://na.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kp.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eb.jianghongdianzi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qu.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gz.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nj.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lt.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://za.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jj.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://my.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cu.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pc.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yj.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ys.521024.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lu.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xc.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gd.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jz.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rm.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://we.gzmigu.cn

================================================================================
来源：http://pc.hnjuh.cn

A. 基础语法与类型
来源：http://qe.szxytkj.cn

================================================================================
来源：http://ga.szsharing.cn

[A01] Hello World
来源：http://ge.huanxung.cn

Py:   print("Hello, World!")
来源：http://he.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://de.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://zi.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cd.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://pd.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://zu.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://ws.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jy.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://up.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xg.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jw.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hd.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://it.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://qt.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://ed.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://tt.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://an.newstarts.cn

[A03] 常量定义
来源：http://xf.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hu.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://ja.nicolike.cn

JS:   const PI = 3.14159;
来源：http://wu.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://ct.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://xq.panjiajie.cn

Go:   const PI = 3.14159
来源：http://tb.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://hj.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://vn.huanxung.cn

[A04] 判断变量类型
来源：http://wu.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yj.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ip.asd995.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tz.521024.cn

TS:   typeof x; x instanceof Date
来源：http://qf.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://he.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bj.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kx.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://gq.wgjwhj.cn

[A05] 整数除法与取模
来源：http://qx.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tz.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vs.shxzskj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cj.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eb.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://rl.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://mx.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://zo.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://ch.shxzukj.cn

[A06] 字符串转数字
来源：http://uh.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://nn.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ou.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ag.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ll.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://st.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://op.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yf.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xk.hahajie.cn

[A07] 数字转字符串
来源：http://qt.jianghongdianzi.cn

Py:   str(42)
来源：http://kt.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://mn.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://fh.yuntaijiaju.cn

TS:   String(42)
来源：http://om.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ra.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://vt.huixiangedu.cn

Ruby: 42.to_s
来源：http://rq.bjjhwx.cn

C#:   42.ToString()
来源：http://wz.9csxet.cn

[A08] 取整与四舍五入
来源：http://wd.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ya.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://do.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://no.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://co.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uf.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qv.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yt.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kh.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://zl.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vk.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kt.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wr.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xi.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dy.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hp.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gx.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tn.bookmarksfly.cn

[A10] 生成随机数
来源：http://pz.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://tf.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://sx.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qg.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nv.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://zt.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gh.panjiajie.cn

Ruby: rand(1..100)
来源：http://he.asd995.cn


<!-- 参考信息 -->