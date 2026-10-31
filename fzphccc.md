代发 wailian999

[U65] PHP：会话
来源：http://ht.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vd.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://hb.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ev.szsharing.cn

[U67] PHP：处理文件上传
来源：http://ho.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xz.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://zz.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tu.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://jr.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://by.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://yt.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ys.hahajie.cn

[U71] PHP：抛出异常
来源：http://fd.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://sj.nszjky.cn

[U72] PHP：写错误日志
来源：http://gf.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://zv.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://wx.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://ca.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://sl.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://wi.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://wk.wgjwhj.cn

composer require psr/container
来源：http://lb.wgjwhj.cn

[U76] PHP：简单路由
来源：http://dd.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://td.shxzskj.cn

[U77] PHP：模板渲染
来源：http://sp.huixinmuqiang.cn

composer require twig/twig
来源：http://sk.shtwfgs.cn

[U78] PHP：单元测试
来源：http://ky.asd995.cn

composer require --dev phpunit/phpunit
来源：http://kf.huanxung.cn

[U79] PHP：静态分析
来源：http://ic.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://zy.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://we.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kp.shxzukj.cn

[U81] JS：初始化项目
来源：http://zx.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://kj.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://ix.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gc.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://ro.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ze.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://bn.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nm.wgjwhj.cn

[U85] JS：可选链
来源：http://fa.jctech888.com.cn

a?.b?.c
来源：http://ri.nszjky.cn

[U86] JS：空值合并
来源：http://db.wgjwhj.cn

a ?? b
来源：http://an.jctech888.com.cn

[U87] JS：解构默认值
来源：http://re.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://jk.szsharing.cn

[U88] JS：对象展开合并
来源：http://ok.nicolike.cn

{ ...a, ...b }
来源：http://sw.muxihuayi.cn

[U89] JS：数组去重
来源：http://aa.jctech888.com.cn

[...new Set(arr)]
来源：http://ou.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://zm.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://hl.colortex.cn

[U91] JS：对象键值遍历
来源：http://wh.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vs.szxytkj.cn

[U92] JS：深拷贝
来源：http://gf.newstarts.cn

structuredClone(obj)
来源：http://yr.jctech888.com.cn

[U93] JS：模板字符串
来源：http://bv.newstarts.cn

`共 ${n} 条`
来源：http://fi.jctech888.com.cn

[U94] JS：箭头函数
来源：http://ds.chemitech.net.cn

const double = x => x * 2;
来源：http://zk.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://hz.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://ls.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://em.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vr.colortex.cn

[U97] JS：并发请求
来源：http://jd.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lr.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://qj.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nm.yuexingan06.cn

[U99] JS：事件监听
来源：http://gz.521024.cn

el.addEventListener("click", e => {})
来源：http://le.shxzskj.cn

[U100] JS：DOM 查询
来源：http://fr.hnjuh.cn

document.querySelector(".item")
来源：http://oo.bjjhwx.cn

[U101] JS：classList 操作
来源：http://vf.colortex.cn

el.classList.toggle("active")
来源：http://xd.hahajie.cn

[U102] JS：本地存储
来源：http://so.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ph.hahajie.cn

[U103] JS：定时器
来源：http://gh.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sz.muxihuayi.cn

[U104] JS：防抖
来源：http://it.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nn.huixinmuqiang.cn

[U105] JS：节流
来源：http://sk.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wh.shxzukj.cn

[U106] JS：日期格式化
来源：http://bq.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ck.9csxet.cn

[U107] JS：数字千分位
来源：http://dn.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tn.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://it.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://py.newstarts.cn

[U109] JS：数组分组
来源：http://ja.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://hn.colortex.cn

[U110] JS：数组分块
来源：http://bp.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ha.shxzukj.cn

[U111] JS：对象转 Map
来源：http://kg.panjiajie.cn

new Map(Object.entries(obj))
来源：http://zh.lnxyls.cn

[U112] JS：字符串补位
来源：http://il.wgjwhj.cn

"7".padStart(3, "0")
来源：http://kp.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://ql.shxzskj.cn

s.replaceAll("a", "b")
来源：http://gb.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://it.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://as.shxzskj.cn

[U115] JS：生成 UUID
来源：http://ee.huixiangedu.cn

crypto.randomUUID()
来源：http://dl.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://wr.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://rx.huixiangedu.cn

[U117] JS：单元测试
来源：http://jt.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://lr.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://fa.9csxet.cn

npm i -D vite;  npx vite
来源：http://hv.521024.cn

[U119] JS：生产构建
来源：http://dh.szxytkj.cn

npx vite build
来源：http://ez.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://fw.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://cr.lnxyls.cn

================================================================================
来源：http://zi.wgjwhj.cn

统计汇总
来源：http://cx.yuntaijiaju.cn

================================================================================
来源：http://ny.shtwfgs.cn

按语言统计（条）：
来源：http://gg.huixiangedu.cn

Python ......... 252
来源：http://ib.asd995.cn

PHP ............ 252
来源：http://og.hahajie.cn

JavaScript ..... 252
来源：http://yb.nicolike.cn

TypeScript ..... 212
来源：http://bt.shtwfgs.cn

Java ........... 212
来源：http://vi.wgjwhj.cn

Go ............. 212
来源：http://sc.szxytkj.cn

Ruby ........... 212
来源：http://xf.szsharing.cn

C# ............. 212
来源：http://mz.hnjuh.cn

C .............. 30
来源：http://to.asd995.cn

C++ ............ 30
来源：http://xc.chemitech.net.cn

SQL ............ 90
来源：http://ac.shxzskj.cn

Bash ........... 80
来源：http://pl.huixinmuqiang.cn

Kotlin ......... 15
来源：http://sp.9csxet.cn

Swift .......... 15
来源：http://cf.huixinmuqiang.cn

Lua ............ 10
来源：http://hw.bookmarksfly.cn

Perl ........... 10
来源：http://pd.newstarts.cn

Scala .......... 10
来源：http://fz.nszjky.cn

------------------------------------
来源：http://ue.panjiajie.cn

合计 ........... 2106 条
来源：http://fb.asd995.cn

按章节统计：
来源：http://bb.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tb.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gk.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fk.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pe.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zb.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cs.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xb.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ts.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jp.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yy.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ge.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lf.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kb.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xv.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lu.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yf.521024.cn

Q SQL 专题                              90
来源：http://gp.hahajie.cn

R Bash 专题                             80
来源：http://mp.shxzskj.cn

S C / C++ 专题                          60
来源：http://zp.asd995.cn

T 其他语言补充                          60
来源：http://dx.colortex.cn

U 高频实用片段                         120
来源：http://oa.panjiajie.cn

------------------------------------
来源：http://ap.521024.cn

合计                                  2106 条
来源：http://ru.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://vq.nicolike.cn

使用提醒
来源：http://xj.szsharing.cn

--------------------------------------------------------------------------------
来源：http://kj.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cm.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zk.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pl.9csxet.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bb.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xj.asd995.cn

—— 文件结束 ——
来源：http://xq.9csxet.cn

================================================================================
来源：http://ek.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://ny.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://td.huixiangedu.cn

================================================================================
来源：http://kf.chemitech.net.cn

【收录内容】
来源：http://jq.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cw.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nn.nicolike.cn

SQL · Bash · C · C++
来源：http://ho.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cf.haigaiapp.cn

【使用说明】
来源：http://gy.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gz.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vk.jianghongdianzi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ca.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gq.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ok.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ef.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://da.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://aw.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lo.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vn.nszjky.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tz.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nb.yuntaijiaju.cn

【文件统计】
来源：http://ey.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gs.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ox.huanxung.cn

目  录
来源：http://px.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://bk.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://al.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ra.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qn.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xg.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dm.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wz.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://th.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hp.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pk.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ak.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ne.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mb.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mx.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uv.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ag.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jz.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ld.huixiangedu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hb.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oj.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tu.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tv.yuexingan06.cn

================================================================================
来源：http://el.jctech888.com.cn

A. 基础语法与类型
来源：http://vm.hahajie.cn

================================================================================
来源：http://lb.hnjuh.cn

[A01] Hello World
来源：http://vq.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://pm.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://ss.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://hr.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ao.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://sx.bjjhwx.cn

Go:   fmt.Println("Hello, World!")
来源：http://ec.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://lj.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xv.shxzukj.cn

[A02] 变量声明与赋值
来源：http://rj.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ng.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xd.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ps.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gw.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://vi.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://vb.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://lb.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://er.jctech888.com.cn

[A03] 常量定义
来源：http://ka.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mo.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://wz.hahajie.cn

JS:   const PI = 3.14159;
来源：http://ct.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://tq.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://yg.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://kh.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://xw.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://rg.panjiajie.cn

[A04] 判断变量类型
来源：http://me.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://my.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fw.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xy.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://hl.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pa.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mm.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ty.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://nq.nszjky.cn

[A05] 整数除法与取模
来源：http://da.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://df.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oc.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vo.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gr.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://yy.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://rc.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://wb.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://qi.panjiajie.cn

[A06] 字符串转数字
来源：http://dt.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://dd.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ej.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://om.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wm.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mu.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sv.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cl.jianghongdianzi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yd.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://ty.hahajie.cn

Py:   str(42)
来源：http://xs.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://yz.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://ac.shtwfgs.cn

TS:   String(42)
来源：http://he.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://is.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://yb.shxzskj.cn

Ruby: 42.to_s
来源：http://wi.lnxyls.cn

C#:   42.ToString()
来源：http://ax.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://yu.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://js.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eg.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gk.jctech888.com.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jj.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yr.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sw.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dq.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uy.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://rq.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dd.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ag.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zh.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kw.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://de.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gs.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://je.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pr.asd995.cn


<!-- 参考信息 -->