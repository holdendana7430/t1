代发 wailian999

[U31] Py：单测
来源：http://xe.yuntaijiaju.cn

python -m pytest -q
来源：http://gy.haigaiapp.cn

[U32] Py：代码格式化
来源：http://jo.huixinmuqiang.cn

ruff format . && ruff check --fix .
来源：http://em.panjiajie.cn

[U33] Py：打包发布
来源：http://by.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://bt.lnxyls.cn

[U34] Py：判断编码
来源：http://hp.haigaiapp.cn

chardet.detect(raw)
来源：http://az.hahajie.cn

[U35] Py：发送邮件
来源：http://cj.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lx.huanxung.cn

[U36] Py：定时任务
来源：http://xz.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://qh.szxytkj.cn

[U37] Py：读写 Excel
来源：http://qu.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gp.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://vg.colortex.cn

Path(__file__).resolve().parent
来源：http://rt.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://oz.nszjky.cn

sys.stdout.isatty()
来源：http://cu.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://mf.panjiajie.cn

print("err", file=sys.stderr)
来源：http://ew.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://va.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ju.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://cj.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ee.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://wc.lnxyls.cn

namespace App\Http;
来源：http://nc.newstarts.cn

[U44] PHP：开启严格类型
来源：http://cx.wgjwhj.cn

declare(strict_types=1);
来源：http://pe.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://ce.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ju.szxytkj.cn

[U46] PHP：可空类型
来源：http://md.haigaiapp.cn

?string $name = null
来源：http://yw.chemitech.net.cn

[U47] PHP：联合类型
来源：http://ai.jctech888.com.cn

int|string $id
来源：http://bx.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://ds.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://io.lnxyls.cn

[U49] PHP：只读属性
来源：http://pw.yuntaijiaju.cn

public readonly string $name
来源：http://wf.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://kb.521024.cn

public function __construct(private int $id) {}
来源：http://ms.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://oc.nszjky.cn

[$a, $b] = $arr;
来源：http://np.szsharing.cn

[U52] PHP：箭头函数
来源：http://dz.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://sk.hahajie.cn

[U53] PHP：空合并运算符
来源：http://wm.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://fa.panjiajie.cn

[U54] PHP：空安全调用
来源：http://lz.haigaiapp.cn

$obj?->method()
来源：http://ho.panjiajie.cn

[U55] PHP：match 表达式
来源：http://nc.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://al.wgjwhj.cn

[U56] PHP：命名参数
来源：http://sq.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://nc.szsharing.cn

[U57] PHP：字符串插值
来源：http://mm.shxzskj.cn

"值: {$a}"
来源：http://ta.nicolike.cn

[U58] PHP：数组三件套
来源：http://un.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mv.9csxet.cn

[U59] PHP：自定义排序
来源：http://nf.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rs.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://zo.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pl.nszjky.cn

[U61] PHP：正则
来源：http://hu.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fo.newstarts.cn

[U62] PHP：日期对象
来源：http://uz.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rf.bjjhwx.cn

[U63] PHP：文件读写
来源：http://ov.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iy.9csxet.cn

[U64] PHP：目录遍历
来源：http://uj.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://bv.jianghongdianzi.cn

[U65] PHP：会话
来源：http://xy.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://av.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://fj.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ii.szsharing.cn

[U67] PHP：处理文件上传
来源：http://zn.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wo.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://ou.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://na.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://fg.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xj.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://db.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ps.szxytkj.cn

[U71] PHP：抛出异常
来源：http://td.gzmigu.cn

throw new RuntimeException("失败", 500);
来源：http://dn.huixinmuqiang.cn

[U72] PHP：写错误日志
来源：http://eo.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://lc.521024.cn

[U73] PHP：读取 ini 配置
来源：http://vl.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://jm.szsharing.cn

[U74] PHP：读取环境变量
来源：http://tf.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://jc.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://lv.9csxet.cn

composer require psr/container
来源：http://gg.bjjhwx.cn

[U76] PHP：简单路由
来源：http://af.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ts.huanxung.cn

[U77] PHP：模板渲染
来源：http://eb.jctech888.com.cn

composer require twig/twig
来源：http://sy.shtwfgs.cn

[U78] PHP：单元测试
来源：http://mf.chemitech.net.cn

composer require --dev phpunit/phpunit
来源：http://iv.wgjwhj.cn

[U79] PHP：静态分析
来源：http://ey.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://bt.huanxung.cn

[U80] PHP：代码规范修复
来源：http://cr.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ze.colortex.cn

[U81] JS：初始化项目
来源：http://ni.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://yr.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://sg.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bs.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://zx.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ac.521024.cn

[U84] JS：CommonJS 写法
来源：http://hy.colortex.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rv.nicolike.cn

[U85] JS：可选链
来源：http://vg.colortex.cn

a?.b?.c
来源：http://kr.szxytkj.cn

[U86] JS：空值合并
来源：http://ld.huixiangedu.cn

a ?? b
来源：http://sv.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://so.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://kh.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://vw.shxzskj.cn

{ ...a, ...b }
来源：http://sz.lnxyls.cn

[U89] JS：数组去重
来源：http://up.panjiajie.cn

[...new Set(arr)]
来源：http://nc.lnxyls.cn

[U90] JS：数字数组排序
来源：http://se.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://tq.nszjky.cn

[U91] JS：对象键值遍历
来源：http://pc.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nt.yuntaijiaju.cn

[U92] JS：深拷贝
来源：http://di.shxzskj.cn

structuredClone(obj)
来源：http://lk.asd995.cn

[U93] JS：模板字符串
来源：http://ma.9csxet.cn

`共 ${n} 条`
来源：http://ei.gzmigu.cn

[U94] JS：箭头函数
来源：http://ot.lnxyls.cn

const double = x => x * 2;
来源：http://fw.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://iz.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://lf.szsharing.cn

[U96] JS：async/await 与异常
来源：http://kx.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mi.shxzukj.cn

[U97] JS：并发请求
来源：http://ah.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zj.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://ea.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tb.9csxet.cn

[U99] JS：事件监听
来源：http://qv.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://mk.hnjuh.cn

[U100] JS：DOM 查询
来源：http://az.chemitech.net.cn

document.querySelector(".item")
来源：http://bb.huixinmuqiang.cn

[U101] JS：classList 操作
来源：http://fi.521024.cn

el.classList.toggle("active")
来源：http://ac.asd995.cn

[U102] JS：本地存储
来源：http://bw.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sq.9csxet.cn

[U103] JS：定时器
来源：http://km.gzmigu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cp.jctech888.com.cn

[U104] JS：防抖
来源：http://vc.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nb.chemitech.net.cn

[U105] JS：节流
来源：http://xa.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fy.nicolike.cn

[U106] JS：日期格式化
来源：http://gi.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ry.shtwfgs.cn

[U107] JS：数字千分位
来源：http://ry.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kg.shtwfgs.cn

[U108] JS：随机整数
来源：http://zz.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yl.521024.cn

[U109] JS：数组分组
来源：http://ht.bjjhwx.cn

Object.groupBy(arr, x => x.type)
来源：http://bs.lnxyls.cn

[U110] JS：数组分块
来源：http://wg.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ii.hahajie.cn

[U111] JS：对象转 Map
来源：http://dl.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://hr.shxzukj.cn

[U112] JS：字符串补位
来源：http://zn.nicolike.cn

"7".padStart(3, "0")
来源：http://fn.shxzukj.cn

[U113] JS：正则替换全部
来源：http://fx.521024.cn

s.replaceAll("a", "b")
来源：http://nc.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://mj.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xo.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://jp.yuntaijiaju.cn

crypto.randomUUID()
来源：http://fk.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://dr.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://aa.szsharing.cn

[U117] JS：单元测试
来源：http://vt.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://nj.colortex.cn

[U118] JS：开发服务器
来源：http://of.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://mt.panjiajie.cn

[U119] JS：生产构建
来源：http://ch.huixinmuqiang.cn

npx vite build
来源：http://zj.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://xe.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://ju.gzmigu.cn

================================================================================
来源：http://rh.huanxung.cn

统计汇总
来源：http://ej.huixinmuqiang.cn

================================================================================
来源：http://hz.asd995.cn

按语言统计（条）：
来源：http://li.huixinmuqiang.cn

Python ......... 252
来源：http://sq.szsharing.cn

PHP ............ 252
来源：http://zh.shxzukj.cn

JavaScript ..... 252
来源：http://io.jianghongdianzi.cn

TypeScript ..... 212
来源：http://jb.bookmarksfly.cn

Java ........... 212
来源：http://qz.muxihuayi.cn

Go ............. 212
来源：http://oh.huixinmuqiang.cn

Ruby ........... 212
来源：http://xl.haigaiapp.cn

C# ............. 212
来源：http://hf.szsharing.cn

C .............. 30
来源：http://bk.bookmarksfly.cn

C++ ............ 30
来源：http://jm.bjjhwx.cn

SQL ............ 90
来源：http://he.asd995.cn

Bash ........... 80
来源：http://cu.521024.cn

Kotlin ......... 15
来源：http://mx.szsharing.cn

Swift .......... 15
来源：http://yb.9csxet.cn

Lua ............ 10
来源：http://lp.shxzukj.cn

Perl ........... 10
来源：http://wi.huixiangedu.cn

Scala .......... 10
来源：http://so.hahajie.cn

------------------------------------
来源：http://mm.bjjhwx.cn

合计 ........... 2106 条
来源：http://bc.huixinmuqiang.cn

按章节统计：
来源：http://sy.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kd.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ke.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ov.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fg.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rm.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://af.haigaiapp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iv.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bw.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://co.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rw.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bk.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jm.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wl.yuexingan06.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hn.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ua.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qj.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://cv.bjjhwx.cn

R Bash 专题                             80
来源：http://ti.lnxyls.cn

S C / C++ 专题                          60
来源：http://il.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://cx.haigaiapp.cn

U 高频实用片段                         120
来源：http://dh.gzmigu.cn

------------------------------------
来源：http://oo.szxytkj.cn

合计                                  2106 条
来源：http://zm.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://as.huixiangedu.cn

使用提醒
来源：http://uz.nszjky.cn

--------------------------------------------------------------------------------
来源：http://fk.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pb.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jn.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ad.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wv.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://es.nszjky.cn

—— 文件结束 ——
来源：http://sh.nszjky.cn

================================================================================
来源：http://cq.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://de.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://lh.wgjwhj.cn

================================================================================
来源：http://pi.panjiajie.cn

【收录内容】
来源：http://wh.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ew.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eq.szxytkj.cn

SQL · Bash · C · C++
来源：http://ux.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xw.huixinmuqiang.cn

【使用说明】
来源：http://er.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://li.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ny.panjiajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cz.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qf.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mk.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pt.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://co.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wo.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zx.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kk.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xp.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mz.huixinmuqiang.cn

【文件统计】
来源：http://ry.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cu.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://xa.jianghongdianzi.cn

目  录
来源：http://pc.hahajie.cn

--------------------------------------------------------------------------------
来源：http://xt.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pt.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ef.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wn.huixiangedu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dw.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dk.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ef.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gh.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nc.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zk.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qa.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hy.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lk.huixinmuqiang.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fh.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xs.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://en.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lj.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yr.huixiangedu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sa.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qp.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wx.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cy.shtwfgs.cn

================================================================================
来源：http://ry.yuntaijiaju.cn

A. 基础语法与类型
来源：http://hy.panjiajie.cn

================================================================================
来源：http://hb.gzmigu.cn

[A01] Hello World
来源：http://yg.hnjuh.cn

Py:   print("Hello, World!")
来源：http://hy.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://go.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://qp.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zu.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://lv.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://ut.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://iv.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bn.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://vv.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hn.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qc.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://eg.hahajie.cn


<!-- 参考信息 -->