代发 wailian999

[U33] Py：打包发布
来源：http://sy.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://co.9csxet.cn

[U34] Py：判断编码
来源：http://ao.shtwfgs.cn

chardet.detect(raw)
来源：http://yd.panjiajie.cn

[U35] Py：发送邮件
来源：http://ky.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ki.bookmarksfly.cn

[U36] Py：定时任务
来源：http://aa.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://ka.asd995.cn

[U37] Py：读写 Excel
来源：http://jk.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ap.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://tq.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://at.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://lr.panjiajie.cn

sys.stdout.isatty()
来源：http://ub.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://am.szxytkj.cn

print("err", file=sys.stderr)
来源：http://aj.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://bx.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ez.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://xs.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nd.newstarts.cn

[U43] PHP：声明命名空间
来源：http://ss.huixinmuqiang.cn

namespace App\Http;
来源：http://us.szsharing.cn

[U44] PHP：开启严格类型
来源：http://vt.bjjhwx.cn

declare(strict_types=1);
来源：http://mf.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://rs.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tg.colortex.cn

[U46] PHP：可空类型
来源：http://bf.szxytkj.cn

?string $name = null
来源：http://wn.chemitech.net.cn

[U47] PHP：联合类型
来源：http://zo.szxytkj.cn

int|string $id
来源：http://wa.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://vw.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ff.szxytkj.cn

[U49] PHP：只读属性
来源：http://dd.panjiajie.cn

public readonly string $name
来源：http://wo.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://ul.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://ah.szsharing.cn

[U51] PHP：数组解构
来源：http://ix.szsharing.cn

[$a, $b] = $arr;
来源：http://nb.asd995.cn

[U52] PHP：箭头函数
来源：http://qg.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://dr.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://hr.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://pw.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://ct.9csxet.cn

$obj?->method()
来源：http://es.huanxung.cn

[U55] PHP：match 表达式
来源：http://jc.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fk.wgjwhj.cn

[U56] PHP：命名参数
来源：http://rt.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://hi.521024.cn

[U57] PHP：字符串插值
来源：http://wi.huanxung.cn

"值: {$a}"
来源：http://vn.panjiajie.cn

[U58] PHP：数组三件套
来源：http://zq.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ng.shxzukj.cn

[U59] PHP：自定义排序
来源：http://aq.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jo.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://hm.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fq.bjjhwx.cn

[U61] PHP：正则
来源：http://tf.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ht.shxzskj.cn

[U62] PHP：日期对象
来源：http://zg.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sq.521024.cn

[U63] PHP：文件读写
来源：http://ba.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tt.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://nr.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://ve.muxihuayi.cn

[U65] PHP：会话
来源：http://un.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nh.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://rf.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vg.asd995.cn

[U67] PHP：处理文件上传
来源：http://ce.huixiangedu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iz.bjjhwx.cn

[U68] PHP：PDO 连接
来源：http://sh.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mp.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://re.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sl.colortex.cn

[U70] PHP：PDO 事务
来源：http://kv.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eh.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://kd.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://ct.shtwfgs.cn

[U72] PHP：写错误日志
来源：http://tz.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://fq.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://wd.521024.cn

parse_ini_file("config.ini", true)
来源：http://qh.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://mx.wgjwhj.cn

getenv("APP_ENV") ?: "production"
来源：http://ax.lnxyls.cn

[U75] PHP：依赖注入
来源：http://di.shxzukj.cn

composer require psr/container
来源：http://yb.asd995.cn

[U76] PHP：简单路由
来源：http://nw.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hd.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://es.panjiajie.cn

composer require twig/twig
来源：http://dv.9csxet.cn

[U78] PHP：单元测试
来源：http://zu.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://vu.panjiajie.cn

[U79] PHP：静态分析
来源：http://th.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://sk.nszjky.cn

[U80] PHP：代码规范修复
来源：http://pg.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ls.szsharing.cn

[U81] JS：初始化项目
来源：http://lw.colortex.cn

npm init -y;  npm i express
来源：http://mk.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://ws.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xr.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://cp.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fh.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://qo.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xk.gzmigu.cn

[U85] JS：可选链
来源：http://yk.yuexingan06.cn

a?.b?.c
来源：http://mi.hnjuh.cn

[U86] JS：空值合并
来源：http://ft.hahajie.cn

a ?? b
来源：http://lm.panjiajie.cn

[U87] JS：解构默认值
来源：http://bl.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://sl.panjiajie.cn

[U88] JS：对象展开合并
来源：http://du.yuexingan06.cn

{ ...a, ...b }
来源：http://xu.chemitech.net.cn

[U89] JS：数组去重
来源：http://ze.huanxung.cn

[...new Set(arr)]
来源：http://fe.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://so.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://na.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://sf.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rb.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://gq.shtwfgs.cn

structuredClone(obj)
来源：http://mw.nicolike.cn

[U93] JS：模板字符串
来源：http://se.shtwfgs.cn

`共 ${n} 条`
来源：http://pj.lnxyls.cn

[U94] JS：箭头函数
来源：http://sb.huanxung.cn

const double = x => x * 2;
来源：http://yk.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://bn.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://ed.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://cc.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://az.colortex.cn

[U97] JS：并发请求
来源：http://mp.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bz.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://ta.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zo.bookmarksfly.cn

[U99] JS：事件监听
来源：http://wz.521024.cn

el.addEventListener("click", e => {})
来源：http://uz.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://jn.jctech888.com.cn

document.querySelector(".item")
来源：http://jf.wgjwhj.cn

[U101] JS：classList 操作
来源：http://vl.muxihuayi.cn

el.classList.toggle("active")
来源：http://xi.jctech888.com.cn

[U102] JS：本地存储
来源：http://aa.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://az.haigaiapp.cn

[U103] JS：定时器
来源：http://gv.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sj.9csxet.cn

[U104] JS：防抖
来源：http://tb.bookmarksfly.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sb.bjjhwx.cn

[U105] JS：节流
来源：http://jr.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lk.hahajie.cn

[U106] JS：日期格式化
来源：http://vq.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zm.haigaiapp.cn

[U107] JS：数字千分位
来源：http://ja.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ba.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://vx.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://by.shxzukj.cn

[U109] JS：数组分组
来源：http://ni.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://zj.9csxet.cn

[U110] JS：数组分块
来源：http://hk.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ds.lnxyls.cn

[U111] JS：对象转 Map
来源：http://ui.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://il.shxzskj.cn

[U112] JS：字符串补位
来源：http://pn.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://rn.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://zk.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://fg.521024.cn

[U114] JS：JSON 深比较
来源：http://zw.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pl.szsharing.cn

[U115] JS：生成 UUID
来源：http://qt.haigaiapp.cn

crypto.randomUUID()
来源：http://ak.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://rc.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://yc.shtwfgs.cn

[U117] JS：单元测试
来源：http://kp.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://bi.jctech888.com.cn

[U118] JS：开发服务器
来源：http://gs.panjiajie.cn

npm i -D vite;  npx vite
来源：http://kv.haigaiapp.cn

[U119] JS：生产构建
来源：http://rm.shxzskj.cn

npx vite build
来源：http://uu.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://pm.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://sj.9csxet.cn

================================================================================
来源：http://br.hahajie.cn

统计汇总
来源：http://gd.lnxyls.cn

================================================================================
来源：http://xf.bookmarksfly.cn

按语言统计（条）：
来源：http://sb.asd995.cn

Python ......... 252
来源：http://qx.chemitech.net.cn

PHP ............ 252
来源：http://xh.jianghongdianzi.cn

JavaScript ..... 252
来源：http://oy.asd995.cn

TypeScript ..... 212
来源：http://rc.yuntaijiaju.cn

Java ........... 212
来源：http://th.wgjwhj.cn

Go ............. 212
来源：http://gr.bookmarksfly.cn

Ruby ........... 212
来源：http://xq.huanxung.cn

C# ............. 212
来源：http://ej.9csxet.cn

C .............. 30
来源：http://pc.asd995.cn

C++ ............ 30
来源：http://jj.bjjhwx.cn

SQL ............ 90
来源：http://ow.bookmarksfly.cn

Bash ........... 80
来源：http://zb.asd995.cn

Kotlin ......... 15
来源：http://xz.yuntaijiaju.cn

Swift .......... 15
来源：http://hm.asd995.cn

Lua ............ 10
来源：http://sy.colortex.cn

Perl ........... 10
来源：http://ej.panjiajie.cn

Scala .......... 10
来源：http://kv.nicolike.cn

------------------------------------
来源：http://sr.chemitech.net.cn

合计 ........... 2106 条
来源：http://td.jctech888.com.cn

按章节统计：
来源：http://la.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sv.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hs.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xl.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ca.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nv.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pz.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wt.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lz.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yl.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://si.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cu.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ca.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bo.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jl.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sn.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hk.bookmarksfly.cn

Q SQL 专题                              90
来源：http://yq.huixinmuqiang.cn

R Bash 专题                             80
来源：http://ny.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://zk.wgjwhj.cn

T 其他语言补充                          60
来源：http://tt.haigaiapp.cn

U 高频实用片段                         120
来源：http://hx.colortex.cn

------------------------------------
来源：http://ia.szxytkj.cn

合计                                  2106 条
来源：http://yw.colortex.cn

--------------------------------------------------------------------------------
来源：http://cd.9csxet.cn

使用提醒
来源：http://vu.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://sq.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xo.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zf.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vm.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ez.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://an.szsharing.cn

—— 文件结束 ——
来源：http://qs.hnjuh.cn

================================================================================
来源：http://zr.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://hx.colortex.cn

Common Programming Examples Cheat Book
来源：http://ix.yuntaijiaju.cn

================================================================================
来源：http://mw.jctech888.com.cn

【收录内容】
来源：http://se.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ro.huixiangedu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ox.szsharing.cn

SQL · Bash · C · C++
来源：http://vu.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bg.shxzskj.cn

【使用说明】
来源：http://co.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ix.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fp.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ut.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vv.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gk.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zz.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ne.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fd.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://op.gzmigu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mi.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dm.bookmarksfly.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oq.asd995.cn

【文件统计】
来源：http://wi.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ey.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://yt.huixiangedu.cn

目  录
来源：http://ub.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ds.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://me.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uw.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wl.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yh.wgjwhj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rr.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ax.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lw.yuexingan06.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iu.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ix.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cw.haigaiapp.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zs.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bh.shtwfgs.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tf.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vu.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dv.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://us.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nb.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yt.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://en.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://af.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mv.shxzskj.cn

================================================================================
来源：http://hj.nicolike.cn

A. 基础语法与类型
来源：http://ux.yuexingan06.cn

================================================================================
来源：http://bz.huixiangedu.cn

[A01] Hello World
来源：http://hv.huanxung.cn

Py:   print("Hello, World!")
来源：http://we.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://jb.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://gj.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yj.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://lt.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://fs.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://ch.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lq.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://hu.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kl.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kv.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ua.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zw.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://uh.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://ps.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://va.jctech888.com.cn


<!-- 参考信息 -->