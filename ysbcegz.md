代发 wailian999

[U43] PHP：声明命名空间
来源：http://bh.bjjhwx.cn

namespace App\Http;
来源：http://gb.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://rv.huixiangedu.cn

declare(strict_types=1);
来源：http://xn.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://th.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uz.hnjuh.cn

[U46] PHP：可空类型
来源：http://se.yuexingan06.cn

?string $name = null
来源：http://yc.chemitech.net.cn

[U47] PHP：联合类型
来源：http://ld.shxzukj.cn

int|string $id
来源：http://qo.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://aw.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://we.szxytkj.cn

[U49] PHP：只读属性
来源：http://ci.hahajie.cn

public readonly string $name
来源：http://ue.asd995.cn

[U50] PHP：构造器属性提升
来源：http://xo.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://ne.huanxung.cn

[U51] PHP：数组解构
来源：http://oe.colortex.cn

[$a, $b] = $arr;
来源：http://dh.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://kq.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://oi.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://vb.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://lo.9csxet.cn

[U54] PHP：空安全调用
来源：http://eq.wgjwhj.cn

$obj?->method()
来源：http://bi.yuntaijiaju.cn

[U55] PHP：match 表达式
来源：http://sf.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tr.shxzskj.cn

[U56] PHP：命名参数
来源：http://of.9csxet.cn

f(a: 1, b: 2)
来源：http://xp.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://kd.chemitech.net.cn

"值: {$a}"
来源：http://zj.gzmigu.cn

[U58] PHP：数组三件套
来源：http://uw.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ef.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://qy.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ex.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://oc.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://it.yuntaijiaju.cn

[U61] PHP：正则
来源：http://do.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lq.asd995.cn

[U62] PHP：日期对象
来源：http://oi.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aa.521024.cn

[U63] PHP：文件读写
来源：http://in.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jv.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://ob.shxzukj.cn

glob("dir/*.php");  scandir("dir");
来源：http://kk.jianghongdianzi.cn

[U65] PHP：会话
来源：http://pi.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tn.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://zv.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zs.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://xn.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://or.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://fv.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ms.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://ln.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wk.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://tf.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uu.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://aa.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://xv.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://cb.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://wk.wgjwhj.cn

[U73] PHP：读取 ini 配置
来源：http://qc.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://gf.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://cl.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://fy.newstarts.cn

[U75] PHP：依赖注入
来源：http://uz.nicolike.cn

composer require psr/container
来源：http://xg.asd995.cn

[U76] PHP：简单路由
来源：http://qd.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yh.colortex.cn

[U77] PHP：模板渲染
来源：http://nl.shxzukj.cn

composer require twig/twig
来源：http://wd.szsharing.cn

[U78] PHP：单元测试
来源：http://tw.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://dz.huixiangedu.cn

[U79] PHP：静态分析
来源：http://rr.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://ve.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://at.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tl.wgjwhj.cn

[U81] JS：初始化项目
来源：http://jg.nicolike.cn

npm init -y;  npm i express
来源：http://hy.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://mm.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bj.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://ys.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://au.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://hl.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lx.wgjwhj.cn

[U85] JS：可选链
来源：http://tk.jianghongdianzi.cn

a?.b?.c
来源：http://ec.521024.cn

[U86] JS：空值合并
来源：http://eq.panjiajie.cn

a ?? b
来源：http://il.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://nr.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://du.9csxet.cn

[U88] JS：对象展开合并
来源：http://kp.haigaiapp.cn

{ ...a, ...b }
来源：http://hg.gzmigu.cn

[U89] JS：数组去重
来源：http://bh.shxzukj.cn

[...new Set(arr)]
来源：http://ut.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://uz.colortex.cn

[...arr].sort((a, b) => a - b)
来源：http://lc.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://dp.bookmarksfly.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ri.chemitech.net.cn

[U92] JS：深拷贝
来源：http://xr.asd995.cn

structuredClone(obj)
来源：http://cs.9csxet.cn

[U93] JS：模板字符串
来源：http://aj.yuexingan06.cn

`共 ${n} 条`
来源：http://ci.jctech888.com.cn

[U94] JS：箭头函数
来源：http://fl.muxihuayi.cn

const double = x => x * 2;
来源：http://xa.panjiajie.cn

[U95] JS：Promise 包装
来源：http://ew.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://hb.9csxet.cn

[U96] JS：async/await 与异常
来源：http://tx.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ie.521024.cn

[U97] JS：并发请求
来源：http://cy.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wy.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://zh.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ta.jctech888.com.cn

[U99] JS：事件监听
来源：http://jc.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://ka.hahajie.cn

[U100] JS：DOM 查询
来源：http://qk.lnxyls.cn

document.querySelector(".item")
来源：http://jo.nszjky.cn

[U101] JS：classList 操作
来源：http://zt.bookmarksfly.cn

el.classList.toggle("active")
来源：http://kc.szsharing.cn

[U102] JS：本地存储
来源：http://xz.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zt.bookmarksfly.cn

[U103] JS：定时器
来源：http://of.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zo.lnxyls.cn

[U104] JS：防抖
来源：http://sn.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hv.bookmarksfly.cn

[U105] JS：节流
来源：http://it.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fq.gzmigu.cn

[U106] JS：日期格式化
来源：http://rd.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zd.lnxyls.cn

[U107] JS：数字千分位
来源：http://mz.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kq.9csxet.cn

[U108] JS：随机整数
来源：http://bl.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uh.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://es.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://wc.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://ar.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lz.521024.cn

[U111] JS：对象转 Map
来源：http://hm.gzmigu.cn

new Map(Object.entries(obj))
来源：http://ok.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://qf.hahajie.cn

"7".padStart(3, "0")
来源：http://do.colortex.cn

[U113] JS：正则替换全部
来源：http://om.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://ck.szsharing.cn

[U114] JS：JSON 深比较
来源：http://je.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gp.szsharing.cn

[U115] JS：生成 UUID
来源：http://td.hahajie.cn

crypto.randomUUID()
来源：http://kx.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://xg.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://mu.chemitech.net.cn

[U117] JS：单元测试
来源：http://xv.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://wy.hnjuh.cn

[U118] JS：开发服务器
来源：http://du.szxytkj.cn

npm i -D vite;  npx vite
来源：http://uv.huixiangedu.cn

[U119] JS：生产构建
来源：http://fr.huanxung.cn

npx vite build
来源：http://rb.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ak.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://he.shtwfgs.cn

================================================================================
来源：http://lz.muxihuayi.cn

统计汇总
来源：http://ho.nszjky.cn

================================================================================
来源：http://tt.newstarts.cn

按语言统计（条）：
来源：http://dx.panjiajie.cn

Python ......... 252
来源：http://xt.lnxyls.cn

PHP ............ 252
来源：http://qh.yuexingan06.cn

JavaScript ..... 252
来源：http://ck.bookmarksfly.cn

TypeScript ..... 212
来源：http://ga.muxihuayi.cn

Java ........... 212
来源：http://uv.chemitech.net.cn

Go ............. 212
来源：http://lr.9csxet.cn

Ruby ........... 212
来源：http://hq.chemitech.net.cn

C# ............. 212
来源：http://fi.nszjky.cn

C .............. 30
来源：http://ze.gzmigu.cn

C++ ............ 30
来源：http://si.yuntaijiaju.cn

SQL ............ 90
来源：http://lm.colortex.cn

Bash ........... 80
来源：http://km.nszjky.cn

Kotlin ......... 15
来源：http://tu.shxzukj.cn

Swift .......... 15
来源：http://as.szxytkj.cn

Lua ............ 10
来源：http://mv.wgjwhj.cn

Perl ........... 10
来源：http://co.bjjhwx.cn

Scala .......... 10
来源：http://is.shtwfgs.cn

------------------------------------
来源：http://qw.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://lp.chemitech.net.cn

按章节统计：
来源：http://nh.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fq.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oy.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wz.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ke.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://un.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hf.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xm.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ow.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hp.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jv.wgjwhj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ci.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://md.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uy.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sg.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tq.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ht.yuexingan06.cn

Q SQL 专题                              90
来源：http://yb.bookmarksfly.cn

R Bash 专题                             80
来源：http://hw.nszjky.cn

S C / C++ 专题                          60
来源：http://zm.colortex.cn

T 其他语言补充                          60
来源：http://jz.hnjuh.cn

U 高频实用片段                         120
来源：http://rz.hnjuh.cn

------------------------------------
来源：http://ow.huixinmuqiang.cn

合计                                  2106 条
来源：http://oe.521024.cn

--------------------------------------------------------------------------------
来源：http://ov.chemitech.net.cn

使用提醒
来源：http://mb.szsharing.cn

--------------------------------------------------------------------------------
来源：http://xk.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vn.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zp.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gg.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kf.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://np.shtwfgs.cn

—— 文件结束 ——
来源：http://vx.lnxyls.cn

================================================================================
来源：http://yq.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://tz.nicolike.cn

Common Programming Examples Cheat Book
来源：http://je.yuntaijiaju.cn

================================================================================
来源：http://sk.szsharing.cn

【收录内容】
来源：http://nz.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oz.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fn.jctech888.com.cn

SQL · Bash · C · C++
来源：http://sb.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pq.bookmarksfly.cn

【使用说明】
来源：http://ff.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gh.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aa.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tp.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vw.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wd.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lk.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://co.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jc.521024.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yb.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ut.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yf.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://um.wgjwhj.cn

【文件统计】
来源：http://hr.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://az.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://oz.bookmarksfly.cn

目  录
来源：http://qw.szsharing.cn

--------------------------------------------------------------------------------
来源：http://wi.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fs.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rn.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dy.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qr.yuntaijiaju.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hn.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mk.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://av.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eb.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tq.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nn.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vf.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xo.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tw.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qy.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dz.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oa.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yc.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qx.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xr.newstarts.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oo.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qx.shtwfgs.cn

================================================================================
来源：http://kk.wgjwhj.cn

A. 基础语法与类型
来源：http://wm.jianghongdianzi.cn

================================================================================
来源：http://um.bjjhwx.cn

[A01] Hello World
来源：http://na.asd995.cn

Py:   print("Hello, World!")
来源：http://zn.colortex.cn

PHP:  echo "Hello, World!";
来源：http://nh.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://pn.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nl.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://cy.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://rb.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://vz.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ck.hnjuh.cn

[A02] 变量声明与赋值
来源：http://fx.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uq.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yl.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://se.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ni.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://nf.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://or.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://kz.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mm.shtwfgs.cn

[A03] 常量定义
来源：http://hg.szsharing.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sr.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://im.nicolike.cn

JS:   const PI = 3.14159;
来源：http://xm.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://cm.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://ez.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://uc.huanxung.cn

Ruby: PI = 3.14159
来源：http://le.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://qx.colortex.cn

[A04] 判断变量类型
来源：http://qa.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sc.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ig.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://af.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://ui.chemitech.net.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zt.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zi.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tx.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://je.wgjwhj.cn

[A05] 整数除法与取模
来源：http://cm.wgjwhj.cn


<!-- 参考信息 -->