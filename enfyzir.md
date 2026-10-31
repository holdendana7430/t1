代发 wailian999

[U57] PHP：字符串插值
来源：http://lv.jctech888.com.cn

"值: {$a}"
来源：http://pr.szxytkj.cn

[U58] PHP：数组三件套
来源：http://yu.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://to.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://sg.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xj.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://dh.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vx.bjjhwx.cn

[U61] PHP：正则
来源：http://df.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://or.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://bg.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tv.asd995.cn

[U63] PHP：文件读写
来源：http://gg.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jc.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://js.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://lw.bjjhwx.cn

[U65] PHP：会话
来源：http://qu.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bb.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://ny.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gi.asd995.cn

[U67] PHP：处理文件上传
来源：http://ko.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://do.nszjky.cn

[U68] PHP：PDO 连接
来源：http://un.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dn.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://dn.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oi.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://xg.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ge.newstarts.cn

[U71] PHP：抛出异常
来源：http://jz.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://on.newstarts.cn

[U72] PHP：写错误日志
来源：http://in.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://pk.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://oj.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://jb.nicolike.cn

[U74] PHP：读取环境变量
来源：http://zu.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://xl.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://rd.lnxyls.cn

composer require psr/container
来源：http://me.muxihuayi.cn

[U76] PHP：简单路由
来源：http://iw.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ej.jctech888.com.cn

[U77] PHP：模板渲染
来源：http://rx.shxzskj.cn

composer require twig/twig
来源：http://ni.panjiajie.cn

[U78] PHP：单元测试
来源：http://jf.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://mh.lnxyls.cn

[U79] PHP：静态分析
来源：http://ex.521024.cn

composer require --dev phpstan/phpstan
来源：http://tw.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://my.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pc.huixiangedu.cn

[U81] JS：初始化项目
来源：http://hq.asd995.cn

npm init -y;  npm i express
来源：http://gm.nszjky.cn

[U82] JS：package.json 脚本
来源：http://yp.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://du.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://uj.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bp.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://nr.nszjky.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iy.shxzskj.cn

[U85] JS：可选链
来源：http://oa.huixinmuqiang.cn

a?.b?.c
来源：http://ib.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://ji.lnxyls.cn

a ?? b
来源：http://ki.asd995.cn

[U87] JS：解构默认值
来源：http://nf.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://in.hahajie.cn

[U88] JS：对象展开合并
来源：http://sm.colortex.cn

{ ...a, ...b }
来源：http://mj.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://es.shxzskj.cn

[...new Set(arr)]
来源：http://cg.hnjuh.cn

[U90] JS：数字数组排序
来源：http://gc.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://pu.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://mt.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lk.9csxet.cn

[U92] JS：深拷贝
来源：http://ve.chemitech.net.cn

structuredClone(obj)
来源：http://ie.shxzskj.cn

[U93] JS：模板字符串
来源：http://xl.shtwfgs.cn

`共 ${n} 条`
来源：http://om.jctech888.com.cn

[U94] JS：箭头函数
来源：http://xt.shtwfgs.cn

const double = x => x * 2;
来源：http://qo.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://nw.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://dt.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://nl.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oz.yuexingan06.cn

[U97] JS：并发请求
来源：http://li.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kv.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://yk.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ac.nicolike.cn

[U99] JS：事件监听
来源：http://hu.nszjky.cn

el.addEventListener("click", e => {})
来源：http://uv.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://jo.haigaiapp.cn

document.querySelector(".item")
来源：http://go.lnxyls.cn

[U101] JS：classList 操作
来源：http://lq.chemitech.net.cn

el.classList.toggle("active")
来源：http://gj.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://ou.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oc.yuntaijiaju.cn

[U103] JS：定时器
来源：http://he.chemitech.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rx.asd995.cn

[U104] JS：防抖
来源：http://mx.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gl.wgjwhj.cn

[U105] JS：节流
来源：http://ke.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uj.jctech888.com.cn

[U106] JS：日期格式化
来源：http://vx.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yo.szxytkj.cn

[U107] JS：数字千分位
来源：http://ro.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://el.asd995.cn

[U108] JS：随机整数
来源：http://no.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xi.haigaiapp.cn

[U109] JS：数组分组
来源：http://cq.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://vo.nszjky.cn

[U110] JS：数组分块
来源：http://dl.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ed.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://tq.hnjuh.cn

new Map(Object.entries(obj))
来源：http://sd.panjiajie.cn

[U112] JS：字符串补位
来源：http://wd.newstarts.cn

"7".padStart(3, "0")
来源：http://te.panjiajie.cn

[U113] JS：正则替换全部
来源：http://jk.shxzskj.cn

s.replaceAll("a", "b")
来源：http://qt.nszjky.cn

[U114] JS：JSON 深比较
来源：http://rn.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rw.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://yx.szsharing.cn

crypto.randomUUID()
来源：http://ur.newstarts.cn

[U116] JS：类型检查（JSDoc）
来源：http://ul.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://in.colortex.cn

[U117] JS：单元测试
来源：http://jn.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://ae.shxzskj.cn

[U118] JS：开发服务器
来源：http://ax.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://qh.hnjuh.cn

[U119] JS：生产构建
来源：http://so.nicolike.cn

npx vite build
来源：http://lx.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://uw.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://bd.gzmigu.cn

================================================================================
来源：http://ay.huanxung.cn

统计汇总
来源：http://pb.nszjky.cn

================================================================================
来源：http://yt.bjjhwx.cn

按语言统计（条）：
来源：http://wv.muxihuayi.cn

Python ......... 252
来源：http://jd.hnjuh.cn

PHP ............ 252
来源：http://eh.521024.cn

JavaScript ..... 252
来源：http://oj.shtwfgs.cn

TypeScript ..... 212
来源：http://gk.gzmigu.cn

Java ........... 212
来源：http://cy.wgjwhj.cn

Go ............. 212
来源：http://qh.shtwfgs.cn

Ruby ........... 212
来源：http://og.shxzukj.cn

C# ............. 212
来源：http://un.bjjhwx.cn

C .............. 30
来源：http://nh.yuexingan06.cn

C++ ............ 30
来源：http://ro.521024.cn

SQL ............ 90
来源：http://ef.muxihuayi.cn

Bash ........... 80
来源：http://al.yuexingan06.cn

Kotlin ......... 15
来源：http://vn.shxzukj.cn

Swift .......... 15
来源：http://fx.jctech888.com.cn

Lua ............ 10
来源：http://gr.wgjwhj.cn

Perl ........... 10
来源：http://sy.haigaiapp.cn

Scala .......... 10
来源：http://el.jctech888.com.cn

------------------------------------
来源：http://uk.bookmarksfly.cn

合计 ........... 2106 条
来源：http://be.nicolike.cn

按章节统计：
来源：http://lj.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vl.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gm.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rg.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ab.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fu.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ck.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kc.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wn.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sc.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gu.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ml.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xv.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vq.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://us.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pi.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dw.lnxyls.cn

Q SQL 专题                              90
来源：http://oi.huanxung.cn

R Bash 专题                             80
来源：http://vr.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://oq.colortex.cn

T 其他语言补充                          60
来源：http://gq.bookmarksfly.cn

U 高频实用片段                         120
来源：http://sm.shxzskj.cn

------------------------------------
来源：http://ct.yuexingan06.cn

合计                                  2106 条
来源：http://bq.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ec.huanxung.cn

使用提醒
来源：http://tk.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://wo.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fg.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gv.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vs.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ug.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lt.shtwfgs.cn

—— 文件结束 ——
来源：http://rg.shxzukj.cn

================================================================================
来源：http://un.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://pz.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://in.haigaiapp.cn

================================================================================
来源：http://bj.yuexingan06.cn

【收录内容】
来源：http://rh.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kb.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ft.wgjwhj.cn

SQL · Bash · C · C++
来源：http://ej.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://id.haigaiapp.cn

【使用说明】
来源：http://jy.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nf.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xt.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zq.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://co.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://op.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://og.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bk.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mk.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ea.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bp.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mo.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dy.shxzukj.cn

【文件统计】
来源：http://vb.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gc.newstarts.cn

--------------------------------------------------------------------------------
来源：http://zx.yuntaijiaju.cn

目  录
来源：http://yb.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://wk.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zq.shxzskj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jt.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ps.szsharing.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tt.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vv.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kg.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://id.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://te.newstarts.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bf.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zd.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ds.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xe.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yb.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hd.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ph.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ir.huixiangedu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cz.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hi.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wy.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kg.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gx.nszjky.cn

================================================================================
来源：http://xj.chemitech.net.cn

A. 基础语法与类型
来源：http://qm.lnxyls.cn

================================================================================
来源：http://bp.asd995.cn

[A01] Hello World
来源：http://at.521024.cn

Py:   print("Hello, World!")
来源：http://ye.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://zd.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://dc.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bh.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://mk.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://yp.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://ep.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://af.shxzukj.cn

[A02] 变量声明与赋值
来源：http://ee.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nt.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dq.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tt.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uf.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://fx.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://ns.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://do.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bf.hnjuh.cn

[A03] 常量定义
来源：http://ln.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://as.colortex.cn

PHP:  const PI = 3.14159;
来源：http://rl.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://xm.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://bx.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://ds.9csxet.cn

Go:   const PI = 3.14159
来源：http://av.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://pe.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://ne.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://dn.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wu.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kg.chemitech.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://of.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://uy.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ct.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zh.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rx.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://lx.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://ni.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ty.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zl.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mo.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zu.shxzskj.cn

Java: 7 / 2; 7 % 2
来源：http://nq.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://tm.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://wb.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://zc.muxihuayi.cn

[A06] 字符串转数字
来源：http://qg.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://qc.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ez.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nu.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ng.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rw.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uj.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vv.shxzukj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ee.muxihuayi.cn

[A07] 数字转字符串
来源：http://if.muxihuayi.cn

Py:   str(42)
来源：http://fd.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://cq.9csxet.cn

JS:   String(42); (42).toString()
来源：http://jy.bjjhwx.cn

TS:   String(42)
来源：http://le.lnxyls.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lk.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://ke.newstarts.cn

Ruby: 42.to_s
来源：http://ij.9csxet.cn

C#:   42.ToString()
来源：http://jw.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://gs.chemitech.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xd.szxytkj.cn


<!-- 参考信息 -->