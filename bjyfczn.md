代发 wailian999

[U63] PHP：文件读写
来源：http://gf.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hk.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://jr.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://dv.huixinmuqiang.cn

[U65] PHP：会话
来源：http://ao.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://po.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://jz.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fg.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://rs.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vo.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://ib.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cf.521024.cn

[U69] PHP：PDO 预处理
来源：http://lr.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hq.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://kc.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ud.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://ls.521024.cn

throw new RuntimeException("失败", 500);
来源：http://po.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://ph.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://ry.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://ra.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://ui.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://us.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://py.huanxung.cn

[U75] PHP：依赖注入
来源：http://fo.bjjhwx.cn

composer require psr/container
来源：http://nt.nszjky.cn

[U76] PHP：简单路由
来源：http://jx.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zk.gzmigu.cn

[U77] PHP：模板渲染
来源：http://lr.muxihuayi.cn

composer require twig/twig
来源：http://ji.newstarts.cn

[U78] PHP：单元测试
来源：http://xf.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://gl.nicolike.cn

[U79] PHP：静态分析
来源：http://sy.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://lm.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://vd.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xx.haigaiapp.cn

[U81] JS：初始化项目
来源：http://ql.9csxet.cn

npm init -y;  npm i express
来源：http://an.jctech888.com.cn

[U82] JS：package.json 脚本
来源：http://qt.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ir.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://zm.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pr.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://xs.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://na.bjjhwx.cn

[U85] JS：可选链
来源：http://tc.jianghongdianzi.cn

a?.b?.c
来源：http://ww.panjiajie.cn

[U86] JS：空值合并
来源：http://db.bjjhwx.cn

a ?? b
来源：http://ei.shtwfgs.cn

[U87] JS：解构默认值
来源：http://gm.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://sk.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://tv.bjjhwx.cn

{ ...a, ...b }
来源：http://rk.chemitech.net.cn

[U89] JS：数组去重
来源：http://si.chemitech.net.cn

[...new Set(arr)]
来源：http://gr.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://uj.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://lr.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://bv.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gp.gzmigu.cn

[U92] JS：深拷贝
来源：http://xd.bookmarksfly.cn

structuredClone(obj)
来源：http://fp.nszjky.cn

[U93] JS：模板字符串
来源：http://qq.panjiajie.cn

`共 ${n} 条`
来源：http://bc.panjiajie.cn

[U94] JS：箭头函数
来源：http://pa.jctech888.com.cn

const double = x => x * 2;
来源：http://cl.9csxet.cn

[U95] JS：Promise 包装
来源：http://gy.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://kb.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://gp.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://et.521024.cn

[U97] JS：并发请求
来源：http://mr.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kg.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://dt.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gz.wgjwhj.cn

[U99] JS：事件监听
来源：http://bx.9csxet.cn

el.addEventListener("click", e => {})
来源：http://tf.hnjuh.cn

[U100] JS：DOM 查询
来源：http://ye.muxihuayi.cn

document.querySelector(".item")
来源：http://vv.yuexingan06.cn

[U101] JS：classList 操作
来源：http://ax.szsharing.cn

el.classList.toggle("active")
来源：http://xi.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://wh.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ai.wgjwhj.cn

[U103] JS：定时器
来源：http://sa.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://so.chemitech.net.cn

[U104] JS：防抖
来源：http://gg.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vu.newstarts.cn

[U105] JS：节流
来源：http://os.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zd.szxytkj.cn

[U106] JS：日期格式化
来源：http://kg.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xa.lnxyls.cn

[U107] JS：数字千分位
来源：http://rd.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lb.shxzskj.cn

[U108] JS：随机整数
来源：http://os.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ew.jctech888.com.cn

[U109] JS：数组分组
来源：http://nh.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://zg.bookmarksfly.cn

[U110] JS：数组分块
来源：http://di.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://te.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://pm.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://rx.asd995.cn

[U112] JS：字符串补位
来源：http://ls.gzmigu.cn

"7".padStart(3, "0")
来源：http://pm.lnxyls.cn

[U113] JS：正则替换全部
来源：http://kt.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://rg.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://go.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fo.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://lg.szxytkj.cn

crypto.randomUUID()
来源：http://in.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://dp.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://zt.nicolike.cn

[U117] JS：单元测试
来源：http://yy.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://ln.yuexingan06.cn

[U118] JS：开发服务器
来源：http://pj.huanxung.cn

npm i -D vite;  npx vite
来源：http://ur.haigaiapp.cn

[U119] JS：生产构建
来源：http://me.yuntaijiaju.cn

npx vite build
来源：http://ol.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://cn.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://cl.nicolike.cn

================================================================================
来源：http://pp.hahajie.cn

统计汇总
来源：http://tg.hahajie.cn

================================================================================
来源：http://gh.521024.cn

按语言统计（条）：
来源：http://hh.chemitech.net.cn

Python ......... 252
来源：http://aw.szsharing.cn

PHP ............ 252
来源：http://ty.lnxyls.cn

JavaScript ..... 252
来源：http://xn.wgjwhj.cn

TypeScript ..... 212
来源：http://vc.muxihuayi.cn

Java ........... 212
来源：http://yx.shxzskj.cn

Go ............. 212
来源：http://oz.huixinmuqiang.cn

Ruby ........... 212
来源：http://qq.hahajie.cn

C# ............. 212
来源：http://ez.yuexingan06.cn

C .............. 30
来源：http://pl.hahajie.cn

C++ ............ 30
来源：http://lh.huixiangedu.cn

SQL ............ 90
来源：http://tj.9csxet.cn

Bash ........... 80
来源：http://pv.yuntaijiaju.cn

Kotlin ......... 15
来源：http://sr.lnxyls.cn

Swift .......... 15
来源：http://gc.szxytkj.cn

Lua ............ 10
来源：http://yy.panjiajie.cn

Perl ........... 10
来源：http://rg.9csxet.cn

Scala .......... 10
来源：http://eu.colortex.cn

------------------------------------
来源：http://pq.jctech888.com.cn

合计 ........... 2106 条
来源：http://cp.colortex.cn

按章节统计：
来源：http://gr.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rt.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ff.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qq.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wh.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fv.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qc.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fy.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gn.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mi.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lw.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ei.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xs.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fu.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cz.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://te.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gf.bjjhwx.cn

Q SQL 专题                              90
来源：http://wa.szsharing.cn

R Bash 专题                             80
来源：http://sj.chemitech.net.cn

S C / C++ 专题                          60
来源：http://tn.hnjuh.cn

T 其他语言补充                          60
来源：http://ew.521024.cn

U 高频实用片段                         120
来源：http://vm.panjiajie.cn

------------------------------------
来源：http://og.nszjky.cn

合计                                  2106 条
来源：http://dv.9csxet.cn

--------------------------------------------------------------------------------
来源：http://gv.huanxung.cn

使用提醒
来源：http://cq.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://dh.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ly.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xz.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jv.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://er.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kd.yuntaijiaju.cn

—— 文件结束 ——
来源：http://lg.9csxet.cn

================================================================================
来源：http://oy.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://al.huanxung.cn

Common Programming Examples Cheat Book
来源：http://ni.szsharing.cn

================================================================================
来源：http://hi.jctech888.com.cn

【收录内容】
来源：http://ht.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qv.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ty.9csxet.cn

SQL · Bash · C · C++
来源：http://pt.nszjky.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pz.panjiajie.cn

【使用说明】
来源：http://ya.shxzskj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vh.lnxyls.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fa.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uo.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kt.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ow.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jf.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ue.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qy.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vs.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xc.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pr.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wj.szxytkj.cn

【文件统计】
来源：http://wz.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wd.huanxung.cn

--------------------------------------------------------------------------------
来源：http://lr.yuexingan06.cn

目  录
来源：http://dv.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://fl.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ma.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rb.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bx.9csxet.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wb.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kv.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yp.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nk.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mz.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zh.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aj.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vk.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fm.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lg.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ff.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qk.asd995.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://op.szsharing.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xn.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xd.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ri.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ou.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xm.muxihuayi.cn

================================================================================
来源：http://uv.yuntaijiaju.cn

A. 基础语法与类型
来源：http://mw.muxihuayi.cn

================================================================================
来源：http://rd.haigaiapp.cn

[A01] Hello World
来源：http://tr.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://ur.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://qw.shxzukj.cn

JS:   console.log("Hello, World!");
来源：http://vt.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xf.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://gr.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://fn.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://cu.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://uq.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://hq.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pt.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oh.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rx.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wq.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://xs.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://wt.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://uc.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zu.yuexingan06.cn

[A03] 常量定义
来源：http://up.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ka.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://vy.jianghongdianzi.cn

JS:   const PI = 3.14159;
来源：http://um.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://vz.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://ny.asd995.cn

Go:   const PI = 3.14159
来源：http://jb.shxzukj.cn

Ruby: PI = 3.14159
来源：http://ue.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://hh.gzmigu.cn

[A04] 判断变量类型
来源：http://ve.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wc.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://na.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pf.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://lb.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ea.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wz.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://su.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://ht.huanxung.cn

[A05] 整数除法与取模
来源：http://zg.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kv.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ix.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ep.asd995.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ds.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://ek.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://uq.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://yu.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://xz.nicolike.cn

[A06] 字符串转数字
来源：http://hy.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://lx.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ii.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pe.huixiangedu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ck.colortex.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ka.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bv.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uq.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bl.nszjky.cn

[A07] 数字转字符串
来源：http://pw.newstarts.cn

Py:   str(42)
来源：http://at.521024.cn

PHP:  (string) 42; strval(42)
来源：http://xo.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://tv.asd995.cn

TS:   String(42)
来源：http://ka.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fn.521024.cn

Go:   strconv.Itoa(42)
来源：http://si.shxzskj.cn

Ruby: 42.to_s
来源：http://px.hnjuh.cn

C#:   42.ToString()
来源：http://az.9csxet.cn

[A08] 取整与四舍五入
来源：http://qn.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bb.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xj.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ya.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dm.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fb.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ey.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hb.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yt.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://qj.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rn.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kh.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ic.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iq.shxzukj.cn


<!-- 参考信息 -->