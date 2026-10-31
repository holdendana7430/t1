代发 wailian999

[U35] Py：发送邮件
来源：http://hw.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zs.bookmarksfly.cn

[U36] Py：定时任务
来源：http://zw.521024.cn

schedule.every(10).minutes.do(job)
来源：http://bj.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://jx.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://to.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://qm.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://ju.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://it.nicolike.cn

sys.stdout.isatty()
来源：http://wa.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://jr.gzmigu.cn

print("err", file=sys.stderr)
来源：http://gt.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://ao.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kw.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://gj.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mt.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://mj.521024.cn

namespace App\Http;
来源：http://yu.szxytkj.cn

[U44] PHP：开启严格类型
来源：http://nx.bjjhwx.cn

declare(strict_types=1);
来源：http://lz.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://vi.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jc.huixiangedu.cn

[U46] PHP：可空类型
来源：http://qc.chemitech.net.cn

?string $name = null
来源：http://af.yuexingan06.cn

[U47] PHP：联合类型
来源：http://qk.hahajie.cn

int|string $id
来源：http://ki.nszjky.cn

[U48] PHP：纯枚举
来源：http://nu.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tv.muxihuayi.cn

[U49] PHP：只读属性
来源：http://qr.colortex.cn

public readonly string $name
来源：http://yq.chemitech.net.cn

[U50] PHP：构造器属性提升
来源：http://rj.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://kz.haigaiapp.cn

[U51] PHP：数组解构
来源：http://gy.shtwfgs.cn

[$a, $b] = $arr;
来源：http://ip.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://xd.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://aj.szsharing.cn

[U53] PHP：空合并运算符
来源：http://ax.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://ix.nszjky.cn

[U54] PHP：空安全调用
来源：http://cl.chemitech.net.cn

$obj?->method()
来源：http://lm.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://bq.wgjwhj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vi.colortex.cn

[U56] PHP：命名参数
来源：http://am.shxzukj.cn

f(a: 1, b: 2)
来源：http://ov.shxzskj.cn

[U57] PHP：字符串插值
来源：http://gh.bookmarksfly.cn

"值: {$a}"
来源：http://fu.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://gq.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xf.lnxyls.cn

[U59] PHP：自定义排序
来源：http://iy.nicolike.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ju.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://zb.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kt.shtwfgs.cn

[U61] PHP：正则
来源：http://hy.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bd.colortex.cn

[U62] PHP：日期对象
来源：http://ti.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yh.hahajie.cn

[U63] PHP：文件读写
来源：http://ws.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ld.shxzukj.cn

[U64] PHP：目录遍历
来源：http://tb.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://gg.szsharing.cn

[U65] PHP：会话
来源：http://qi.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lg.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://cz.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://re.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://zx.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jf.nicolike.cn

[U68] PHP：PDO 连接
来源：http://ku.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pm.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://mi.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://st.szsharing.cn

[U70] PHP：PDO 事务
来源：http://an.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pf.gzmigu.cn

[U71] PHP：抛出异常
来源：http://le.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://gq.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://qf.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://gg.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://mg.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://ty.colortex.cn

[U74] PHP：读取环境变量
来源：http://mu.hnjuh.cn

getenv("APP_ENV") ?: "production"
来源：http://uq.shxzukj.cn

[U75] PHP：依赖注入
来源：http://fx.yuntaijiaju.cn

composer require psr/container
来源：http://mo.gzmigu.cn

[U76] PHP：简单路由
来源：http://rk.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://st.panjiajie.cn

[U77] PHP：模板渲染
来源：http://lu.nszjky.cn

composer require twig/twig
来源：http://li.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://ma.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://tr.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://gw.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://uz.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://oq.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zb.shxzukj.cn

[U81] JS：初始化项目
来源：http://cp.colortex.cn

npm init -y;  npm i express
来源：http://cz.newstarts.cn

[U82] JS：package.json 脚本
来源：http://fn.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lh.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://ot.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cw.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://wf.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hy.9csxet.cn

[U85] JS：可选链
来源：http://ye.muxihuayi.cn

a?.b?.c
来源：http://zo.shxzukj.cn

[U86] JS：空值合并
来源：http://yc.shxzukj.cn

a ?? b
来源：http://xz.jctech888.com.cn

[U87] JS：解构默认值
来源：http://gb.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://dm.panjiajie.cn

[U88] JS：对象展开合并
来源：http://wn.jctech888.com.cn

{ ...a, ...b }
来源：http://pe.newstarts.cn

[U89] JS：数组去重
来源：http://rw.szsharing.cn

[...new Set(arr)]
来源：http://ir.nszjky.cn

[U90] JS：数字数组排序
来源：http://wm.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://uc.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://ci.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vt.chemitech.net.cn

[U92] JS：深拷贝
来源：http://tn.jianghongdianzi.cn

structuredClone(obj)
来源：http://qu.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://as.hnjuh.cn

`共 ${n} 条`
来源：http://wk.shtwfgs.cn

[U94] JS：箭头函数
来源：http://gm.nicolike.cn

const double = x => x * 2;
来源：http://tn.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://vm.521024.cn

new Promise((resolve, reject) => {})
来源：http://mu.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://cj.hnjuh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ay.hahajie.cn

[U97] JS：并发请求
来源：http://om.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ic.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://fv.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ih.jctech888.com.cn

[U99] JS：事件监听
来源：http://ji.521024.cn

el.addEventListener("click", e => {})
来源：http://vt.colortex.cn

[U100] JS：DOM 查询
来源：http://fz.haigaiapp.cn

document.querySelector(".item")
来源：http://fy.colortex.cn

[U101] JS：classList 操作
来源：http://pt.szsharing.cn

el.classList.toggle("active")
来源：http://hu.szsharing.cn

[U102] JS：本地存储
来源：http://ou.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rz.gzmigu.cn

[U103] JS：定时器
来源：http://qf.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ma.gzmigu.cn

[U104] JS：防抖
来源：http://ma.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://es.huixinmuqiang.cn

[U105] JS：节流
来源：http://xf.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://it.521024.cn

[U106] JS：日期格式化
来源：http://jz.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://je.chemitech.net.cn

[U107] JS：数字千分位
来源：http://ww.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ic.wgjwhj.cn

[U108] JS：随机整数
来源：http://ur.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qf.szsharing.cn

[U109] JS：数组分组
来源：http://rc.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://fe.shxzukj.cn

[U110] JS：数组分块
来源：http://sw.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xk.szxytkj.cn

[U111] JS：对象转 Map
来源：http://am.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://te.shtwfgs.cn

[U112] JS：字符串补位
来源：http://ts.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://ud.hnjuh.cn

[U113] JS：正则替换全部
来源：http://bm.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://hf.9csxet.cn

[U114] JS：JSON 深比较
来源：http://km.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://li.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://xm.muxihuayi.cn

crypto.randomUUID()
来源：http://jh.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://vo.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://qi.huanxung.cn

[U117] JS：单元测试
来源：http://ms.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://mh.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://lh.chemitech.net.cn

npm i -D vite;  npx vite
来源：http://ak.nszjky.cn

[U119] JS：生产构建
来源：http://qz.asd995.cn

npx vite build
来源：http://qm.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://nm.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://bo.yuntaijiaju.cn

================================================================================
来源：http://bk.nszjky.cn

统计汇总
来源：http://ag.asd995.cn

================================================================================
来源：http://rb.hahajie.cn

按语言统计（条）：
来源：http://mv.9csxet.cn

Python ......... 252
来源：http://tn.shxzukj.cn

PHP ............ 252
来源：http://bp.szxytkj.cn

JavaScript ..... 252
来源：http://qa.hnjuh.cn

TypeScript ..... 212
来源：http://ds.9csxet.cn

Java ........... 212
来源：http://sy.shtwfgs.cn

Go ............. 212
来源：http://kx.9csxet.cn

Ruby ........... 212
来源：http://hk.wgjwhj.cn

C# ............. 212
来源：http://ip.muxihuayi.cn

C .............. 30
来源：http://ms.nicolike.cn

C++ ............ 30
来源：http://qv.muxihuayi.cn

SQL ............ 90
来源：http://he.szxytkj.cn

Bash ........... 80
来源：http://ru.gzmigu.cn

Kotlin ......... 15
来源：http://ai.jianghongdianzi.cn

Swift .......... 15
来源：http://gz.nicolike.cn

Lua ............ 10
来源：http://qt.shtwfgs.cn

Perl ........... 10
来源：http://gp.newstarts.cn

Scala .......... 10
来源：http://he.szsharing.cn

------------------------------------
来源：http://st.hahajie.cn

合计 ........... 2106 条
来源：http://ys.shxzskj.cn

按章节统计：
来源：http://cw.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bx.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tn.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ab.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sn.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sd.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uz.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://od.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qp.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jc.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ow.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://re.jianghongdianzi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jb.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yg.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bh.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tj.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ei.nszjky.cn

Q SQL 专题                              90
来源：http://re.hnjuh.cn

R Bash 专题                             80
来源：http://nm.bjjhwx.cn

S C / C++ 专题                          60
来源：http://bo.bookmarksfly.cn

T 其他语言补充                          60
来源：http://fs.shxzskj.cn

U 高频实用片段                         120
来源：http://pj.shxzukj.cn

------------------------------------
来源：http://do.shxzskj.cn

合计                                  2106 条
来源：http://zq.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ms.huixinmuqiang.cn

使用提醒
来源：http://wu.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ih.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wz.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gy.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://km.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dr.bookmarksfly.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yk.szxytkj.cn

—— 文件结束 ——
来源：http://sy.panjiajie.cn

================================================================================
来源：http://gt.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://jk.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://gv.huixinmuqiang.cn

================================================================================
来源：http://hu.newstarts.cn

【收录内容】
来源：http://ne.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sj.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bi.huixinmuqiang.cn

SQL · Bash · C · C++
来源：http://sg.newstarts.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wl.shxzukj.cn

【使用说明】
来源：http://dm.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fy.panjiajie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dp.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ez.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nj.shxzukj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wt.yuexingan06.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ar.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fu.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qc.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yg.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pu.521024.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ju.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ga.jctech888.com.cn

【文件统计】
来源：http://ri.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sw.szsharing.cn

--------------------------------------------------------------------------------
来源：http://ad.asd995.cn

目  录
来源：http://si.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://uv.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hs.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mn.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mw.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ba.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oo.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gs.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hp.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xf.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qb.panjiajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yi.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tr.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zo.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://js.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fu.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hk.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zn.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nw.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ri.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bl.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ck.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://re.colortex.cn

================================================================================
来源：http://ct.gzmigu.cn

A. 基础语法与类型
来源：http://kx.bookmarksfly.cn

================================================================================
来源：http://nf.shtwfgs.cn

[A01] Hello World
来源：http://rb.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://xm.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://hs.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://ib.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lz.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://se.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://wf.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://hv.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hc.jianghongdianzi.cn

[A02] 变量声明与赋值
来源：http://wb.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vq.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bk.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://eg.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yk.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://ow.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://cr.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://da.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mj.jianghongdianzi.cn

[A03] 常量定义
来源：http://vk.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lg.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://go.jianghongdianzi.cn


<!-- 参考信息 -->