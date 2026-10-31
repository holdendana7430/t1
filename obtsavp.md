代发 wailian999

[U59] PHP：自定义排序
来源：http://qz.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://os.asd995.cn

[U60] PHP：JSON 编解码
来源：http://sp.wgjwhj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oh.yuntaijiaju.cn

[U61] PHP：正则
来源：http://iw.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cw.521024.cn

[U62] PHP：日期对象
来源：http://gz.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://af.wgjwhj.cn

[U63] PHP：文件读写
来源：http://wm.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sc.asd995.cn

[U64] PHP：目录遍历
来源：http://lk.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://bo.panjiajie.cn

[U65] PHP：会话
来源：http://gd.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mi.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://zp.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zl.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://vi.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fy.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://jf.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gh.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://wk.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iq.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://dl.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lv.nszjky.cn

[U71] PHP：抛出异常
来源：http://ob.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://dz.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://zk.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://jn.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://vh.panjiajie.cn

parse_ini_file("config.ini", true)
来源：http://xc.hahajie.cn

[U74] PHP：读取环境变量
来源：http://cs.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://gb.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://rw.yuexingan06.cn

composer require psr/container
来源：http://pk.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://km.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dk.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://nj.szsharing.cn

composer require twig/twig
来源：http://ro.newstarts.cn

[U78] PHP：单元测试
来源：http://ru.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://xr.bjjhwx.cn

[U79] PHP：静态分析
来源：http://tt.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://bm.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://ph.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qa.yuexingan06.cn

[U81] JS：初始化项目
来源：http://wj.panjiajie.cn

npm init -y;  npm i express
来源：http://se.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://do.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mi.bookmarksfly.cn

[U83] JS：ES Module 导入导出
来源：http://jh.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ea.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://pt.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tr.chemitech.net.cn

[U85] JS：可选链
来源：http://xn.jianghongdianzi.cn

a?.b?.c
来源：http://ll.bjjhwx.cn

[U86] JS：空值合并
来源：http://gu.nszjky.cn

a ?? b
来源：http://ad.nicolike.cn

[U87] JS：解构默认值
来源：http://zo.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://au.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://ji.colortex.cn

{ ...a, ...b }
来源：http://fl.lnxyls.cn

[U89] JS：数组去重
来源：http://yy.huixiangedu.cn

[...new Set(arr)]
来源：http://ad.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://ae.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://hj.521024.cn

[U91] JS：对象键值遍历
来源：http://or.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nd.wgjwhj.cn

[U92] JS：深拷贝
来源：http://ow.521024.cn

structuredClone(obj)
来源：http://fh.bjjhwx.cn

[U93] JS：模板字符串
来源：http://oj.9csxet.cn

`共 ${n} 条`
来源：http://ms.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://dj.521024.cn

const double = x => x * 2;
来源：http://gq.gzmigu.cn

[U95] JS：Promise 包装
来源：http://cq.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://gf.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://yh.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://da.colortex.cn

[U97] JS：并发请求
来源：http://yg.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tn.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://ac.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://me.chemitech.net.cn

[U99] JS：事件监听
来源：http://kf.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://jb.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://np.nicolike.cn

document.querySelector(".item")
来源：http://fs.yuexingan06.cn

[U101] JS：classList 操作
来源：http://xh.szsharing.cn

el.classList.toggle("active")
来源：http://ha.bookmarksfly.cn

[U102] JS：本地存储
来源：http://sc.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vi.521024.cn

[U103] JS：定时器
来源：http://ss.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gg.panjiajie.cn

[U104] JS：防抖
来源：http://hd.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ss.szsharing.cn

[U105] JS：节流
来源：http://tu.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sb.shxzskj.cn

[U106] JS：日期格式化
来源：http://cj.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yi.521024.cn

[U107] JS：数字千分位
来源：http://pg.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://go.9csxet.cn

[U108] JS：随机整数
来源：http://av.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bf.yuntaijiaju.cn

[U109] JS：数组分组
来源：http://iy.hahajie.cn

Object.groupBy(arr, x => x.type)
来源：http://ly.panjiajie.cn

[U110] JS：数组分块
来源：http://yb.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uw.nicolike.cn

[U111] JS：对象转 Map
来源：http://ol.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://fr.colortex.cn

[U112] JS：字符串补位
来源：http://ri.szsharing.cn

"7".padStart(3, "0")
来源：http://we.nszjky.cn

[U113] JS：正则替换全部
来源：http://gq.hnjuh.cn

s.replaceAll("a", "b")
来源：http://pq.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://pd.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://or.hahajie.cn

[U115] JS：生成 UUID
来源：http://yr.hahajie.cn

crypto.randomUUID()
来源：http://cm.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://nj.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://ur.bookmarksfly.cn

[U117] JS：单元测试
来源：http://od.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://ou.colortex.cn

[U118] JS：开发服务器
来源：http://gz.newstarts.cn

npm i -D vite;  npx vite
来源：http://uq.jctech888.com.cn

[U119] JS：生产构建
来源：http://hf.wgjwhj.cn

npx vite build
来源：http://hc.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://mt.asd995.cn

import.meta.env.VITE_API_URL
来源：http://em.shxzukj.cn

================================================================================
来源：http://hg.haigaiapp.cn

统计汇总
来源：http://oc.shtwfgs.cn

================================================================================
来源：http://sc.huanxung.cn

按语言统计（条）：
来源：http://cv.muxihuayi.cn

Python ......... 252
来源：http://jc.shxzskj.cn

PHP ............ 252
来源：http://ny.huixinmuqiang.cn

JavaScript ..... 252
来源：http://ki.szxytkj.cn

TypeScript ..... 212
来源：http://fd.jctech888.com.cn

Java ........... 212
来源：http://wm.yuexingan06.cn

Go ............. 212
来源：http://dm.huanxung.cn

Ruby ........... 212
来源：http://at.szsharing.cn

C# ............. 212
来源：http://xd.lnxyls.cn

C .............. 30
来源：http://ps.jctech888.com.cn

C++ ............ 30
来源：http://ch.colortex.cn

SQL ............ 90
来源：http://nj.szxytkj.cn

Bash ........... 80
来源：http://gv.hahajie.cn

Kotlin ......... 15
来源：http://yt.hnjuh.cn

Swift .......... 15
来源：http://gi.shtwfgs.cn

Lua ............ 10
来源：http://ly.muxihuayi.cn

Perl ........... 10
来源：http://xy.chemitech.net.cn

Scala .......... 10
来源：http://kv.jianghongdianzi.cn

------------------------------------
来源：http://ux.shxzskj.cn

合计 ........... 2106 条
来源：http://fi.shxzskj.cn

按章节统计：
来源：http://ej.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vy.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gb.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dy.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://is.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gz.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ip.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wu.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qx.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ox.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pf.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ex.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rk.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://an.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ad.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mv.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://if.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://ug.asd995.cn

R Bash 专题                             80
来源：http://je.panjiajie.cn

S C / C++ 专题                          60
来源：http://yp.shxzukj.cn

T 其他语言补充                          60
来源：http://oy.jctech888.com.cn

U 高频实用片段                         120
来源：http://pn.panjiajie.cn

------------------------------------
来源：http://fl.asd995.cn

合计                                  2106 条
来源：http://xw.huanxung.cn

--------------------------------------------------------------------------------
来源：http://xy.gzmigu.cn

使用提醒
来源：http://ca.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://fx.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mr.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zk.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wg.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ar.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://md.newstarts.cn

—— 文件结束 ——
来源：http://in.panjiajie.cn

================================================================================
来源：http://rk.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://wx.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://tu.shxzukj.cn

================================================================================
来源：http://yb.newstarts.cn

【收录内容】
来源：http://th.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jc.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fz.colortex.cn

SQL · Bash · C · C++
来源：http://am.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://od.huixiangedu.cn

【使用说明】
来源：http://ac.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://de.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hm.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vp.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ff.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rc.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eu.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nf.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://of.wgjwhj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lh.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yg.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yl.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ag.nszjky.cn

【文件统计】
来源：http://xt.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zi.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://vs.wgjwhj.cn

目  录
来源：http://ve.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ds.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mv.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mm.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://om.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ld.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gd.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xz.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yj.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oy.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qq.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sm.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ly.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nr.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jj.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://re.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xw.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://up.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zi.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ef.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ge.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bu.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vn.huixinmuqiang.cn

================================================================================
来源：http://kq.gzmigu.cn

A. 基础语法与类型
来源：http://id.nszjky.cn

================================================================================
来源：http://xu.haigaiapp.cn

[A01] Hello World
来源：http://vs.panjiajie.cn

Py:   print("Hello, World!")
来源：http://hi.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://rd.shxzukj.cn

JS:   console.log("Hello, World!");
来源：http://ka.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ds.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://mt.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://wv.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://ak.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qs.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://wd.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://br.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mp.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ew.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ph.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://jk.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://qd.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://ez.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qu.haigaiapp.cn

[A03] 常量定义
来源：http://un.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uh.colortex.cn

PHP:  const PI = 3.14159;
来源：http://ds.colortex.cn

JS:   const PI = 3.14159;
来源：http://xz.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://hh.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://xm.szsharing.cn

Go:   const PI = 3.14159
来源：http://xl.szxytkj.cn

Ruby: PI = 3.14159
来源：http://py.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://qi.newstarts.cn

[A04] 判断变量类型
来源：http://ip.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tg.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vz.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zi.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://ge.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cv.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xj.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pq.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://ku.shxzukj.cn

[A05] 整数除法与取模
来源：http://qy.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ay.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lm.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jm.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yo.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://sg.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://cu.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://cs.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://jt.9csxet.cn

[A06] 字符串转数字
来源：http://pp.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://nv.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jl.shtwfgs.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rh.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ad.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mq.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tl.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xz.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ek.9csxet.cn

[A07] 数字转字符串
来源：http://lb.bjjhwx.cn

Py:   str(42)
来源：http://qf.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://pc.nicolike.cn

JS:   String(42); (42).toString()
来源：http://wl.yuexingan06.cn

TS:   String(42)
来源：http://pb.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wv.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://fi.nszjky.cn

Ruby: 42.to_s
来源：http://de.bookmarksfly.cn

C#:   42.ToString()
来源：http://jy.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://yd.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://df.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ls.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fr.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ok.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://af.yuntaijiaju.cn


<!-- 参考信息 -->