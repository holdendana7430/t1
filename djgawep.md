代发 wailian999

[U31] Py：单测
来源：http://en.gzmigu.cn

python -m pytest -q
来源：http://ew.asd995.cn

[U32] Py：代码格式化
来源：http://np.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://sx.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://ax.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ca.hahajie.cn

[U34] Py：判断编码
来源：http://vy.haigaiapp.cn

chardet.detect(raw)
来源：http://qv.asd995.cn

[U35] Py：发送邮件
来源：http://up.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lg.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://rz.521024.cn

schedule.every(10).minutes.do(job)
来源：http://ia.nicolike.cn

[U37] Py：读写 Excel
来源：http://ts.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oc.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://vl.huanxung.cn

Path(__file__).resolve().parent
来源：http://ja.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://of.haigaiapp.cn

sys.stdout.isatty()
来源：http://cb.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://kd.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://ff.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://bw.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lz.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://ok.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wm.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://ry.huanxung.cn

namespace App\Http;
来源：http://gv.asd995.cn

[U44] PHP：开启严格类型
来源：http://na.shxzukj.cn

declare(strict_types=1);
来源：http://cf.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://mr.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wl.haigaiapp.cn

[U46] PHP：可空类型
来源：http://xo.chemitech.net.cn

?string $name = null
来源：http://hv.chemitech.net.cn

[U47] PHP：联合类型
来源：http://uu.jctech888.com.cn

int|string $id
来源：http://st.huixinmuqiang.cn

[U48] PHP：纯枚举
来源：http://rj.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wf.yuexingan06.cn

[U49] PHP：只读属性
来源：http://bg.huanxung.cn

public readonly string $name
来源：http://nu.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://qa.nszjky.cn

public function __construct(private int $id) {}
来源：http://ri.hnjuh.cn

[U51] PHP：数组解构
来源：http://ia.chemitech.net.cn

[$a, $b] = $arr;
来源：http://ed.shxzskj.cn

[U52] PHP：箭头函数
来源：http://sq.huixiangedu.cn

$double = fn($x) => $x * 2;
来源：http://hn.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://xk.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://ex.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://bq.haigaiapp.cn

$obj?->method()
来源：http://yi.hahajie.cn

[U55] PHP：match 表达式
来源：http://kn.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nh.gzmigu.cn

[U56] PHP：命名参数
来源：http://pl.jctech888.com.cn

f(a: 1, b: 2)
来源：http://yj.lnxyls.cn

[U57] PHP：字符串插值
来源：http://qp.asd995.cn

"值: {$a}"
来源：http://sv.nicolike.cn

[U58] PHP：数组三件套
来源：http://mp.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ug.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://vq.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gv.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://ul.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cf.shtwfgs.cn

[U61] PHP：正则
来源：http://nl.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://go.shtwfgs.cn

[U62] PHP：日期对象
来源：http://ad.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rf.nicolike.cn

[U63] PHP：文件读写
来源：http://oj.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oi.hnjuh.cn

[U64] PHP：目录遍历
来源：http://wk.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://hf.huanxung.cn

[U65] PHP：会话
来源：http://gf.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qw.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://sf.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rv.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://jn.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ik.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://ch.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zu.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://zq.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nh.9csxet.cn

[U70] PHP：PDO 事务
来源：http://ie.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fl.asd995.cn

[U71] PHP：抛出异常
来源：http://lr.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://wg.huanxung.cn

[U72] PHP：写错误日志
来源：http://br.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://pj.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://xv.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://bb.hahajie.cn

[U74] PHP：读取环境变量
来源：http://aw.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://cn.colortex.cn

[U75] PHP：依赖注入
来源：http://hj.lnxyls.cn

composer require psr/container
来源：http://nq.9csxet.cn

[U76] PHP：简单路由
来源：http://fo.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://en.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://nz.asd995.cn

composer require twig/twig
来源：http://se.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://vc.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://je.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://hz.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://yu.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://kx.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tw.huanxung.cn

[U81] JS：初始化项目
来源：http://ao.nicolike.cn

npm init -y;  npm i express
来源：http://dz.9csxet.cn

[U82] JS：package.json 脚本
来源：http://dl.gzmigu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hv.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://yd.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oa.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://cf.szsharing.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hb.huixinmuqiang.cn

[U85] JS：可选链
来源：http://dx.muxihuayi.cn

a?.b?.c
来源：http://si.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://hx.huixiangedu.cn

a ?? b
来源：http://ux.gzmigu.cn

[U87] JS：解构默认值
来源：http://zm.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://qs.nicolike.cn

[U88] JS：对象展开合并
来源：http://iq.yuexingan06.cn

{ ...a, ...b }
来源：http://nt.bjjhwx.cn

[U89] JS：数组去重
来源：http://uc.huixinmuqiang.cn

[...new Set(arr)]
来源：http://cw.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://gb.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://dw.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://dl.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cu.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://bj.huixiangedu.cn

structuredClone(obj)
来源：http://oi.bjjhwx.cn

[U93] JS：模板字符串
来源：http://bh.colortex.cn

`共 ${n} 条`
来源：http://xs.shxzukj.cn

[U94] JS：箭头函数
来源：http://pt.colortex.cn

const double = x => x * 2;
来源：http://vq.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://jn.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://se.newstarts.cn

[U96] JS：async/await 与异常
来源：http://kp.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rb.newstarts.cn

[U97] JS：并发请求
来源：http://dp.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fq.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://rv.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oz.haigaiapp.cn

[U99] JS：事件监听
来源：http://dn.9csxet.cn

el.addEventListener("click", e => {})
来源：http://rr.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://xt.nicolike.cn

document.querySelector(".item")
来源：http://sg.jctech888.com.cn

[U101] JS：classList 操作
来源：http://pq.jctech888.com.cn

el.classList.toggle("active")
来源：http://kf.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://ks.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qv.huixiangedu.cn

[U103] JS：定时器
来源：http://au.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yi.huanxung.cn

[U104] JS：防抖
来源：http://vr.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jd.bjjhwx.cn

[U105] JS：节流
来源：http://vr.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://px.szsharing.cn

[U106] JS：日期格式化
来源：http://pa.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ir.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://vx.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iu.wgjwhj.cn

[U108] JS：随机整数
来源：http://ij.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mf.muxihuayi.cn

[U109] JS：数组分组
来源：http://wa.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://ip.huanxung.cn

[U110] JS：数组分块
来源：http://xd.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mn.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://lg.nszjky.cn

new Map(Object.entries(obj))
来源：http://bh.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://wx.gzmigu.cn

"7".padStart(3, "0")
来源：http://ia.hnjuh.cn

[U113] JS：正则替换全部
来源：http://bb.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://xa.nicolike.cn

[U114] JS：JSON 深比较
来源：http://sw.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fr.szxytkj.cn

[U115] JS：生成 UUID
来源：http://wr.newstarts.cn

crypto.randomUUID()
来源：http://oo.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://pk.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://hk.hnjuh.cn

[U117] JS：单元测试
来源：http://au.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://pi.newstarts.cn

[U118] JS：开发服务器
来源：http://yy.szsharing.cn

npm i -D vite;  npx vite
来源：http://tn.huixiangedu.cn

[U119] JS：生产构建
来源：http://ye.colortex.cn

npx vite build
来源：http://ud.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://bj.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://mp.yuntaijiaju.cn

================================================================================
来源：http://mq.jianghongdianzi.cn

统计汇总
来源：http://by.shxzskj.cn

================================================================================
来源：http://gg.huixinmuqiang.cn

按语言统计（条）：
来源：http://jq.huanxung.cn

Python ......... 252
来源：http://cx.panjiajie.cn

PHP ............ 252
来源：http://wi.9csxet.cn

JavaScript ..... 252
来源：http://zy.jianghongdianzi.cn

TypeScript ..... 212
来源：http://mn.yuntaijiaju.cn

Java ........... 212
来源：http://nv.yuexingan06.cn

Go ............. 212
来源：http://qh.yuexingan06.cn

Ruby ........... 212
来源：http://qn.bookmarksfly.cn

C# ............. 212
来源：http://et.gzmigu.cn

C .............. 30
来源：http://yr.haigaiapp.cn

C++ ............ 30
来源：http://mc.shxzukj.cn

SQL ............ 90
来源：http://rl.jianghongdianzi.cn

Bash ........... 80
来源：http://se.nicolike.cn

Kotlin ......... 15
来源：http://cm.haigaiapp.cn

Swift .......... 15
来源：http://ut.shxzskj.cn

Lua ............ 10
来源：http://eu.hnjuh.cn

Perl ........... 10
来源：http://ce.szsharing.cn

Scala .......... 10
来源：http://hy.hnjuh.cn

------------------------------------
来源：http://pk.lnxyls.cn

合计 ........... 2106 条
来源：http://ew.huanxung.cn

按章节统计：
来源：http://oh.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dh.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uz.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mf.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yb.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cu.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ln.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lf.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gs.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://el.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qj.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vy.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ga.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zc.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ef.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nl.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kt.hnjuh.cn

Q SQL 专题                              90
来源：http://hr.szxytkj.cn

R Bash 专题                             80
来源：http://cw.9csxet.cn

S C / C++ 专题                          60
来源：http://ru.lnxyls.cn

T 其他语言补充                          60
来源：http://hp.9csxet.cn

U 高频实用片段                         120
来源：http://gu.nszjky.cn

------------------------------------
来源：http://ae.chemitech.net.cn

合计                                  2106 条
来源：http://ox.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://dd.shtwfgs.cn

使用提醒
来源：http://hy.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://gi.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fk.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ly.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gn.huanxung.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uc.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jx.newstarts.cn

—— 文件结束 ——
来源：http://mm.panjiajie.cn

================================================================================
来源：http://rx.jianghongdianzi.cn

程序语言常见例子速查手册（2024 版）
来源：http://og.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://ae.bookmarksfly.cn

================================================================================
来源：http://px.chemitech.net.cn

【收录内容】
来源：http://gy.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://un.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ec.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://gt.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dq.szsharing.cn

【使用说明】
来源：http://oi.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mi.yuntaijiaju.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wf.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pu.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dd.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://iv.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jx.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lh.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xg.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rl.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://np.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bj.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vw.521024.cn

【文件统计】
来源：http://en.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://om.colortex.cn

--------------------------------------------------------------------------------
来源：http://bh.nszjky.cn

目  录
来源：http://fi.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://gm.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iv.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lh.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qt.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tv.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nl.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oc.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://br.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nc.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pz.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ft.shxzskj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sf.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://we.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rl.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tm.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oq.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fd.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://eg.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ti.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zy.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zn.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nv.hahajie.cn

================================================================================
来源：http://fv.nicolike.cn

A. 基础语法与类型
来源：http://zr.hnjuh.cn

================================================================================
来源：http://hw.shxzukj.cn

[A01] Hello World
来源：http://fm.colortex.cn

Py:   print("Hello, World!")
来源：http://hu.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://cl.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://uj.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gy.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://hp.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://ze.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://wt.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xz.nicolike.cn

[A02] 变量声明与赋值
来源：http://kh.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xp.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ny.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://px.panjiajie.cn


<!-- 参考信息 -->