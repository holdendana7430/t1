代发 wailian999

[U25] Py：CSV 按字典读
来源：http://kh.asd995.cn

csv.DictReader(f)
来源：http://tn.nicolike.cn

[U26] Py：并发下载
来源：http://fx.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ev.nicolike.cn

[U27] Py：异步 HTTP
来源：http://pg.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://bp.jctech888.com.cn

[U28] Py：类型别名
来源：http://vq.shxzukj.cn

UserId = int
来源：http://ne.bjjhwx.cn

[U29] Py：属性校验
来源：http://eq.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://ur.haigaiapp.cn

[U30] Py：数据类
来源：http://hk.521024.cn

@dataclass(slots=True)
来源：http://rd.bjjhwx.cn

[U31] Py：单测
来源：http://gf.szsharing.cn

python -m pytest -q
来源：http://zb.gzmigu.cn

[U32] Py：代码格式化
来源：http://rv.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://rz.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://tg.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://gf.shxzukj.cn

[U34] Py：判断编码
来源：http://tx.hahajie.cn

chardet.detect(raw)
来源：http://pn.hahajie.cn

[U35] Py：发送邮件
来源：http://iy.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pm.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://ln.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://yx.nicolike.cn

[U37] Py：读写 Excel
来源：http://nt.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wb.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://qh.huixiangedu.cn

Path(__file__).resolve().parent
来源：http://it.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://vy.nszjky.cn

sys.stdout.isatty()
来源：http://lc.asd995.cn

[U40] Py：打印到标准错误
来源：http://ko.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://iw.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://fv.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mk.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://gu.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://am.521024.cn

[U43] PHP：声明命名空间
来源：http://he.bjjhwx.cn

namespace App\Http;
来源：http://kh.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://ft.jianghongdianzi.cn

declare(strict_types=1);
来源：http://vw.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://eq.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pc.shxzukj.cn

[U46] PHP：可空类型
来源：http://fd.wgjwhj.cn

?string $name = null
来源：http://km.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://ns.szxytkj.cn

int|string $id
来源：http://hx.shxzukj.cn

[U48] PHP：纯枚举
来源：http://hu.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://go.szsharing.cn

[U49] PHP：只读属性
来源：http://gv.jianghongdianzi.cn

public readonly string $name
来源：http://mk.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://fc.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://xg.huanxung.cn

[U51] PHP：数组解构
来源：http://dg.panjiajie.cn

[$a, $b] = $arr;
来源：http://ws.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://ws.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://gu.muxihuayi.cn

[U53] PHP：空合并运算符
来源：http://vn.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://jz.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://uw.bjjhwx.cn

$obj?->method()
来源：http://ra.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://cl.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://du.nszjky.cn

[U56] PHP：命名参数
来源：http://ya.shxzukj.cn

f(a: 1, b: 2)
来源：http://qx.huanxung.cn

[U57] PHP：字符串插值
来源：http://ht.hahajie.cn

"值: {$a}"
来源：http://kg.nicolike.cn

[U58] PHP：数组三件套
来源：http://nl.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ky.hahajie.cn

[U59] PHP：自定义排序
来源：http://ga.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jd.hahajie.cn

[U60] PHP：JSON 编解码
来源：http://ai.panjiajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://al.huanxung.cn

[U61] PHP：正则
来源：http://gb.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mt.nszjky.cn

[U62] PHP：日期对象
来源：http://ji.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mw.nszjky.cn

[U63] PHP：文件读写
来源：http://qk.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bv.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://im.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://oj.huixiangedu.cn

[U65] PHP：会话
来源：http://tw.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ep.bookmarksfly.cn

[U66] PHP：设置 Cookie
来源：http://om.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ef.nicolike.cn

[U67] PHP：处理文件上传
来源：http://pm.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ad.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://qq.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zg.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://ia.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iq.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://bi.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fw.bjjhwx.cn

[U71] PHP：抛出异常
来源：http://jb.521024.cn

throw new RuntimeException("失败", 500);
来源：http://qc.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://ay.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://my.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://jo.haigaiapp.cn

parse_ini_file("config.ini", true)
来源：http://ua.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://pb.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://rr.szsharing.cn

[U75] PHP：依赖注入
来源：http://xr.jctech888.com.cn

composer require psr/container
来源：http://cs.yuexingan06.cn

[U76] PHP：简单路由
来源：http://jd.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ay.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://dn.bjjhwx.cn

composer require twig/twig
来源：http://qy.huixiangedu.cn

[U78] PHP：单元测试
来源：http://kr.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://bc.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://sd.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://lk.9csxet.cn

[U80] PHP：代码规范修复
来源：http://zj.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lc.panjiajie.cn

[U81] JS：初始化项目
来源：http://nj.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://nh.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://km.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ey.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://dh.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lg.nszjky.cn

[U84] JS：CommonJS 写法
来源：http://oj.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ru.haigaiapp.cn

[U85] JS：可选链
来源：http://av.haigaiapp.cn

a?.b?.c
来源：http://fz.lnxyls.cn

[U86] JS：空值合并
来源：http://iz.yuexingan06.cn

a ?? b
来源：http://xh.shxzukj.cn

[U87] JS：解构默认值
来源：http://qt.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://cd.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://lo.gzmigu.cn

{ ...a, ...b }
来源：http://ud.nszjky.cn

[U89] JS：数组去重
来源：http://gr.panjiajie.cn

[...new Set(arr)]
来源：http://zp.521024.cn

[U90] JS：数字数组排序
来源：http://rt.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://ew.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://rx.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mc.hahajie.cn

[U92] JS：深拷贝
来源：http://hg.szsharing.cn

structuredClone(obj)
来源：http://de.haigaiapp.cn

[U93] JS：模板字符串
来源：http://kd.huixinmuqiang.cn

`共 ${n} 条`
来源：http://nh.521024.cn

[U94] JS：箭头函数
来源：http://fq.chemitech.net.cn

const double = x => x * 2;
来源：http://ev.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://za.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://eq.nszjky.cn

[U96] JS：async/await 与异常
来源：http://tk.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://th.bjjhwx.cn

[U97] JS：并发请求
来源：http://jy.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://co.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://zb.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ny.lnxyls.cn

[U99] JS：事件监听
来源：http://lw.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://cj.panjiajie.cn

[U100] JS：DOM 查询
来源：http://tz.521024.cn

document.querySelector(".item")
来源：http://pe.muxihuayi.cn

[U101] JS：classList 操作
来源：http://sa.wgjwhj.cn

el.classList.toggle("active")
来源：http://af.haigaiapp.cn

[U102] JS：本地存储
来源：http://hx.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gi.szsharing.cn

[U103] JS：定时器
来源：http://to.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eh.shxzskj.cn

[U104] JS：防抖
来源：http://fw.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ry.panjiajie.cn

[U105] JS：节流
来源：http://rt.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wd.huanxung.cn

[U106] JS：日期格式化
来源：http://wu.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wb.shxzskj.cn

[U107] JS：数字千分位
来源：http://hv.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://id.hnjuh.cn

[U108] JS：随机整数
来源：http://ge.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ku.hnjuh.cn

[U109] JS：数组分组
来源：http://zi.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://uc.gzmigu.cn

[U110] JS：数组分块
来源：http://bj.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fj.hahajie.cn

[U111] JS：对象转 Map
来源：http://wq.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://md.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://or.hahajie.cn

"7".padStart(3, "0")
来源：http://pl.lnxyls.cn

[U113] JS：正则替换全部
来源：http://ku.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://bl.asd995.cn

[U114] JS：JSON 深比较
来源：http://ut.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ls.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://wi.huixinmuqiang.cn

crypto.randomUUID()
来源：http://ps.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://sj.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://fx.nicolike.cn

[U117] JS：单元测试
来源：http://az.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://qp.chemitech.net.cn

[U118] JS：开发服务器
来源：http://pn.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://fo.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://vq.9csxet.cn

npx vite build
来源：http://ik.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://yu.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://zd.colortex.cn

================================================================================
来源：http://hg.yuexingan06.cn

统计汇总
来源：http://yr.szsharing.cn

================================================================================
来源：http://hk.bjjhwx.cn

按语言统计（条）：
来源：http://ri.yuexingan06.cn

Python ......... 252
来源：http://jz.hahajie.cn

PHP ............ 252
来源：http://ev.nszjky.cn

JavaScript ..... 252
来源：http://ds.nszjky.cn

TypeScript ..... 212
来源：http://ql.muxihuayi.cn

Java ........... 212
来源：http://gu.jianghongdianzi.cn

Go ............. 212
来源：http://cj.shtwfgs.cn

Ruby ........... 212
来源：http://xr.huanxung.cn

C# ............. 212
来源：http://yu.gzmigu.cn

C .............. 30
来源：http://el.shxzukj.cn

C++ ............ 30
来源：http://zz.lnxyls.cn

SQL ............ 90
来源：http://pl.huixinmuqiang.cn

Bash ........... 80
来源：http://id.newstarts.cn

Kotlin ......... 15
来源：http://xp.huixinmuqiang.cn

Swift .......... 15
来源：http://jg.wgjwhj.cn

Lua ............ 10
来源：http://mm.panjiajie.cn

Perl ........... 10
来源：http://ky.9csxet.cn

Scala .......... 10
来源：http://oi.huanxung.cn

------------------------------------
来源：http://ja.colortex.cn

合计 ........... 2106 条
来源：http://zk.szsharing.cn

按章节统计：
来源：http://qu.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xl.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ne.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lc.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tv.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hy.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mb.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sl.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nv.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://py.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lf.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ba.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rv.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wx.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://df.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ot.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pk.szsharing.cn

Q SQL 专题                              90
来源：http://lg.bjjhwx.cn

R Bash 专题                             80
来源：http://ay.shxzukj.cn

S C / C++ 专题                          60
来源：http://xw.wgjwhj.cn

T 其他语言补充                          60
来源：http://oo.szsharing.cn

U 高频实用片段                         120
来源：http://fy.bjjhwx.cn

------------------------------------
来源：http://hg.huixiangedu.cn

合计                                  2106 条
来源：http://xo.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://lb.yuntaijiaju.cn

使用提醒
来源：http://ur.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://uw.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://em.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jh.huanxung.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jz.yuexingan06.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uw.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xk.shxzukj.cn

—— 文件结束 ——
来源：http://aw.wgjwhj.cn

================================================================================
来源：http://gd.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://bl.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://rh.hnjuh.cn

================================================================================
来源：http://kz.nszjky.cn

【收录内容】
来源：http://ef.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qw.yuntaijiaju.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ms.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://lp.nicolike.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://os.szsharing.cn

【使用说明】
来源：http://sk.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yc.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ng.huixinmuqiang.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qz.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gd.asd995.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kl.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zn.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://am.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ba.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kr.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sr.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cv.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qq.bjjhwx.cn

【文件统计】
来源：http://yd.szsharing.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mi.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://rk.shtwfgs.cn

目  录
来源：http://gh.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://pu.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yb.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mc.jctech888.com.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oq.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lf.jianghongdianzi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cc.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gt.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://in.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wl.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ev.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ix.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nf.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iv.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mw.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eg.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iu.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kq.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wv.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mg.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://of.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rt.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bt.asd995.cn

================================================================================
来源：http://mw.gzmigu.cn

A. 基础语法与类型
来源：http://xk.muxihuayi.cn

================================================================================
来源：http://pl.9csxet.cn

[A01] Hello World
来源：http://es.bjjhwx.cn


<!-- 参考信息 -->