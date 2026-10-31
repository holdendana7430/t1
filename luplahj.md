代发 wailian999

[U61] PHP：正则
来源：http://gl.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ax.newstarts.cn

[U62] PHP：日期对象
来源：http://ry.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ax.szsharing.cn

[U63] PHP：文件读写
来源：http://tj.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eh.szsharing.cn

[U64] PHP：目录遍历
来源：http://de.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://vn.521024.cn

[U65] PHP：会话
来源：http://rz.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pl.panjiajie.cn

[U66] PHP：设置 Cookie
来源：http://eg.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wx.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://ek.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sv.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://hs.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sp.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://ri.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dg.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://xm.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hj.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://vv.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://tg.shxzukj.cn

[U72] PHP：写错误日志
来源：http://hy.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://wd.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://ja.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://vo.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://iv.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://lo.521024.cn

[U75] PHP：依赖注入
来源：http://gu.colortex.cn

composer require psr/container
来源：http://kd.nszjky.cn

[U76] PHP：简单路由
来源：http://nh.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zg.nszjky.cn

[U77] PHP：模板渲染
来源：http://xz.bookmarksfly.cn

composer require twig/twig
来源：http://oe.521024.cn

[U78] PHP：单元测试
来源：http://ei.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://ko.szxytkj.cn

[U79] PHP：静态分析
来源：http://oh.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://pe.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://yx.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://km.9csxet.cn

[U81] JS：初始化项目
来源：http://xy.wgjwhj.cn

npm init -y;  npm i express
来源：http://lj.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://wt.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ks.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://qu.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mm.colortex.cn

[U84] JS：CommonJS 写法
来源：http://lb.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xa.shtwfgs.cn

[U85] JS：可选链
来源：http://oc.521024.cn

a?.b?.c
来源：http://rv.bjjhwx.cn

[U86] JS：空值合并
来源：http://sj.huanxung.cn

a ?? b
来源：http://yg.szsharing.cn

[U87] JS：解构默认值
来源：http://ut.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://qq.shxzskj.cn

[U88] JS：对象展开合并
来源：http://iz.shxzskj.cn

{ ...a, ...b }
来源：http://ak.jctech888.com.cn

[U89] JS：数组去重
来源：http://jd.hnjuh.cn

[...new Set(arr)]
来源：http://uv.521024.cn

[U90] JS：数字数组排序
来源：http://ti.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://gk.nicolike.cn

[U91] JS：对象键值遍历
来源：http://mf.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ah.shxzukj.cn

[U92] JS：深拷贝
来源：http://fm.newstarts.cn

structuredClone(obj)
来源：http://pc.yuexingan06.cn

[U93] JS：模板字符串
来源：http://zd.nszjky.cn

`共 ${n} 条`
来源：http://go.gzmigu.cn

[U94] JS：箭头函数
来源：http://qb.muxihuayi.cn

const double = x => x * 2;
来源：http://uh.nicolike.cn

[U95] JS：Promise 包装
来源：http://bf.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://aq.shtwfgs.cn

[U96] JS：async/await 与异常
来源：http://ya.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jr.bookmarksfly.cn

[U97] JS：并发请求
来源：http://sr.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://if.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://cx.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xj.yuexingan06.cn

[U99] JS：事件监听
来源：http://di.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://xi.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://ix.9csxet.cn

document.querySelector(".item")
来源：http://wl.shxzukj.cn

[U101] JS：classList 操作
来源：http://fp.haigaiapp.cn

el.classList.toggle("active")
来源：http://bz.muxihuayi.cn

[U102] JS：本地存储
来源：http://ek.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://du.chemitech.net.cn

[U103] JS：定时器
来源：http://kj.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yr.huixiangedu.cn

[U104] JS：防抖
来源：http://bt.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pn.hnjuh.cn

[U105] JS：节流
来源：http://tm.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lk.chemitech.net.cn

[U106] JS：日期格式化
来源：http://pv.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ja.chemitech.net.cn

[U107] JS：数字千分位
来源：http://cq.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rb.haigaiapp.cn

[U108] JS：随机整数
来源：http://bv.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://il.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://ux.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://sg.yuexingan06.cn

[U110] JS：数组分块
来源：http://st.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sd.shxzukj.cn

[U111] JS：对象转 Map
来源：http://ju.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://gj.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://eo.521024.cn

"7".padStart(3, "0")
来源：http://zf.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://ni.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://ct.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://uz.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gu.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://gi.wgjwhj.cn

crypto.randomUUID()
来源：http://kk.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://qy.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://mr.nicolike.cn

[U117] JS：单元测试
来源：http://hp.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://ch.jctech888.com.cn

[U118] JS：开发服务器
来源：http://jt.colortex.cn

npm i -D vite;  npx vite
来源：http://ng.yuexingan06.cn

[U119] JS：生产构建
来源：http://ae.huixiangedu.cn

npx vite build
来源：http://ep.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://db.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://mu.nszjky.cn

================================================================================
来源：http://cx.haigaiapp.cn

统计汇总
来源：http://tc.nicolike.cn

================================================================================
来源：http://sj.521024.cn

按语言统计（条）：
来源：http://ub.szxytkj.cn

Python ......... 252
来源：http://nv.shxzskj.cn

PHP ............ 252
来源：http://td.wgjwhj.cn

JavaScript ..... 252
来源：http://xo.bjjhwx.cn

TypeScript ..... 212
来源：http://wh.9csxet.cn

Java ........... 212
来源：http://mn.hahajie.cn

Go ............. 212
来源：http://bn.szsharing.cn

Ruby ........... 212
来源：http://ka.wgjwhj.cn

C# ............. 212
来源：http://mk.hahajie.cn

C .............. 30
来源：http://yx.huixinmuqiang.cn

C++ ............ 30
来源：http://ib.bookmarksfly.cn

SQL ............ 90
来源：http://ce.nicolike.cn

Bash ........... 80
来源：http://vf.colortex.cn

Kotlin ......... 15
来源：http://pq.yuexingan06.cn

Swift .......... 15
来源：http://wf.huanxung.cn

Lua ............ 10
来源：http://fz.shtwfgs.cn

Perl ........... 10
来源：http://ld.huanxung.cn

Scala .......... 10
来源：http://vk.yuexingan06.cn

------------------------------------
来源：http://ad.shxzskj.cn

合计 ........... 2106 条
来源：http://xu.yuexingan06.cn

按章节统计：
来源：http://ya.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://io.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xw.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cv.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bm.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hk.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rh.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jo.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tm.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ok.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fc.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ng.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cg.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pl.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ew.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sr.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ml.huanxung.cn

Q SQL 专题                              90
来源：http://bg.jianghongdianzi.cn

R Bash 专题                             80
来源：http://oy.huixiangedu.cn

S C / C++ 专题                          60
来源：http://xf.gzmigu.cn

T 其他语言补充                          60
来源：http://xi.hahajie.cn

U 高频实用片段                         120
来源：http://pv.szsharing.cn

------------------------------------
来源：http://xt.wgjwhj.cn

合计                                  2106 条
来源：http://wl.9csxet.cn

--------------------------------------------------------------------------------
来源：http://pg.newstarts.cn

使用提醒
来源：http://jp.asd995.cn

--------------------------------------------------------------------------------
来源：http://de.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cu.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://is.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ci.huanxung.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uj.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lx.chemitech.net.cn

—— 文件结束 ——
来源：http://ln.gzmigu.cn

================================================================================
来源：http://ki.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://si.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://hg.huanxung.cn

================================================================================
来源：http://xg.chemitech.net.cn

【收录内容】
来源：http://ts.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bw.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rd.hahajie.cn

SQL · Bash · C · C++
来源：http://df.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ud.lnxyls.cn

【使用说明】
来源：http://vy.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://po.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://js.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jn.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lv.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fo.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vd.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://co.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dc.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://us.szxytkj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rr.huixinmuqiang.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lv.chemitech.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uj.colortex.cn

【文件统计】
来源：http://nd.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jp.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://iu.hahajie.cn

目  录
来源：http://rd.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://pw.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ju.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bc.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kw.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ac.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vf.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ow.nszjky.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ct.yuexingan06.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yt.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://df.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://im.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ea.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bs.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dw.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gx.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://io.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hh.bjjhwx.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cd.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pj.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aa.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ns.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xc.huixiangedu.cn

================================================================================
来源：http://xj.shxzukj.cn

A. 基础语法与类型
来源：http://rq.gzmigu.cn

================================================================================
来源：http://ov.wgjwhj.cn

[A01] Hello World
来源：http://qz.9csxet.cn

Py:   print("Hello, World!")
来源：http://si.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://du.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://zr.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cx.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://re.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://dm.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://uo.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fv.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://cl.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://we.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wp.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ib.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bn.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://md.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://on.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://zd.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yw.asd995.cn

[A03] 常量定义
来源：http://sx.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://he.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://yd.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://ee.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://zg.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://fl.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://tl.szxytkj.cn

Ruby: PI = 3.14159
来源：http://qf.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://qm.bjjhwx.cn

[A04] 判断变量类型
来源：http://xf.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lm.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ge.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nv.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://lz.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://md.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fo.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kh.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://re.huanxung.cn

[A05] 整数除法与取模
来源：http://jd.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tz.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tu.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bb.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sx.shxzukj.cn

Java: 7 / 2; 7 % 2
来源：http://no.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://bl.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://dg.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://pr.panjiajie.cn

[A06] 字符串转数字
来源：http://ux.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://uy.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://da.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hn.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ma.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vc.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ox.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gs.hnjuh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mx.wgjwhj.cn

[A07] 数字转字符串
来源：http://zs.szsharing.cn

Py:   str(42)
来源：http://wz.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://ja.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://bw.huanxung.cn

TS:   String(42)
来源：http://vl.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fx.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://be.shxzskj.cn

Ruby: 42.to_s
来源：http://uh.huanxung.cn

C#:   42.ToString()
来源：http://rm.hnjuh.cn

[A08] 取整与四舍五入
来源：http://gz.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://df.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yv.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bf.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wq.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qr.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zi.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://il.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://st.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://cz.9csxet.cn


<!-- 参考信息 -->