代发 wailian999

[U65] PHP：会话
来源：http://gh.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hi.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://wj.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nx.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://yy.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://do.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://dy.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ye.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://cu.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rf.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://gz.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bq.colortex.cn

[U71] PHP：抛出异常
来源：http://sl.521024.cn

throw new RuntimeException("失败", 500);
来源：http://ya.panjiajie.cn

[U72] PHP：写错误日志
来源：http://sr.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://tm.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://jc.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://rm.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://cr.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://qd.asd995.cn

[U75] PHP：依赖注入
来源：http://na.panjiajie.cn

composer require psr/container
来源：http://kz.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://kj.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://db.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://jg.newstarts.cn

composer require twig/twig
来源：http://yp.haigaiapp.cn

[U78] PHP：单元测试
来源：http://xj.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://wt.shxzukj.cn

[U79] PHP：静态分析
来源：http://le.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://eo.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://kz.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ii.chemitech.net.cn

[U81] JS：初始化项目
来源：http://wt.bjjhwx.cn

npm init -y;  npm i express
来源：http://yk.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://us.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sh.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://vq.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lm.asd995.cn

[U84] JS：CommonJS 写法
来源：http://hm.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bl.lnxyls.cn

[U85] JS：可选链
来源：http://tq.newstarts.cn

a?.b?.c
来源：http://vh.nszjky.cn

[U86] JS：空值合并
来源：http://kt.huixiangedu.cn

a ?? b
来源：http://tr.wgjwhj.cn

[U87] JS：解构默认值
来源：http://nl.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://kf.521024.cn

[U88] JS：对象展开合并
来源：http://ol.hnjuh.cn

{ ...a, ...b }
来源：http://kh.gzmigu.cn

[U89] JS：数组去重
来源：http://hy.nicolike.cn

[...new Set(arr)]
来源：http://xe.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://oq.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://zg.521024.cn

[U91] JS：对象键值遍历
来源：http://su.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qr.shxzukj.cn

[U92] JS：深拷贝
来源：http://uu.521024.cn

structuredClone(obj)
来源：http://hr.huanxung.cn

[U93] JS：模板字符串
来源：http://oq.521024.cn

`共 ${n} 条`
来源：http://hq.9csxet.cn

[U94] JS：箭头函数
来源：http://uk.shtwfgs.cn

const double = x => x * 2;
来源：http://cq.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://nv.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://kk.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://qq.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ez.huixiangedu.cn

[U97] JS：并发请求
来源：http://qp.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pr.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://oi.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wh.bjjhwx.cn

[U99] JS：事件监听
来源：http://le.521024.cn

el.addEventListener("click", e => {})
来源：http://gz.huanxung.cn

[U100] JS：DOM 查询
来源：http://th.huixinmuqiang.cn

document.querySelector(".item")
来源：http://nv.panjiajie.cn

[U101] JS：classList 操作
来源：http://sz.hahajie.cn

el.classList.toggle("active")
来源：http://zy.hahajie.cn

[U102] JS：本地存储
来源：http://pz.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://se.9csxet.cn

[U103] JS：定时器
来源：http://xx.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ii.nszjky.cn

[U104] JS：防抖
来源：http://kf.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ap.szsharing.cn

[U105] JS：节流
来源：http://iv.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ur.panjiajie.cn

[U106] JS：日期格式化
来源：http://bv.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yp.szxytkj.cn

[U107] JS：数字千分位
来源：http://fy.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bf.521024.cn

[U108] JS：随机整数
来源：http://kf.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xa.hahajie.cn

[U109] JS：数组分组
来源：http://hv.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://ic.panjiajie.cn

[U110] JS：数组分块
来源：http://gv.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ae.colortex.cn

[U111] JS：对象转 Map
来源：http://yf.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://ot.panjiajie.cn

[U112] JS：字符串补位
来源：http://qc.bjjhwx.cn

"7".padStart(3, "0")
来源：http://wy.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://tg.nszjky.cn

s.replaceAll("a", "b")
来源：http://qv.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://na.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ri.lnxyls.cn

[U115] JS：生成 UUID
来源：http://tm.panjiajie.cn

crypto.randomUUID()
来源：http://dw.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://tv.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://us.hnjuh.cn

[U117] JS：单元测试
来源：http://cs.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://xz.hnjuh.cn

[U118] JS：开发服务器
来源：http://he.huanxung.cn

npm i -D vite;  npx vite
来源：http://us.9csxet.cn

[U119] JS：生产构建
来源：http://pg.gzmigu.cn

npx vite build
来源：http://fr.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://dx.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://wx.yuntaijiaju.cn

================================================================================
来源：http://br.jctech888.com.cn

统计汇总
来源：http://tp.jianghongdianzi.cn

================================================================================
来源：http://tp.shxzskj.cn

按语言统计（条）：
来源：http://zs.lnxyls.cn

Python ......... 252
来源：http://bd.szsharing.cn

PHP ............ 252
来源：http://xp.hahajie.cn

JavaScript ..... 252
来源：http://sq.chemitech.net.cn

TypeScript ..... 212
来源：http://em.bookmarksfly.cn

Java ........... 212
来源：http://sb.szxytkj.cn

Go ............. 212
来源：http://bz.huanxung.cn

Ruby ........... 212
来源：http://lw.gzmigu.cn

C# ............. 212
来源：http://dj.jctech888.com.cn

C .............. 30
来源：http://js.szxytkj.cn

C++ ............ 30
来源：http://ws.huixinmuqiang.cn

SQL ............ 90
来源：http://ic.9csxet.cn

Bash ........... 80
来源：http://jo.lnxyls.cn

Kotlin ......... 15
来源：http://bq.asd995.cn

Swift .......... 15
来源：http://kh.asd995.cn

Lua ............ 10
来源：http://wy.haigaiapp.cn

Perl ........... 10
来源：http://ez.shxzskj.cn

Scala .......... 10
来源：http://cj.colortex.cn

------------------------------------
来源：http://cx.bookmarksfly.cn

合计 ........... 2106 条
来源：http://ni.hnjuh.cn

按章节统计：
来源：http://mp.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ol.9csxet.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cm.shtwfgs.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yx.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xe.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dw.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ye.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jw.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ft.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uq.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xa.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ma.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kk.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bu.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wb.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://da.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ia.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://sq.jianghongdianzi.cn

R Bash 专题                             80
来源：http://wf.hnjuh.cn

S C / C++ 专题                          60
来源：http://wj.9csxet.cn

T 其他语言补充                          60
来源：http://bj.haigaiapp.cn

U 高频实用片段                         120
来源：http://rk.gzmigu.cn

------------------------------------
来源：http://am.szxytkj.cn

合计                                  2106 条
来源：http://af.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://mp.szxytkj.cn

使用提醒
来源：http://xq.nicolike.cn

--------------------------------------------------------------------------------
来源：http://gz.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dn.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wy.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dg.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uk.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gi.szsharing.cn

—— 文件结束 ——
来源：http://gw.szsharing.cn

================================================================================
来源：http://ku.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://cu.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://yb.szsharing.cn

================================================================================
来源：http://tn.huixinmuqiang.cn

【收录内容】
来源：http://zo.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lp.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tg.huanxung.cn

SQL · Bash · C · C++
来源：http://hi.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cl.nicolike.cn

【使用说明】
来源：http://dg.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://op.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ya.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yl.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zq.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uz.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kh.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jl.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pw.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gq.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ou.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://em.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dv.9csxet.cn

【文件统计】
来源：http://ih.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gk.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://vv.jianghongdianzi.cn

目  录
来源：http://hs.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ra.shtwfgs.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ij.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://in.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jm.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bp.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oz.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://me.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jl.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cl.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xx.panjiajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fy.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xw.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oq.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oo.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ap.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ro.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tk.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ov.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xh.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qt.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gs.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vr.huixiangedu.cn

================================================================================
来源：http://on.shxzukj.cn

A. 基础语法与类型
来源：http://hu.colortex.cn

================================================================================
来源：http://go.nszjky.cn

[A01] Hello World
来源：http://iu.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://ju.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://zn.521024.cn

JS:   console.log("Hello, World!");
来源：http://lk.bookmarksfly.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sb.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://cd.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://mk.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://sd.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vh.hahajie.cn

[A02] 变量声明与赋值
来源：http://yb.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://at.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jd.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qk.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zh.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://cz.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://md.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://st.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://iw.asd995.cn

[A03] 常量定义
来源：http://tx.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vf.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://xg.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://no.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://gy.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://ee.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://qi.nicolike.cn

Ruby: PI = 3.14159
来源：http://rt.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://yx.szxytkj.cn

[A04] 判断变量类型
来源：http://uv.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ne.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rn.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qj.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://za.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pw.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jw.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pb.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://ip.bjjhwx.cn

[A05] 整数除法与取模
来源：http://ip.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ly.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ki.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ok.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bb.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://tk.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://zo.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://in.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://ei.9csxet.cn

[A06] 字符串转数字
来源：http://ca.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://ea.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bq.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://go.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vk.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dp.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ic.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rb.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cn.colortex.cn

[A07] 数字转字符串
来源：http://dr.gzmigu.cn

Py:   str(42)
来源：http://vl.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://xd.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://nw.panjiajie.cn

TS:   String(42)
来源：http://lf.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kq.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://jg.szxytkj.cn

Ruby: 42.to_s
来源：http://aa.jctech888.com.cn

C#:   42.ToString()
来源：http://zf.colortex.cn

[A08] 取整与四舍五入
来源：http://vm.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ft.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ag.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yj.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ea.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mc.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ah.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zm.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zv.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://mo.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://id.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rf.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cx.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://il.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bg.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://co.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yx.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ed.newstarts.cn


<!-- 参考信息 -->