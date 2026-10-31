代发 wailian999

[U63] PHP：文件读写
来源：http://pe.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://om.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://bv.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://lu.haigaiapp.cn

[U65] PHP：会话
来源：http://no.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ny.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://ez.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://li.huanxung.cn

[U67] PHP：处理文件上传
来源：http://zu.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cu.521024.cn

[U68] PHP：PDO 连接
来源：http://gk.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hn.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://hb.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xf.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://ls.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zc.hahajie.cn

[U71] PHP：抛出异常
来源：http://zv.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://id.szsharing.cn

[U72] PHP：写错误日志
来源：http://dj.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://wa.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://qs.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://oy.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://de.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://sw.nicolike.cn

[U75] PHP：依赖注入
来源：http://yd.chemitech.net.cn

composer require psr/container
来源：http://ei.bjjhwx.cn

[U76] PHP：简单路由
来源：http://gh.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jp.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://tn.bookmarksfly.cn

composer require twig/twig
来源：http://ua.haigaiapp.cn

[U78] PHP：单元测试
来源：http://cg.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://mq.huanxung.cn

[U79] PHP：静态分析
来源：http://qt.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://fx.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://tu.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://re.yuexingan06.cn

[U81] JS：初始化项目
来源：http://ir.yuexingan06.cn

npm init -y;  npm i express
来源：http://ov.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://rd.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bj.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://sd.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mk.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://ip.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vv.panjiajie.cn

[U85] JS：可选链
来源：http://xq.shxzukj.cn

a?.b?.c
来源：http://wp.szxytkj.cn

[U86] JS：空值合并
来源：http://em.wgjwhj.cn

a ?? b
来源：http://ju.wgjwhj.cn

[U87] JS：解构默认值
来源：http://rw.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://dq.asd995.cn

[U88] JS：对象展开合并
来源：http://yj.lnxyls.cn

{ ...a, ...b }
来源：http://ae.hnjuh.cn

[U89] JS：数组去重
来源：http://ot.lnxyls.cn

[...new Set(arr)]
来源：http://hm.nicolike.cn

[U90] JS：数字数组排序
来源：http://ns.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://tm.panjiajie.cn

[U91] JS：对象键值遍历
来源：http://xw.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oc.bjjhwx.cn

[U92] JS：深拷贝
来源：http://rp.colortex.cn

structuredClone(obj)
来源：http://dq.newstarts.cn

[U93] JS：模板字符串
来源：http://kq.shxzskj.cn

`共 ${n} 条`
来源：http://hq.jctech888.com.cn

[U94] JS：箭头函数
来源：http://pi.newstarts.cn

const double = x => x * 2;
来源：http://ur.hahajie.cn

[U95] JS：Promise 包装
来源：http://mq.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://wy.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://hk.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vx.colortex.cn

[U97] JS：并发请求
来源：http://tn.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hv.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://ip.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jj.wgjwhj.cn

[U99] JS：事件监听
来源：http://hd.nicolike.cn

el.addEventListener("click", e => {})
来源：http://xl.gzmigu.cn

[U100] JS：DOM 查询
来源：http://rf.gzmigu.cn

document.querySelector(".item")
来源：http://yd.9csxet.cn

[U101] JS：classList 操作
来源：http://ym.haigaiapp.cn

el.classList.toggle("active")
来源：http://yy.szsharing.cn

[U102] JS：本地存储
来源：http://yz.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pe.9csxet.cn

[U103] JS：定时器
来源：http://ov.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://on.yuntaijiaju.cn

[U104] JS：防抖
来源：http://tb.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://da.nszjky.cn

[U105] JS：节流
来源：http://io.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kr.hahajie.cn

[U106] JS：日期格式化
来源：http://tq.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ez.huixiangedu.cn

[U107] JS：数字千分位
来源：http://zw.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ue.hnjuh.cn

[U108] JS：随机整数
来源：http://as.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bx.wgjwhj.cn

[U109] JS：数组分组
来源：http://vt.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://ej.yuexingan06.cn

[U110] JS：数组分块
来源：http://yo.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rq.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://jp.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://dh.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://jr.nszjky.cn

"7".padStart(3, "0")
来源：http://pj.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://pt.521024.cn

s.replaceAll("a", "b")
来源：http://nq.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://zn.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cb.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://th.yuexingan06.cn

crypto.randomUUID()
来源：http://ru.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://nc.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://th.asd995.cn

[U117] JS：单元测试
来源：http://og.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://hf.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://by.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://jx.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://ia.newstarts.cn

npx vite build
来源：http://tf.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://lk.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://tj.szsharing.cn

================================================================================
来源：http://hw.521024.cn

统计汇总
来源：http://pj.nicolike.cn

================================================================================
来源：http://eh.yuexingan06.cn

按语言统计（条）：
来源：http://eb.hahajie.cn

Python ......... 252
来源：http://ax.yuexingan06.cn

PHP ............ 252
来源：http://rk.hnjuh.cn

JavaScript ..... 252
来源：http://jo.shxzukj.cn

TypeScript ..... 212
来源：http://wc.9csxet.cn

Java ........... 212
来源：http://nb.newstarts.cn

Go ............. 212
来源：http://qo.haigaiapp.cn

Ruby ........... 212
来源：http://ng.newstarts.cn

C# ............. 212
来源：http://bw.521024.cn

C .............. 30
来源：http://cf.asd995.cn

C++ ............ 30
来源：http://jf.asd995.cn

SQL ............ 90
来源：http://su.nszjky.cn

Bash ........... 80
来源：http://ju.hahajie.cn

Kotlin ......... 15
来源：http://sd.huixinmuqiang.cn

Swift .......... 15
来源：http://am.newstarts.cn

Lua ............ 10
来源：http://tz.wgjwhj.cn

Perl ........... 10
来源：http://yd.nszjky.cn

Scala .......... 10
来源：http://df.bookmarksfly.cn

------------------------------------
来源：http://eb.newstarts.cn

合计 ........... 2106 条
来源：http://ae.bjjhwx.cn

按章节统计：
来源：http://fj.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yz.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ca.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://if.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dm.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ug.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://az.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pk.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nd.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zn.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yx.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wq.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tn.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kw.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lm.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qh.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bi.9csxet.cn

Q SQL 专题                              90
来源：http://io.shtwfgs.cn

R Bash 专题                             80
来源：http://dj.521024.cn

S C / C++ 专题                          60
来源：http://sd.panjiajie.cn

T 其他语言补充                          60
来源：http://ac.szxytkj.cn

U 高频实用片段                         120
来源：http://sq.haigaiapp.cn

------------------------------------
来源：http://bq.yuexingan06.cn

合计                                  2106 条
来源：http://ys.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://pu.nszjky.cn

使用提醒
来源：http://sk.colortex.cn

--------------------------------------------------------------------------------
来源：http://zi.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ro.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dp.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vf.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mr.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zo.shxzskj.cn

—— 文件结束 ——
来源：http://ya.yuexingan06.cn

================================================================================
来源：http://gs.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://nl.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://qg.huixinmuqiang.cn

================================================================================
来源：http://ln.nszjky.cn

【收录内容】
来源：http://lb.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ri.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zq.panjiajie.cn

SQL · Bash · C · C++
来源：http://cm.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rf.jianghongdianzi.cn

【使用说明】
来源：http://dd.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hi.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nq.colortex.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yh.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gr.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rw.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pu.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wm.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://da.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kw.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ex.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sk.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sx.nszjky.cn

【文件统计】
来源：http://po.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qn.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ls.lnxyls.cn

目  录
来源：http://sv.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://dx.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wb.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ha.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gy.9csxet.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ho.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vc.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zj.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hy.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mb.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xo.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rw.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ge.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ox.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://if.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ux.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hf.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://we.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vj.huixiangedu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tg.panjiajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wr.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://db.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ft.bookmarksfly.cn

================================================================================
来源：http://hd.gzmigu.cn

A. 基础语法与类型
来源：http://tc.huanxung.cn

================================================================================
来源：http://kh.shxzukj.cn

[A01] Hello World
来源：http://ny.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://re.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://rw.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://wp.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://db.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://lf.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://rd.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://pe.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.colortex.cn

[A02] 变量声明与赋值
来源：http://is.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ep.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hn.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wa.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fv.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://pj.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://vu.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://dj.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ke.nszjky.cn

[A03] 常量定义
来源：http://lq.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ez.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://ux.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://cw.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://jx.asd995.cn

Java: static final double PI = 3.14159;
来源：http://el.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://wp.huanxung.cn

Ruby: PI = 3.14159
来源：http://lm.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://ce.lnxyls.cn

[A04] 判断变量类型
来源：http://wr.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cy.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hn.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tx.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://jv.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ls.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pv.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://it.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://aw.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://ku.szxytkj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://si.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rz.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hn.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vo.nszjky.cn

Java: 7 / 2; 7 % 2
来源：http://bz.muxihuayi.cn

Go:   7 / 2; 7 % 2
来源：http://rx.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://hc.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://gd.yuexingan06.cn

[A06] 字符串转数字
来源：http://lm.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://tn.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dh.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ty.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zi.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dj.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://an.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ou.chemitech.net.cn

[A07] 数字转字符串
来源：http://va.huixinmuqiang.cn

Py:   str(42)
来源：http://iz.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://ol.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://nh.521024.cn

TS:   String(42)
来源：http://uu.shtwfgs.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gv.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://ze.yuexingan06.cn

Ruby: 42.to_s
来源：http://dj.huixiangedu.cn

C#:   42.ToString()
来源：http://nu.shxzukj.cn

[A08] 取整与四舍五入
来源：http://dt.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gs.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wj.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sm.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kn.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yg.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ah.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pr.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jl.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://it.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cl.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ba.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://il.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vm.szsharing.cn


<!-- 参考信息 -->