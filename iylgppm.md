代发 wailian999

[U27] Py：异步 HTTP
来源：http://xi.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://lr.huanxung.cn

[U28] Py：类型别名
来源：http://zf.hahajie.cn

UserId = int
来源：http://tr.yuexingan06.cn

[U29] Py：属性校验
来源：http://bs.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://za.haigaiapp.cn

[U30] Py：数据类
来源：http://uw.huanxung.cn

@dataclass(slots=True)
来源：http://wk.haigaiapp.cn

[U31] Py：单测
来源：http://sa.nicolike.cn

python -m pytest -q
来源：http://xx.jctech888.com.cn

[U32] Py：代码格式化
来源：http://kl.9csxet.cn

ruff format . && ruff check --fix .
来源：http://us.shtwfgs.cn

[U33] Py：打包发布
来源：http://mq.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://gh.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://bn.jianghongdianzi.cn

chardet.detect(raw)
来源：http://mt.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://oh.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://or.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://rc.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://gq.shxzskj.cn

[U37] Py：读写 Excel
来源：http://uo.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jm.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://jk.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://op.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://eu.bjjhwx.cn

sys.stdout.isatty()
来源：http://lw.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://cu.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://co.shxzukj.cn

[U41] PHP：初始化 Composer 项目
来源：http://gb.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://il.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://bg.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ah.huanxung.cn

[U43] PHP：声明命名空间
来源：http://oi.huixiangedu.cn

namespace App\Http;
来源：http://xp.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://mx.newstarts.cn

declare(strict_types=1);
来源：http://zh.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://vq.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://be.521024.cn

[U46] PHP：可空类型
来源：http://qr.gzmigu.cn

?string $name = null
来源：http://bp.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://ba.huixiangedu.cn

int|string $id
来源：http://qg.shxzukj.cn

[U48] PHP：纯枚举
来源：http://ky.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ce.hahajie.cn

[U49] PHP：只读属性
来源：http://dl.haigaiapp.cn

public readonly string $name
来源：http://iv.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://is.nszjky.cn

public function __construct(private int $id) {}
来源：http://vr.hnjuh.cn

[U51] PHP：数组解构
来源：http://oz.szxytkj.cn

[$a, $b] = $arr;
来源：http://rj.521024.cn

[U52] PHP：箭头函数
来源：http://ql.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://ni.nszjky.cn

[U53] PHP：空合并运算符
来源：http://md.521024.cn

$v = $a ?? $b ?? "default";
来源：http://cs.panjiajie.cn

[U54] PHP：空安全调用
来源：http://ac.huixiangedu.cn

$obj?->method()
来源：http://tr.nicolike.cn

[U55] PHP：match 表达式
来源：http://ld.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ov.shxzukj.cn

[U56] PHP：命名参数
来源：http://fa.shxzukj.cn

f(a: 1, b: 2)
来源：http://mf.hnjuh.cn

[U57] PHP：字符串插值
来源：http://ga.chemitech.net.cn

"值: {$a}"
来源：http://iy.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://lx.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ex.9csxet.cn

[U59] PHP：自定义排序
来源：http://hq.gzmigu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wb.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://cw.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wn.jctech888.com.cn

[U61] PHP：正则
来源：http://ca.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://my.9csxet.cn

[U62] PHP：日期对象
来源：http://ip.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ci.szsharing.cn

[U63] PHP：文件读写
来源：http://fc.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yw.asd995.cn

[U64] PHP：目录遍历
来源：http://zp.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://db.yuexingan06.cn

[U65] PHP：会话
来源：http://dw.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aq.asd995.cn

[U66] PHP：设置 Cookie
来源：http://uy.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jf.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://hm.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bh.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://nb.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dj.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://dx.jctech888.com.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gu.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://sa.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uh.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://ik.521024.cn

throw new RuntimeException("失败", 500);
来源：http://ys.nicolike.cn

[U72] PHP：写错误日志
来源：http://oc.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://xs.jianghongdianzi.cn

[U73] PHP：读取 ini 配置
来源：http://ar.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://is.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://gq.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://wy.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://mk.lnxyls.cn

composer require psr/container
来源：http://gk.muxihuayi.cn

[U76] PHP：简单路由
来源：http://la.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pb.huanxung.cn

[U77] PHP：模板渲染
来源：http://pz.lnxyls.cn

composer require twig/twig
来源：http://uz.9csxet.cn

[U78] PHP：单元测试
来源：http://yy.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://kp.szsharing.cn

[U79] PHP：静态分析
来源：http://fx.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://it.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://yd.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qc.521024.cn

[U81] JS：初始化项目
来源：http://hb.hnjuh.cn

npm init -y;  npm i express
来源：http://yf.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://gp.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bl.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://fr.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kz.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://jk.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lq.szsharing.cn

[U85] JS：可选链
来源：http://gm.jianghongdianzi.cn

a?.b?.c
来源：http://mt.nicolike.cn

[U86] JS：空值合并
来源：http://mw.huixiangedu.cn

a ?? b
来源：http://zk.newstarts.cn

[U87] JS：解构默认值
来源：http://cl.hnjuh.cn

const { a = 1, b = 2 } = obj;
来源：http://qz.gzmigu.cn

[U88] JS：对象展开合并
来源：http://np.huixinmuqiang.cn

{ ...a, ...b }
来源：http://aw.gzmigu.cn

[U89] JS：数组去重
来源：http://ah.panjiajie.cn

[...new Set(arr)]
来源：http://bg.gzmigu.cn

[U90] JS：数字数组排序
来源：http://ds.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://ds.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://yx.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ne.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://di.yuexingan06.cn

structuredClone(obj)
来源：http://vc.chemitech.net.cn

[U93] JS：模板字符串
来源：http://tr.hnjuh.cn

`共 ${n} 条`
来源：http://nz.muxihuayi.cn

[U94] JS：箭头函数
来源：http://kd.bookmarksfly.cn

const double = x => x * 2;
来源：http://av.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://cl.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://mx.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://oq.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tb.chemitech.net.cn

[U97] JS：并发请求
来源：http://bb.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ed.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://rr.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cy.szxytkj.cn

[U99] JS：事件监听
来源：http://pk.hahajie.cn

el.addEventListener("click", e => {})
来源：http://yx.colortex.cn

[U100] JS：DOM 查询
来源：http://uq.hnjuh.cn

document.querySelector(".item")
来源：http://rh.gzmigu.cn

[U101] JS：classList 操作
来源：http://sb.jctech888.com.cn

el.classList.toggle("active")
来源：http://he.shtwfgs.cn

[U102] JS：本地存储
来源：http://cs.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sj.yuntaijiaju.cn

[U103] JS：定时器
来源：http://ic.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yk.jianghongdianzi.cn

[U104] JS：防抖
来源：http://cc.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hg.wgjwhj.cn

[U105] JS：节流
来源：http://pr.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jz.shxzukj.cn

[U106] JS：日期格式化
来源：http://cu.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kt.szxytkj.cn

[U107] JS：数字千分位
来源：http://hg.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zl.521024.cn

[U108] JS：随机整数
来源：http://ac.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kb.huixiangedu.cn

[U109] JS：数组分组
来源：http://cm.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://ik.haigaiapp.cn

[U110] JS：数组分块
来源：http://dc.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://df.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://fe.szsharing.cn

new Map(Object.entries(obj))
来源：http://jg.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://le.shtwfgs.cn

"7".padStart(3, "0")
来源：http://cz.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://zn.huanxung.cn

s.replaceAll("a", "b")
来源：http://ju.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://cv.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oj.colortex.cn

[U115] JS：生成 UUID
来源：http://fe.jctech888.com.cn

crypto.randomUUID()
来源：http://sj.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://dl.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://ff.yuexingan06.cn

[U117] JS：单元测试
来源：http://xm.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://zq.lnxyls.cn

[U118] JS：开发服务器
来源：http://rm.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://xs.szsharing.cn

[U119] JS：生产构建
来源：http://gq.huixiangedu.cn

npx vite build
来源：http://zl.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://ur.colortex.cn

import.meta.env.VITE_API_URL
来源：http://ed.nicolike.cn

================================================================================
来源：http://yp.newstarts.cn

统计汇总
来源：http://du.szxytkj.cn

================================================================================
来源：http://da.huixinmuqiang.cn

按语言统计（条）：
来源：http://nx.hnjuh.cn

Python ......... 252
来源：http://ga.hnjuh.cn

PHP ............ 252
来源：http://wl.newstarts.cn

JavaScript ..... 252
来源：http://om.wgjwhj.cn

TypeScript ..... 212
来源：http://ma.yuntaijiaju.cn

Java ........... 212
来源：http://ra.newstarts.cn

Go ............. 212
来源：http://yh.muxihuayi.cn

Ruby ........... 212
来源：http://ve.shxzukj.cn

C# ............. 212
来源：http://ty.haigaiapp.cn

C .............. 30
来源：http://fs.nszjky.cn

C++ ............ 30
来源：http://xd.shxzukj.cn

SQL ............ 90
来源：http://wz.yuexingan06.cn

Bash ........... 80
来源：http://wb.huanxung.cn

Kotlin ......... 15
来源：http://gx.shxzskj.cn

Swift .......... 15
来源：http://lo.hnjuh.cn

Lua ............ 10
来源：http://bh.szsharing.cn

Perl ........... 10
来源：http://db.lnxyls.cn

Scala .......... 10
来源：http://kv.colortex.cn

------------------------------------
来源：http://bp.521024.cn

合计 ........... 2106 条
来源：http://gr.huixinmuqiang.cn

按章节统计：
来源：http://nw.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ez.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hx.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ww.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qj.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://se.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://am.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fd.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://we.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sp.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mf.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eu.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ev.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zk.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wu.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ht.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xj.muxihuayi.cn

Q SQL 专题                              90
来源：http://ly.huanxung.cn

R Bash 专题                             80
来源：http://ut.9csxet.cn

S C / C++ 专题                          60
来源：http://ut.nicolike.cn

T 其他语言补充                          60
来源：http://fj.newstarts.cn

U 高频实用片段                         120
来源：http://tt.bjjhwx.cn

------------------------------------
来源：http://ih.hahajie.cn

合计                                  2106 条
来源：http://dq.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://jg.asd995.cn

使用提醒
来源：http://gk.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://xb.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://va.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://id.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zg.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mv.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ph.gzmigu.cn

—— 文件结束 ——
来源：http://vv.hahajie.cn

================================================================================
来源：http://zl.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://hk.hahajie.cn

Common Programming Examples Cheat Book
来源：http://qw.bjjhwx.cn

================================================================================
来源：http://dn.colortex.cn

【收录内容】
来源：http://ll.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sx.9csxet.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lf.shxzukj.cn

SQL · Bash · C · C++
来源：http://ew.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qk.haigaiapp.cn

【使用说明】
来源：http://ru.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tc.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hg.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ij.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pq.asd995.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lr.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wd.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lz.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://re.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mi.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jt.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ss.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rd.shtwfgs.cn

【文件统计】
来源：http://fr.jctech888.com.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lt.9csxet.cn

--------------------------------------------------------------------------------
来源：http://xi.hnjuh.cn

目  录
来源：http://wb.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://am.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fl.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ke.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yj.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wi.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vg.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oj.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wb.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xe.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yi.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vn.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://te.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vo.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ek.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://um.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mn.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rn.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oz.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qu.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yv.jctech888.com.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sa.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qj.jianghongdianzi.cn

================================================================================
来源：http://dk.szsharing.cn

A. 基础语法与类型
来源：http://bx.hnjuh.cn

================================================================================
来源：http://xb.hnjuh.cn

[A01] Hello World
来源：http://ot.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://cm.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://eo.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://kt.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wj.shxzskj.cn


<!-- 参考信息 -->