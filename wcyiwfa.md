代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://ol.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sp.521024.cn

[U46] PHP：可空类型
来源：http://fl.huixinmuqiang.cn

?string $name = null
来源：http://sx.panjiajie.cn

[U47] PHP：联合类型
来源：http://tj.gzmigu.cn

int|string $id
来源：http://ei.szsharing.cn

[U48] PHP：纯枚举
来源：http://lx.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://og.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://qc.yuntaijiaju.cn

public readonly string $name
来源：http://hq.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://jo.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://eg.hahajie.cn

[U51] PHP：数组解构
来源：http://jd.yuexingan06.cn

[$a, $b] = $arr;
来源：http://io.gzmigu.cn

[U52] PHP：箭头函数
来源：http://zr.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://sh.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://cg.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://rg.colortex.cn

[U54] PHP：空安全调用
来源：http://xf.colortex.cn

$obj?->method()
来源：http://cq.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://gq.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qm.huanxung.cn

[U56] PHP：命名参数
来源：http://pa.yuexingan06.cn

f(a: 1, b: 2)
来源：http://wz.nicolike.cn

[U57] PHP：字符串插值
来源：http://sl.asd995.cn

"值: {$a}"
来源：http://mo.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://zl.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lc.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://wq.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://us.asd995.cn

[U60] PHP：JSON 编解码
来源：http://qo.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lq.huixinmuqiang.cn

[U61] PHP：正则
来源：http://kr.hahajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iy.9csxet.cn

[U62] PHP：日期对象
来源：http://gi.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mp.hnjuh.cn

[U63] PHP：文件读写
来源：http://fe.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kp.nszjky.cn

[U64] PHP：目录遍历
来源：http://bm.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://vw.hnjuh.cn

[U65] PHP：会话
来源：http://po.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zo.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://df.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uq.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://vt.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://di.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://jo.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://co.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://fr.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ov.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://ia.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bi.nicolike.cn

[U71] PHP：抛出异常
来源：http://yg.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://dg.huanxung.cn

[U72] PHP：写错误日志
来源：http://fh.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://lt.nszjky.cn

[U73] PHP：读取 ini 配置
来源：http://to.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://gd.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://bb.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://wy.jianghongdianzi.cn

[U75] PHP：依赖注入
来源：http://ca.szsharing.cn

composer require psr/container
来源：http://hm.jianghongdianzi.cn

[U76] PHP：简单路由
来源：http://pn.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ve.nszjky.cn

[U77] PHP：模板渲染
来源：http://zz.gzmigu.cn

composer require twig/twig
来源：http://vy.panjiajie.cn

[U78] PHP：单元测试
来源：http://mk.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://im.nicolike.cn

[U79] PHP：静态分析
来源：http://aj.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://kw.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://om.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aw.9csxet.cn

[U81] JS：初始化项目
来源：http://xf.gzmigu.cn

npm init -y;  npm i express
来源：http://eb.521024.cn

[U82] JS：package.json 脚本
来源：http://kf.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ds.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://ry.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ax.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://mf.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wn.yuntaijiaju.cn

[U85] JS：可选链
来源：http://md.szsharing.cn

a?.b?.c
来源：http://gz.szxytkj.cn

[U86] JS：空值合并
来源：http://em.szxytkj.cn

a ?? b
来源：http://lx.nszjky.cn

[U87] JS：解构默认值
来源：http://hu.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://ea.colortex.cn

[U88] JS：对象展开合并
来源：http://pa.wgjwhj.cn

{ ...a, ...b }
来源：http://rn.huanxung.cn

[U89] JS：数组去重
来源：http://hi.hnjuh.cn

[...new Set(arr)]
来源：http://ka.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://nq.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://ao.nszjky.cn

[U91] JS：对象键值遍历
来源：http://pg.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iw.jctech888.com.cn

[U92] JS：深拷贝
来源：http://qa.huixiangedu.cn

structuredClone(obj)
来源：http://do.bjjhwx.cn

[U93] JS：模板字符串
来源：http://ia.bjjhwx.cn

`共 ${n} 条`
来源：http://ki.nicolike.cn

[U94] JS：箭头函数
来源：http://cf.colortex.cn

const double = x => x * 2;
来源：http://mi.chemitech.net.cn

[U95] JS：Promise 包装
来源：http://un.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://up.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://vi.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qg.shtwfgs.cn

[U97] JS：并发请求
来源：http://ei.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qq.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://xz.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ze.asd995.cn

[U99] JS：事件监听
来源：http://qq.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://se.hnjuh.cn

[U100] JS：DOM 查询
来源：http://id.haigaiapp.cn

document.querySelector(".item")
来源：http://xc.nicolike.cn

[U101] JS：classList 操作
来源：http://nz.colortex.cn

el.classList.toggle("active")
来源：http://lw.colortex.cn

[U102] JS：本地存储
来源：http://tp.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hu.hnjuh.cn

[U103] JS：定时器
来源：http://ap.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sy.asd995.cn

[U104] JS：防抖
来源：http://dv.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://km.shxzskj.cn

[U105] JS：节流
来源：http://md.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uf.hnjuh.cn

[U106] JS：日期格式化
来源：http://pp.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dv.szxytkj.cn

[U107] JS：数字千分位
来源：http://gq.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zh.nicolike.cn

[U108] JS：随机整数
来源：http://zy.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://em.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://qp.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://uf.huanxung.cn

[U110] JS：数组分块
来源：http://du.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bj.nicolike.cn

[U111] JS：对象转 Map
来源：http://fk.shxzskj.cn

new Map(Object.entries(obj))
来源：http://fi.haigaiapp.cn

[U112] JS：字符串补位
来源：http://rk.hnjuh.cn

"7".padStart(3, "0")
来源：http://pm.szsharing.cn

[U113] JS：正则替换全部
来源：http://dn.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://vt.nicolike.cn

[U114] JS：JSON 深比较
来源：http://tk.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jp.asd995.cn

[U115] JS：生成 UUID
来源：http://nb.gzmigu.cn

crypto.randomUUID()
来源：http://wp.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://bc.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://hj.szsharing.cn

[U117] JS：单元测试
来源：http://oi.shxzukj.cn

npm i -D vitest;  npx vitest
来源：http://cb.muxihuayi.cn

[U118] JS：开发服务器
来源：http://oo.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://nw.szsharing.cn

[U119] JS：生产构建
来源：http://dl.nszjky.cn

npx vite build
来源：http://fx.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://xv.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://ic.colortex.cn

================================================================================
来源：http://bf.shtwfgs.cn

统计汇总
来源：http://wp.bjjhwx.cn

================================================================================
来源：http://tq.bjjhwx.cn

按语言统计（条）：
来源：http://ez.shtwfgs.cn

Python ......... 252
来源：http://lq.yuntaijiaju.cn

PHP ............ 252
来源：http://zl.huixinmuqiang.cn

JavaScript ..... 252
来源：http://bs.newstarts.cn

TypeScript ..... 212
来源：http://ln.bookmarksfly.cn

Java ........... 212
来源：http://xu.521024.cn

Go ............. 212
来源：http://ko.newstarts.cn

Ruby ........... 212
来源：http://bh.wgjwhj.cn

C# ............. 212
来源：http://ks.hnjuh.cn

C .............. 30
来源：http://sd.yuntaijiaju.cn

C++ ............ 30
来源：http://tp.yuntaijiaju.cn

SQL ............ 90
来源：http://nv.nicolike.cn

Bash ........... 80
来源：http://xo.chemitech.net.cn

Kotlin ......... 15
来源：http://tw.gzmigu.cn

Swift .......... 15
来源：http://cw.bookmarksfly.cn

Lua ............ 10
来源：http://ir.hahajie.cn

Perl ........... 10
来源：http://rz.panjiajie.cn

Scala .......... 10
来源：http://ci.bookmarksfly.cn

------------------------------------
来源：http://sc.newstarts.cn

合计 ........... 2106 条
来源：http://fj.nszjky.cn

按章节统计：
来源：http://mo.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gj.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://as.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rg.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://er.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kw.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ku.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yd.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://af.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kp.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xb.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tf.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xp.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ud.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zi.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zq.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wk.hahajie.cn

Q SQL 专题                              90
来源：http://vo.jianghongdianzi.cn

R Bash 专题                             80
来源：http://dt.colortex.cn

S C / C++ 专题                          60
来源：http://yj.huanxung.cn

T 其他语言补充                          60
来源：http://ar.shtwfgs.cn

U 高频实用片段                         120
来源：http://jc.wgjwhj.cn

------------------------------------
来源：http://oj.haigaiapp.cn

合计                                  2106 条
来源：http://go.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://vn.newstarts.cn

使用提醒
来源：http://ez.szsharing.cn

--------------------------------------------------------------------------------
来源：http://eg.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qn.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zv.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wn.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://om.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ys.bjjhwx.cn

—— 文件结束 ——
来源：http://yw.hahajie.cn

================================================================================
来源：http://vh.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://kp.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://df.colortex.cn

================================================================================
来源：http://vc.haigaiapp.cn

【收录内容】
来源：http://pq.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://eh.haigaiapp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xr.shxzskj.cn

SQL · Bash · C · C++
来源：http://gx.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nt.chemitech.net.cn

【使用说明】
来源：http://me.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yr.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qe.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kh.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bx.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sv.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ws.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fm.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://js.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rl.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aw.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tq.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lm.bookmarksfly.cn

【文件统计】
来源：http://sd.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cd.hahajie.cn

--------------------------------------------------------------------------------
来源：http://wj.jctech888.com.cn

目  录
来源：http://ht.huanxung.cn

--------------------------------------------------------------------------------
来源：http://oq.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ky.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yn.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yz.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://me.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ck.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xk.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uc.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rt.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fg.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gq.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qg.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ut.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ks.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bt.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dp.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nr.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hk.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ng.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fb.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ok.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fx.shxzskj.cn

================================================================================
来源：http://ir.521024.cn

A. 基础语法与类型
来源：http://sv.huixinmuqiang.cn

================================================================================
来源：http://qy.bjjhwx.cn

[A01] Hello World
来源：http://dm.huanxung.cn

Py:   print("Hello, World!")
来源：http://qb.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://go.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://gt.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sz.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://si.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://xi.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://nu.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://aj.nicolike.cn

[A02] 变量声明与赋值
来源：http://yj.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ho.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sy.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iy.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zf.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://bi.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://uu.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://tv.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bp.szxytkj.cn

[A03] 常量定义
来源：http://na.bjjhwx.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hr.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://ud.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://vf.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://ug.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://wb.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://fc.lnxyls.cn

Ruby: PI = 3.14159
来源：http://bm.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://cv.jctech888.com.cn

[A04] 判断变量类型
来源：http://ae.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ax.colortex.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nx.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jy.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://em.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cs.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nw.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vi.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://uc.shxzukj.cn

[A05] 整数除法与取模
来源：http://ig.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yp.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cd.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://of.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ua.panjiajie.cn


<!-- 参考信息 -->