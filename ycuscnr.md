代发 wailian999

[U35] Py：发送邮件
来源：http://dj.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rg.bjjhwx.cn

[U36] Py：定时任务
来源：http://oe.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://sq.haigaiapp.cn

[U37] Py：读写 Excel
来源：http://zx.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ry.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://cc.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://gt.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://wa.521024.cn

sys.stdout.isatty()
来源：http://ho.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://yz.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://yq.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://bl.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hp.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://ss.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ba.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://bg.521024.cn

namespace App\Http;
来源：http://tr.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://vl.huixinmuqiang.cn

declare(strict_types=1);
来源：http://zd.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://ce.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yt.bjjhwx.cn

[U46] PHP：可空类型
来源：http://oy.bookmarksfly.cn

?string $name = null
来源：http://vw.lnxyls.cn

[U47] PHP：联合类型
来源：http://ov.yuntaijiaju.cn

int|string $id
来源：http://ly.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://lb.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qk.nicolike.cn

[U49] PHP：只读属性
来源：http://ih.newstarts.cn

public readonly string $name
来源：http://dx.szsharing.cn

[U50] PHP：构造器属性提升
来源：http://pk.lnxyls.cn

public function __construct(private int $id) {}
来源：http://bp.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://oi.szxytkj.cn

[$a, $b] = $arr;
来源：http://th.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://az.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://ar.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://qz.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://ip.huanxung.cn

[U54] PHP：空安全调用
来源：http://cu.hnjuh.cn

$obj?->method()
来源：http://ch.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://ch.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hx.chemitech.net.cn

[U56] PHP：命名参数
来源：http://te.panjiajie.cn

f(a: 1, b: 2)
来源：http://gx.szsharing.cn

[U57] PHP：字符串插值
来源：http://kq.nicolike.cn

"值: {$a}"
来源：http://be.colortex.cn

[U58] PHP：数组三件套
来源：http://ki.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nn.szsharing.cn

[U59] PHP：自定义排序
来源：http://is.hahajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fh.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://on.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hl.huanxung.cn

[U61] PHP：正则
来源：http://wa.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gz.szsharing.cn

[U62] PHP：日期对象
来源：http://pu.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sh.yuexingan06.cn

[U63] PHP：文件读写
来源：http://mj.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ta.shxzukj.cn

[U64] PHP：目录遍历
来源：http://lu.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://bv.hnjuh.cn

[U65] PHP：会话
来源：http://mt.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ih.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://jn.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kj.9csxet.cn

[U67] PHP：处理文件上传
来源：http://jr.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yx.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://np.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mr.colortex.cn

[U69] PHP：PDO 预处理
来源：http://mm.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rl.hahajie.cn

[U70] PHP：PDO 事务
来源：http://fh.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://be.szsharing.cn

[U71] PHP：抛出异常
来源：http://aw.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://jy.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://fs.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://by.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://eb.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://tb.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://rt.huixiangedu.cn

getenv("APP_ENV") ?: "production"
来源：http://eq.gzmigu.cn

[U75] PHP：依赖注入
来源：http://je.huixinmuqiang.cn

composer require psr/container
来源：http://qs.newstarts.cn

[U76] PHP：简单路由
来源：http://xf.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ut.huanxung.cn

[U77] PHP：模板渲染
来源：http://oc.nszjky.cn

composer require twig/twig
来源：http://fx.szsharing.cn

[U78] PHP：单元测试
来源：http://mo.huixiangedu.cn

composer require --dev phpunit/phpunit
来源：http://xv.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://zu.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://fp.yuexingan06.cn

[U80] PHP：代码规范修复
来源：http://xr.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jr.colortex.cn

[U81] JS：初始化项目
来源：http://hy.lnxyls.cn

npm init -y;  npm i express
来源：http://jf.9csxet.cn

[U82] JS：package.json 脚本
来源：http://gd.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ah.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://kc.shtwfgs.cn

export const a = 1;  import { a } from "./m.js";
来源：http://re.colortex.cn

[U84] JS：CommonJS 写法
来源：http://sh.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ba.colortex.cn

[U85] JS：可选链
来源：http://nj.szxytkj.cn

a?.b?.c
来源：http://gu.huixinmuqiang.cn

[U86] JS：空值合并
来源：http://nk.shxzskj.cn

a ?? b
来源：http://qp.panjiajie.cn

[U87] JS：解构默认值
来源：http://gt.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://uk.hahajie.cn

[U88] JS：对象展开合并
来源：http://ud.chemitech.net.cn

{ ...a, ...b }
来源：http://be.chemitech.net.cn

[U89] JS：数组去重
来源：http://mb.yuexingan06.cn

[...new Set(arr)]
来源：http://vt.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://bu.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://qw.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://ud.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bz.9csxet.cn

[U92] JS：深拷贝
来源：http://ly.shxzskj.cn

structuredClone(obj)
来源：http://ph.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://bz.bookmarksfly.cn

`共 ${n} 条`
来源：http://sg.shtwfgs.cn

[U94] JS：箭头函数
来源：http://bx.huixiangedu.cn

const double = x => x * 2;
来源：http://nq.huanxung.cn

[U95] JS：Promise 包装
来源：http://af.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://rc.nicolike.cn

[U96] JS：async/await 与异常
来源：http://io.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://om.gzmigu.cn

[U97] JS：并发请求
来源：http://aw.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ew.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://ng.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ql.panjiajie.cn

[U99] JS：事件监听
来源：http://lp.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://cp.nszjky.cn

[U100] JS：DOM 查询
来源：http://of.jianghongdianzi.cn

document.querySelector(".item")
来源：http://kd.hnjuh.cn

[U101] JS：classList 操作
来源：http://wm.huixiangedu.cn

el.classList.toggle("active")
来源：http://fd.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://qn.shxzskj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zt.asd995.cn

[U103] JS：定时器
来源：http://fz.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vk.hnjuh.cn

[U104] JS：防抖
来源：http://cd.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mm.chemitech.net.cn

[U105] JS：节流
来源：http://jk.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ti.lnxyls.cn

[U106] JS：日期格式化
来源：http://gw.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nc.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://qf.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://we.yuexingan06.cn

[U108] JS：随机整数
来源：http://ye.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ev.newstarts.cn

[U109] JS：数组分组
来源：http://gs.szxytkj.cn

Object.groupBy(arr, x => x.type)
来源：http://wu.shxzskj.cn

[U110] JS：数组分块
来源：http://hv.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dk.shxzskj.cn

[U111] JS：对象转 Map
来源：http://dv.szxytkj.cn

new Map(Object.entries(obj))
来源：http://vv.hahajie.cn

[U112] JS：字符串补位
来源：http://pt.shxzskj.cn

"7".padStart(3, "0")
来源：http://il.szsharing.cn

[U113] JS：正则替换全部
来源：http://vx.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://go.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://au.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bf.panjiajie.cn

[U115] JS：生成 UUID
来源：http://fu.9csxet.cn

crypto.randomUUID()
来源：http://uz.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://mj.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://ke.szsharing.cn

[U117] JS：单元测试
来源：http://sg.asd995.cn

npm i -D vitest;  npx vitest
来源：http://pr.huanxung.cn

[U118] JS：开发服务器
来源：http://kl.lnxyls.cn

npm i -D vite;  npx vite
来源：http://kt.szxytkj.cn

[U119] JS：生产构建
来源：http://nz.521024.cn

npx vite build
来源：http://cm.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ox.jctech888.com.cn

import.meta.env.VITE_API_URL
来源：http://xj.jianghongdianzi.cn

================================================================================
来源：http://us.bookmarksfly.cn

统计汇总
来源：http://al.nszjky.cn

================================================================================
来源：http://py.hahajie.cn

按语言统计（条）：
来源：http://cl.shxzskj.cn

Python ......... 252
来源：http://fd.shtwfgs.cn

PHP ............ 252
来源：http://tw.nszjky.cn

JavaScript ..... 252
来源：http://ie.nicolike.cn

TypeScript ..... 212
来源：http://vt.hahajie.cn

Java ........... 212
来源：http://ta.hahajie.cn

Go ............. 212
来源：http://dj.colortex.cn

Ruby ........... 212
来源：http://mz.shtwfgs.cn

C# ............. 212
来源：http://ob.521024.cn

C .............. 30
来源：http://fp.yuexingan06.cn

C++ ............ 30
来源：http://yg.yuntaijiaju.cn

SQL ............ 90
来源：http://eh.yuexingan06.cn

Bash ........... 80
来源：http://vz.nicolike.cn

Kotlin ......... 15
来源：http://cr.muxihuayi.cn

Swift .......... 15
来源：http://el.asd995.cn

Lua ............ 10
来源：http://ii.colortex.cn

Perl ........... 10
来源：http://jn.shxzukj.cn

Scala .......... 10
来源：http://qr.szxytkj.cn

------------------------------------
来源：http://bd.huanxung.cn

合计 ........... 2106 条
来源：http://ew.colortex.cn

按章节统计：
来源：http://im.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bi.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dc.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qd.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nc.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ze.newstarts.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ao.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oc.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tp.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wa.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tx.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mj.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ap.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ry.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vo.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zn.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xf.hnjuh.cn

Q SQL 专题                              90
来源：http://eo.hahajie.cn

R Bash 专题                             80
来源：http://zh.nszjky.cn

S C / C++ 专题                          60
来源：http://cn.gzmigu.cn

T 其他语言补充                          60
来源：http://kx.nicolike.cn

U 高频实用片段                         120
来源：http://hx.huanxung.cn

------------------------------------
来源：http://ay.haigaiapp.cn

合计                                  2106 条
来源：http://gj.colortex.cn

--------------------------------------------------------------------------------
来源：http://gr.gzmigu.cn

使用提醒
来源：http://ud.521024.cn

--------------------------------------------------------------------------------
来源：http://fs.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bm.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zl.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://th.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ev.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nt.nicolike.cn

—— 文件结束 ——
来源：http://bf.9csxet.cn

================================================================================
来源：http://zv.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://cg.hahajie.cn

Common Programming Examples Cheat Book
来源：http://vi.szxytkj.cn

================================================================================
来源：http://sy.asd995.cn

【收录内容】
来源：http://so.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gc.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yg.newstarts.cn

SQL · Bash · C · C++
来源：http://mk.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dg.chemitech.net.cn

【使用说明】
来源：http://ie.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jt.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eo.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ow.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cr.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rz.yuexingan06.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ib.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qs.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://de.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ml.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yj.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kz.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qd.newstarts.cn

【文件统计】
来源：http://pu.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jv.nszjky.cn

--------------------------------------------------------------------------------
来源：http://je.nicolike.cn

目  录
来源：http://zl.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://yv.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vv.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://li.panjiajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nf.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://al.szxytkj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wx.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hu.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ih.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hl.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://om.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bl.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sb.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bv.szsharing.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vm.szxytkj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hy.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iu.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tm.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ka.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://me.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ew.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xz.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hj.colortex.cn

================================================================================
来源：http://eh.huixinmuqiang.cn

A. 基础语法与类型
来源：http://vz.gzmigu.cn

================================================================================
来源：http://qd.huanxung.cn

[A01] Hello World
来源：http://vs.9csxet.cn

Py:   print("Hello, World!")
来源：http://ia.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://qr.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://nw.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pi.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://wk.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://bh.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://ao.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kt.hnjuh.cn

[A02] 变量声明与赋值
来源：http://tw.nszjky.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qh.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ye.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hx.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://my.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://fp.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://mz.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://ua.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oq.szxytkj.cn

[A03] 常量定义
来源：http://ci.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fi.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://tv.521024.cn


<!-- 参考信息 -->