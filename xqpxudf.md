代发 wailian999

[U37] Py：读写 Excel
来源：http://su.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ej.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://sx.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://lg.521024.cn

[U39] Py：判断是否在交互环境
来源：http://gv.szxytkj.cn

sys.stdout.isatty()
来源：http://ya.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://ka.shxzukj.cn

print("err", file=sys.stderr)
来源：http://ha.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://vr.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uj.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://db.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tf.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://eo.huixiangedu.cn

namespace App\Http;
来源：http://uo.szsharing.cn

[U44] PHP：开启严格类型
来源：http://cs.shxzskj.cn

declare(strict_types=1);
来源：http://dt.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://vz.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kp.521024.cn

[U46] PHP：可空类型
来源：http://zj.shtwfgs.cn

?string $name = null
来源：http://cx.panjiajie.cn

[U47] PHP：联合类型
来源：http://rm.shxzskj.cn

int|string $id
来源：http://al.shxzukj.cn

[U48] PHP：纯枚举
来源：http://cz.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jv.panjiajie.cn

[U49] PHP：只读属性
来源：http://np.hnjuh.cn

public readonly string $name
来源：http://pn.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://zj.hahajie.cn

public function __construct(private int $id) {}
来源：http://rj.nicolike.cn

[U51] PHP：数组解构
来源：http://fn.nszjky.cn

[$a, $b] = $arr;
来源：http://qw.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://xm.muxihuayi.cn

$double = fn($x) => $x * 2;
来源：http://io.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://en.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://bk.newstarts.cn

[U54] PHP：空安全调用
来源：http://sx.hahajie.cn

$obj?->method()
来源：http://bx.hahajie.cn

[U55] PHP：match 表达式
来源：http://xu.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tc.hahajie.cn

[U56] PHP：命名参数
来源：http://gn.shxzskj.cn

f(a: 1, b: 2)
来源：http://mi.shxzukj.cn

[U57] PHP：字符串插值
来源：http://my.haigaiapp.cn

"值: {$a}"
来源：http://dx.hahajie.cn

[U58] PHP：数组三件套
来源：http://dq.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nj.nszjky.cn

[U59] PHP：自定义排序
来源：http://jj.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yo.521024.cn

[U60] PHP：JSON 编解码
来源：http://ot.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ya.nicolike.cn

[U61] PHP：正则
来源：http://pa.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ob.shxzskj.cn

[U62] PHP：日期对象
来源：http://cm.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tq.nszjky.cn

[U63] PHP：文件读写
来源：http://bv.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ll.nicolike.cn

[U64] PHP：目录遍历
来源：http://qo.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://uy.asd995.cn

[U65] PHP：会话
来源：http://ff.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mz.colortex.cn

[U66] PHP：设置 Cookie
来源：http://sy.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://np.szsharing.cn

[U67] PHP：处理文件上传
来源：http://bv.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ct.gzmigu.cn

[U68] PHP：PDO 连接
来源：http://ml.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kp.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://ya.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vx.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://rs.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pf.lnxyls.cn

[U71] PHP：抛出异常
来源：http://ve.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://ym.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://bs.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://xm.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://na.wgjwhj.cn

parse_ini_file("config.ini", true)
来源：http://bg.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://jj.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://fx.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://zd.bookmarksfly.cn

composer require psr/container
来源：http://nw.9csxet.cn

[U76] PHP：简单路由
来源：http://sb.szxytkj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wc.gzmigu.cn

[U77] PHP：模板渲染
来源：http://zs.bjjhwx.cn

composer require twig/twig
来源：http://fn.yuexingan06.cn

[U78] PHP：单元测试
来源：http://bg.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://qz.521024.cn

[U79] PHP：静态分析
来源：http://wd.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://qw.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://di.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zx.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://hq.yuexingan06.cn

npm init -y;  npm i express
来源：http://iv.hahajie.cn

[U82] JS：package.json 脚本
来源：http://mj.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nl.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://wu.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ho.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://zs.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eu.huixiangedu.cn

[U85] JS：可选链
来源：http://xm.shxzskj.cn

a?.b?.c
来源：http://um.newstarts.cn

[U86] JS：空值合并
来源：http://kh.szsharing.cn

a ?? b
来源：http://su.hahajie.cn

[U87] JS：解构默认值
来源：http://lr.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://kt.gzmigu.cn

[U88] JS：对象展开合并
来源：http://mr.yuexingan06.cn

{ ...a, ...b }
来源：http://zy.bjjhwx.cn

[U89] JS：数组去重
来源：http://rr.gzmigu.cn

[...new Set(arr)]
来源：http://fu.asd995.cn

[U90] JS：数字数组排序
来源：http://uo.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://zt.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://ed.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qe.huixiangedu.cn

[U92] JS：深拷贝
来源：http://rd.haigaiapp.cn

structuredClone(obj)
来源：http://zr.gzmigu.cn

[U93] JS：模板字符串
来源：http://tg.asd995.cn

`共 ${n} 条`
来源：http://lx.hnjuh.cn

[U94] JS：箭头函数
来源：http://pa.521024.cn

const double = x => x * 2;
来源：http://zj.hnjuh.cn

[U95] JS：Promise 包装
来源：http://kz.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://jq.newstarts.cn

[U96] JS：async/await 与异常
来源：http://sr.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zb.colortex.cn

[U97] JS：并发请求
来源：http://sr.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hj.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://qh.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hb.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://pw.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://rd.huanxung.cn

[U100] JS：DOM 查询
来源：http://sq.huanxung.cn

document.querySelector(".item")
来源：http://ry.yuexingan06.cn

[U101] JS：classList 操作
来源：http://ra.huixiangedu.cn

el.classList.toggle("active")
来源：http://pj.nszjky.cn

[U102] JS：本地存储
来源：http://bd.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pf.yuntaijiaju.cn

[U103] JS：定时器
来源：http://vn.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vu.yuexingan06.cn

[U104] JS：防抖
来源：http://cf.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ae.shxzukj.cn

[U105] JS：节流
来源：http://qi.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kl.newstarts.cn

[U106] JS：日期格式化
来源：http://si.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qr.bjjhwx.cn

[U107] JS：数字千分位
来源：http://cp.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tc.huanxung.cn

[U108] JS：随机整数
来源：http://lv.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fz.gzmigu.cn

[U109] JS：数组分组
来源：http://va.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://iu.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://nb.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gd.lnxyls.cn

[U111] JS：对象转 Map
来源：http://ak.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://bh.nicolike.cn

[U112] JS：字符串补位
来源：http://ni.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://uh.asd995.cn

[U113] JS：正则替换全部
来源：http://eq.hnjuh.cn

s.replaceAll("a", "b")
来源：http://by.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://ca.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ts.lnxyls.cn

[U115] JS：生成 UUID
来源：http://ef.muxihuayi.cn

crypto.randomUUID()
来源：http://zo.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://eo.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://qt.shxzskj.cn

[U117] JS：单元测试
来源：http://tn.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://sw.szxytkj.cn

[U118] JS：开发服务器
来源：http://bq.nicolike.cn

npm i -D vite;  npx vite
来源：http://fo.yuntaijiaju.cn

[U119] JS：生产构建
来源：http://pm.chemitech.net.cn

npx vite build
来源：http://qq.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://ip.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://iz.huixiangedu.cn

================================================================================
来源：http://yg.hnjuh.cn

统计汇总
来源：http://ki.hahajie.cn

================================================================================
来源：http://pe.hnjuh.cn

按语言统计（条）：
来源：http://ni.hnjuh.cn

Python ......... 252
来源：http://cd.shtwfgs.cn

PHP ............ 252
来源：http://bg.huixiangedu.cn

JavaScript ..... 252
来源：http://zu.newstarts.cn

TypeScript ..... 212
来源：http://en.muxihuayi.cn

Java ........... 212
来源：http://nq.huixinmuqiang.cn

Go ............. 212
来源：http://ie.9csxet.cn

Ruby ........... 212
来源：http://sq.lnxyls.cn

C# ............. 212
来源：http://tn.colortex.cn

C .............. 30
来源：http://sq.jctech888.com.cn

C++ ............ 30
来源：http://rh.newstarts.cn

SQL ............ 90
来源：http://yb.panjiajie.cn

Bash ........... 80
来源：http://jt.huixinmuqiang.cn

Kotlin ......... 15
来源：http://kw.colortex.cn

Swift .......... 15
来源：http://op.shxzskj.cn

Lua ............ 10
来源：http://vj.shxzukj.cn

Perl ........... 10
来源：http://xm.colortex.cn

Scala .......... 10
来源：http://oi.hnjuh.cn

------------------------------------
来源：http://pi.huixiangedu.cn

合计 ........... 2106 条
来源：http://rb.bookmarksfly.cn

按章节统计：
来源：http://fn.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ub.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kg.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://st.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pl.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bx.nszjky.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pe.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vt.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eo.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gw.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sn.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://is.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yx.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bv.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qn.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ct.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lj.huanxung.cn

Q SQL 专题                              90
来源：http://yb.shxzskj.cn

R Bash 专题                             80
来源：http://iv.shtwfgs.cn

S C / C++ 专题                          60
来源：http://de.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://lu.muxihuayi.cn

U 高频实用片段                         120
来源：http://gg.szsharing.cn

------------------------------------
来源：http://jb.nszjky.cn

合计                                  2106 条
来源：http://rc.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://xt.9csxet.cn

使用提醒
来源：http://wt.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ga.lnxyls.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zw.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sb.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jy.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yh.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ui.szxytkj.cn

—— 文件结束 ——
来源：http://ik.9csxet.cn

================================================================================
来源：http://hw.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://gx.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://hu.nszjky.cn

================================================================================
来源：http://xj.shxzukj.cn

【收录内容】
来源：http://bj.huixiangedu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bo.hahajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tk.asd995.cn

SQL · Bash · C · C++
来源：http://zz.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qz.9csxet.cn

【使用说明】
来源：http://ra.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yi.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hf.huixinmuqiang.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bl.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ug.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yp.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ft.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sj.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ym.521024.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xi.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zx.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ue.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ah.huixiangedu.cn

【文件统计】
来源：http://ql.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pi.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://gg.huixinmuqiang.cn

目  录
来源：http://uj.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://gx.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mv.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tg.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pz.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wa.jctech888.com.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://as.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fl.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fk.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ho.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wz.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vt.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wc.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gw.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xz.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zg.huixiangedu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xj.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mu.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oq.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mq.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ys.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jx.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fl.szxytkj.cn

================================================================================
来源：http://so.nszjky.cn

A. 基础语法与类型
来源：http://lm.wgjwhj.cn

================================================================================
来源：http://ka.yuntaijiaju.cn

[A01] Hello World
来源：http://kt.hnjuh.cn

Py:   print("Hello, World!")
来源：http://an.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://ce.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://be.lnxyls.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tr.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://by.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://zm.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://tl.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ah.newstarts.cn

[A02] 变量声明与赋值
来源：http://sb.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kv.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hs.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://js.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://na.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://wr.9csxet.cn

Go:   name := "Alex"; age := 20
来源：http://xx.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://pb.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vy.nszjky.cn

[A03] 常量定义
来源：http://fp.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xi.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://wh.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://yu.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://vr.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://wk.521024.cn

Go:   const PI = 3.14159
来源：http://vi.panjiajie.cn


<!-- 参考信息 -->