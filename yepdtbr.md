代发 wailian999

[U65] PHP：会话
来源：http://wn.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zb.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://ll.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jv.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://gg.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cj.nszjky.cn

[U68] PHP：PDO 连接
来源：http://gi.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pc.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://fl.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hl.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://lv.szxytkj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pj.9csxet.cn

[U71] PHP：抛出异常
来源：http://jx.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://zh.szsharing.cn

[U72] PHP：写错误日志
来源：http://et.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://dc.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://no.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://ud.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://mk.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://ah.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://mq.lnxyls.cn

composer require psr/container
来源：http://op.haigaiapp.cn

[U76] PHP：简单路由
来源：http://ix.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ns.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://xn.szsharing.cn

composer require twig/twig
来源：http://zq.newstarts.cn

[U78] PHP：单元测试
来源：http://lf.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://as.hnjuh.cn

[U79] PHP：静态分析
来源：http://jj.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://do.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://id.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rw.shxzukj.cn

[U81] JS：初始化项目
来源：http://aq.gzmigu.cn

npm init -y;  npm i express
来源：http://wg.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://vj.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ei.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://nc.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hi.hnjuh.cn

[U84] JS：CommonJS 写法
来源：http://zq.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fg.yuexingan06.cn

[U85] JS：可选链
来源：http://po.shtwfgs.cn

a?.b?.c
来源：http://bs.hahajie.cn

[U86] JS：空值合并
来源：http://sw.shxzukj.cn

a ?? b
来源：http://pj.colortex.cn

[U87] JS：解构默认值
来源：http://eh.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://ld.szsharing.cn

[U88] JS：对象展开合并
来源：http://qf.gzmigu.cn

{ ...a, ...b }
来源：http://tx.shtwfgs.cn

[U89] JS：数组去重
来源：http://hv.bookmarksfly.cn

[...new Set(arr)]
来源：http://bj.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://lt.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://hh.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://zd.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mx.newstarts.cn

[U92] JS：深拷贝
来源：http://vm.szxytkj.cn

structuredClone(obj)
来源：http://kd.szxytkj.cn

[U93] JS：模板字符串
来源：http://mk.hahajie.cn

`共 ${n} 条`
来源：http://iz.chemitech.net.cn

[U94] JS：箭头函数
来源：http://tb.chemitech.net.cn

const double = x => x * 2;
来源：http://bx.gzmigu.cn

[U95] JS：Promise 包装
来源：http://pn.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://tk.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://dp.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ou.gzmigu.cn

[U97] JS：并发请求
来源：http://pq.yuntaijiaju.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hn.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://fl.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ay.jctech888.com.cn

[U99] JS：事件监听
来源：http://xk.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://re.nszjky.cn

[U100] JS：DOM 查询
来源：http://pj.huixiangedu.cn

document.querySelector(".item")
来源：http://ky.panjiajie.cn

[U101] JS：classList 操作
来源：http://qx.lnxyls.cn

el.classList.toggle("active")
来源：http://ib.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://nt.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cy.hahajie.cn

[U103] JS：定时器
来源：http://kc.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jb.nicolike.cn

[U104] JS：防抖
来源：http://ct.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tr.521024.cn

[U105] JS：节流
来源：http://rq.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://be.asd995.cn

[U106] JS：日期格式化
来源：http://vv.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ea.huixiangedu.cn

[U107] JS：数字千分位
来源：http://bl.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fo.szsharing.cn

[U108] JS：随机整数
来源：http://py.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kh.yuexingan06.cn

[U109] JS：数组分组
来源：http://ig.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://bl.jctech888.com.cn

[U110] JS：数组分块
来源：http://uc.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ms.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://qj.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://cm.shxzskj.cn

[U112] JS：字符串补位
来源：http://dz.szxytkj.cn

"7".padStart(3, "0")
来源：http://dy.newstarts.cn

[U113] JS：正则替换全部
来源：http://kq.szxytkj.cn

s.replaceAll("a", "b")
来源：http://sh.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://vy.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rb.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://th.jctech888.com.cn

crypto.randomUUID()
来源：http://cu.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://ih.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://hd.muxihuayi.cn

[U117] JS：单元测试
来源：http://st.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://ou.shxzskj.cn

[U118] JS：开发服务器
来源：http://mh.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://ak.521024.cn

[U119] JS：生产构建
来源：http://in.hahajie.cn

npx vite build
来源：http://tw.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://en.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://te.jctech888.com.cn

================================================================================
来源：http://tr.asd995.cn

统计汇总
来源：http://hs.panjiajie.cn

================================================================================
来源：http://fq.haigaiapp.cn

按语言统计（条）：
来源：http://ic.huixinmuqiang.cn

Python ......... 252
来源：http://gh.newstarts.cn

PHP ............ 252
来源：http://aa.yuexingan06.cn

JavaScript ..... 252
来源：http://gz.lnxyls.cn

TypeScript ..... 212
来源：http://ap.huanxung.cn

Java ........... 212
来源：http://da.yuexingan06.cn

Go ............. 212
来源：http://sa.gzmigu.cn

Ruby ........... 212
来源：http://yj.hahajie.cn

C# ............. 212
来源：http://le.shxzukj.cn

C .............. 30
来源：http://pa.yuntaijiaju.cn

C++ ............ 30
来源：http://en.haigaiapp.cn

SQL ............ 90
来源：http://zg.shxzskj.cn

Bash ........... 80
来源：http://dm.lnxyls.cn

Kotlin ......... 15
来源：http://ut.szxytkj.cn

Swift .......... 15
来源：http://pi.nszjky.cn

Lua ............ 10
来源：http://ai.bjjhwx.cn

Perl ........... 10
来源：http://gn.yuntaijiaju.cn

Scala .......... 10
来源：http://hc.bookmarksfly.cn

------------------------------------
来源：http://vp.nicolike.cn

合计 ........... 2106 条
来源：http://ev.jctech888.com.cn

按章节统计：
来源：http://dc.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cj.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://em.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dt.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fa.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xo.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kx.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wk.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mb.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vh.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cs.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pj.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zr.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yg.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bq.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mw.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sq.chemitech.net.cn

Q SQL 专题                              90
来源：http://bh.bookmarksfly.cn

R Bash 专题                             80
来源：http://wz.hahajie.cn

S C / C++ 专题                          60
来源：http://wj.jianghongdianzi.cn

T 其他语言补充                          60
来源：http://yf.haigaiapp.cn

U 高频实用片段                         120
来源：http://en.bookmarksfly.cn

------------------------------------
来源：http://ur.lnxyls.cn

合计                                  2106 条
来源：http://yi.nszjky.cn

--------------------------------------------------------------------------------
来源：http://no.szsharing.cn

使用提醒
来源：http://uu.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://dz.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://op.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://af.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ks.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gk.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fr.gzmigu.cn

—— 文件结束 ——
来源：http://dp.wgjwhj.cn

================================================================================
来源：http://ta.lnxyls.cn

程序语言常见例子速查手册（2024 版）
来源：http://so.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://yb.gzmigu.cn

================================================================================
来源：http://fu.bookmarksfly.cn

【收录内容】
来源：http://au.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qq.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://me.panjiajie.cn

SQL · Bash · C · C++
来源：http://jv.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vt.colortex.cn

【使用说明】
来源：http://ey.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zp.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yc.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rx.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ko.yuntaijiaju.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zd.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ar.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rb.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xt.wgjwhj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lj.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eu.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dz.nszjky.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sb.jianghongdianzi.cn

【文件统计】
来源：http://de.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ye.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://ox.lnxyls.cn

目  录
来源：http://fr.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://nb.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://of.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ci.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dd.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gs.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eg.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ji.shxzskj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ye.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ws.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kx.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mi.shxzskj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xv.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fp.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wz.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pp.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://db.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yb.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xu.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ci.shtwfgs.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tb.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lb.lnxyls.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://me.panjiajie.cn

================================================================================
来源：http://cv.asd995.cn

A. 基础语法与类型
来源：http://en.huixinmuqiang.cn

================================================================================
来源：http://kf.yuexingan06.cn

[A01] Hello World
来源：http://um.asd995.cn

Py:   print("Hello, World!")
来源：http://qq.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://tv.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://ly.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kx.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://ep.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://my.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://gm.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ua.newstarts.cn

[A02] 变量声明与赋值
来源：http://bc.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ej.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pv.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xm.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fy.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://fj.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://xw.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://cz.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zz.shtwfgs.cn

[A03] 常量定义
来源：http://su.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wb.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://jb.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://gn.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://xh.asd995.cn

Java: static final double PI = 3.14159;
来源：http://kt.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://ni.newstarts.cn

Ruby: PI = 3.14159
来源：http://fm.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://cl.nszjky.cn

[A04] 判断变量类型
来源：http://sq.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cv.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mz.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wu.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://xt.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bc.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rz.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sg.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://pz.panjiajie.cn

[A05] 整数除法与取模
来源：http://mf.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xt.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vs.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pn.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://aw.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://yw.9csxet.cn

Go:   7 / 2; 7 % 2
来源：http://vk.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://go.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://la.huixiangedu.cn

[A06] 字符串转数字
来源：http://pe.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://om.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yl.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lk.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dt.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pa.yuntaijiaju.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xi.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fh.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mj.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://au.shtwfgs.cn

Py:   str(42)
来源：http://ry.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://iu.hnjuh.cn

JS:   String(42); (42).toString()
来源：http://yb.yuntaijiaju.cn

TS:   String(42)
来源：http://by.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ga.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://jb.bjjhwx.cn

Ruby: 42.to_s
来源：http://ll.asd995.cn

C#:   42.ToString()
来源：http://jv.panjiajie.cn

[A08] 取整与四舍五入
来源：http://ox.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zj.9csxet.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ab.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lq.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tr.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ah.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ck.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rr.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jm.newstarts.cn

[A09] 绝对值与最大最小值
来源：http://df.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vp.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vy.lnxyls.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rm.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fu.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tk.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://av.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tf.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rp.nicolike.cn


<!-- 参考信息 -->