代发 wailian999

[U31] Py：单测
来源：http://pu.jianghongdianzi.cn

python -m pytest -q
来源：http://dn.hahajie.cn

[U32] Py：代码格式化
来源：http://oj.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://dc.9csxet.cn

[U33] Py：打包发布
来源：http://uq.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://gh.shtwfgs.cn

[U34] Py：判断编码
来源：http://ee.wgjwhj.cn

chardet.detect(raw)
来源：http://lf.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://ad.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://df.shxzskj.cn

[U36] Py：定时任务
来源：http://nq.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://jq.shxzskj.cn

[U37] Py：读写 Excel
来源：http://gd.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gx.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://fo.nszjky.cn

Path(__file__).resolve().parent
来源：http://vw.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://si.nicolike.cn

sys.stdout.isatty()
来源：http://gk.colortex.cn

[U40] Py：打印到标准错误
来源：http://yc.panjiajie.cn

print("err", file=sys.stderr)
来源：http://zf.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://ly.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rh.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://ai.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ip.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://tt.chemitech.net.cn

namespace App\Http;
来源：http://lj.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://ox.lnxyls.cn

declare(strict_types=1);
来源：http://oi.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://ei.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ge.gzmigu.cn

[U46] PHP：可空类型
来源：http://jt.yuexingan06.cn

?string $name = null
来源：http://jf.huixiangedu.cn

[U47] PHP：联合类型
来源：http://wu.lnxyls.cn

int|string $id
来源：http://pl.lnxyls.cn

[U48] PHP：纯枚举
来源：http://kw.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yu.521024.cn

[U49] PHP：只读属性
来源：http://qe.huixiangedu.cn

public readonly string $name
来源：http://cu.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://rg.colortex.cn

public function __construct(private int $id) {}
来源：http://pl.szxytkj.cn

[U51] PHP：数组解构
来源：http://we.szsharing.cn

[$a, $b] = $arr;
来源：http://nn.9csxet.cn

[U52] PHP：箭头函数
来源：http://ib.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://lh.bjjhwx.cn

[U53] PHP：空合并运算符
来源：http://qd.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://pf.panjiajie.cn

[U54] PHP：空安全调用
来源：http://zl.newstarts.cn

$obj?->method()
来源：http://xg.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://ck.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pj.lnxyls.cn

[U56] PHP：命名参数
来源：http://az.huixiangedu.cn

f(a: 1, b: 2)
来源：http://rp.bjjhwx.cn

[U57] PHP：字符串插值
来源：http://lt.shtwfgs.cn

"值: {$a}"
来源：http://dc.colortex.cn

[U58] PHP：数组三件套
来源：http://ur.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yk.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://uw.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://do.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://eo.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ji.lnxyls.cn

[U61] PHP：正则
来源：http://sy.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ba.9csxet.cn

[U62] PHP：日期对象
来源：http://hl.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hh.panjiajie.cn

[U63] PHP：文件读写
来源：http://ut.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ib.hahajie.cn

[U64] PHP：目录遍历
来源：http://gj.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://md.szxytkj.cn

[U65] PHP：会话
来源：http://fo.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://js.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://od.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tn.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://xh.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sw.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://bs.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://do.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://rk.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yf.huanxung.cn

[U70] PHP：PDO 事务
来源：http://ph.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ug.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://zb.shtwfgs.cn

throw new RuntimeException("失败", 500);
来源：http://ip.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://he.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://lg.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://zh.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://ie.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://xv.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://kf.nszjky.cn

[U75] PHP：依赖注入
来源：http://tw.shxzukj.cn

composer require psr/container
来源：http://tg.szxytkj.cn

[U76] PHP：简单路由
来源：http://id.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wt.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://lr.shxzskj.cn

composer require twig/twig
来源：http://lk.bjjhwx.cn

[U78] PHP：单元测试
来源：http://by.asd995.cn

composer require --dev phpunit/phpunit
来源：http://ly.huixiangedu.cn

[U79] PHP：静态分析
来源：http://rk.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://dr.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://ay.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qt.yuntaijiaju.cn

[U81] JS：初始化项目
来源：http://gi.panjiajie.cn

npm init -y;  npm i express
来源：http://hm.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://hm.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ok.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://sl.shxzukj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ia.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://kf.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hn.asd995.cn

[U85] JS：可选链
来源：http://oj.521024.cn

a?.b?.c
来源：http://ty.szxytkj.cn

[U86] JS：空值合并
来源：http://ij.bookmarksfly.cn

a ?? b
来源：http://vh.newstarts.cn

[U87] JS：解构默认值
来源：http://mp.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://jc.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://pk.wgjwhj.cn

{ ...a, ...b }
来源：http://ty.nszjky.cn

[U89] JS：数组去重
来源：http://hr.szsharing.cn

[...new Set(arr)]
来源：http://hk.panjiajie.cn

[U90] JS：数字数组排序
来源：http://xy.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://hk.nszjky.cn

[U91] JS：对象键值遍历
来源：http://wf.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pd.chemitech.net.cn

[U92] JS：深拷贝
来源：http://pn.jctech888.com.cn

structuredClone(obj)
来源：http://nr.huixiangedu.cn

[U93] JS：模板字符串
来源：http://ey.huanxung.cn

`共 ${n} 条`
来源：http://vm.haigaiapp.cn

[U94] JS：箭头函数
来源：http://ac.colortex.cn

const double = x => x * 2;
来源：http://dt.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://ch.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://iv.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://uj.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zc.newstarts.cn

[U97] JS：并发请求
来源：http://ro.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wq.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://to.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oo.bjjhwx.cn

[U99] JS：事件监听
来源：http://rk.9csxet.cn

el.addEventListener("click", e => {})
来源：http://bv.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://jq.bookmarksfly.cn

document.querySelector(".item")
来源：http://xl.haigaiapp.cn

[U101] JS：classList 操作
来源：http://hh.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://np.newstarts.cn

[U102] JS：本地存储
来源：http://or.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://an.jctech888.com.cn

[U103] JS：定时器
来源：http://nv.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pp.asd995.cn

[U104] JS：防抖
来源：http://sz.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ei.asd995.cn

[U105] JS：节流
来源：http://hu.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mf.jctech888.com.cn

[U106] JS：日期格式化
来源：http://ql.nicolike.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ty.nicolike.cn

[U107] JS：数字千分位
来源：http://yd.wgjwhj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vf.chemitech.net.cn

[U108] JS：随机整数
来源：http://ph.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pm.huixiangedu.cn

[U109] JS：数组分组
来源：http://ar.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://lh.colortex.cn

[U110] JS：数组分块
来源：http://qm.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://or.asd995.cn

[U111] JS：对象转 Map
来源：http://xk.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://mv.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://db.muxihuayi.cn

"7".padStart(3, "0")
来源：http://tj.szsharing.cn

[U113] JS：正则替换全部
来源：http://vt.szxytkj.cn

s.replaceAll("a", "b")
来源：http://wo.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://dc.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://da.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://gs.szsharing.cn

crypto.randomUUID()
来源：http://zz.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://vw.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://ns.szsharing.cn

[U117] JS：单元测试
来源：http://aw.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://wv.wgjwhj.cn

[U118] JS：开发服务器
来源：http://hf.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://vw.shxzukj.cn

[U119] JS：生产构建
来源：http://db.jianghongdianzi.cn

npx vite build
来源：http://lc.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://ly.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://gu.shxzukj.cn

================================================================================
来源：http://fr.szxytkj.cn

统计汇总
来源：http://on.nszjky.cn

================================================================================
来源：http://qo.colortex.cn

按语言统计（条）：
来源：http://jb.yuntaijiaju.cn

Python ......... 252
来源：http://cd.panjiajie.cn

PHP ............ 252
来源：http://xw.nicolike.cn

JavaScript ..... 252
来源：http://zn.huixinmuqiang.cn

TypeScript ..... 212
来源：http://tp.jctech888.com.cn

Java ........... 212
来源：http://ef.hahajie.cn

Go ............. 212
来源：http://rf.nszjky.cn

Ruby ........... 212
来源：http://pm.bjjhwx.cn

C# ............. 212
来源：http://fl.nszjky.cn

C .............. 30
来源：http://ja.gzmigu.cn

C++ ............ 30
来源：http://wc.newstarts.cn

SQL ............ 90
来源：http://pd.haigaiapp.cn

Bash ........... 80
来源：http://db.muxihuayi.cn

Kotlin ......... 15
来源：http://do.jianghongdianzi.cn

Swift .......... 15
来源：http://nd.colortex.cn

Lua ............ 10
来源：http://lm.newstarts.cn

Perl ........... 10
来源：http://qh.huanxung.cn

Scala .......... 10
来源：http://ax.szsharing.cn

------------------------------------
来源：http://nv.nicolike.cn

合计 ........... 2106 条
来源：http://ys.hnjuh.cn

按章节统计：
来源：http://nn.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ji.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ts.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ul.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sm.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uj.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yn.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ea.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wc.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jy.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wx.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xr.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ja.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ht.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://de.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bk.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hm.muxihuayi.cn

Q SQL 专题                              90
来源：http://ww.huixinmuqiang.cn

R Bash 专题                             80
来源：http://cj.521024.cn

S C / C++ 专题                          60
来源：http://jj.szsharing.cn

T 其他语言补充                          60
来源：http://bb.szxytkj.cn

U 高频实用片段                         120
来源：http://ec.chemitech.net.cn

------------------------------------
来源：http://ru.newstarts.cn

合计                                  2106 条
来源：http://vx.521024.cn

--------------------------------------------------------------------------------
来源：http://qr.panjiajie.cn

使用提醒
来源：http://gu.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://zi.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qh.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lx.jctech888.com.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bv.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://da.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xv.chemitech.net.cn

—— 文件结束 ——
来源：http://kb.panjiajie.cn

================================================================================
来源：http://sr.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://my.bjjhwx.cn

Common Programming Examples Cheat Book
来源：http://yz.bookmarksfly.cn

================================================================================
来源：http://fk.nicolike.cn

【收录内容】
来源：http://lo.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iu.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ga.nszjky.cn

SQL · Bash · C · C++
来源：http://hz.521024.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://db.lnxyls.cn

【使用说明】
来源：http://lg.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gu.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gj.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://se.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zb.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lm.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ez.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kr.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cw.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tb.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zq.huanxung.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kr.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vn.jianghongdianzi.cn

【文件统计】
来源：http://gv.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wy.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://dm.shtwfgs.cn

目  录
来源：http://np.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://py.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ok.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kw.gzmigu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ql.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ok.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://db.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hj.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kl.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yj.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wj.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ni.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ms.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jt.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gu.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wc.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mv.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fd.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dy.huixiangedu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wd.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oh.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gy.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vb.muxihuayi.cn

================================================================================
来源：http://ug.521024.cn

A. 基础语法与类型
来源：http://oa.panjiajie.cn

================================================================================
来源：http://rk.szsharing.cn

[A01] Hello World
来源：http://tt.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://jc.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://lq.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://cz.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ps.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://eo.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://sj.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://ga.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://eo.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://ub.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kq.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ph.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sl.shtwfgs.cn


<!-- 参考信息 -->