代发 wailian999

[U37] Py：读写 Excel
来源：http://ot.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mx.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://ds.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://jm.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://df.szsharing.cn

sys.stdout.isatty()
来源：http://tw.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://pi.huanxung.cn

print("err", file=sys.stderr)
来源：http://lg.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://bp.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jl.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://xk.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kv.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://xk.nszjky.cn

namespace App\Http;
来源：http://gp.nicolike.cn

[U44] PHP：开启严格类型
来源：http://cg.nicolike.cn

declare(strict_types=1);
来源：http://eb.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://du.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://se.nicolike.cn

[U46] PHP：可空类型
来源：http://jt.gzmigu.cn

?string $name = null
来源：http://oy.hahajie.cn

[U47] PHP：联合类型
来源：http://ph.muxihuayi.cn

int|string $id
来源：http://lc.shxzukj.cn

[U48] PHP：纯枚举
来源：http://et.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zj.hahajie.cn

[U49] PHP：只读属性
来源：http://uy.hnjuh.cn

public readonly string $name
来源：http://bl.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://hf.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://xu.haigaiapp.cn

[U51] PHP：数组解构
来源：http://zs.yuexingan06.cn

[$a, $b] = $arr;
来源：http://nw.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://cb.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://do.hahajie.cn

[U53] PHP：空合并运算符
来源：http://th.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://td.huanxung.cn

[U54] PHP：空安全调用
来源：http://sg.bookmarksfly.cn

$obj?->method()
来源：http://xd.9csxet.cn

[U55] PHP：match 表达式
来源：http://yo.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zx.hnjuh.cn

[U56] PHP：命名参数
来源：http://iz.haigaiapp.cn

f(a: 1, b: 2)
来源：http://qb.hnjuh.cn

[U57] PHP：字符串插值
来源：http://ai.asd995.cn

"值: {$a}"
来源：http://sr.9csxet.cn

[U58] PHP：数组三件套
来源：http://xm.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iu.lnxyls.cn

[U59] PHP：自定义排序
来源：http://ze.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://th.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://ul.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bt.huixiangedu.cn

[U61] PHP：正则
来源：http://aj.newstarts.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ye.panjiajie.cn

[U62] PHP：日期对象
来源：http://un.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eg.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://cd.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gy.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://uj.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ez.haigaiapp.cn

[U65] PHP：会话
来源：http://tl.huixiangedu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oy.colortex.cn

[U66] PHP：设置 Cookie
来源：http://vo.shtwfgs.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kk.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://tu.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ha.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://yk.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bk.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://ld.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yu.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://dl.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qr.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://jq.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://pd.shxzskj.cn

[U72] PHP：写错误日志
来源：http://qe.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://cd.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://cf.yuexingan06.cn

parse_ini_file("config.ini", true)
来源：http://ij.lnxyls.cn

[U74] PHP：读取环境变量
来源：http://np.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://nq.shxzskj.cn

[U75] PHP：依赖注入
来源：http://se.bookmarksfly.cn

composer require psr/container
来源：http://mi.9csxet.cn

[U76] PHP：简单路由
来源：http://vq.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eb.colortex.cn

[U77] PHP：模板渲染
来源：http://vj.huixiangedu.cn

composer require twig/twig
来源：http://nz.haigaiapp.cn

[U78] PHP：单元测试
来源：http://mc.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://is.panjiajie.cn

[U79] PHP：静态分析
来源：http://xp.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://na.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://yj.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oz.asd995.cn

[U81] JS：初始化项目
来源：http://fi.szsharing.cn

npm init -y;  npm i express
来源：http://jd.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://rm.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vu.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://rj.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://od.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://fe.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bc.hahajie.cn

[U85] JS：可选链
来源：http://ap.wgjwhj.cn

a?.b?.c
来源：http://bb.shxzukj.cn

[U86] JS：空值合并
来源：http://nh.newstarts.cn

a ?? b
来源：http://kp.wgjwhj.cn

[U87] JS：解构默认值
来源：http://bu.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://pa.asd995.cn

[U88] JS：对象展开合并
来源：http://rf.newstarts.cn

{ ...a, ...b }
来源：http://xq.lnxyls.cn

[U89] JS：数组去重
来源：http://cj.huixinmuqiang.cn

[...new Set(arr)]
来源：http://fr.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://pt.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://yc.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://lb.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vk.asd995.cn

[U92] JS：深拷贝
来源：http://kl.nicolike.cn

structuredClone(obj)
来源：http://gl.hnjuh.cn

[U93] JS：模板字符串
来源：http://ip.shxzskj.cn

`共 ${n} 条`
来源：http://vs.asd995.cn

[U94] JS：箭头函数
来源：http://vc.huixinmuqiang.cn

const double = x => x * 2;
来源：http://gl.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://ps.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://pp.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://jo.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mk.szxytkj.cn

[U97] JS：并发请求
来源：http://ps.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rl.521024.cn

[U98] JS：fetch 带 JSON
来源：http://ub.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yv.szxytkj.cn

[U99] JS：事件监听
来源：http://gp.wgjwhj.cn

el.addEventListener("click", e => {})
来源：http://dp.hahajie.cn

[U100] JS：DOM 查询
来源：http://wv.lnxyls.cn

document.querySelector(".item")
来源：http://wz.muxihuayi.cn

[U101] JS：classList 操作
来源：http://zn.panjiajie.cn

el.classList.toggle("active")
来源：http://zq.haigaiapp.cn

[U102] JS：本地存储
来源：http://al.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hy.wgjwhj.cn

[U103] JS：定时器
来源：http://iq.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ac.yuexingan06.cn

[U104] JS：防抖
来源：http://ap.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kg.szsharing.cn

[U105] JS：节流
来源：http://uh.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xp.bjjhwx.cn

[U106] JS：日期格式化
来源：http://uk.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ci.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://zk.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kt.asd995.cn

[U108] JS：随机整数
来源：http://bh.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mz.lnxyls.cn

[U109] JS：数组分组
来源：http://ut.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://ko.bookmarksfly.cn

[U110] JS：数组分块
来源：http://fy.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hk.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://hm.asd995.cn

new Map(Object.entries(obj))
来源：http://rh.shxzskj.cn

[U112] JS：字符串补位
来源：http://pj.colortex.cn

"7".padStart(3, "0")
来源：http://do.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://zx.colortex.cn

s.replaceAll("a", "b")
来源：http://ia.chemitech.net.cn

[U114] JS：JSON 深比较
来源：http://xn.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zy.huanxung.cn

[U115] JS：生成 UUID
来源：http://ec.asd995.cn

crypto.randomUUID()
来源：http://fp.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://tv.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://eu.521024.cn

[U117] JS：单元测试
来源：http://gc.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://ox.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://th.nszjky.cn

npm i -D vite;  npx vite
来源：http://mw.newstarts.cn

[U119] JS：生产构建
来源：http://jh.nicolike.cn

npx vite build
来源：http://az.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://ep.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://do.yuexingan06.cn

================================================================================
来源：http://kn.nicolike.cn

统计汇总
来源：http://dn.huanxung.cn

================================================================================
来源：http://tg.colortex.cn

按语言统计（条）：
来源：http://jf.hnjuh.cn

Python ......... 252
来源：http://wf.chemitech.net.cn

PHP ............ 252
来源：http://re.lnxyls.cn

JavaScript ..... 252
来源：http://pj.nicolike.cn

TypeScript ..... 212
来源：http://ob.shxzukj.cn

Java ........... 212
来源：http://zm.huanxung.cn

Go ............. 212
来源：http://ng.hahajie.cn

Ruby ........... 212
来源：http://au.haigaiapp.cn

C# ............. 212
来源：http://ak.521024.cn

C .............. 30
来源：http://ry.jianghongdianzi.cn

C++ ............ 30
来源：http://me.panjiajie.cn

SQL ............ 90
来源：http://fr.bjjhwx.cn

Bash ........... 80
来源：http://rx.yuexingan06.cn

Kotlin ......... 15
来源：http://hg.panjiajie.cn

Swift .......... 15
来源：http://fz.szsharing.cn

Lua ............ 10
来源：http://bn.hnjuh.cn

Perl ........... 10
来源：http://aa.huixinmuqiang.cn

Scala .......... 10
来源：http://ao.jctech888.com.cn

------------------------------------
来源：http://ws.szsharing.cn

合计 ........... 2106 条
来源：http://ik.panjiajie.cn

按章节统计：
来源：http://ij.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xn.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xj.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://of.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uj.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nj.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bt.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xw.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rm.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mk.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://we.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dm.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rl.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://px.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://er.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zx.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zq.asd995.cn

Q SQL 专题                              90
来源：http://rh.haigaiapp.cn

R Bash 专题                             80
来源：http://vc.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://ca.521024.cn

T 其他语言补充                          60
来源：http://eh.hahajie.cn

U 高频实用片段                         120
来源：http://eg.shxzukj.cn

------------------------------------
来源：http://ps.yuexingan06.cn

合计                                  2106 条
来源：http://cj.asd995.cn

--------------------------------------------------------------------------------
来源：http://mg.muxihuayi.cn

使用提醒
来源：http://vn.hahajie.cn

--------------------------------------------------------------------------------
来源：http://bf.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cc.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zl.haigaiapp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gq.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hq.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ro.nszjky.cn

—— 文件结束 ——
来源：http://np.shxzukj.cn

================================================================================
来源：http://yo.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://ij.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://dw.colortex.cn

================================================================================
来源：http://op.yuntaijiaju.cn

【收录内容】
来源：http://yo.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tu.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jy.muxihuayi.cn

SQL · Bash · C · C++
来源：http://za.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hk.hahajie.cn

【使用说明】
来源：http://wh.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fs.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hw.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vf.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yi.shtwfgs.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vz.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mq.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://id.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kb.shxzukj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mr.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vx.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rg.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ov.huanxung.cn

【文件统计】
来源：http://ly.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rl.nicolike.cn

--------------------------------------------------------------------------------
来源：http://xn.huanxung.cn

目  录
来源：http://km.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://di.huixiangedu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fk.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fw.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hj.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vd.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ew.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rm.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fs.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oa.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ca.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vt.521024.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://we.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sl.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ho.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xq.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ul.yuntaijiaju.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pp.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nu.huixiangedu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ho.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mu.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://si.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ur.yuntaijiaju.cn

================================================================================
来源：http://xv.yuntaijiaju.cn

A. 基础语法与类型
来源：http://ny.521024.cn

================================================================================
来源：http://ah.521024.cn

[A01] Hello World
来源：http://ae.shxzukj.cn

Py:   print("Hello, World!")
来源：http://hh.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://fr.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://cs.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yx.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://hm.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://kp.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://bg.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ch.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://yg.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ij.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yd.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jp.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tx.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://xs.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://oh.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://ga.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dd.521024.cn

[A03] 常量定义
来源：http://vm.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rx.colortex.cn

PHP:  const PI = 3.14159;
来源：http://kf.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://mm.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://li.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://dw.shxzskj.cn

Go:   const PI = 3.14159
来源：http://gt.bjjhwx.cn


<!-- 参考信息 -->