代发 wailian999

[U43] PHP：声明命名空间
来源：http://vm.huixiangedu.cn

namespace App\Http;
来源：http://hv.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://aw.521024.cn

declare(strict_types=1);
来源：http://lx.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://ty.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yt.huanxung.cn

[U46] PHP：可空类型
来源：http://ws.chemitech.net.cn

?string $name = null
来源：http://ns.szsharing.cn

[U47] PHP：联合类型
来源：http://fq.chemitech.net.cn

int|string $id
来源：http://pc.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://by.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nc.shxzskj.cn

[U49] PHP：只读属性
来源：http://wi.panjiajie.cn

public readonly string $name
来源：http://vd.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://ed.nszjky.cn

public function __construct(private int $id) {}
来源：http://rl.haigaiapp.cn

[U51] PHP：数组解构
来源：http://rs.shxzskj.cn

[$a, $b] = $arr;
来源：http://uz.huanxung.cn

[U52] PHP：箭头函数
来源：http://wj.521024.cn

$double = fn($x) => $x * 2;
来源：http://zl.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://mp.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://wp.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://iq.jctech888.com.cn

$obj?->method()
来源：http://wa.newstarts.cn

[U55] PHP：match 表达式
来源：http://bk.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qt.hnjuh.cn

[U56] PHP：命名参数
来源：http://op.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://tt.szxytkj.cn

[U57] PHP：字符串插值
来源：http://lm.muxihuayi.cn

"值: {$a}"
来源：http://zw.gzmigu.cn

[U58] PHP：数组三件套
来源：http://pv.yuntaijiaju.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mf.huanxung.cn

[U59] PHP：自定义排序
来源：http://xe.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qr.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://qc.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vf.521024.cn

[U61] PHP：正则
来源：http://xl.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dl.shxzukj.cn

[U62] PHP：日期对象
来源：http://fp.shtwfgs.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ka.szxytkj.cn

[U63] PHP：文件读写
来源：http://qd.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vr.shxzskj.cn

[U64] PHP：目录遍历
来源：http://hs.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://hy.521024.cn

[U65] PHP：会话
来源：http://hn.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fi.gzmigu.cn

[U66] PHP：设置 Cookie
来源：http://hf.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gg.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://lc.szsharing.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ka.szsharing.cn

[U68] PHP：PDO 连接
来源：http://kh.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bn.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://qh.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dg.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://dg.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dh.shxzskj.cn

[U71] PHP：抛出异常
来源：http://mv.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://wf.shxzukj.cn

[U72] PHP：写错误日志
来源：http://ck.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://by.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://tb.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://xc.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://mz.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://hx.shxzskj.cn

[U75] PHP：依赖注入
来源：http://en.muxihuayi.cn

composer require psr/container
来源：http://rf.colortex.cn

[U76] PHP：简单路由
来源：http://nf.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ln.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://fc.shtwfgs.cn

composer require twig/twig
来源：http://ab.lnxyls.cn

[U78] PHP：单元测试
来源：http://fp.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://la.nicolike.cn

[U79] PHP：静态分析
来源：http://th.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://bo.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://et.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ua.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://hg.bookmarksfly.cn

npm init -y;  npm i express
来源：http://fm.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://ti.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kg.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://dv.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ww.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://je.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dm.521024.cn

[U85] JS：可选链
来源：http://gw.colortex.cn

a?.b?.c
来源：http://ku.lnxyls.cn

[U86] JS：空值合并
来源：http://zd.521024.cn

a ?? b
来源：http://fy.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://hb.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://yd.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://xf.lnxyls.cn

{ ...a, ...b }
来源：http://hl.lnxyls.cn

[U89] JS：数组去重
来源：http://ol.wgjwhj.cn

[...new Set(arr)]
来源：http://sp.newstarts.cn

[U90] JS：数字数组排序
来源：http://lc.lnxyls.cn

[...arr].sort((a, b) => a - b)
来源：http://qe.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://sj.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lk.nicolike.cn

[U92] JS：深拷贝
来源：http://ax.huixinmuqiang.cn

structuredClone(obj)
来源：http://be.panjiajie.cn

[U93] JS：模板字符串
来源：http://if.newstarts.cn

`共 ${n} 条`
来源：http://rq.panjiajie.cn

[U94] JS：箭头函数
来源：http://hi.szsharing.cn

const double = x => x * 2;
来源：http://dw.panjiajie.cn

[U95] JS：Promise 包装
来源：http://mq.9csxet.cn

new Promise((resolve, reject) => {})
来源：http://zo.hahajie.cn

[U96] JS：async/await 与异常
来源：http://if.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rv.9csxet.cn

[U97] JS：并发请求
来源：http://ez.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vq.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://hg.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uq.hahajie.cn

[U99] JS：事件监听
来源：http://zj.9csxet.cn

el.addEventListener("click", e => {})
来源：http://qt.gzmigu.cn

[U100] JS：DOM 查询
来源：http://oq.panjiajie.cn

document.querySelector(".item")
来源：http://bz.szsharing.cn

[U101] JS：classList 操作
来源：http://tj.szsharing.cn

el.classList.toggle("active")
来源：http://rk.haigaiapp.cn

[U102] JS：本地存储
来源：http://tp.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ov.yuntaijiaju.cn

[U103] JS：定时器
来源：http://ap.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rr.bjjhwx.cn

[U104] JS：防抖
来源：http://aa.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wm.bjjhwx.cn

[U105] JS：节流
来源：http://fm.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yc.jctech888.com.cn

[U106] JS：日期格式化
来源：http://pn.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dv.shxzskj.cn

[U107] JS：数字千分位
来源：http://wd.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fg.521024.cn

[U108] JS：随机整数
来源：http://ux.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oh.yuexingan06.cn

[U109] JS：数组分组
来源：http://ae.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://ya.chemitech.net.cn

[U110] JS：数组分块
来源：http://ov.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cg.szsharing.cn

[U111] JS：对象转 Map
来源：http://pe.lnxyls.cn

new Map(Object.entries(obj))
来源：http://xj.shxzskj.cn

[U112] JS：字符串补位
来源：http://ww.shtwfgs.cn

"7".padStart(3, "0")
来源：http://ei.hnjuh.cn

[U113] JS：正则替换全部
来源：http://dv.asd995.cn

s.replaceAll("a", "b")
来源：http://qc.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://ny.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xm.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://px.lnxyls.cn

crypto.randomUUID()
来源：http://cp.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://ea.nicolike.cn

/** @param {string} name */ function f(name) {}
来源：http://lk.szxytkj.cn

[U117] JS：单元测试
来源：http://hf.asd995.cn

npm i -D vitest;  npx vitest
来源：http://tv.haigaiapp.cn

[U118] JS：开发服务器
来源：http://ue.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://th.wgjwhj.cn

[U119] JS：生产构建
来源：http://vw.asd995.cn

npx vite build
来源：http://oi.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://rz.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://sd.gzmigu.cn

================================================================================
来源：http://bv.yuntaijiaju.cn

统计汇总
来源：http://tk.shtwfgs.cn

================================================================================
来源：http://hc.shxzskj.cn

按语言统计（条）：
来源：http://je.muxihuayi.cn

Python ......... 252
来源：http://sw.bjjhwx.cn

PHP ............ 252
来源：http://cw.nicolike.cn

JavaScript ..... 252
来源：http://cg.colortex.cn

TypeScript ..... 212
来源：http://ke.bookmarksfly.cn

Java ........... 212
来源：http://xu.panjiajie.cn

Go ............. 212
来源：http://nu.jianghongdianzi.cn

Ruby ........... 212
来源：http://lk.bjjhwx.cn

C# ............. 212
来源：http://ca.gzmigu.cn

C .............. 30
来源：http://pw.bjjhwx.cn

C++ ............ 30
来源：http://lq.haigaiapp.cn

SQL ............ 90
来源：http://tw.szxytkj.cn

Bash ........... 80
来源：http://jc.bookmarksfly.cn

Kotlin ......... 15
来源：http://ir.jctech888.com.cn

Swift .......... 15
来源：http://py.asd995.cn

Lua ............ 10
来源：http://xb.huixiangedu.cn

Perl ........... 10
来源：http://xd.huixiangedu.cn

Scala .......... 10
来源：http://pm.shxzskj.cn

------------------------------------
来源：http://wp.asd995.cn

合计 ........... 2106 条
来源：http://zh.shtwfgs.cn

按章节统计：
来源：http://wx.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://od.gzmigu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yw.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pg.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cf.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qq.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tk.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ep.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vn.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ul.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gt.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wq.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://on.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://to.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hn.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://si.huixinmuqiang.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://by.huanxung.cn

Q SQL 专题                              90
来源：http://ln.haigaiapp.cn

R Bash 专题                             80
来源：http://ty.muxihuayi.cn

S C / C++ 专题                          60
来源：http://qp.haigaiapp.cn

T 其他语言补充                          60
来源：http://ir.hnjuh.cn

U 高频实用片段                         120
来源：http://ll.huixiangedu.cn

------------------------------------
来源：http://gf.shxzukj.cn

合计                                  2106 条
来源：http://ho.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://rb.szxytkj.cn

使用提醒
来源：http://ro.hahajie.cn

--------------------------------------------------------------------------------
来源：http://tv.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://na.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gm.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://db.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ve.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uf.nszjky.cn

—— 文件结束 ——
来源：http://dt.panjiajie.cn

================================================================================
来源：http://si.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://wb.colortex.cn

Common Programming Examples Cheat Book
来源：http://gu.hnjuh.cn

================================================================================
来源：http://ne.bookmarksfly.cn

【收录内容】
来源：http://ek.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qa.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ji.gzmigu.cn

SQL · Bash · C · C++
来源：http://wg.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vc.bjjhwx.cn

【使用说明】
来源：http://cz.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jv.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pc.huixinmuqiang.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fu.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vo.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cb.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fe.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rw.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ur.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hn.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yu.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://il.panjiajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ml.hahajie.cn

【文件统计】
来源：http://ss.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kd.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://lo.hnjuh.cn

目  录
来源：http://wh.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://do.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hl.jianghongdianzi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ct.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jt.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uw.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lo.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bo.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fo.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dd.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fy.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://do.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ug.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bo.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bq.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bc.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mk.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xu.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tp.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nv.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ql.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pn.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ol.jctech888.com.cn

================================================================================
来源：http://ft.wgjwhj.cn

A. 基础语法与类型
来源：http://ui.yuntaijiaju.cn

================================================================================
来源：http://wr.huixinmuqiang.cn

[A01] Hello World
来源：http://yf.shxzukj.cn

Py:   print("Hello, World!")
来源：http://yv.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://kp.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://ta.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tu.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://gr.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://rx.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://to.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vo.hahajie.cn

[A02] 变量声明与赋值
来源：http://kn.muxihuayi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sh.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nm.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yg.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pu.nicolike.cn

Java: String name = "Alex"; int age = 20;
来源：http://ek.huixinmuqiang.cn

Go:   name := "Alex"; age := 20
来源：http://jo.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://jo.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cv.newstarts.cn

[A03] 常量定义
来源：http://en.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fn.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://qz.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://ud.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://wm.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://tr.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://tl.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://yt.521024.cn

C#:   const double PI = 3.14159;
来源：http://ge.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://hw.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qk.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yv.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ap.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://op.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rl.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hr.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://re.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://km.jctech888.com.cn

[A05] 整数除法与取模
来源：http://wt.yuexingan06.cn


<!-- 参考信息 -->