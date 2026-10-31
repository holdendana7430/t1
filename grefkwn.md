代发 wailian999

[U65] PHP：会话
来源：http://kt.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://id.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://eo.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cv.szsharing.cn

[U67] PHP：处理文件上传
来源：http://xw.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qh.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://tx.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jv.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://hc.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xf.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://ts.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zl.huanxung.cn

[U71] PHP：抛出异常
来源：http://md.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://hx.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://uf.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://dr.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://io.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://qd.asd995.cn

[U74] PHP：读取环境变量
来源：http://iq.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://cy.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://nm.chemitech.net.cn

composer require psr/container
来源：http://ii.9csxet.cn

[U76] PHP：简单路由
来源：http://jg.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rb.shxzukj.cn

[U77] PHP：模板渲染
来源：http://pv.muxihuayi.cn

composer require twig/twig
来源：http://zw.bjjhwx.cn

[U78] PHP：单元测试
来源：http://fs.521024.cn

composer require --dev phpunit/phpunit
来源：http://hw.chemitech.net.cn

[U79] PHP：静态分析
来源：http://jj.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://qw.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://zm.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yb.hnjuh.cn

[U81] JS：初始化项目
来源：http://xd.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://av.521024.cn

[U82] JS：package.json 脚本
来源：http://mo.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eq.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://jw.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ku.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://pm.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://py.bjjhwx.cn

[U85] JS：可选链
来源：http://fg.wgjwhj.cn

a?.b?.c
来源：http://kh.huanxung.cn

[U86] JS：空值合并
来源：http://xt.shxzskj.cn

a ?? b
来源：http://io.huanxung.cn

[U87] JS：解构默认值
来源：http://uz.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://mt.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://og.wgjwhj.cn

{ ...a, ...b }
来源：http://zd.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://nm.wgjwhj.cn

[...new Set(arr)]
来源：http://ob.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://rj.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://nl.newstarts.cn

[U91] JS：对象键值遍历
来源：http://zu.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mp.nszjky.cn

[U92] JS：深拷贝
来源：http://ul.jctech888.com.cn

structuredClone(obj)
来源：http://eq.shxzukj.cn

[U93] JS：模板字符串
来源：http://gz.muxihuayi.cn

`共 ${n} 条`
来源：http://ce.jctech888.com.cn

[U94] JS：箭头函数
来源：http://ro.gzmigu.cn

const double = x => x * 2;
来源：http://vd.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://wc.asd995.cn

new Promise((resolve, reject) => {})
来源：http://us.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://ct.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vt.bjjhwx.cn

[U97] JS：并发请求
来源：http://jz.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zc.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://hr.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://md.521024.cn

[U99] JS：事件监听
来源：http://bu.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://sq.521024.cn

[U100] JS：DOM 查询
来源：http://ly.lnxyls.cn

document.querySelector(".item")
来源：http://cw.hnjuh.cn

[U101] JS：classList 操作
来源：http://di.asd995.cn

el.classList.toggle("active")
来源：http://bx.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://xd.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kq.jctech888.com.cn

[U103] JS：定时器
来源：http://gq.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zi.szxytkj.cn

[U104] JS：防抖
来源：http://rg.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://id.colortex.cn

[U105] JS：节流
来源：http://mm.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lc.yuexingan06.cn

[U106] JS：日期格式化
来源：http://te.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lf.asd995.cn

[U107] JS：数字千分位
来源：http://qf.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xv.shxzukj.cn

[U108] JS：随机整数
来源：http://cf.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xm.nicolike.cn

[U109] JS：数组分组
来源：http://ac.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://nn.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://wl.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hd.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://zh.gzmigu.cn

new Map(Object.entries(obj))
来源：http://cm.shtwfgs.cn

[U112] JS：字符串补位
来源：http://gl.panjiajie.cn

"7".padStart(3, "0")
来源：http://nm.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://nn.huanxung.cn

s.replaceAll("a", "b")
来源：http://lb.huanxung.cn

[U114] JS：JSON 深比较
来源：http://mw.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://it.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://vu.wgjwhj.cn

crypto.randomUUID()
来源：http://xz.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://ew.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://rj.chemitech.net.cn

[U117] JS：单元测试
来源：http://pd.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://mc.jctech888.com.cn

[U118] JS：开发服务器
来源：http://df.shxzskj.cn

npm i -D vite;  npx vite
来源：http://uj.asd995.cn

[U119] JS：生产构建
来源：http://ny.chemitech.net.cn

npx vite build
来源：http://oe.colortex.cn

[U120] JS：读取环境变量（Vite）
来源：http://ow.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://dh.huixinmuqiang.cn

================================================================================
来源：http://yi.jctech888.com.cn

统计汇总
来源：http://hc.9csxet.cn

================================================================================
来源：http://om.haigaiapp.cn

按语言统计（条）：
来源：http://ct.shtwfgs.cn

Python ......... 252
来源：http://pi.bjjhwx.cn

PHP ............ 252
来源：http://ee.colortex.cn

JavaScript ..... 252
来源：http://yt.chemitech.net.cn

TypeScript ..... 212
来源：http://po.panjiajie.cn

Java ........... 212
来源：http://sy.shxzskj.cn

Go ............. 212
来源：http://ox.asd995.cn

Ruby ........... 212
来源：http://ku.szxytkj.cn

C# ............. 212
来源：http://ku.yuntaijiaju.cn

C .............. 30
来源：http://ey.huixinmuqiang.cn

C++ ............ 30
来源：http://lu.jianghongdianzi.cn

SQL ............ 90
来源：http://mu.shxzukj.cn

Bash ........... 80
来源：http://kx.newstarts.cn

Kotlin ......... 15
来源：http://zu.huixinmuqiang.cn

Swift .......... 15
来源：http://ji.huixiangedu.cn

Lua ............ 10
来源：http://qs.bjjhwx.cn

Perl ........... 10
来源：http://xj.nszjky.cn

Scala .......... 10
来源：http://zq.521024.cn

------------------------------------
来源：http://so.bookmarksfly.cn

合计 ........... 2106 条
来源：http://jm.gzmigu.cn

按章节统计：
来源：http://pe.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gz.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ik.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qw.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dq.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uz.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tf.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iq.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kt.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jt.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lk.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ck.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ux.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zr.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kw.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tm.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aw.lnxyls.cn

Q SQL 专题                              90
来源：http://et.colortex.cn

R Bash 专题                             80
来源：http://tt.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://ln.jctech888.com.cn

T 其他语言补充                          60
来源：http://ro.szsharing.cn

U 高频实用片段                         120
来源：http://av.newstarts.cn

------------------------------------
来源：http://fi.gzmigu.cn

合计                                  2106 条
来源：http://lb.nszjky.cn

--------------------------------------------------------------------------------
来源：http://el.shtwfgs.cn

使用提醒
来源：http://qk.nszjky.cn

--------------------------------------------------------------------------------
来源：http://fa.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://je.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ge.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qu.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xf.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://il.521024.cn

—— 文件结束 ——
来源：http://hu.szxytkj.cn

================================================================================
来源：http://mj.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://dk.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://ut.gzmigu.cn

================================================================================
来源：http://ca.nszjky.cn

【收录内容】
来源：http://cz.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nd.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hl.chemitech.net.cn

SQL · Bash · C · C++
来源：http://fe.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dy.lnxyls.cn

【使用说明】
来源：http://ma.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://on.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vk.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ul.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kw.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qs.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vj.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kf.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lc.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oo.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://md.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xv.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iz.yuntaijiaju.cn

【文件统计】
来源：http://av.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://de.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ib.nszjky.cn

目  录
来源：http://yl.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://kk.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qd.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://we.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qh.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ho.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://my.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ey.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ny.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://il.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lp.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tz.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pz.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://le.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uw.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://da.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mk.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gv.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ng.shxzukj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tj.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ul.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lr.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zp.9csxet.cn

================================================================================
来源：http://jx.newstarts.cn

A. 基础语法与类型
来源：http://hc.lnxyls.cn

================================================================================
来源：http://bd.jianghongdianzi.cn

[A01] Hello World
来源：http://zp.szsharing.cn

Py:   print("Hello, World!")
来源：http://fh.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://ft.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://kl.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://po.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://xl.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://is.521024.cn

Ruby: puts "Hello, World!"
来源：http://hi.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rq.nicolike.cn

[A02] 变量声明与赋值
来源：http://pj.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ye.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ji.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fe.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oo.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://kj.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://sl.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://fe.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ou.huixiangedu.cn

[A03] 常量定义
来源：http://ie.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tu.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://fl.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://yp.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://vq.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://aa.lnxyls.cn

Go:   const PI = 3.14159
来源：http://vg.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://ud.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://oj.bookmarksfly.cn

[A04] 判断变量类型
来源：http://tm.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://us.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gj.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nx.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://al.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mf.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rh.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://te.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://je.bjjhwx.cn

[A05] 整数除法与取模
来源：http://xc.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lm.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ie.haigaiapp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tk.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qc.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://hm.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://kk.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://my.huixinmuqiang.cn

C#:   7 / 2; 7 % 2
来源：http://bj.wgjwhj.cn

[A06] 字符串转数字
来源：http://kd.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://qz.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fs.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nn.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ul.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ns.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ag.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bz.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hk.shtwfgs.cn

[A07] 数字转字符串
来源：http://mu.newstarts.cn

Py:   str(42)
来源：http://uh.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://wp.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://ox.shxzukj.cn

TS:   String(42)
来源：http://yx.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tz.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://au.nszjky.cn

Ruby: 42.to_s
来源：http://hh.huanxung.cn

C#:   42.ToString()
来源：http://wy.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://nf.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fs.huixinmuqiang.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pq.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ca.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rp.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jk.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rz.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tj.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://go.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://fu.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yi.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tb.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ro.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://np.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bx.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cd.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://on.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rb.haigaiapp.cn


<!-- 参考信息 -->