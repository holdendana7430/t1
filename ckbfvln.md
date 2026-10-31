代发 wailian999

[U35] Py：发送邮件
来源：http://ba.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lm.jctech888.com.cn

[U36] Py：定时任务
来源：http://mv.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://qd.jianghongdianzi.cn

[U37] Py：读写 Excel
来源：http://sy.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://if.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://zi.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://yz.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://fd.szxytkj.cn

sys.stdout.isatty()
来源：http://pm.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://js.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://la.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://tc.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hx.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://we.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ib.hahajie.cn

[U43] PHP：声明命名空间
来源：http://kd.shtwfgs.cn

namespace App\Http;
来源：http://ha.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://za.huixinmuqiang.cn

declare(strict_types=1);
来源：http://pn.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://bl.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lj.nszjky.cn

[U46] PHP：可空类型
来源：http://rt.chemitech.net.cn

?string $name = null
来源：http://lf.panjiajie.cn

[U47] PHP：联合类型
来源：http://ve.asd995.cn

int|string $id
来源：http://yj.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://oh.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://he.szsharing.cn

[U49] PHP：只读属性
来源：http://so.jctech888.com.cn

public readonly string $name
来源：http://uu.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://wy.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://yl.shtwfgs.cn

[U51] PHP：数组解构
来源：http://di.yuexingan06.cn

[$a, $b] = $arr;
来源：http://ch.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://ef.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://ec.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://rz.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://jm.huixiangedu.cn

[U54] PHP：空安全调用
来源：http://mg.haigaiapp.cn

$obj?->method()
来源：http://sw.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://rx.haigaiapp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xy.asd995.cn

[U56] PHP：命名参数
来源：http://ix.huixiangedu.cn

f(a: 1, b: 2)
来源：http://be.nszjky.cn

[U57] PHP：字符串插值
来源：http://ks.nszjky.cn

"值: {$a}"
来源：http://pw.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://xe.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jj.colortex.cn

[U59] PHP：自定义排序
来源：http://ho.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vo.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://om.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iw.szsharing.cn

[U61] PHP：正则
来源：http://vh.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zc.colortex.cn

[U62] PHP：日期对象
来源：http://cp.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ro.lnxyls.cn

[U63] PHP：文件读写
来源：http://cf.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lm.hnjuh.cn

[U64] PHP：目录遍历
来源：http://ia.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://dr.bookmarksfly.cn

[U65] PHP：会话
来源：http://lj.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nc.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://tf.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://in.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://jb.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sk.nszjky.cn

[U68] PHP：PDO 连接
来源：http://nf.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ng.9csxet.cn

[U69] PHP：PDO 预处理
来源：http://uu.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sf.shtwfgs.cn

[U70] PHP：PDO 事务
来源：http://vn.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pt.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://ay.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://dp.gzmigu.cn

[U72] PHP：写错误日志
来源：http://ku.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://lf.shxzskj.cn

[U73] PHP：读取 ini 配置
来源：http://wg.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://ke.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://cq.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://is.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://oz.yuntaijiaju.cn

composer require psr/container
来源：http://ug.szsharing.cn

[U76] PHP：简单路由
来源：http://wb.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xh.szxytkj.cn

[U77] PHP：模板渲染
来源：http://ee.szsharing.cn

composer require twig/twig
来源：http://rt.huanxung.cn

[U78] PHP：单元测试
来源：http://es.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://ql.shtwfgs.cn

[U79] PHP：静态分析
来源：http://oq.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://wv.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://kq.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vs.9csxet.cn

[U81] JS：初始化项目
来源：http://nb.asd995.cn

npm init -y;  npm i express
来源：http://dh.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://ve.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sz.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://ox.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hc.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://qm.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uy.muxihuayi.cn

[U85] JS：可选链
来源：http://rh.lnxyls.cn

a?.b?.c
来源：http://nm.panjiajie.cn

[U86] JS：空值合并
来源：http://ik.bjjhwx.cn

a ?? b
来源：http://tn.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://mm.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://xc.szxytkj.cn

[U88] JS：对象展开合并
来源：http://fq.nicolike.cn

{ ...a, ...b }
来源：http://oa.wgjwhj.cn

[U89] JS：数组去重
来源：http://pq.bookmarksfly.cn

[...new Set(arr)]
来源：http://zr.szsharing.cn

[U90] JS：数字数组排序
来源：http://zl.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://op.hahajie.cn

[U91] JS：对象键值遍历
来源：http://oq.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uc.hnjuh.cn

[U92] JS：深拷贝
来源：http://df.gzmigu.cn

structuredClone(obj)
来源：http://ds.asd995.cn

[U93] JS：模板字符串
来源：http://md.newstarts.cn

`共 ${n} 条`
来源：http://pi.nicolike.cn

[U94] JS：箭头函数
来源：http://uc.panjiajie.cn

const double = x => x * 2;
来源：http://sy.gzmigu.cn

[U95] JS：Promise 包装
来源：http://lk.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://dd.szsharing.cn

[U96] JS：async/await 与异常
来源：http://dh.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nz.nicolike.cn

[U97] JS：并发请求
来源：http://bd.muxihuayi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hj.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://bh.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oa.yuexingan06.cn

[U99] JS：事件监听
来源：http://oi.521024.cn

el.addEventListener("click", e => {})
来源：http://ha.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://uh.wgjwhj.cn

document.querySelector(".item")
来源：http://ij.colortex.cn

[U101] JS：classList 操作
来源：http://wx.yuexingan06.cn

el.classList.toggle("active")
来源：http://yc.panjiajie.cn

[U102] JS：本地存储
来源：http://bx.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lx.panjiajie.cn

[U103] JS：定时器
来源：http://ne.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jz.shtwfgs.cn

[U104] JS：防抖
来源：http://qi.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yl.huanxung.cn

[U105] JS：节流
来源：http://sy.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://co.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://le.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yr.wgjwhj.cn

[U107] JS：数字千分位
来源：http://sw.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qd.bjjhwx.cn

[U108] JS：随机整数
来源：http://ay.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ik.yuexingan06.cn

[U109] JS：数组分组
来源：http://zp.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://ug.jctech888.com.cn

[U110] JS：数组分块
来源：http://te.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iu.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://yp.huanxung.cn

new Map(Object.entries(obj))
来源：http://nk.lnxyls.cn

[U112] JS：字符串补位
来源：http://et.nicolike.cn

"7".padStart(3, "0")
来源：http://iu.lnxyls.cn

[U113] JS：正则替换全部
来源：http://tc.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://bx.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://el.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://go.hahajie.cn

[U115] JS：生成 UUID
来源：http://th.yuntaijiaju.cn

crypto.randomUUID()
来源：http://aq.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ld.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://qw.521024.cn

[U117] JS：单元测试
来源：http://sn.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://bc.szsharing.cn

[U118] JS：开发服务器
来源：http://ws.huanxung.cn

npm i -D vite;  npx vite
来源：http://to.521024.cn

[U119] JS：生产构建
来源：http://ye.bookmarksfly.cn

npx vite build
来源：http://la.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://tx.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://sm.huixinmuqiang.cn

================================================================================
来源：http://lk.lnxyls.cn

统计汇总
来源：http://sk.shxzskj.cn

================================================================================
来源：http://nc.shxzskj.cn

按语言统计（条）：
来源：http://en.jianghongdianzi.cn

Python ......... 252
来源：http://bz.shxzukj.cn

PHP ............ 252
来源：http://dh.hnjuh.cn

JavaScript ..... 252
来源：http://ns.bookmarksfly.cn

TypeScript ..... 212
来源：http://ui.9csxet.cn

Java ........... 212
来源：http://we.lnxyls.cn

Go ............. 212
来源：http://nz.jianghongdianzi.cn

Ruby ........... 212
来源：http://eo.hnjuh.cn

C# ............. 212
来源：http://ov.haigaiapp.cn

C .............. 30
来源：http://yc.shxzskj.cn

C++ ............ 30
来源：http://ro.521024.cn

SQL ............ 90
来源：http://sb.yuntaijiaju.cn

Bash ........... 80
来源：http://wq.huanxung.cn

Kotlin ......... 15
来源：http://hm.gzmigu.cn

Swift .......... 15
来源：http://lg.521024.cn

Lua ............ 10
来源：http://uy.newstarts.cn

Perl ........... 10
来源：http://qz.nszjky.cn

Scala .......... 10
来源：http://qp.asd995.cn

------------------------------------
来源：http://zh.jctech888.com.cn

合计 ........... 2106 条
来源：http://wj.lnxyls.cn

按章节统计：
来源：http://ez.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bm.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nu.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wn.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jz.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pl.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pm.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bq.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ib.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bc.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ki.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xl.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uo.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://op.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sm.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ae.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tn.muxihuayi.cn

Q SQL 专题                              90
来源：http://fr.shtwfgs.cn

R Bash 专题                             80
来源：http://kt.shxzukj.cn

S C / C++ 专题                          60
来源：http://uh.haigaiapp.cn

T 其他语言补充                          60
来源：http://jc.colortex.cn

U 高频实用片段                         120
来源：http://ob.jctech888.com.cn

------------------------------------
来源：http://rs.huixiangedu.cn

合计                                  2106 条
来源：http://lp.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://vd.chemitech.net.cn

使用提醒
来源：http://ba.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://zt.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pe.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ri.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vu.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://au.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mx.panjiajie.cn

—— 文件结束 ——
来源：http://ty.bjjhwx.cn

================================================================================
来源：http://yz.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://iz.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://md.asd995.cn

================================================================================
来源：http://vp.huixinmuqiang.cn

【收录内容】
来源：http://es.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cl.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yz.hnjuh.cn

SQL · Bash · C · C++
来源：http://nb.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xl.bookmarksfly.cn

【使用说明】
来源：http://zm.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hn.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cd.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xk.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sz.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://me.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ct.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ox.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://or.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hq.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hf.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kx.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rs.hnjuh.cn

【文件统计】
来源：http://vo.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hc.9csxet.cn

--------------------------------------------------------------------------------
来源：http://cr.lnxyls.cn

目  录
来源：http://qu.521024.cn

--------------------------------------------------------------------------------
来源：http://jv.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uu.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qi.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://eb.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zl.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tj.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qh.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://er.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xy.wgjwhj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pc.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ou.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mu.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sc.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mn.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qi.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fw.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qg.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zr.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cg.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ou.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uq.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jy.haigaiapp.cn

================================================================================
来源：http://hm.nicolike.cn

A. 基础语法与类型
来源：http://kj.huixinmuqiang.cn

================================================================================
来源：http://dc.nicolike.cn

[A01] Hello World
来源：http://ry.shxzukj.cn

Py:   print("Hello, World!")
来源：http://ua.colortex.cn

PHP:  echo "Hello, World!";
来源：http://yk.colortex.cn

JS:   console.log("Hello, World!");
来源：http://uw.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iu.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://ge.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://gj.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://bm.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vi.huanxung.cn

[A02] 变量声明与赋值
来源：http://gd.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rm.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ee.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mw.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rz.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://la.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://al.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://nf.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sr.huixinmuqiang.cn

[A03] 常量定义
来源：http://qm.haigaiapp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qq.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://zj.nicolike.cn


<!-- 参考信息 -->