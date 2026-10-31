代发 wailian999

[U65] PHP：会话
来源：http://gf.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gw.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://ge.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xw.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://wq.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dd.nszjky.cn

[U68] PHP：PDO 连接
来源：http://hd.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kx.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://tn.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kj.nszjky.cn

[U70] PHP：PDO 事务
来源：http://cu.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eo.newstarts.cn

[U71] PHP：抛出异常
来源：http://sf.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://hw.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://qx.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://uf.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://ji.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://sq.nicolike.cn

[U74] PHP：读取环境变量
来源：http://sk.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://ja.shtwfgs.cn

[U75] PHP：依赖注入
来源：http://ru.shxzskj.cn

composer require psr/container
来源：http://pi.hahajie.cn

[U76] PHP：简单路由
来源：http://ji.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gk.shxzskj.cn

[U77] PHP：模板渲染
来源：http://mp.jianghongdianzi.cn

composer require twig/twig
来源：http://ik.521024.cn

[U78] PHP：单元测试
来源：http://vj.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://mb.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://zm.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://io.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://sj.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qy.huixiangedu.cn

[U81] JS：初始化项目
来源：http://wb.chemitech.net.cn

npm init -y;  npm i express
来源：http://as.521024.cn

[U82] JS：package.json 脚本
来源：http://xl.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nu.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://um.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://be.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://ju.huanxung.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bw.huixiangedu.cn

[U85] JS：可选链
来源：http://ic.hahajie.cn

a?.b?.c
来源：http://rv.muxihuayi.cn

[U86] JS：空值合并
来源：http://vz.9csxet.cn

a ?? b
来源：http://gl.9csxet.cn

[U87] JS：解构默认值
来源：http://vj.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://pn.asd995.cn

[U88] JS：对象展开合并
来源：http://gq.yuntaijiaju.cn

{ ...a, ...b }
来源：http://xl.9csxet.cn

[U89] JS：数组去重
来源：http://gu.huixinmuqiang.cn

[...new Set(arr)]
来源：http://jg.nszjky.cn

[U90] JS：数字数组排序
来源：http://ss.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://eo.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://fy.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fg.huixiangedu.cn

[U92] JS：深拷贝
来源：http://yh.shxzukj.cn

structuredClone(obj)
来源：http://px.shxzukj.cn

[U93] JS：模板字符串
来源：http://hv.yuntaijiaju.cn

`共 ${n} 条`
来源：http://fq.wgjwhj.cn

[U94] JS：箭头函数
来源：http://fw.huixinmuqiang.cn

const double = x => x * 2;
来源：http://ar.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://oe.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://ne.9csxet.cn

[U96] JS：async/await 与异常
来源：http://uw.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ee.521024.cn

[U97] JS：并发请求
来源：http://qs.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://up.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://jn.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mp.bookmarksfly.cn

[U99] JS：事件监听
来源：http://yh.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://ew.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://vf.hahajie.cn

document.querySelector(".item")
来源：http://yu.521024.cn

[U101] JS：classList 操作
来源：http://sw.huanxung.cn

el.classList.toggle("active")
来源：http://tq.asd995.cn

[U102] JS：本地存储
来源：http://ei.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dc.jctech888.com.cn

[U103] JS：定时器
来源：http://xw.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xm.shxzskj.cn

[U104] JS：防抖
来源：http://wk.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://az.lnxyls.cn

[U105] JS：节流
来源：http://ru.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ec.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://qg.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bj.newstarts.cn

[U107] JS：数字千分位
来源：http://gi.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ng.hnjuh.cn

[U108] JS：随机整数
来源：http://bt.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gm.haigaiapp.cn

[U109] JS：数组分组
来源：http://jp.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://ux.huixiangedu.cn

[U110] JS：数组分块
来源：http://ke.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vr.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://nx.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://pn.panjiajie.cn

[U112] JS：字符串补位
来源：http://rq.shtwfgs.cn

"7".padStart(3, "0")
来源：http://wq.szsharing.cn

[U113] JS：正则替换全部
来源：http://dn.szsharing.cn

s.replaceAll("a", "b")
来源：http://nb.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://na.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gq.nszjky.cn

[U115] JS：生成 UUID
来源：http://hg.asd995.cn

crypto.randomUUID()
来源：http://vm.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://ax.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://sm.jctech888.com.cn

[U117] JS：单元测试
来源：http://sa.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://gq.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://rm.newstarts.cn

npm i -D vite;  npx vite
来源：http://xj.hahajie.cn

[U119] JS：生产构建
来源：http://tn.yuntaijiaju.cn

npx vite build
来源：http://bg.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://ji.521024.cn

import.meta.env.VITE_API_URL
来源：http://xp.yuntaijiaju.cn

================================================================================
来源：http://oj.wgjwhj.cn

统计汇总
来源：http://bs.nszjky.cn

================================================================================
来源：http://nj.shxzskj.cn

按语言统计（条）：
来源：http://qj.bjjhwx.cn

Python ......... 252
来源：http://km.szsharing.cn

PHP ............ 252
来源：http://yd.9csxet.cn

JavaScript ..... 252
来源：http://nx.muxihuayi.cn

TypeScript ..... 212
来源：http://yu.panjiajie.cn

Java ........... 212
来源：http://cr.521024.cn

Go ............. 212
来源：http://sw.hnjuh.cn

Ruby ........... 212
来源：http://eq.gzmigu.cn

C# ............. 212
来源：http://nj.huanxung.cn

C .............. 30
来源：http://zv.huixinmuqiang.cn

C++ ............ 30
来源：http://oo.lnxyls.cn

SQL ............ 90
来源：http://bx.9csxet.cn

Bash ........... 80
来源：http://tp.nszjky.cn

Kotlin ......... 15
来源：http://tf.9csxet.cn

Swift .......... 15
来源：http://rp.521024.cn

Lua ............ 10
来源：http://ga.huixinmuqiang.cn

Perl ........... 10
来源：http://fw.haigaiapp.cn

Scala .......... 10
来源：http://gj.shtwfgs.cn

------------------------------------
来源：http://ad.nicolike.cn

合计 ........... 2106 条
来源：http://rz.szxytkj.cn

按章节统计：
来源：http://su.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hc.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yq.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aj.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fm.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ic.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wx.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zi.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://em.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bx.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gs.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dy.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mm.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://do.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://op.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ue.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://er.nszjky.cn

Q SQL 专题                              90
来源：http://fj.bookmarksfly.cn

R Bash 专题                             80
来源：http://os.shxzskj.cn

S C / C++ 专题                          60
来源：http://po.muxihuayi.cn

T 其他语言补充                          60
来源：http://ml.szsharing.cn

U 高频实用片段                         120
来源：http://de.bjjhwx.cn

------------------------------------
来源：http://ju.jianghongdianzi.cn

合计                                  2106 条
来源：http://sz.521024.cn

--------------------------------------------------------------------------------
来源：http://wq.newstarts.cn

使用提醒
来源：http://si.newstarts.cn

--------------------------------------------------------------------------------
来源：http://iw.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uq.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zr.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uo.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bj.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zi.gzmigu.cn

—— 文件结束 ——
来源：http://tt.jctech888.com.cn

================================================================================
来源：http://cl.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://ir.asd995.cn

Common Programming Examples Cheat Book
来源：http://eq.huanxung.cn

================================================================================
来源：http://bj.muxihuayi.cn

【收录内容】
来源：http://id.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nc.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cq.hahajie.cn

SQL · Bash · C · C++
来源：http://lk.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ya.hahajie.cn

【使用说明】
来源：http://cr.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ci.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fx.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bv.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vr.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bn.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dx.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uv.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hb.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ox.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sb.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://su.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fw.jianghongdianzi.cn

【文件统计】
来源：http://kx.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rw.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://px.hnjuh.cn

目  录
来源：http://jm.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://cy.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pu.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jb.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ay.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ma.jctech888.com.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bw.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mh.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ce.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ku.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yv.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hm.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xu.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yr.colortex.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pn.nicolike.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ql.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ea.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cd.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ls.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jp.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vh.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cy.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ym.jianghongdianzi.cn

================================================================================
来源：http://op.yuexingan06.cn

A. 基础语法与类型
来源：http://iy.lnxyls.cn

================================================================================
来源：http://xj.chemitech.net.cn

[A01] Hello World
来源：http://xu.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://nu.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://uu.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://mk.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nw.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://bb.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://kn.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://dh.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cj.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://nr.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mq.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lu.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xm.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bj.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://pk.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://iy.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://vx.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ul.yuntaijiaju.cn

[A03] 常量定义
来源：http://ux.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vq.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://zj.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://kw.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://jx.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://ki.colortex.cn

Go:   const PI = 3.14159
来源：http://cf.hnjuh.cn

Ruby: PI = 3.14159
来源：http://ft.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://un.huanxung.cn

[A04] 判断变量类型
来源：http://eq.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zp.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hy.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sr.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://ao.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ca.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xd.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yk.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://lr.shtwfgs.cn

[A05] 整数除法与取模
来源：http://wo.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://be.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ir.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oi.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dw.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://if.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://nb.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://ru.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://rf.hahajie.cn

[A06] 字符串转数字
来源：http://hh.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://ms.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kl.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wo.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tq.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qk.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pw.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rb.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rb.wgjwhj.cn

[A07] 数字转字符串
来源：http://pm.newstarts.cn

Py:   str(42)
来源：http://fp.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://tt.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://vh.yuntaijiaju.cn

TS:   String(42)
来源：http://ep.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yl.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://tk.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://ev.shtwfgs.cn

C#:   42.ToString()
来源：http://sj.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://ev.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://km.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://br.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kv.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bk.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sk.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xn.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mb.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wo.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://iw.nicolike.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qy.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ib.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qt.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ee.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://de.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qf.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://se.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kh.huanxung.cn


<!-- 参考信息 -->