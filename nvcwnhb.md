代发 wailian999

[U27] Py：异步 HTTP
来源：http://kk.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://hg.haigaiapp.cn

[U28] Py：类型别名
来源：http://bs.521024.cn

UserId = int
来源：http://ga.haigaiapp.cn

[U29] Py：属性校验
来源：http://if.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://wj.bookmarksfly.cn

[U30] Py：数据类
来源：http://if.panjiajie.cn

@dataclass(slots=True)
来源：http://uh.panjiajie.cn

[U31] Py：单测
来源：http://yv.szxytkj.cn

python -m pytest -q
来源：http://rq.muxihuayi.cn

[U32] Py：代码格式化
来源：http://gr.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://bh.jctech888.com.cn

[U33] Py：打包发布
来源：http://dt.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://fn.bjjhwx.cn

[U34] Py：判断编码
来源：http://um.chemitech.net.cn

chardet.detect(raw)
来源：http://nm.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://ap.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://en.521024.cn

[U36] Py：定时任务
来源：http://zm.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://hq.szsharing.cn

[U37] Py：读写 Excel
来源：http://hq.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ke.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://fz.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://me.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://zo.jctech888.com.cn

sys.stdout.isatty()
来源：http://so.newstarts.cn

[U40] Py：打印到标准错误
来源：http://ag.hnjuh.cn

print("err", file=sys.stderr)
来源：http://tn.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://fl.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kp.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://dv.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nl.nszjky.cn

[U43] PHP：声明命名空间
来源：http://ov.muxihuayi.cn

namespace App\Http;
来源：http://ym.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://ik.shxzskj.cn

declare(strict_types=1);
来源：http://lg.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://jg.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ra.shxzukj.cn

[U46] PHP：可空类型
来源：http://zs.newstarts.cn

?string $name = null
来源：http://sw.haigaiapp.cn

[U47] PHP：联合类型
来源：http://ts.shxzskj.cn

int|string $id
来源：http://av.lnxyls.cn

[U48] PHP：纯枚举
来源：http://tu.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cy.shxzskj.cn

[U49] PHP：只读属性
来源：http://jb.gzmigu.cn

public readonly string $name
来源：http://ny.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://ah.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://yb.bjjhwx.cn

[U51] PHP：数组解构
来源：http://sa.colortex.cn

[$a, $b] = $arr;
来源：http://ce.nicolike.cn

[U52] PHP：箭头函数
来源：http://bf.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://xq.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://mc.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://ue.521024.cn

[U54] PHP：空安全调用
来源：http://it.521024.cn

$obj?->method()
来源：http://cr.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://uj.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://en.jctech888.com.cn

[U56] PHP：命名参数
来源：http://ay.hahajie.cn

f(a: 1, b: 2)
来源：http://ki.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://hc.yuntaijiaju.cn

"值: {$a}"
来源：http://wh.asd995.cn

[U58] PHP：数组三件套
来源：http://yo.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ar.9csxet.cn

[U59] PHP：自定义排序
来源：http://kx.jianghongdianzi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lz.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://jm.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://my.bookmarksfly.cn

[U61] PHP：正则
来源：http://is.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vd.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://vy.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fs.bjjhwx.cn

[U63] PHP：文件读写
来源：http://ez.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yj.asd995.cn

[U64] PHP：目录遍历
来源：http://uy.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://sg.bookmarksfly.cn

[U65] PHP：会话
来源：http://na.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rk.huixinmuqiang.cn

[U66] PHP：设置 Cookie
来源：http://yh.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wm.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://ww.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://po.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://xh.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kk.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://ya.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pk.nszjky.cn

[U70] PHP：PDO 事务
来源：http://yu.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://de.huanxung.cn

[U71] PHP：抛出异常
来源：http://vc.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://ie.szsharing.cn

[U72] PHP：写错误日志
来源：http://ev.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://zo.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://yq.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://hi.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://ze.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://to.huanxung.cn

[U75] PHP：依赖注入
来源：http://qc.shtwfgs.cn

composer require psr/container
来源：http://mi.jctech888.com.cn

[U76] PHP：简单路由
来源：http://ul.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://me.nicolike.cn

[U77] PHP：模板渲染
来源：http://xo.asd995.cn

composer require twig/twig
来源：http://pj.521024.cn

[U78] PHP：单元测试
来源：http://ju.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://dr.newstarts.cn

[U79] PHP：静态分析
来源：http://mx.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://ft.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://rc.haigaiapp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bm.nszjky.cn

[U81] JS：初始化项目
来源：http://lr.wgjwhj.cn

npm init -y;  npm i express
来源：http://lf.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://le.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wo.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://re.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bl.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://vi.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ov.shxzukj.cn

[U85] JS：可选链
来源：http://tj.shxzukj.cn

a?.b?.c
来源：http://ha.shxzskj.cn

[U86] JS：空值合并
来源：http://hf.jctech888.com.cn

a ?? b
来源：http://tw.nicolike.cn

[U87] JS：解构默认值
来源：http://jg.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://qh.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://qb.jctech888.com.cn

{ ...a, ...b }
来源：http://ts.9csxet.cn

[U89] JS：数组去重
来源：http://dg.yuntaijiaju.cn

[...new Set(arr)]
来源：http://ji.huanxung.cn

[U90] JS：数字数组排序
来源：http://vg.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://fk.nicolike.cn

[U91] JS：对象键值遍历
来源：http://dd.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://my.shxzskj.cn

[U92] JS：深拷贝
来源：http://zr.muxihuayi.cn

structuredClone(obj)
来源：http://ei.hnjuh.cn

[U93] JS：模板字符串
来源：http://qn.colortex.cn

`共 ${n} 条`
来源：http://zb.wgjwhj.cn

[U94] JS：箭头函数
来源：http://ge.shtwfgs.cn

const double = x => x * 2;
来源：http://th.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://qc.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://ye.hahajie.cn

[U96] JS：async/await 与异常
来源：http://gl.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rg.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://cy.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://js.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://vs.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bq.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://xr.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://cb.hnjuh.cn

[U100] JS：DOM 查询
来源：http://jo.bookmarksfly.cn

document.querySelector(".item")
来源：http://ga.gzmigu.cn

[U101] JS：classList 操作
来源：http://jy.shxzukj.cn

el.classList.toggle("active")
来源：http://ku.wgjwhj.cn

[U102] JS：本地存储
来源：http://mz.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yi.bookmarksfly.cn

[U103] JS：定时器
来源：http://ta.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dq.hahajie.cn

[U104] JS：防抖
来源：http://lg.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xx.huixiangedu.cn

[U105] JS：节流
来源：http://kz.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fz.wgjwhj.cn

[U106] JS：日期格式化
来源：http://nk.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jt.muxihuayi.cn

[U107] JS：数字千分位
来源：http://af.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hw.colortex.cn

[U108] JS：随机整数
来源：http://lc.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gi.huixiangedu.cn

[U109] JS：数组分组
来源：http://kw.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://dy.wgjwhj.cn

[U110] JS：数组分块
来源：http://wi.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://id.gzmigu.cn

[U111] JS：对象转 Map
来源：http://qq.nicolike.cn

new Map(Object.entries(obj))
来源：http://im.9csxet.cn

[U112] JS：字符串补位
来源：http://me.nszjky.cn

"7".padStart(3, "0")
来源：http://ev.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://bu.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://hb.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://wo.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ze.nszjky.cn

[U115] JS：生成 UUID
来源：http://tb.shxzskj.cn

crypto.randomUUID()
来源：http://cs.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://sn.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://yp.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://yl.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://iy.yuexingan06.cn

[U118] JS：开发服务器
来源：http://dr.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://yo.szsharing.cn

[U119] JS：生产构建
来源：http://ib.szxytkj.cn

npx vite build
来源：http://fk.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://dr.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://ho.nicolike.cn

================================================================================
来源：http://iy.jianghongdianzi.cn

统计汇总
来源：http://jd.jianghongdianzi.cn

================================================================================
来源：http://cp.huixinmuqiang.cn

按语言统计（条）：
来源：http://gq.newstarts.cn

Python ......... 252
来源：http://gj.bookmarksfly.cn

PHP ............ 252
来源：http://ax.colortex.cn

JavaScript ..... 252
来源：http://ua.shxzukj.cn

TypeScript ..... 212
来源：http://oy.hahajie.cn

Java ........... 212
来源：http://xf.haigaiapp.cn

Go ............. 212
来源：http://yk.yuntaijiaju.cn

Ruby ........... 212
来源：http://mg.nicolike.cn

C# ............. 212
来源：http://sk.shtwfgs.cn

C .............. 30
来源：http://za.huixiangedu.cn

C++ ............ 30
来源：http://fj.nicolike.cn

SQL ............ 90
来源：http://af.szsharing.cn

Bash ........... 80
来源：http://st.9csxet.cn

Kotlin ......... 15
来源：http://oe.panjiajie.cn

Swift .......... 15
来源：http://xw.yuexingan06.cn

Lua ............ 10
来源：http://uv.521024.cn

Perl ........... 10
来源：http://kw.newstarts.cn

Scala .......... 10
来源：http://np.haigaiapp.cn

------------------------------------
来源：http://eq.yuntaijiaju.cn

合计 ........... 2106 条
来源：http://wh.gzmigu.cn

按章节统计：
来源：http://nc.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jy.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lm.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ce.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://an.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vf.haigaiapp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ao.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gv.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hi.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vs.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dg.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rf.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://id.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hy.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yv.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tt.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yf.colortex.cn

Q SQL 专题                              90
来源：http://mn.panjiajie.cn

R Bash 专题                             80
来源：http://oc.muxihuayi.cn

S C / C++ 专题                          60
来源：http://vp.nicolike.cn

T 其他语言补充                          60
来源：http://bm.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://ij.muxihuayi.cn

------------------------------------
来源：http://la.nicolike.cn

合计                                  2106 条
来源：http://tg.asd995.cn

--------------------------------------------------------------------------------
来源：http://lp.shxzskj.cn

使用提醒
来源：http://rn.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://ek.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mk.huixinmuqiang.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wk.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://py.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zz.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wr.nicolike.cn

—— 文件结束 ——
来源：http://tz.huixinmuqiang.cn

================================================================================
来源：http://oh.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://aw.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://dj.wgjwhj.cn

================================================================================
来源：http://el.shxzskj.cn

【收录内容】
来源：http://re.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sh.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kl.9csxet.cn

SQL · Bash · C · C++
来源：http://xu.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yg.gzmigu.cn

【使用说明】
来源：http://qb.huixiangedu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gl.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zk.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dp.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yr.asd995.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dg.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eg.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zn.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ms.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fm.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://af.shxzukj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pv.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qn.shtwfgs.cn

【文件统计】
来源：http://yf.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sh.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://mk.bookmarksfly.cn

目  录
来源：http://pn.colortex.cn

--------------------------------------------------------------------------------
来源：http://xn.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uh.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://up.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nr.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zt.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://op.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gl.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xo.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uz.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tj.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vg.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eh.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wv.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jr.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pr.szxytkj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aj.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cj.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lq.huixiangedu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dk.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xg.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tj.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ad.jctech888.com.cn

================================================================================
来源：http://na.nszjky.cn

A. 基础语法与类型
来源：http://ry.newstarts.cn

================================================================================
来源：http://pf.wgjwhj.cn

[A01] Hello World
来源：http://ag.huixinmuqiang.cn

Py:   print("Hello, World!")
来源：http://ep.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://km.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://gz.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hr.chemitech.net.cn


<!-- 参考信息 -->