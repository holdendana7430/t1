代发 wailian999

[U43] PHP：声明命名空间
来源：http://lj.yuexingan06.cn

namespace App\Http;
来源：http://kl.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://iy.huixiangedu.cn

declare(strict_types=1);
来源：http://tv.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://er.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qw.nicolike.cn

[U46] PHP：可空类型
来源：http://jd.szxytkj.cn

?string $name = null
来源：http://pz.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://fb.huixinmuqiang.cn

int|string $id
来源：http://lj.lnxyls.cn

[U48] PHP：纯枚举
来源：http://wv.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cb.lnxyls.cn

[U49] PHP：只读属性
来源：http://di.9csxet.cn

public readonly string $name
来源：http://vt.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://to.nicolike.cn

public function __construct(private int $id) {}
来源：http://xt.lnxyls.cn

[U51] PHP：数组解构
来源：http://ja.huanxung.cn

[$a, $b] = $arr;
来源：http://xh.hnjuh.cn

[U52] PHP：箭头函数
来源：http://pi.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://dz.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://dt.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://hs.nszjky.cn

[U54] PHP：空安全调用
来源：http://eb.huanxung.cn

$obj?->method()
来源：http://fi.szsharing.cn

[U55] PHP：match 表达式
来源：http://xv.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wu.chemitech.net.cn

[U56] PHP：命名参数
来源：http://fy.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://ya.szsharing.cn

[U57] PHP：字符串插值
来源：http://as.bookmarksfly.cn

"值: {$a}"
来源：http://ze.szsharing.cn

[U58] PHP：数组三件套
来源：http://zk.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vd.chemitech.net.cn

[U59] PHP：自定义排序
来源：http://rl.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rj.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://wy.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://od.wgjwhj.cn

[U61] PHP：正则
来源：http://vy.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sn.gzmigu.cn

[U62] PHP：日期对象
来源：http://pl.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xd.szxytkj.cn

[U63] PHP：文件读写
来源：http://ar.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qq.521024.cn

[U64] PHP：目录遍历
来源：http://fs.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://jh.panjiajie.cn

[U65] PHP：会话
来源：http://tn.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xt.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://yr.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zv.colortex.cn

[U67] PHP：处理文件上传
来源：http://ie.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ia.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://fe.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ko.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://dw.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://no.huanxung.cn

[U70] PHP：PDO 事务
来源：http://dk.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jg.gzmigu.cn

[U71] PHP：抛出异常
来源：http://hh.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://jj.szxytkj.cn

[U72] PHP：写错误日志
来源：http://pg.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://af.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://zs.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://eg.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://mr.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://ok.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://et.colortex.cn

composer require psr/container
来源：http://tm.huixinmuqiang.cn

[U76] PHP：简单路由
来源：http://gw.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ks.521024.cn

[U77] PHP：模板渲染
来源：http://oh.gzmigu.cn

composer require twig/twig
来源：http://rl.yuntaijiaju.cn

[U78] PHP：单元测试
来源：http://xm.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://hx.muxihuayi.cn

[U79] PHP：静态分析
来源：http://nj.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://re.521024.cn

[U80] PHP：代码规范修复
来源：http://mk.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tj.521024.cn

[U81] JS：初始化项目
来源：http://dz.nszjky.cn

npm init -y;  npm i express
来源：http://mv.huanxung.cn

[U82] JS：package.json 脚本
来源：http://mb.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rh.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://ho.lnxyls.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gh.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://vn.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ha.shtwfgs.cn

[U85] JS：可选链
来源：http://xu.muxihuayi.cn

a?.b?.c
来源：http://ee.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://zj.shxzskj.cn

a ?? b
来源：http://tu.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://dk.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://oa.szsharing.cn

[U88] JS：对象展开合并
来源：http://fp.huixinmuqiang.cn

{ ...a, ...b }
来源：http://dr.bjjhwx.cn

[U89] JS：数组去重
来源：http://wk.521024.cn

[...new Set(arr)]
来源：http://zm.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://ap.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://jy.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://md.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ak.huanxung.cn

[U92] JS：深拷贝
来源：http://jg.huixiangedu.cn

structuredClone(obj)
来源：http://hc.chemitech.net.cn

[U93] JS：模板字符串
来源：http://gr.haigaiapp.cn

`共 ${n} 条`
来源：http://vx.huanxung.cn

[U94] JS：箭头函数
来源：http://zv.jctech888.com.cn

const double = x => x * 2;
来源：http://rb.hnjuh.cn

[U95] JS：Promise 包装
来源：http://yi.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://ut.newstarts.cn

[U96] JS：async/await 与异常
来源：http://lj.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ko.colortex.cn

[U97] JS：并发请求
来源：http://mn.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fi.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://pn.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://la.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://ds.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://wg.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://kx.panjiajie.cn

document.querySelector(".item")
来源：http://sc.bjjhwx.cn

[U101] JS：classList 操作
来源：http://fp.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://ib.muxihuayi.cn

[U102] JS：本地存储
来源：http://zq.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://om.shxzskj.cn

[U103] JS：定时器
来源：http://dd.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jm.huixinmuqiang.cn

[U104] JS：防抖
来源：http://je.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hv.hnjuh.cn

[U105] JS：节流
来源：http://vo.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ip.9csxet.cn

[U106] JS：日期格式化
来源：http://rs.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://og.haigaiapp.cn

[U107] JS：数字千分位
来源：http://if.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wq.shtwfgs.cn

[U108] JS：随机整数
来源：http://yj.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ax.asd995.cn

[U109] JS：数组分组
来源：http://jf.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://om.muxihuayi.cn

[U110] JS：数组分块
来源：http://pd.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mw.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://jl.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://oz.521024.cn

[U112] JS：字符串补位
来源：http://io.bjjhwx.cn

"7".padStart(3, "0")
来源：http://da.hnjuh.cn

[U113] JS：正则替换全部
来源：http://yt.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://yw.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://sx.colortex.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kf.shxzukj.cn

[U115] JS：生成 UUID
来源：http://uc.hahajie.cn

crypto.randomUUID()
来源：http://np.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://zd.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://to.haigaiapp.cn

[U117] JS：单元测试
来源：http://gz.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://lm.colortex.cn

[U118] JS：开发服务器
来源：http://bz.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://tq.huixiangedu.cn

[U119] JS：生产构建
来源：http://mj.gzmigu.cn

npx vite build
来源：http://yd.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ja.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://sz.nicolike.cn

================================================================================
来源：http://uz.wgjwhj.cn

统计汇总
来源：http://fj.jctech888.com.cn

================================================================================
来源：http://kj.bookmarksfly.cn

按语言统计（条）：
来源：http://yu.jctech888.com.cn

Python ......... 252
来源：http://fz.jctech888.com.cn

PHP ............ 252
来源：http://ws.wgjwhj.cn

JavaScript ..... 252
来源：http://fw.nszjky.cn

TypeScript ..... 212
来源：http://eg.shtwfgs.cn

Java ........... 212
来源：http://dv.huixiangedu.cn

Go ............. 212
来源：http://se.huixiangedu.cn

Ruby ........... 212
来源：http://vz.hahajie.cn

C# ............. 212
来源：http://qw.shxzskj.cn

C .............. 30
来源：http://qq.shtwfgs.cn

C++ ............ 30
来源：http://ra.521024.cn

SQL ............ 90
来源：http://sh.lnxyls.cn

Bash ........... 80
来源：http://hc.nszjky.cn

Kotlin ......... 15
来源：http://pk.nszjky.cn

Swift .......... 15
来源：http://ky.chemitech.net.cn

Lua ............ 10
来源：http://qt.9csxet.cn

Perl ........... 10
来源：http://vc.bjjhwx.cn

Scala .......... 10
来源：http://ao.nicolike.cn

------------------------------------
来源：http://pl.jctech888.com.cn

合计 ........... 2106 条
来源：http://yh.shxzskj.cn

按章节统计：
来源：http://eb.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fx.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lk.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sn.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://io.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tz.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dt.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cl.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yk.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rp.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ev.szsharing.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dd.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pu.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bd.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ml.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qk.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wl.shtwfgs.cn

Q SQL 专题                              90
来源：http://yl.jianghongdianzi.cn

R Bash 专题                             80
来源：http://pz.yuexingan06.cn

S C / C++ 专题                          60
来源：http://qq.9csxet.cn

T 其他语言补充                          60
来源：http://wh.shtwfgs.cn

U 高频实用片段                         120
来源：http://yp.lnxyls.cn

------------------------------------
来源：http://xg.521024.cn

合计                                  2106 条
来源：http://jg.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://iu.yuexingan06.cn

使用提醒
来源：http://se.huanxung.cn

--------------------------------------------------------------------------------
来源：http://mf.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tq.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jy.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sb.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://db.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gv.nszjky.cn

—— 文件结束 ——
来源：http://ef.panjiajie.cn

================================================================================
来源：http://wm.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://nj.9csxet.cn

Common Programming Examples Cheat Book
来源：http://hu.huanxung.cn

================================================================================
来源：http://df.huixinmuqiang.cn

【收录内容】
来源：http://wb.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://by.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cy.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://bl.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ka.nszjky.cn

【使用说明】
来源：http://mg.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ih.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xd.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wm.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xg.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hj.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sk.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ng.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mt.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ia.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://be.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cg.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ap.bookmarksfly.cn

【文件统计】
来源：http://wy.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mj.colortex.cn

--------------------------------------------------------------------------------
来源：http://hg.wgjwhj.cn

目  录
来源：http://rm.nicolike.cn

--------------------------------------------------------------------------------
来源：http://ga.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://am.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sm.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qx.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jg.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ig.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vr.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kd.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ys.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iv.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pf.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wd.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bo.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://af.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fm.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ph.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ay.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lm.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qp.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hc.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jk.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gd.szsharing.cn

================================================================================
来源：http://pz.haigaiapp.cn

A. 基础语法与类型
来源：http://ks.hnjuh.cn

================================================================================
来源：http://ky.newstarts.cn

[A01] Hello World
来源：http://cy.lnxyls.cn

Py:   print("Hello, World!")
来源：http://bb.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://bk.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://gr.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gg.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://cj.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://ng.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://vy.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://le.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://qi.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vg.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ge.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hu.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pp.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://ga.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://ls.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://sc.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zo.hahajie.cn

[A03] 常量定义
来源：http://mo.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dy.colortex.cn

PHP:  const PI = 3.14159;
来源：http://ld.hahajie.cn

JS:   const PI = 3.14159;
来源：http://ac.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://tp.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://uc.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://iu.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://jt.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://mo.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://hp.hnjuh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://be.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://be.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jr.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://vl.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wn.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ev.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://av.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://hn.lnxyls.cn

[A05] 整数除法与取模
来源：http://gk.chemitech.net.cn


<!-- 参考信息 -->