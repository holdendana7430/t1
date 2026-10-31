代发 wailian999

[U47] PHP：联合类型
来源：http://qh.colortex.cn

int|string $id
来源：http://cf.hnjuh.cn

[U48] PHP：纯枚举
来源：http://yf.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tv.newstarts.cn

[U49] PHP：只读属性
来源：http://zy.szsharing.cn

public readonly string $name
来源：http://bf.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://ko.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://pz.9csxet.cn

[U51] PHP：数组解构
来源：http://wm.521024.cn

[$a, $b] = $arr;
来源：http://wf.9csxet.cn

[U52] PHP：箭头函数
来源：http://dy.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://tp.asd995.cn

[U53] PHP：空合并运算符
来源：http://on.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://cg.szsharing.cn

[U54] PHP：空安全调用
来源：http://qz.wgjwhj.cn

$obj?->method()
来源：http://fv.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://ue.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tt.nszjky.cn

[U56] PHP：命名参数
来源：http://xd.9csxet.cn

f(a: 1, b: 2)
来源：http://bd.colortex.cn

[U57] PHP：字符串插值
来源：http://es.szsharing.cn

"值: {$a}"
来源：http://bu.shxzskj.cn

[U58] PHP：数组三件套
来源：http://um.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rr.lnxyls.cn

[U59] PHP：自定义排序
来源：http://pr.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ll.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://or.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wc.bjjhwx.cn

[U61] PHP：正则
来源：http://xc.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ys.szsharing.cn

[U62] PHP：日期对象
来源：http://go.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dq.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://iu.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ft.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://tg.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://eo.9csxet.cn

[U65] PHP：会话
来源：http://cl.asd995.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sq.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://cc.521024.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ou.9csxet.cn

[U67] PHP：处理文件上传
来源：http://qy.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oq.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://mj.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ew.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://xs.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sh.newstarts.cn

[U70] PHP：PDO 事务
来源：http://mn.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xa.9csxet.cn

[U71] PHP：抛出异常
来源：http://wm.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://nl.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://cn.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://ea.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://ru.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://hu.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://lj.nszjky.cn

getenv("APP_ENV") ?: "production"
来源：http://qs.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://df.wgjwhj.cn

composer require psr/container
来源：http://qh.521024.cn

[U76] PHP：简单路由
来源：http://wp.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jx.hahajie.cn

[U77] PHP：模板渲染
来源：http://no.hahajie.cn

composer require twig/twig
来源：http://xn.9csxet.cn

[U78] PHP：单元测试
来源：http://ob.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://ph.asd995.cn

[U79] PHP：静态分析
来源：http://rv.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://bu.panjiajie.cn

[U80] PHP：代码规范修复
来源：http://fi.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fh.muxihuayi.cn

[U81] JS：初始化项目
来源：http://zm.shtwfgs.cn

npm init -y;  npm i express
来源：http://hy.521024.cn

[U82] JS：package.json 脚本
来源：http://qt.hnjuh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://el.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://mn.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bf.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://dt.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hu.huixiangedu.cn

[U85] JS：可选链
来源：http://nd.asd995.cn

a?.b?.c
来源：http://ub.szxytkj.cn

[U86] JS：空值合并
来源：http://an.nicolike.cn

a ?? b
来源：http://rl.gzmigu.cn

[U87] JS：解构默认值
来源：http://yj.lnxyls.cn

const { a = 1, b = 2 } = obj;
来源：http://db.huanxung.cn

[U88] JS：对象展开合并
来源：http://za.lnxyls.cn

{ ...a, ...b }
来源：http://id.asd995.cn

[U89] JS：数组去重
来源：http://hp.muxihuayi.cn

[...new Set(arr)]
来源：http://io.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://qr.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://rs.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://sg.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wh.nicolike.cn

[U92] JS：深拷贝
来源：http://uo.panjiajie.cn

structuredClone(obj)
来源：http://lo.hnjuh.cn

[U93] JS：模板字符串
来源：http://zn.jianghongdianzi.cn

`共 ${n} 条`
来源：http://hz.shxzskj.cn

[U94] JS：箭头函数
来源：http://dr.asd995.cn

const double = x => x * 2;
来源：http://oi.521024.cn

[U95] JS：Promise 包装
来源：http://cj.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://ue.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://ec.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xu.nszjky.cn

[U97] JS：并发请求
来源：http://fx.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yn.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://id.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sx.gzmigu.cn

[U99] JS：事件监听
来源：http://cp.nicolike.cn

el.addEventListener("click", e => {})
来源：http://jd.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://rq.panjiajie.cn

document.querySelector(".item")
来源：http://ym.colortex.cn

[U101] JS：classList 操作
来源：http://mw.gzmigu.cn

el.classList.toggle("active")
来源：http://qf.lnxyls.cn

[U102] JS：本地存储
来源：http://po.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oy.nszjky.cn

[U103] JS：定时器
来源：http://ba.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fa.szsharing.cn

[U104] JS：防抖
来源：http://jy.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yl.hahajie.cn

[U105] JS：节流
来源：http://lo.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aw.huanxung.cn

[U106] JS：日期格式化
来源：http://jw.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jf.lnxyls.cn

[U107] JS：数字千分位
来源：http://gm.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ge.huanxung.cn

[U108] JS：随机整数
来源：http://sh.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zp.chemitech.net.cn

[U109] JS：数组分组
来源：http://bj.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://kt.bookmarksfly.cn

[U110] JS：数组分块
来源：http://mt.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cy.asd995.cn

[U111] JS：对象转 Map
来源：http://tx.szsharing.cn

new Map(Object.entries(obj))
来源：http://lx.gzmigu.cn

[U112] JS：字符串补位
来源：http://oi.huixiangedu.cn

"7".padStart(3, "0")
来源：http://sr.shxzukj.cn

[U113] JS：正则替换全部
来源：http://nq.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://fw.asd995.cn

[U114] JS：JSON 深比较
来源：http://np.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gz.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://sd.bookmarksfly.cn

crypto.randomUUID()
来源：http://tu.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://rq.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://ac.szsharing.cn

[U117] JS：单元测试
来源：http://io.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://tu.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://co.szsharing.cn

npm i -D vite;  npx vite
来源：http://bp.gzmigu.cn

[U119] JS：生产构建
来源：http://gs.shxzskj.cn

npx vite build
来源：http://ji.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://go.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://bc.jianghongdianzi.cn

================================================================================
来源：http://ta.nszjky.cn

统计汇总
来源：http://ee.szsharing.cn

================================================================================
来源：http://zh.haigaiapp.cn

按语言统计（条）：
来源：http://oz.yuexingan06.cn

Python ......... 252
来源：http://hj.newstarts.cn

PHP ............ 252
来源：http://je.hahajie.cn

JavaScript ..... 252
来源：http://mr.9csxet.cn

TypeScript ..... 212
来源：http://up.huixinmuqiang.cn

Java ........... 212
来源：http://ld.521024.cn

Go ............. 212
来源：http://va.shtwfgs.cn

Ruby ........... 212
来源：http://lp.yuntaijiaju.cn

C# ............. 212
来源：http://sf.shxzskj.cn

C .............. 30
来源：http://hu.newstarts.cn

C++ ............ 30
来源：http://xe.yuntaijiaju.cn

SQL ............ 90
来源：http://ts.panjiajie.cn

Bash ........... 80
来源：http://qb.jctech888.com.cn

Kotlin ......... 15
来源：http://de.shtwfgs.cn

Swift .......... 15
来源：http://ze.colortex.cn

Lua ............ 10
来源：http://gu.hahajie.cn

Perl ........... 10
来源：http://hl.yuexingan06.cn

Scala .......... 10
来源：http://ku.huanxung.cn

------------------------------------
来源：http://se.yuexingan06.cn

合计 ........... 2106 条
来源：http://kp.huixinmuqiang.cn

按章节统计：
来源：http://ix.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rv.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gn.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ct.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zc.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nj.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vz.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ny.newstarts.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ih.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lw.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rv.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oh.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qs.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ak.haigaiapp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yu.haigaiapp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ua.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kc.shxzskj.cn

Q SQL 专题                              90
来源：http://cr.shxzukj.cn

R Bash 专题                             80
来源：http://sr.shtwfgs.cn

S C / C++ 专题                          60
来源：http://gd.lnxyls.cn

T 其他语言补充                          60
来源：http://ca.hnjuh.cn

U 高频实用片段                         120
来源：http://no.hahajie.cn

------------------------------------
来源：http://xs.huixinmuqiang.cn

合计                                  2106 条
来源：http://no.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://yk.huanxung.cn

使用提醒
来源：http://zt.nszjky.cn

--------------------------------------------------------------------------------
来源：http://se.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tz.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xw.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qq.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vr.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jh.jctech888.com.cn

—— 文件结束 ——
来源：http://kk.muxihuayi.cn

================================================================================
来源：http://cb.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://sr.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://lr.szsharing.cn

================================================================================
来源：http://sj.shxzskj.cn

【收录内容】
来源：http://io.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hd.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vt.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://lv.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oe.hahajie.cn

【使用说明】
来源：http://qf.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ob.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wx.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mr.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dc.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://aq.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mc.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zn.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xn.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ul.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ty.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bm.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ii.nicolike.cn

【文件统计】
来源：http://al.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pq.521024.cn

--------------------------------------------------------------------------------
来源：http://db.521024.cn

目  录
来源：http://vv.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://xx.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yd.huixinmuqiang.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ed.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sj.shxzskj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uk.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hn.hahajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iu.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uj.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ax.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lh.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rf.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zj.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ba.shxzskj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cn.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mn.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rj.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wc.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ab.panjiajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rr.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iy.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dq.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ic.jianghongdianzi.cn

================================================================================
来源：http://nx.muxihuayi.cn

A. 基础语法与类型
来源：http://jv.huanxung.cn

================================================================================
来源：http://wo.colortex.cn

[A01] Hello World
来源：http://cj.521024.cn

Py:   print("Hello, World!")
来源：http://wq.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://ye.shxzukj.cn

JS:   console.log("Hello, World!");
来源：http://nl.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pp.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://tk.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://fu.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://fh.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bp.nicolike.cn

[A02] 变量声明与赋值
来源：http://fb.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://up.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vz.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oy.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gi.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://ou.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://by.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://wy.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ow.shtwfgs.cn

[A03] 常量定义
来源：http://zw.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wt.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://ng.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://yv.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://ns.yuntaijiaju.cn

Java: static final double PI = 3.14159;
来源：http://pf.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://zl.gzmigu.cn

Ruby: PI = 3.14159
来源：http://ey.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://zi.huixiangedu.cn

[A04] 判断变量类型
来源：http://yc.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://aq.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sv.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pe.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://ub.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nt.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vv.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vg.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://yr.haigaiapp.cn

[A05] 整数除法与取模
来源：http://eo.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hd.colortex.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://im.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ro.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cy.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://wl.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://wr.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://px.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://gu.hahajie.cn


<!-- 参考信息 -->