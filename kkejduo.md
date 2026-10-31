代发 wailian999

[U65] PHP：会话
来源：http://ft.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wf.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://sg.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dk.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://kn.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ad.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://be.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ss.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://hz.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zg.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://xv.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bj.9csxet.cn

[U71] PHP：抛出异常
来源：http://em.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://bw.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://vc.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://fo.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://oy.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://qr.newstarts.cn

[U74] PHP：读取环境变量
来源：http://pn.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://be.gzmigu.cn

[U75] PHP：依赖注入
来源：http://le.bookmarksfly.cn

composer require psr/container
来源：http://va.gzmigu.cn

[U76] PHP：简单路由
来源：http://pf.gzmigu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xb.nicolike.cn

[U77] PHP：模板渲染
来源：http://qw.haigaiapp.cn

composer require twig/twig
来源：http://at.bjjhwx.cn

[U78] PHP：单元测试
来源：http://dw.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://lj.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://rj.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://hj.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://em.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rs.jctech888.com.cn

[U81] JS：初始化项目
来源：http://gr.bookmarksfly.cn

npm init -y;  npm i express
来源：http://sx.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://gy.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bj.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://qv.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kh.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://re.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yh.huixinmuqiang.cn

[U85] JS：可选链
来源：http://uj.colortex.cn

a?.b?.c
来源：http://ev.shxzukj.cn

[U86] JS：空值合并
来源：http://zg.yuexingan06.cn

a ?? b
来源：http://ek.huixiangedu.cn

[U87] JS：解构默认值
来源：http://jn.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://yn.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://pi.hnjuh.cn

{ ...a, ...b }
来源：http://xk.bookmarksfly.cn

[U89] JS：数组去重
来源：http://jk.panjiajie.cn

[...new Set(arr)]
来源：http://dh.521024.cn

[U90] JS：数字数组排序
来源：http://kw.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://cn.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://qk.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mk.muxihuayi.cn

[U92] JS：深拷贝
来源：http://jw.jctech888.com.cn

structuredClone(obj)
来源：http://nr.asd995.cn

[U93] JS：模板字符串
来源：http://jv.jianghongdianzi.cn

`共 ${n} 条`
来源：http://dv.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://ld.chemitech.net.cn

const double = x => x * 2;
来源：http://kl.hnjuh.cn

[U95] JS：Promise 包装
来源：http://jk.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://gr.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://jj.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zo.jctech888.com.cn

[U97] JS：并发请求
来源：http://as.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ll.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://pu.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lh.shtwfgs.cn

[U99] JS：事件监听
来源：http://al.colortex.cn

el.addEventListener("click", e => {})
来源：http://io.newstarts.cn

[U100] JS：DOM 查询
来源：http://zl.shxzukj.cn

document.querySelector(".item")
来源：http://ks.shtwfgs.cn

[U101] JS：classList 操作
来源：http://dy.muxihuayi.cn

el.classList.toggle("active")
来源：http://ly.huixiangedu.cn

[U102] JS：本地存储
来源：http://zp.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zn.colortex.cn

[U103] JS：定时器
来源：http://rc.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hy.muxihuayi.cn

[U104] JS：防抖
来源：http://xp.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ti.bookmarksfly.cn

[U105] JS：节流
来源：http://fs.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vo.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://ma.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ug.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://bw.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://se.bjjhwx.cn

[U108] JS：随机整数
来源：http://cl.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://le.nicolike.cn

[U109] JS：数组分组
来源：http://fa.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://gm.huanxung.cn

[U110] JS：数组分块
来源：http://vt.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rz.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://ht.gzmigu.cn

new Map(Object.entries(obj))
来源：http://jf.9csxet.cn

[U112] JS：字符串补位
来源：http://wi.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://sn.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://ty.szxytkj.cn

s.replaceAll("a", "b")
来源：http://yz.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://fk.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ww.szsharing.cn

[U115] JS：生成 UUID
来源：http://eu.lnxyls.cn

crypto.randomUUID()
来源：http://gn.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://lk.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://rs.huixiangedu.cn

[U117] JS：单元测试
来源：http://pb.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://ii.asd995.cn

[U118] JS：开发服务器
来源：http://hu.521024.cn

npm i -D vite;  npx vite
来源：http://jz.gzmigu.cn

[U119] JS：生产构建
来源：http://qz.bookmarksfly.cn

npx vite build
来源：http://hj.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://lr.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://ow.yuntaijiaju.cn

================================================================================
来源：http://nm.colortex.cn

统计汇总
来源：http://im.nszjky.cn

================================================================================
来源：http://oh.hahajie.cn

按语言统计（条）：
来源：http://wm.shxzukj.cn

Python ......... 252
来源：http://ze.haigaiapp.cn

PHP ............ 252
来源：http://uj.jianghongdianzi.cn

JavaScript ..... 252
来源：http://mx.szsharing.cn

TypeScript ..... 212
来源：http://ux.9csxet.cn

Java ........... 212
来源：http://fa.szsharing.cn

Go ............. 212
来源：http://cf.nszjky.cn

Ruby ........... 212
来源：http://gd.9csxet.cn

C# ............. 212
来源：http://ux.521024.cn

C .............. 30
来源：http://on.wgjwhj.cn

C++ ............ 30
来源：http://ry.chemitech.net.cn

SQL ............ 90
来源：http://qy.nicolike.cn

Bash ........... 80
来源：http://io.shxzukj.cn

Kotlin ......... 15
来源：http://ba.jctech888.com.cn

Swift .......... 15
来源：http://iu.huixiangedu.cn

Lua ............ 10
来源：http://fu.nszjky.cn

Perl ........... 10
来源：http://ha.colortex.cn

Scala .......... 10
来源：http://gx.9csxet.cn

------------------------------------
来源：http://tt.panjiajie.cn

合计 ........... 2106 条
来源：http://fw.9csxet.cn

按章节统计：
来源：http://it.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tb.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yy.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qm.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://am.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vi.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://na.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ci.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ev.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tn.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pv.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://by.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ih.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kw.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jd.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rn.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xz.bookmarksfly.cn

Q SQL 专题                              90
来源：http://eq.shxzskj.cn

R Bash 专题                             80
来源：http://ot.newstarts.cn

S C / C++ 专题                          60
来源：http://xv.szxytkj.cn

T 其他语言补充                          60
来源：http://mv.hnjuh.cn

U 高频实用片段                         120
来源：http://by.haigaiapp.cn

------------------------------------
来源：http://cz.hnjuh.cn

合计                                  2106 条
来源：http://pp.szsharing.cn

--------------------------------------------------------------------------------
来源：http://kp.9csxet.cn

使用提醒
来源：http://rr.521024.cn

--------------------------------------------------------------------------------
来源：http://io.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://re.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oj.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ya.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ci.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sz.panjiajie.cn

—— 文件结束 ——
来源：http://ih.9csxet.cn

================================================================================
来源：http://bf.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://zi.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://kd.gzmigu.cn

================================================================================
来源：http://nq.panjiajie.cn

【收录内容】
来源：http://ft.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jw.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gv.asd995.cn

SQL · Bash · C · C++
来源：http://hq.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lh.muxihuayi.cn

【使用说明】
来源：http://of.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fe.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oa.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qb.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fn.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uj.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ry.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ip.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cq.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://km.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://di.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gp.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yt.yuexingan06.cn

【文件统计】
来源：http://bi.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ka.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://yr.bjjhwx.cn

目  录
来源：http://at.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://ok.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wq.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bh.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ki.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ci.asd995.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uw.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ib.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gl.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qo.yuexingan06.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fk.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://db.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ce.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hf.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pc.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zo.nicolike.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kh.hahajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qo.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fm.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wd.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yf.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jv.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gb.shtwfgs.cn

================================================================================
来源：http://to.szsharing.cn

A. 基础语法与类型
来源：http://hs.colortex.cn

================================================================================
来源：http://xp.panjiajie.cn

[A01] Hello World
来源：http://bh.lnxyls.cn

Py:   print("Hello, World!")
来源：http://ga.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://tj.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://jx.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://et.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://ss.huixinmuqiang.cn

Go:   fmt.Println("Hello, World!")
来源：http://ev.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://dx.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://uk.szsharing.cn

[A02] 变量声明与赋值
来源：http://kv.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gb.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zr.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vf.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wa.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://cb.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://uu.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://ox.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wu.hnjuh.cn

[A03] 常量定义
来源：http://qm.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ei.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://lf.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://uy.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://to.521024.cn

Java: static final double PI = 3.14159;
来源：http://pk.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://nd.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://ap.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://kh.gzmigu.cn

[A04] 判断变量类型
来源：http://nf.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cd.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ue.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kf.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://bc.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oa.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hp.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dm.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://co.9csxet.cn

[A05] 整数除法与取模
来源：http://pa.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://em.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hv.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://re.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vf.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://be.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://sp.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://as.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://ki.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://ng.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://rk.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wh.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xv.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xj.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ky.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sc.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://da.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pe.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://jn.bjjhwx.cn

Py:   str(42)
来源：http://hj.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://bs.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://zi.wgjwhj.cn

TS:   String(42)
来源：http://oq.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qi.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://lq.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://cr.chemitech.net.cn

C#:   42.ToString()
来源：http://ln.shxzskj.cn

[A08] 取整与四舍五入
来源：http://ay.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yk.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hw.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mb.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ay.lnxyls.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rh.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qg.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zw.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sa.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://sl.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jx.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gw.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gt.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kz.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cq.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qq.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wg.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ic.nicolike.cn


<!-- 参考信息 -->