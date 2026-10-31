代发 wailian999

[U27] Py：异步 HTTP
来源：http://rz.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://ia.haigaiapp.cn

[U28] Py：类型别名
来源：http://us.lnxyls.cn

UserId = int
来源：http://rw.shxzukj.cn

[U29] Py：属性校验
来源：http://rf.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://co.huanxung.cn

[U30] Py：数据类
来源：http://rb.jctech888.com.cn

@dataclass(slots=True)
来源：http://ps.yuexingan06.cn

[U31] Py：单测
来源：http://th.newstarts.cn

python -m pytest -q
来源：http://do.nicolike.cn

[U32] Py：代码格式化
来源：http://xn.newstarts.cn

ruff format . && ruff check --fix .
来源：http://aw.colortex.cn

[U33] Py：打包发布
来源：http://qp.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://be.szsharing.cn

[U34] Py：判断编码
来源：http://bm.yuexingan06.cn

chardet.detect(raw)
来源：http://oi.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://vv.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zx.hnjuh.cn

[U36] Py：定时任务
来源：http://ya.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://qh.szxytkj.cn

[U37] Py：读写 Excel
来源：http://rb.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mx.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://rk.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://ze.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://oo.newstarts.cn

sys.stdout.isatty()
来源：http://kn.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://ty.huanxung.cn

print("err", file=sys.stderr)
来源：http://jt.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://hx.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qz.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://pm.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nd.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://ud.nszjky.cn

namespace App\Http;
来源：http://xo.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://rz.szsharing.cn

declare(strict_types=1);
来源：http://bk.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://po.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lp.hnjuh.cn

[U46] PHP：可空类型
来源：http://cx.huanxung.cn

?string $name = null
来源：http://dt.shxzskj.cn

[U47] PHP：联合类型
来源：http://pr.wgjwhj.cn

int|string $id
来源：http://zb.521024.cn

[U48] PHP：纯枚举
来源：http://re.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yp.szsharing.cn

[U49] PHP：只读属性
来源：http://gn.newstarts.cn

public readonly string $name
来源：http://ct.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://yy.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://os.lnxyls.cn

[U51] PHP：数组解构
来源：http://yx.colortex.cn

[$a, $b] = $arr;
来源：http://hv.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://pk.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://nq.newstarts.cn

[U53] PHP：空合并运算符
来源：http://vd.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://nu.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://jr.hahajie.cn

$obj?->method()
来源：http://zs.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://lb.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ov.panjiajie.cn

[U56] PHP：命名参数
来源：http://sx.huixiangedu.cn

f(a: 1, b: 2)
来源：http://ci.asd995.cn

[U57] PHP：字符串插值
来源：http://wl.bookmarksfly.cn

"值: {$a}"
来源：http://st.nicolike.cn

[U58] PHP：数组三件套
来源：http://ea.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hp.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://pf.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tz.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://zc.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ou.jctech888.com.cn

[U61] PHP：正则
来源：http://cq.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iq.colortex.cn

[U62] PHP：日期对象
来源：http://qk.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ek.hnjuh.cn

[U63] PHP：文件读写
来源：http://cp.huixiangedu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zz.szsharing.cn

[U64] PHP：目录遍历
来源：http://lw.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://xh.chemitech.net.cn

[U65] PHP：会话
来源：http://ls.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://us.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://ds.yuntaijiaju.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://at.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://on.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rc.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://bw.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lo.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://qc.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zu.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://az.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kf.nszjky.cn

[U71] PHP：抛出异常
来源：http://oa.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://zg.newstarts.cn

[U72] PHP：写错误日志
来源：http://ab.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://hl.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://hs.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://gn.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://dl.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://ds.lnxyls.cn

[U75] PHP：依赖注入
来源：http://ej.huixinmuqiang.cn

composer require psr/container
来源：http://dx.asd995.cn

[U76] PHP：简单路由
来源：http://gj.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ib.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://fr.panjiajie.cn

composer require twig/twig
来源：http://lh.shxzskj.cn

[U78] PHP：单元测试
来源：http://bq.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://bj.yuexingan06.cn

[U79] PHP：静态分析
来源：http://nt.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://hs.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://mr.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lh.wgjwhj.cn

[U81] JS：初始化项目
来源：http://uu.hnjuh.cn

npm init -y;  npm i express
来源：http://ns.szsharing.cn

[U82] JS：package.json 脚本
来源：http://mx.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lq.521024.cn

[U83] JS：ES Module 导入导出
来源：http://on.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gc.wgjwhj.cn

[U84] JS：CommonJS 写法
来源：http://ld.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sp.hahajie.cn

[U85] JS：可选链
来源：http://op.jctech888.com.cn

a?.b?.c
来源：http://bp.9csxet.cn

[U86] JS：空值合并
来源：http://cx.shtwfgs.cn

a ?? b
来源：http://mh.9csxet.cn

[U87] JS：解构默认值
来源：http://ay.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://mw.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://hl.newstarts.cn

{ ...a, ...b }
来源：http://aj.szxytkj.cn

[U89] JS：数组去重
来源：http://xn.asd995.cn

[...new Set(arr)]
来源：http://ug.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://qt.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://oh.hahajie.cn

[U91] JS：对象键值遍历
来源：http://iu.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hr.colortex.cn

[U92] JS：深拷贝
来源：http://xf.szsharing.cn

structuredClone(obj)
来源：http://lp.muxihuayi.cn

[U93] JS：模板字符串
来源：http://co.yuntaijiaju.cn

`共 ${n} 条`
来源：http://yd.panjiajie.cn

[U94] JS：箭头函数
来源：http://no.shxzukj.cn

const double = x => x * 2;
来源：http://sb.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://ze.asd995.cn

new Promise((resolve, reject) => {})
来源：http://ew.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://zn.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fb.huanxung.cn

[U97] JS：并发请求
来源：http://ya.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iz.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://ed.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gs.jctech888.com.cn

[U99] JS：事件监听
来源：http://ew.lnxyls.cn

el.addEventListener("click", e => {})
来源：http://do.lnxyls.cn

[U100] JS：DOM 查询
来源：http://ro.shtwfgs.cn

document.querySelector(".item")
来源：http://qg.muxihuayi.cn

[U101] JS：classList 操作
来源：http://we.hahajie.cn

el.classList.toggle("active")
来源：http://kn.jctech888.com.cn

[U102] JS：本地存储
来源：http://us.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qd.bookmarksfly.cn

[U103] JS：定时器
来源：http://wx.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nu.bookmarksfly.cn

[U104] JS：防抖
来源：http://bj.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xw.chemitech.net.cn

[U105] JS：节流
来源：http://mh.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xc.gzmigu.cn

[U106] JS：日期格式化
来源：http://fy.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wd.szxytkj.cn

[U107] JS：数字千分位
来源：http://lf.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vp.gzmigu.cn

[U108] JS：随机整数
来源：http://qg.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sg.jctech888.com.cn

[U109] JS：数组分组
来源：http://rm.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://ct.nszjky.cn

[U110] JS：数组分块
来源：http://yk.chemitech.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pn.shxzskj.cn

[U111] JS：对象转 Map
来源：http://go.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://kt.asd995.cn

[U112] JS：字符串补位
来源：http://cc.nicolike.cn

"7".padStart(3, "0")
来源：http://mf.hnjuh.cn

[U113] JS：正则替换全部
来源：http://zw.shxzukj.cn

s.replaceAll("a", "b")
来源：http://or.colortex.cn

[U114] JS：JSON 深比较
来源：http://xx.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ad.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://ud.shtwfgs.cn

crypto.randomUUID()
来源：http://bn.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://gk.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://cf.huanxung.cn

[U117] JS：单元测试
来源：http://ya.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://vf.asd995.cn

[U118] JS：开发服务器
来源：http://rx.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://cb.asd995.cn

[U119] JS：生产构建
来源：http://ba.jianghongdianzi.cn

npx vite build
来源：http://vf.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://nz.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://es.nszjky.cn

================================================================================
来源：http://wy.jctech888.com.cn

统计汇总
来源：http://mx.newstarts.cn

================================================================================
来源：http://dd.huixinmuqiang.cn

按语言统计（条）：
来源：http://sd.colortex.cn

Python ......... 252
来源：http://fx.szsharing.cn

PHP ............ 252
来源：http://cg.colortex.cn

JavaScript ..... 252
来源：http://hv.hahajie.cn

TypeScript ..... 212
来源：http://jq.szsharing.cn

Java ........... 212
来源：http://po.szsharing.cn

Go ............. 212
来源：http://ag.asd995.cn

Ruby ........... 212
来源：http://ki.9csxet.cn

C# ............. 212
来源：http://dy.szxytkj.cn

C .............. 30
来源：http://ej.haigaiapp.cn

C++ ............ 30
来源：http://br.521024.cn

SQL ............ 90
来源：http://qc.nicolike.cn

Bash ........... 80
来源：http://vl.wgjwhj.cn

Kotlin ......... 15
来源：http://es.szxytkj.cn

Swift .......... 15
来源：http://az.huixinmuqiang.cn

Lua ............ 10
来源：http://kc.shxzskj.cn

Perl ........... 10
来源：http://bm.haigaiapp.cn

Scala .......... 10
来源：http://cd.newstarts.cn

------------------------------------
来源：http://kx.hnjuh.cn

合计 ........... 2106 条
来源：http://za.huixiangedu.cn

按章节统计：
来源：http://rg.newstarts.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mz.9csxet.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rv.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jl.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oe.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qx.colortex.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yd.bjjhwx.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sk.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kj.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fh.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ct.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ok.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zt.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oo.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lu.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bq.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gq.bookmarksfly.cn

Q SQL 专题                              90
来源：http://um.shtwfgs.cn

R Bash 专题                             80
来源：http://lk.shxzukj.cn

S C / C++ 专题                          60
来源：http://hu.gzmigu.cn

T 其他语言补充                          60
来源：http://pr.hnjuh.cn

U 高频实用片段                         120
来源：http://ff.gzmigu.cn

------------------------------------
来源：http://ci.szsharing.cn

合计                                  2106 条
来源：http://gy.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ng.haigaiapp.cn

使用提醒
来源：http://kd.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://la.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tz.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mc.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kl.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wn.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ed.yuexingan06.cn

—— 文件结束 ——
来源：http://iq.shxzskj.cn

================================================================================
来源：http://oz.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://lk.hahajie.cn

Common Programming Examples Cheat Book
来源：http://ek.panjiajie.cn

================================================================================
来源：http://lc.szxytkj.cn

【收录内容】
来源：http://ke.hnjuh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ab.wgjwhj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://de.lnxyls.cn

SQL · Bash · C · C++
来源：http://jt.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tn.huixinmuqiang.cn

【使用说明】
来源：http://mz.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://aw.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nl.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iy.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qu.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://do.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oa.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vh.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://en.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://un.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zv.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://er.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wf.haigaiapp.cn

【文件统计】
来源：http://ls.huanxung.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cc.nicolike.cn

--------------------------------------------------------------------------------
来源：http://ls.gzmigu.cn

目  录
来源：http://ae.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://ab.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ej.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ip.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qq.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wd.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ga.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pf.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lx.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zl.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ex.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sf.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://om.shxzskj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qk.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pp.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://br.hnjuh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ct.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sw.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cj.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uf.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kh.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bb.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qt.jianghongdianzi.cn

================================================================================
来源：http://aa.colortex.cn

A. 基础语法与类型
来源：http://tu.yuntaijiaju.cn

================================================================================
来源：http://av.huixinmuqiang.cn

[A01] Hello World
来源：http://ec.nicolike.cn

Py:   print("Hello, World!")
来源：http://df.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://bg.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://re.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aj.bookmarksfly.cn


<!-- 参考信息 -->