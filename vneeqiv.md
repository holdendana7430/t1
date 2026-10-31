代发 wailian999

[U61] PHP：正则
来源：http://lg.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xs.nicolike.cn

[U62] PHP：日期对象
来源：http://vu.521024.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ov.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://sf.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xt.shxzukj.cn

[U64] PHP：目录遍历
来源：http://jr.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://tt.huanxung.cn

[U65] PHP：会话
来源：http://wz.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ua.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://ft.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qi.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://pi.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qm.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://gl.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ej.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://pr.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://de.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://bg.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zi.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://dk.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://dw.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://yi.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://uu.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://ec.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://nx.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://ed.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://hp.hahajie.cn

[U75] PHP：依赖注入
来源：http://wx.yuexingan06.cn

composer require psr/container
来源：http://cy.haigaiapp.cn

[U76] PHP：简单路由
来源：http://lj.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pk.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://ky.hahajie.cn

composer require twig/twig
来源：http://jb.jctech888.com.cn

[U78] PHP：单元测试
来源：http://pl.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://if.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://dp.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://ol.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://kb.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yp.nicolike.cn

[U81] JS：初始化项目
来源：http://pe.yuexingan06.cn

npm init -y;  npm i express
来源：http://zv.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://ia.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ys.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://sj.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lo.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://as.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ay.huanxung.cn

[U85] JS：可选链
来源：http://dc.muxihuayi.cn

a?.b?.c
来源：http://pf.chemitech.net.cn

[U86] JS：空值合并
来源：http://kc.lnxyls.cn

a ?? b
来源：http://nn.nszjky.cn

[U87] JS：解构默认值
来源：http://ks.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://mk.shxzskj.cn

[U88] JS：对象展开合并
来源：http://ph.huixinmuqiang.cn

{ ...a, ...b }
来源：http://lf.hnjuh.cn

[U89] JS：数组去重
来源：http://cn.huanxung.cn

[...new Set(arr)]
来源：http://ld.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://jn.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://nj.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://el.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mp.yuexingan06.cn

[U92] JS：深拷贝
来源：http://oz.shxzskj.cn

structuredClone(obj)
来源：http://wp.asd995.cn

[U93] JS：模板字符串
来源：http://ms.colortex.cn

`共 ${n} 条`
来源：http://zt.hnjuh.cn

[U94] JS：箭头函数
来源：http://zj.lnxyls.cn

const double = x => x * 2;
来源：http://jp.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://zp.521024.cn

new Promise((resolve, reject) => {})
来源：http://zs.nszjky.cn

[U96] JS：async/await 与异常
来源：http://yx.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hl.nszjky.cn

[U97] JS：并发请求
来源：http://yo.huanxung.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ty.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://uk.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mv.nicolike.cn

[U99] JS：事件监听
来源：http://ug.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://zo.shxzskj.cn

[U100] JS：DOM 查询
来源：http://hi.bookmarksfly.cn

document.querySelector(".item")
来源：http://we.wgjwhj.cn

[U101] JS：classList 操作
来源：http://ig.newstarts.cn

el.classList.toggle("active")
来源：http://lb.shxzukj.cn

[U102] JS：本地存储
来源：http://ml.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rv.nicolike.cn

[U103] JS：定时器
来源：http://wc.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xm.haigaiapp.cn

[U104] JS：防抖
来源：http://xn.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vn.newstarts.cn

[U105] JS：节流
来源：http://qo.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qr.newstarts.cn

[U106] JS：日期格式化
来源：http://ad.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://go.haigaiapp.cn

[U107] JS：数字千分位
来源：http://mn.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oh.hnjuh.cn

[U108] JS：随机整数
来源：http://hv.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kp.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://tg.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://vw.jctech888.com.cn

[U110] JS：数组分块
来源：http://ci.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tn.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://sw.521024.cn

new Map(Object.entries(obj))
来源：http://nc.panjiajie.cn

[U112] JS：字符串补位
来源：http://lz.yuexingan06.cn

"7".padStart(3, "0")
来源：http://pc.asd995.cn

[U113] JS：正则替换全部
来源：http://cq.huanxung.cn

s.replaceAll("a", "b")
来源：http://ks.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://de.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oo.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://qj.yuexingan06.cn

crypto.randomUUID()
来源：http://lj.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://yp.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://nc.newstarts.cn

[U117] JS：单元测试
来源：http://za.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://hx.newstarts.cn

[U118] JS：开发服务器
来源：http://sx.colortex.cn

npm i -D vite;  npx vite
来源：http://co.hahajie.cn

[U119] JS：生产构建
来源：http://zo.yuntaijiaju.cn

npx vite build
来源：http://cg.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://nl.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://it.lnxyls.cn

================================================================================
来源：http://xe.lnxyls.cn

统计汇总
来源：http://un.shtwfgs.cn

================================================================================
来源：http://io.asd995.cn

按语言统计（条）：
来源：http://kq.jctech888.com.cn

Python ......... 252
来源：http://uf.asd995.cn

PHP ............ 252
来源：http://il.shxzukj.cn

JavaScript ..... 252
来源：http://iu.shxzukj.cn

TypeScript ..... 212
来源：http://mm.haigaiapp.cn

Java ........... 212
来源：http://pi.jianghongdianzi.cn

Go ............. 212
来源：http://uo.wgjwhj.cn

Ruby ........... 212
来源：http://ed.haigaiapp.cn

C# ............. 212
来源：http://sh.szsharing.cn

C .............. 30
来源：http://sl.wgjwhj.cn

C++ ............ 30
来源：http://ky.yuntaijiaju.cn

SQL ............ 90
来源：http://qj.nicolike.cn

Bash ........... 80
来源：http://br.szxytkj.cn

Kotlin ......... 15
来源：http://xb.nicolike.cn

Swift .......... 15
来源：http://ld.huixiangedu.cn

Lua ............ 10
来源：http://rd.hnjuh.cn

Perl ........... 10
来源：http://az.asd995.cn

Scala .......... 10
来源：http://yj.lnxyls.cn

------------------------------------
来源：http://nb.colortex.cn

合计 ........... 2106 条
来源：http://rn.panjiajie.cn

按章节统计：
来源：http://gx.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lg.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iv.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yh.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://po.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ka.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xz.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hg.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ru.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fm.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fs.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cv.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kl.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pu.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eq.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://of.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ch.shxzskj.cn

Q SQL 专题                              90
来源：http://md.szxytkj.cn

R Bash 专题                             80
来源：http://gp.gzmigu.cn

S C / C++ 专题                          60
来源：http://qs.bjjhwx.cn

T 其他语言补充                          60
来源：http://gh.shtwfgs.cn

U 高频实用片段                         120
来源：http://rf.huixinmuqiang.cn

------------------------------------
来源：http://jj.colortex.cn

合计                                  2106 条
来源：http://yn.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ij.szxytkj.cn

使用提醒
来源：http://yg.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://mq.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cm.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rv.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dd.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://eu.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pc.asd995.cn

—— 文件结束 ——
来源：http://rz.huixiangedu.cn

================================================================================
来源：http://qs.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://pi.521024.cn

Common Programming Examples Cheat Book
来源：http://ku.asd995.cn

================================================================================
来源：http://la.gzmigu.cn

【收录内容】
来源：http://xy.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gq.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jo.wgjwhj.cn

SQL · Bash · C · C++
来源：http://on.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sf.huixiangedu.cn

【使用说明】
来源：http://qx.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nk.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ax.huixinmuqiang.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ke.newstarts.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dk.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nj.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://so.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jt.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wa.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ry.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://el.huixinmuqiang.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mi.bookmarksfly.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vu.wgjwhj.cn

【文件统计】
来源：http://zq.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ys.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://rz.lnxyls.cn

目  录
来源：http://sw.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://dm.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bc.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mf.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jd.lnxyls.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wh.asd995.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ga.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zm.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://az.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kc.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fl.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wr.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ym.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zs.chemitech.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yy.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ta.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gd.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zz.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ki.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yl.panjiajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kq.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pk.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gg.chemitech.net.cn

================================================================================
来源：http://ot.shxzukj.cn

A. 基础语法与类型
来源：http://xd.gzmigu.cn

================================================================================
来源：http://zv.szxytkj.cn

[A01] Hello World
来源：http://zd.huanxung.cn

Py:   print("Hello, World!")
来源：http://br.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://we.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://ae.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sa.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://kc.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://za.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://ce.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rl.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://le.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://on.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ay.nicolike.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dp.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sp.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://yy.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://cr.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://on.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jh.jianghongdianzi.cn

[A03] 常量定义
来源：http://wl.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cs.huixinmuqiang.cn

PHP:  const PI = 3.14159;
来源：http://al.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://hr.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://et.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://tc.lnxyls.cn

Go:   const PI = 3.14159
来源：http://qh.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://qg.nszjky.cn

C#:   const double PI = 3.14159;
来源：http://tc.bookmarksfly.cn

[A04] 判断变量类型
来源：http://mh.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vj.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sp.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wn.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://ri.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tu.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vd.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mm.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://xi.asd995.cn

[A05] 整数除法与取模
来源：http://uy.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://im.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pg.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ba.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fi.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://zs.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://el.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://zc.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://lg.shxzukj.cn

[A06] 字符串转数字
来源：http://zu.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://ug.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bw.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vx.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fy.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rg.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wb.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jy.wgjwhj.cn

[A07] 数字转字符串
来源：http://ag.colortex.cn

Py:   str(42)
来源：http://wp.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://du.huanxung.cn

JS:   String(42); (42).toString()
来源：http://hx.haigaiapp.cn

TS:   String(42)
来源：http://oe.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xi.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://xx.colortex.cn

Ruby: 42.to_s
来源：http://jm.chemitech.net.cn

C#:   42.ToString()
来源：http://ig.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://xz.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ht.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fb.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jl.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nk.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fe.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qi.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vm.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ry.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://zb.gzmigu.cn


<!-- 参考信息 -->