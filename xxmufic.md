代发 wailian999

[U49] PHP：只读属性
来源：http://hl.9csxet.cn

public readonly string $name
来源：http://ml.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://tq.panjiajie.cn

public function __construct(private int $id) {}
来源：http://id.jctech888.com.cn

[U51] PHP：数组解构
来源：http://qg.huixiangedu.cn

[$a, $b] = $arr;
来源：http://tb.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://sl.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://nx.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://zd.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://xe.szsharing.cn

[U54] PHP：空安全调用
来源：http://yh.shxzukj.cn

$obj?->method()
来源：http://cg.szsharing.cn

[U55] PHP：match 表达式
来源：http://ty.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sm.chemitech.net.cn

[U56] PHP：命名参数
来源：http://jg.shxzskj.cn

f(a: 1, b: 2)
来源：http://lf.huanxung.cn

[U57] PHP：字符串插值
来源：http://zr.colortex.cn

"值: {$a}"
来源：http://ed.hahajie.cn

[U58] PHP：数组三件套
来源：http://kz.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ru.hnjuh.cn

[U59] PHP：自定义排序
来源：http://eo.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://az.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://pr.hnjuh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oy.chemitech.net.cn

[U61] PHP：正则
来源：http://tc.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bo.haigaiapp.cn

[U62] PHP：日期对象
来源：http://hi.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ju.panjiajie.cn

[U63] PHP：文件读写
来源：http://dk.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vt.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://uo.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://aj.huixiangedu.cn

[U65] PHP：会话
来源：http://dj.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qo.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://ns.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aq.asd995.cn

[U67] PHP：处理文件上传
来源：http://ki.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xa.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://se.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ym.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://vw.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wc.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://sv.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lu.szxytkj.cn

[U71] PHP：抛出异常
来源：http://nw.521024.cn

throw new RuntimeException("失败", 500);
来源：http://bv.panjiajie.cn

[U72] PHP：写错误日志
来源：http://kn.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://vl.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://dk.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://ck.colortex.cn

[U74] PHP：读取环境变量
来源：http://zj.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://un.hnjuh.cn

[U75] PHP：依赖注入
来源：http://hi.haigaiapp.cn

composer require psr/container
来源：http://rf.521024.cn

[U76] PHP：简单路由
来源：http://wl.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pn.szsharing.cn

[U77] PHP：模板渲染
来源：http://vc.shxzukj.cn

composer require twig/twig
来源：http://hc.szsharing.cn

[U78] PHP：单元测试
来源：http://ky.hahajie.cn

composer require --dev phpunit/phpunit
来源：http://ld.gzmigu.cn

[U79] PHP：静态分析
来源：http://ir.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://re.521024.cn

[U80] PHP：代码规范修复
来源：http://mf.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ez.shxzskj.cn

[U81] JS：初始化项目
来源：http://gl.lnxyls.cn

npm init -y;  npm i express
来源：http://ib.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://ib.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mt.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://ml.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oh.colortex.cn

[U84] JS：CommonJS 写法
来源：http://vp.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fi.bookmarksfly.cn

[U85] JS：可选链
来源：http://kc.yuexingan06.cn

a?.b?.c
来源：http://dt.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://dq.jianghongdianzi.cn

a ?? b
来源：http://nw.haigaiapp.cn

[U87] JS：解构默认值
来源：http://gw.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://ir.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://xy.yuexingan06.cn

{ ...a, ...b }
来源：http://hz.521024.cn

[U89] JS：数组去重
来源：http://iw.521024.cn

[...new Set(arr)]
来源：http://jo.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://tw.yuntaijiaju.cn

[...arr].sort((a, b) => a - b)
来源：http://kd.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://hm.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xu.panjiajie.cn

[U92] JS：深拷贝
来源：http://aa.jianghongdianzi.cn

structuredClone(obj)
来源：http://yu.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://oe.huixiangedu.cn

`共 ${n} 条`
来源：http://ro.asd995.cn

[U94] JS：箭头函数
来源：http://qp.shxzukj.cn

const double = x => x * 2;
来源：http://yp.haigaiapp.cn

[U95] JS：Promise 包装
来源：http://bg.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://fa.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://pc.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fa.shxzskj.cn

[U97] JS：并发请求
来源：http://pk.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ng.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://ry.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ar.hnjuh.cn

[U99] JS：事件监听
来源：http://uv.521024.cn

el.addEventListener("click", e => {})
来源：http://hz.shxzukj.cn

[U100] JS：DOM 查询
来源：http://nk.jctech888.com.cn

document.querySelector(".item")
来源：http://ur.hnjuh.cn

[U101] JS：classList 操作
来源：http://wl.chemitech.net.cn

el.classList.toggle("active")
来源：http://qx.shtwfgs.cn

[U102] JS：本地存储
来源：http://tf.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bd.yuntaijiaju.cn

[U103] JS：定时器
来源：http://zb.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jd.newstarts.cn

[U104] JS：防抖
来源：http://il.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://em.wgjwhj.cn

[U105] JS：节流
来源：http://la.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ev.nicolike.cn

[U106] JS：日期格式化
来源：http://kp.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://en.hnjuh.cn

[U107] JS：数字千分位
来源：http://yo.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zp.huixiangedu.cn

[U108] JS：随机整数
来源：http://lq.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oo.hahajie.cn

[U109] JS：数组分组
来源：http://it.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://lz.wgjwhj.cn

[U110] JS：数组分块
来源：http://ow.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ux.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://pv.hahajie.cn

new Map(Object.entries(obj))
来源：http://ga.jctech888.com.cn

[U112] JS：字符串补位
来源：http://nk.szsharing.cn

"7".padStart(3, "0")
来源：http://pb.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://zp.szsharing.cn

s.replaceAll("a", "b")
来源：http://lh.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://ld.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://go.nszjky.cn

[U115] JS：生成 UUID
来源：http://yn.bjjhwx.cn

crypto.randomUUID()
来源：http://ey.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://xx.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://ja.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://vh.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://ah.newstarts.cn

[U118] JS：开发服务器
来源：http://ll.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://hg.nicolike.cn

[U119] JS：生产构建
来源：http://bi.chemitech.net.cn

npx vite build
来源：http://xi.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://hs.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://oh.nicolike.cn

================================================================================
来源：http://id.9csxet.cn

统计汇总
来源：http://lo.huanxung.cn

================================================================================
来源：http://uh.yuntaijiaju.cn

按语言统计（条）：
来源：http://dg.huixiangedu.cn

Python ......... 252
来源：http://kk.gzmigu.cn

PHP ............ 252
来源：http://un.jctech888.com.cn

JavaScript ..... 252
来源：http://ma.szsharing.cn

TypeScript ..... 212
来源：http://ap.yuexingan06.cn

Java ........... 212
来源：http://bx.jianghongdianzi.cn

Go ............. 212
来源：http://wt.bookmarksfly.cn

Ruby ........... 212
来源：http://il.521024.cn

C# ............. 212
来源：http://ay.jctech888.com.cn

C .............. 30
来源：http://pk.muxihuayi.cn

C++ ............ 30
来源：http://dt.yuntaijiaju.cn

SQL ............ 90
来源：http://mh.huixiangedu.cn

Bash ........... 80
来源：http://jp.nszjky.cn

Kotlin ......... 15
来源：http://qr.jctech888.com.cn

Swift .......... 15
来源：http://ua.colortex.cn

Lua ............ 10
来源：http://dy.huanxung.cn

Perl ........... 10
来源：http://pm.bjjhwx.cn

Scala .......... 10
来源：http://oi.nszjky.cn

------------------------------------
来源：http://su.nicolike.cn

合计 ........... 2106 条
来源：http://zo.hahajie.cn

按章节统计：
来源：http://az.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ib.gzmigu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ol.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wz.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://th.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uk.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ow.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vx.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jy.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://om.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lt.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ee.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gz.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://id.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tx.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zm.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yy.lnxyls.cn

Q SQL 专题                              90
来源：http://bx.panjiajie.cn

R Bash 专题                             80
来源：http://on.9csxet.cn

S C / C++ 专题                          60
来源：http://wl.haigaiapp.cn

T 其他语言补充                          60
来源：http://dt.shxzskj.cn

U 高频实用片段                         120
来源：http://dn.hahajie.cn

------------------------------------
来源：http://ni.asd995.cn

合计                                  2106 条
来源：http://dz.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://jm.jianghongdianzi.cn

使用提醒
来源：http://gj.szsharing.cn

--------------------------------------------------------------------------------
来源：http://bb.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xi.newstarts.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xh.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rv.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nm.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nx.huixinmuqiang.cn

—— 文件结束 ——
来源：http://oo.asd995.cn

================================================================================
来源：http://vl.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://ba.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://lm.hahajie.cn

================================================================================
来源：http://tm.jianghongdianzi.cn

【收录内容】
来源：http://pd.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://go.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tv.huixiangedu.cn

SQL · Bash · C · C++
来源：http://sk.yuexingan06.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sp.521024.cn

【使用说明】
来源：http://ir.shxzskj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xc.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tu.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ej.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fm.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rm.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jq.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ws.jianghongdianzi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jk.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ni.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mf.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vo.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kl.chemitech.net.cn

【文件统计】
来源：http://ju.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ua.hahajie.cn

--------------------------------------------------------------------------------
来源：http://in.hahajie.cn

目  录
来源：http://bj.521024.cn

--------------------------------------------------------------------------------
来源：http://pz.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://is.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://de.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lz.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yz.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://md.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rh.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yh.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zw.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ch.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://se.shxzskj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vk.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ar.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oq.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qw.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://et.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mq.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cb.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sb.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xu.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pd.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fz.bookmarksfly.cn

================================================================================
来源：http://ge.newstarts.cn

A. 基础语法与类型
来源：http://yr.haigaiapp.cn

================================================================================
来源：http://dv.nicolike.cn

[A01] Hello World
来源：http://gr.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://ye.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://ee.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://vs.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aa.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://dh.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://qo.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://ub.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ny.nicolike.cn

[A02] 变量声明与赋值
来源：http://dg.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hn.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bd.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sp.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ue.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://iz.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://zu.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://hq.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wb.jianghongdianzi.cn

[A03] 常量定义
来源：http://mp.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wz.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://qu.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://iz.521024.cn

TS:   const PI: number = 3.14159;
来源：http://zf.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://fu.asd995.cn

Go:   const PI = 3.14159
来源：http://qi.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://jc.hahajie.cn

C#:   const double PI = 3.14159;
来源：http://mt.jctech888.com.cn

[A04] 判断变量类型
来源：http://yq.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wj.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tc.yuntaijiaju.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bo.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://dy.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xk.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://iq.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mb.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://om.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://zp.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://td.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mn.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://om.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yl.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://db.newstarts.cn

Go:   7 / 2; 7 % 2
来源：http://es.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://mp.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://sa.panjiajie.cn

[A06] 字符串转数字
来源：http://se.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://hx.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tq.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ii.szsharing.cn


<!-- 参考信息 -->