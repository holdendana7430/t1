代发 wailian999

[U33] Py：打包发布
来源：http://mg.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://qa.yuexingan06.cn

[U34] Py：判断编码
来源：http://ci.huixinmuqiang.cn

chardet.detect(raw)
来源：http://kz.colortex.cn

[U35] Py：发送邮件
来源：http://cr.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gy.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://ek.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://sj.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://ur.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://md.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://us.asd995.cn

Path(__file__).resolve().parent
来源：http://kf.521024.cn

[U39] Py：判断是否在交互环境
来源：http://oq.huixiangedu.cn

sys.stdout.isatty()
来源：http://to.hahajie.cn

[U40] Py：打印到标准错误
来源：http://vq.haigaiapp.cn

print("err", file=sys.stderr)
来源：http://gx.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://qv.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ak.chemitech.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://yy.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xr.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://eu.muxihuayi.cn

namespace App\Http;
来源：http://ws.colortex.cn

[U44] PHP：开启严格类型
来源：http://gi.yuexingan06.cn

declare(strict_types=1);
来源：http://vd.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://wx.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tw.521024.cn

[U46] PHP：可空类型
来源：http://ti.hahajie.cn

?string $name = null
来源：http://jk.szsharing.cn

[U47] PHP：联合类型
来源：http://cg.muxihuayi.cn

int|string $id
来源：http://dp.lnxyls.cn

[U48] PHP：纯枚举
来源：http://dd.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://im.hnjuh.cn

[U49] PHP：只读属性
来源：http://kj.jctech888.com.cn

public readonly string $name
来源：http://jg.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://re.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://ry.9csxet.cn

[U51] PHP：数组解构
来源：http://cn.nicolike.cn

[$a, $b] = $arr;
来源：http://wl.shxzskj.cn

[U52] PHP：箭头函数
来源：http://ax.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://cp.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://tr.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://ar.newstarts.cn

[U54] PHP：空安全调用
来源：http://ta.huixinmuqiang.cn

$obj?->method()
来源：http://ba.hnjuh.cn

[U55] PHP：match 表达式
来源：http://cc.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zo.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://sa.yuntaijiaju.cn

f(a: 1, b: 2)
来源：http://tz.lnxyls.cn

[U57] PHP：字符串插值
来源：http://ne.jctech888.com.cn

"值: {$a}"
来源：http://hg.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://pa.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kf.newstarts.cn

[U59] PHP：自定义排序
来源：http://bz.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yh.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://ow.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fl.huixinmuqiang.cn

[U61] PHP：正则
来源：http://uu.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bw.shxzukj.cn

[U62] PHP：日期对象
来源：http://lr.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://jh.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ir.lnxyls.cn

[U64] PHP：目录遍历
来源：http://fd.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://ti.9csxet.cn

[U65] PHP：会话
来源：http://mg.shxzukj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oc.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://xw.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pk.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://fa.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bn.haigaiapp.cn

[U68] PHP：PDO 连接
来源：http://fp.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ob.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://mn.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://al.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://tf.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bw.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://gt.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://yl.yuexingan06.cn

[U72] PHP：写错误日志
来源：http://za.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://ae.gzmigu.cn

[U73] PHP：读取 ini 配置
来源：http://ua.521024.cn

parse_ini_file("config.ini", true)
来源：http://tf.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://cp.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://gs.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://va.huixiangedu.cn

composer require psr/container
来源：http://oi.gzmigu.cn

[U76] PHP：简单路由
来源：http://is.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hy.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://ez.nicolike.cn

composer require twig/twig
来源：http://jx.wgjwhj.cn

[U78] PHP：单元测试
来源：http://sg.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://kg.nicolike.cn

[U79] PHP：静态分析
来源：http://oc.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://jb.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://jh.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qe.9csxet.cn

[U81] JS：初始化项目
来源：http://ml.hahajie.cn

npm init -y;  npm i express
来源：http://oh.huanxung.cn

[U82] JS：package.json 脚本
来源：http://ia.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://et.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://xj.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fg.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://nb.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fd.newstarts.cn

[U85] JS：可选链
来源：http://yc.9csxet.cn

a?.b?.c
来源：http://ck.muxihuayi.cn

[U86] JS：空值合并
来源：http://vz.chemitech.net.cn

a ?? b
来源：http://on.lnxyls.cn

[U87] JS：解构默认值
来源：http://zu.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://hi.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://zg.chemitech.net.cn

{ ...a, ...b }
来源：http://wf.huixiangedu.cn

[U89] JS：数组去重
来源：http://bi.haigaiapp.cn

[...new Set(arr)]
来源：http://cc.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://qi.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://ox.szsharing.cn

[U91] JS：对象键值遍历
来源：http://ef.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yr.shxzukj.cn

[U92] JS：深拷贝
来源：http://ee.jctech888.com.cn

structuredClone(obj)
来源：http://fa.shxzukj.cn

[U93] JS：模板字符串
来源：http://ph.haigaiapp.cn

`共 ${n} 条`
来源：http://qt.newstarts.cn

[U94] JS：箭头函数
来源：http://aj.huixinmuqiang.cn

const double = x => x * 2;
来源：http://ay.szxytkj.cn

[U95] JS：Promise 包装
来源：http://iw.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://uo.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://sy.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aj.wgjwhj.cn

[U97] JS：并发请求
来源：http://yf.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nh.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://oh.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ja.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://fw.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://el.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://sb.newstarts.cn

document.querySelector(".item")
来源：http://ki.hnjuh.cn

[U101] JS：classList 操作
来源：http://xj.newstarts.cn

el.classList.toggle("active")
来源：http://zr.9csxet.cn

[U102] JS：本地存储
来源：http://na.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vi.hahajie.cn

[U103] JS：定时器
来源：http://wm.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fg.shtwfgs.cn

[U104] JS：防抖
来源：http://me.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gb.hnjuh.cn

[U105] JS：节流
来源：http://bf.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xe.bjjhwx.cn

[U106] JS：日期格式化
来源：http://uh.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rq.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://ve.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rq.newstarts.cn

[U108] JS：随机整数
来源：http://rr.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cm.haigaiapp.cn

[U109] JS：数组分组
来源：http://od.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://zd.muxihuayi.cn

[U110] JS：数组分块
来源：http://ho.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://os.panjiajie.cn

[U111] JS：对象转 Map
来源：http://hd.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://zr.panjiajie.cn

[U112] JS：字符串补位
来源：http://yh.shtwfgs.cn

"7".padStart(3, "0")
来源：http://cr.szsharing.cn

[U113] JS：正则替换全部
来源：http://lo.huanxung.cn

s.replaceAll("a", "b")
来源：http://az.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://dp.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kc.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://ac.muxihuayi.cn

crypto.randomUUID()
来源：http://qd.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://jq.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://xz.shxzukj.cn

[U117] JS：单元测试
来源：http://px.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://tf.haigaiapp.cn

[U118] JS：开发服务器
来源：http://kz.nicolike.cn

npm i -D vite;  npx vite
来源：http://ag.shxzukj.cn

[U119] JS：生产构建
来源：http://rm.huixiangedu.cn

npx vite build
来源：http://wg.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://ao.huixinmuqiang.cn

import.meta.env.VITE_API_URL
来源：http://re.shxzukj.cn

================================================================================
来源：http://gz.szxytkj.cn

统计汇总
来源：http://ck.521024.cn

================================================================================
来源：http://cm.panjiajie.cn

按语言统计（条）：
来源：http://dx.bookmarksfly.cn

Python ......... 252
来源：http://uw.lnxyls.cn

PHP ............ 252
来源：http://ft.521024.cn

JavaScript ..... 252
来源：http://ta.panjiajie.cn

TypeScript ..... 212
来源：http://fa.nszjky.cn

Java ........... 212
来源：http://vp.521024.cn

Go ............. 212
来源：http://ug.nicolike.cn

Ruby ........... 212
来源：http://ax.shxzskj.cn

C# ............. 212
来源：http://eh.yuntaijiaju.cn

C .............. 30
来源：http://jm.nszjky.cn

C++ ............ 30
来源：http://ak.jianghongdianzi.cn

SQL ............ 90
来源：http://bj.szsharing.cn

Bash ........... 80
来源：http://el.newstarts.cn

Kotlin ......... 15
来源：http://ls.colortex.cn

Swift .......... 15
来源：http://fw.huanxung.cn

Lua ............ 10
来源：http://ro.shxzukj.cn

Perl ........... 10
来源：http://uh.shxzukj.cn

Scala .......... 10
来源：http://tj.yuntaijiaju.cn

------------------------------------
来源：http://pj.nicolike.cn

合计 ........... 2106 条
来源：http://te.shxzskj.cn

按章节统计：
来源：http://uv.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wf.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bz.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kt.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lc.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jk.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://va.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jp.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zl.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rk.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xf.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pi.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cp.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gh.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bv.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yy.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://em.nicolike.cn

Q SQL 专题                              90
来源：http://cf.jianghongdianzi.cn

R Bash 专题                             80
来源：http://hx.newstarts.cn

S C / C++ 专题                          60
来源：http://cf.haigaiapp.cn

T 其他语言补充                          60
来源：http://ju.huanxung.cn

U 高频实用片段                         120
来源：http://cw.panjiajie.cn

------------------------------------
来源：http://nx.bjjhwx.cn

合计                                  2106 条
来源：http://en.nicolike.cn

--------------------------------------------------------------------------------
来源：http://bl.jctech888.com.cn

使用提醒
来源：http://vr.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://qp.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pe.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bn.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qh.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fr.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jv.szxytkj.cn

—— 文件结束 ——
来源：http://wh.huixiangedu.cn

================================================================================
来源：http://io.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://ye.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://dv.9csxet.cn

================================================================================
来源：http://en.muxihuayi.cn

【收录内容】
来源：http://pt.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tx.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xt.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://vs.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gj.huixiangedu.cn

【使用说明】
来源：http://pa.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tw.bookmarksfly.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vy.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lc.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://as.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hh.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lf.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dp.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pl.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ld.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tq.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ju.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cx.chemitech.net.cn

【文件统计】
来源：http://pf.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nm.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ht.muxihuayi.cn

目  录
来源：http://qw.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://lu.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://km.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://up.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://or.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tq.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lx.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jo.9csxet.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://em.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uc.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://er.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ob.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sp.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ee.shxzukj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qt.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://br.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ho.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ol.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wh.huixinmuqiang.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gl.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jm.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ax.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gj.gzmigu.cn

================================================================================
来源：http://xd.muxihuayi.cn

A. 基础语法与类型
来源：http://au.nicolike.cn

================================================================================
来源：http://kw.yuntaijiaju.cn

[A01] Hello World
来源：http://nc.newstarts.cn

Py:   print("Hello, World!")
来源：http://ts.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://dl.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://sl.bookmarksfly.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tr.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://rr.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://ho.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://mj.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cm.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://yd.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bs.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pa.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ui.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ym.shtwfgs.cn

Java: String name = "Alex"; int age = 20;
来源：http://uf.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://mz.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://gk.nszjky.cn


<!-- 参考信息 -->