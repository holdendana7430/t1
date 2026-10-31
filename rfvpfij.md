代发 wailian999

[U43] PHP：声明命名空间
来源：http://ig.yuntaijiaju.cn

namespace App\Http;
来源：http://ig.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://cc.panjiajie.cn

declare(strict_types=1);
来源：http://ya.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://cy.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tw.szxytkj.cn

[U46] PHP：可空类型
来源：http://qt.yuntaijiaju.cn

?string $name = null
来源：http://uk.nicolike.cn

[U47] PHP：联合类型
来源：http://rz.9csxet.cn

int|string $id
来源：http://ri.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://bf.huanxung.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rw.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://fc.newstarts.cn

public readonly string $name
来源：http://xu.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://ld.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://yh.nszjky.cn

[U51] PHP：数组解构
来源：http://pl.huixiangedu.cn

[$a, $b] = $arr;
来源：http://dv.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://gh.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://xx.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://ae.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://gr.521024.cn

[U54] PHP：空安全调用
来源：http://ql.gzmigu.cn

$obj?->method()
来源：http://rl.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://ne.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ec.lnxyls.cn

[U56] PHP：命名参数
来源：http://ip.9csxet.cn

f(a: 1, b: 2)
来源：http://pu.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://xn.lnxyls.cn

"值: {$a}"
来源：http://yg.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://gt.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pn.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://xf.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://db.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://hg.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mk.9csxet.cn

[U61] PHP：正则
来源：http://te.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iy.wgjwhj.cn

[U62] PHP：日期对象
来源：http://gx.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xj.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://pu.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gk.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://gv.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://km.nicolike.cn

[U65] PHP：会话
来源：http://wn.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kt.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://ut.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zn.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://rg.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ij.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://ao.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://av.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://df.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aq.nszjky.cn

[U70] PHP：PDO 事务
来源：http://ru.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yj.gzmigu.cn

[U71] PHP：抛出异常
来源：http://gg.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://iq.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://ov.szsharing.cn

error_log("失败: " . $e->getMessage());
来源：http://mf.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://ow.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://fj.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://dm.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://gk.shxzukj.cn

[U75] PHP：依赖注入
来源：http://tn.9csxet.cn

composer require psr/container
来源：http://lc.jctech888.com.cn

[U76] PHP：简单路由
来源：http://yd.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hk.hnjuh.cn

[U77] PHP：模板渲染
来源：http://sm.hnjuh.cn

composer require twig/twig
来源：http://mt.521024.cn

[U78] PHP：单元测试
来源：http://ze.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://io.9csxet.cn

[U79] PHP：静态分析
来源：http://zk.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://wb.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://sz.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://co.jctech888.com.cn

[U81] JS：初始化项目
来源：http://ch.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://xl.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://ur.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cg.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://sf.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://px.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://ey.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oo.shtwfgs.cn

[U85] JS：可选链
来源：http://ep.jianghongdianzi.cn

a?.b?.c
来源：http://tu.lnxyls.cn

[U86] JS：空值合并
来源：http://kk.wgjwhj.cn

a ?? b
来源：http://fz.shtwfgs.cn

[U87] JS：解构默认值
来源：http://ng.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://zb.colortex.cn

[U88] JS：对象展开合并
来源：http://vc.gzmigu.cn

{ ...a, ...b }
来源：http://sd.hahajie.cn

[U89] JS：数组去重
来源：http://ck.szxytkj.cn

[...new Set(arr)]
来源：http://ul.nszjky.cn

[U90] JS：数字数组排序
来源：http://fm.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://xt.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://wm.gzmigu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zu.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://wd.yuexingan06.cn

structuredClone(obj)
来源：http://gs.nicolike.cn

[U93] JS：模板字符串
来源：http://jv.521024.cn

`共 ${n} 条`
来源：http://qw.gzmigu.cn

[U94] JS：箭头函数
来源：http://wr.yuntaijiaju.cn

const double = x => x * 2;
来源：http://wi.panjiajie.cn

[U95] JS：Promise 包装
来源：http://bv.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://hd.szsharing.cn

[U96] JS：async/await 与异常
来源：http://ix.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gm.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://fz.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ev.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://xe.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yh.nicolike.cn

[U99] JS：事件监听
来源：http://zj.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://vt.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://kw.huanxung.cn

document.querySelector(".item")
来源：http://nb.wgjwhj.cn

[U101] JS：classList 操作
来源：http://qn.huanxung.cn

el.classList.toggle("active")
来源：http://rb.nszjky.cn

[U102] JS：本地存储
来源：http://vj.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://en.huixinmuqiang.cn

[U103] JS：定时器
来源：http://bq.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ur.9csxet.cn

[U104] JS：防抖
来源：http://hu.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qk.szsharing.cn

[U105] JS：节流
来源：http://bw.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qd.chemitech.net.cn

[U106] JS：日期格式化
来源：http://gy.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lt.bjjhwx.cn

[U107] JS：数字千分位
来源：http://uv.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vk.yuexingan06.cn

[U108] JS：随机整数
来源：http://fq.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xv.shxzskj.cn

[U109] JS：数组分组
来源：http://mp.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://vc.hahajie.cn

[U110] JS：数组分块
来源：http://zm.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://om.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://jl.lnxyls.cn

new Map(Object.entries(obj))
来源：http://ar.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://fm.shtwfgs.cn

"7".padStart(3, "0")
来源：http://xj.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://ue.hnjuh.cn

s.replaceAll("a", "b")
来源：http://sc.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://kl.hahajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xe.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://nq.szxytkj.cn

crypto.randomUUID()
来源：http://qt.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://vp.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://bw.panjiajie.cn

[U117] JS：单元测试
来源：http://sm.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://ri.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://ng.521024.cn

npm i -D vite;  npx vite
来源：http://rl.bjjhwx.cn

[U119] JS：生产构建
来源：http://rz.shtwfgs.cn

npx vite build
来源：http://ur.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://um.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://km.szxytkj.cn

================================================================================
来源：http://xa.shxzukj.cn

统计汇总
来源：http://ub.gzmigu.cn

================================================================================
来源：http://zp.nszjky.cn

按语言统计（条）：
来源：http://qz.hahajie.cn

Python ......... 252
来源：http://wb.huixiangedu.cn

PHP ............ 252
来源：http://hn.521024.cn

JavaScript ..... 252
来源：http://yv.hahajie.cn

TypeScript ..... 212
来源：http://cl.szsharing.cn

Java ........... 212
来源：http://my.bookmarksfly.cn

Go ............. 212
来源：http://xj.jctech888.com.cn

Ruby ........... 212
来源：http://rv.muxihuayi.cn

C# ............. 212
来源：http://rl.jctech888.com.cn

C .............. 30
来源：http://mx.shxzukj.cn

C++ ............ 30
来源：http://fr.jctech888.com.cn

SQL ............ 90
来源：http://ge.muxihuayi.cn

Bash ........... 80
来源：http://dx.yuexingan06.cn

Kotlin ......... 15
来源：http://ec.newstarts.cn

Swift .......... 15
来源：http://mi.hnjuh.cn

Lua ............ 10
来源：http://qs.nicolike.cn

Perl ........... 10
来源：http://ks.521024.cn

Scala .......... 10
来源：http://sv.bjjhwx.cn

------------------------------------
来源：http://dw.chemitech.net.cn

合计 ........... 2106 条
来源：http://rc.huixinmuqiang.cn

按章节统计：
来源：http://la.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sn.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ce.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ry.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zg.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ck.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uq.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cj.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sa.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bo.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qd.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wj.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nx.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iw.jianghongdianzi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tt.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zb.colortex.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sl.muxihuayi.cn

Q SQL 专题                              90
来源：http://dj.colortex.cn

R Bash 专题                             80
来源：http://yo.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://ov.huixiangedu.cn

T 其他语言补充                          60
来源：http://an.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://ik.colortex.cn

------------------------------------
来源：http://bo.newstarts.cn

合计                                  2106 条
来源：http://rg.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://mc.jianghongdianzi.cn

使用提醒
来源：http://cy.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ym.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jc.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zw.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hy.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sm.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://st.wgjwhj.cn

—— 文件结束 ——
来源：http://qw.yuexingan06.cn

================================================================================
来源：http://db.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://zl.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://kp.yuexingan06.cn

================================================================================
来源：http://ik.521024.cn

【收录内容】
来源：http://cl.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://co.huixiangedu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://es.wgjwhj.cn

SQL · Bash · C · C++
来源：http://qm.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bz.nicolike.cn

【使用说明】
来源：http://ju.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fy.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nl.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hj.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://de.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zf.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yw.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uo.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hx.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qj.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zr.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pc.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ym.jctech888.com.cn

【文件统计】
来源：http://wg.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fn.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ar.asd995.cn

目  录
来源：http://ks.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://th.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://je.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qw.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vp.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mc.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dt.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://em.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hm.shtwfgs.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vy.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zt.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uy.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mm.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gl.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bf.hahajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ot.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dl.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qj.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ok.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jm.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fx.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xk.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bs.yuexingan06.cn

================================================================================
来源：http://ik.nicolike.cn

A. 基础语法与类型
来源：http://qj.muxihuayi.cn

================================================================================
来源：http://bm.yuntaijiaju.cn

[A01] Hello World
来源：http://fs.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://by.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://ob.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://hx.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ul.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://nz.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://oj.asd995.cn

Ruby: puts "Hello, World!"
来源：http://cv.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://eb.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://yi.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vu.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://le.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rs.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sp.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://la.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://im.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://ze.huixiangedu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dl.nszjky.cn

[A03] 常量定义
来源：http://nc.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qx.521024.cn

PHP:  const PI = 3.14159;
来源：http://pv.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://ba.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://ss.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://ps.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://bt.szxytkj.cn

Ruby: PI = 3.14159
来源：http://sw.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://af.9csxet.cn

[A04] 判断变量类型
来源：http://tt.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://km.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xk.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hm.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://jj.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tb.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://se.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fd.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://yo.newstarts.cn

[A05] 整数除法与取模
来源：http://ku.asd995.cn


<!-- 参考信息 -->