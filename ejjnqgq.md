代发 wailian999

[U35] Py：发送邮件
来源：http://it.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vh.bjjhwx.cn

[U36] Py：定时任务
来源：http://bk.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://cz.nszjky.cn

[U37] Py：读写 Excel
来源：http://pq.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rh.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://ad.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://kk.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://vs.shxzukj.cn

sys.stdout.isatty()
来源：http://af.521024.cn

[U40] Py：打印到标准错误
来源：http://lz.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://iy.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://is.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://to.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://wh.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gl.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://ax.bookmarksfly.cn

namespace App\Http;
来源：http://lx.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://wz.yuexingan06.cn

declare(strict_types=1);
来源：http://ru.szxytkj.cn

[U45] PHP：类型声明与返回类型
来源：http://ds.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bo.gzmigu.cn

[U46] PHP：可空类型
来源：http://uc.lnxyls.cn

?string $name = null
来源：http://ye.9csxet.cn

[U47] PHP：联合类型
来源：http://wl.bjjhwx.cn

int|string $id
来源：http://ni.9csxet.cn

[U48] PHP：纯枚举
来源：http://ga.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zp.haigaiapp.cn

[U49] PHP：只读属性
来源：http://bd.hnjuh.cn

public readonly string $name
来源：http://lv.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://mv.asd995.cn

public function __construct(private int $id) {}
来源：http://th.nicolike.cn

[U51] PHP：数组解构
来源：http://rd.huixiangedu.cn

[$a, $b] = $arr;
来源：http://dd.nicolike.cn

[U52] PHP：箭头函数
来源：http://it.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://on.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://wy.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://et.shxzukj.cn

[U54] PHP：空安全调用
来源：http://hj.gzmigu.cn

$obj?->method()
来源：http://rf.gzmigu.cn

[U55] PHP：match 表达式
来源：http://tt.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ar.haigaiapp.cn

[U56] PHP：命名参数
来源：http://gr.wgjwhj.cn

f(a: 1, b: 2)
来源：http://cl.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://db.szxytkj.cn

"值: {$a}"
来源：http://yl.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://ds.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qv.panjiajie.cn

[U59] PHP：自定义排序
来源：http://qf.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ru.asd995.cn

[U60] PHP：JSON 编解码
来源：http://rv.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dq.9csxet.cn

[U61] PHP：正则
来源：http://ue.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tc.nszjky.cn

[U62] PHP：日期对象
来源：http://ta.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mm.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://au.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://un.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://ad.hnjuh.cn

glob("dir/*.php");  scandir("dir");
来源：http://ak.bookmarksfly.cn

[U65] PHP：会话
来源：http://hh.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tp.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://dh.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gj.nicolike.cn

[U67] PHP：处理文件上传
来源：http://wh.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://il.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://ga.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tp.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://iv.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://py.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://vj.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vj.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://ug.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://bx.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://fe.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://nb.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://ap.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://bf.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://cc.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://mp.szsharing.cn

[U75] PHP：依赖注入
来源：http://or.asd995.cn

composer require psr/container
来源：http://zl.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://qb.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ng.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://nk.huanxung.cn

composer require twig/twig
来源：http://ji.huixinmuqiang.cn

[U78] PHP：单元测试
来源：http://jn.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://vo.hnjuh.cn

[U79] PHP：静态分析
来源：http://lo.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://cy.newstarts.cn

[U80] PHP：代码规范修复
来源：http://xd.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zt.panjiajie.cn

[U81] JS：初始化项目
来源：http://am.szsharing.cn

npm init -y;  npm i express
来源：http://cy.szsharing.cn

[U82] JS：package.json 脚本
来源：http://ux.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://di.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://gl.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ib.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://kx.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sj.jianghongdianzi.cn

[U85] JS：可选链
来源：http://wa.huixinmuqiang.cn

a?.b?.c
来源：http://gx.wgjwhj.cn

[U86] JS：空值合并
来源：http://db.hnjuh.cn

a ?? b
来源：http://no.colortex.cn

[U87] JS：解构默认值
来源：http://xb.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://fb.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://dg.panjiajie.cn

{ ...a, ...b }
来源：http://na.colortex.cn

[U89] JS：数组去重
来源：http://xb.haigaiapp.cn

[...new Set(arr)]
来源：http://gl.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://ra.newstarts.cn

[...arr].sort((a, b) => a - b)
来源：http://lo.asd995.cn

[U91] JS：对象键值遍历
来源：http://li.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nj.szsharing.cn

[U92] JS：深拷贝
来源：http://ze.lnxyls.cn

structuredClone(obj)
来源：http://mt.bjjhwx.cn

[U93] JS：模板字符串
来源：http://sd.gzmigu.cn

`共 ${n} 条`
来源：http://gr.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://mu.newstarts.cn

const double = x => x * 2;
来源：http://uv.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://eh.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://lo.hahajie.cn

[U96] JS：async/await 与异常
来源：http://kw.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ap.bookmarksfly.cn

[U97] JS：并发请求
来源：http://qt.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xu.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://an.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://us.newstarts.cn

[U99] JS：事件监听
来源：http://vf.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://hd.panjiajie.cn

[U100] JS：DOM 查询
来源：http://yb.yuntaijiaju.cn

document.querySelector(".item")
来源：http://xc.shtwfgs.cn

[U101] JS：classList 操作
来源：http://tg.bookmarksfly.cn

el.classList.toggle("active")
来源：http://hg.bookmarksfly.cn

[U102] JS：本地存储
来源：http://wa.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jl.huanxung.cn

[U103] JS：定时器
来源：http://lk.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fi.newstarts.cn

[U104] JS：防抖
来源：http://sl.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qo.colortex.cn

[U105] JS：节流
来源：http://fu.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qb.szsharing.cn

[U106] JS：日期格式化
来源：http://me.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://af.jctech888.com.cn

[U107] JS：数字千分位
来源：http://nz.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bl.wgjwhj.cn

[U108] JS：随机整数
来源：http://th.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ua.yuexingan06.cn

[U109] JS：数组分组
来源：http://ra.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://ng.521024.cn

[U110] JS：数组分块
来源：http://cl.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://si.szxytkj.cn

[U111] JS：对象转 Map
来源：http://md.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://ns.bjjhwx.cn

[U112] JS：字符串补位
来源：http://sc.jctech888.com.cn

"7".padStart(3, "0")
来源：http://zo.muxihuayi.cn

[U113] JS：正则替换全部
来源：http://et.nicolike.cn

s.replaceAll("a", "b")
来源：http://xa.nicolike.cn

[U114] JS：JSON 深比较
来源：http://my.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uh.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://ns.huixinmuqiang.cn

crypto.randomUUID()
来源：http://iy.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://oo.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://pd.huanxung.cn

[U117] JS：单元测试
来源：http://ri.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://kg.yuexingan06.cn

[U118] JS：开发服务器
来源：http://bk.colortex.cn

npm i -D vite;  npx vite
来源：http://vt.shxzukj.cn

[U119] JS：生产构建
来源：http://zq.shxzukj.cn

npx vite build
来源：http://ay.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://ge.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://lz.huixinmuqiang.cn

================================================================================
来源：http://vt.nicolike.cn

统计汇总
来源：http://lq.yuexingan06.cn

================================================================================
来源：http://za.shtwfgs.cn

按语言统计（条）：
来源：http://nx.colortex.cn

Python ......... 252
来源：http://dy.szsharing.cn

PHP ............ 252
来源：http://fx.lnxyls.cn

JavaScript ..... 252
来源：http://on.haigaiapp.cn

TypeScript ..... 212
来源：http://tm.szsharing.cn

Java ........... 212
来源：http://om.bjjhwx.cn

Go ............. 212
来源：http://vt.szsharing.cn

Ruby ........... 212
来源：http://kb.huixiangedu.cn

C# ............. 212
来源：http://zj.jianghongdianzi.cn

C .............. 30
来源：http://wp.huanxung.cn

C++ ............ 30
来源：http://rz.muxihuayi.cn

SQL ............ 90
来源：http://nf.huixinmuqiang.cn

Bash ........... 80
来源：http://tx.huixiangedu.cn

Kotlin ......... 15
来源：http://nf.shtwfgs.cn

Swift .......... 15
来源：http://zz.huanxung.cn

Lua ............ 10
来源：http://kw.jctech888.com.cn

Perl ........... 10
来源：http://za.shxzskj.cn

Scala .......... 10
来源：http://ix.shxzskj.cn

------------------------------------
来源：http://vb.panjiajie.cn

合计 ........... 2106 条
来源：http://pe.szsharing.cn

按章节统计：
来源：http://ps.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qr.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jy.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nw.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nw.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://my.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ew.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rn.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zj.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zi.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mm.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jx.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yv.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ji.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sr.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qz.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ht.9csxet.cn

Q SQL 专题                              90
来源：http://lh.muxihuayi.cn

R Bash 专题                             80
来源：http://uh.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://pj.lnxyls.cn

T 其他语言补充                          60
来源：http://qf.yuntaijiaju.cn

U 高频实用片段                         120
来源：http://jr.bjjhwx.cn

------------------------------------
来源：http://jw.asd995.cn

合计                                  2106 条
来源：http://ty.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://op.gzmigu.cn

使用提醒
来源：http://pm.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://zl.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ic.jctech888.com.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tw.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nr.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jm.bookmarksfly.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uu.shxzukj.cn

—— 文件结束 ——
来源：http://wp.yuexingan06.cn

================================================================================
来源：http://or.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://nr.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://wi.haigaiapp.cn

================================================================================
来源：http://kf.lnxyls.cn

【收录内容】
来源：http://yx.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bl.9csxet.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kr.shxzukj.cn

SQL · Bash · C · C++
来源：http://vr.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rh.521024.cn

【使用说明】
来源：http://ec.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sw.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yp.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zc.jianghongdianzi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dc.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://em.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yc.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ux.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ef.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mv.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jl.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qo.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nk.szxytkj.cn

【文件统计】
来源：http://wq.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mr.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://tm.shxzskj.cn

目  录
来源：http://wr.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://rh.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jt.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ny.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ps.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nz.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jt.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fx.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aj.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cm.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wl.jianghongdianzi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jd.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zh.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sz.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ec.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fx.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aw.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kp.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ci.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gi.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lr.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vp.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pt.jianghongdianzi.cn

================================================================================
来源：http://oe.panjiajie.cn

A. 基础语法与类型
来源：http://qt.szsharing.cn

================================================================================
来源：http://sa.shxzukj.cn

[A01] Hello World
来源：http://hc.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://uw.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://vm.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://wm.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gu.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://pc.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://yf.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://ju.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ot.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://uw.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ua.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fm.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ym.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://km.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://lx.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://vy.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://eb.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pn.lnxyls.cn

[A03] 常量定义
来源：http://za.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wj.521024.cn

PHP:  const PI = 3.14159;
来源：http://bo.jctech888.com.cn


<!-- 参考信息 -->