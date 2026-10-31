代发 wailian999

[U29] Py：属性校验
来源：http://mj.lnxyls.cn

@property 与 @x.setter 配合
来源：http://hl.nicolike.cn

[U30] Py：数据类
来源：http://hi.yuexingan06.cn

@dataclass(slots=True)
来源：http://fe.shxzskj.cn

[U31] Py：单测
来源：http://qt.szxytkj.cn

python -m pytest -q
来源：http://io.hahajie.cn

[U32] Py：代码格式化
来源：http://vs.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://xt.shxzskj.cn

[U33] Py：打包发布
来源：http://ij.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://kd.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://al.muxihuayi.cn

chardet.detect(raw)
来源：http://oi.shtwfgs.cn

[U35] Py：发送邮件
来源：http://kn.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lb.huixiangedu.cn

[U36] Py：定时任务
来源：http://lb.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://aq.panjiajie.cn

[U37] Py：读写 Excel
来源：http://bv.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jj.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://pv.nszjky.cn

Path(__file__).resolve().parent
来源：http://fu.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://cg.szxytkj.cn

sys.stdout.isatty()
来源：http://oz.newstarts.cn

[U40] Py：打印到标准错误
来源：http://bq.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://qf.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://sp.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qq.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://jc.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kq.newstarts.cn

[U43] PHP：声明命名空间
来源：http://ea.chemitech.net.cn

namespace App\Http;
来源：http://fs.colortex.cn

[U44] PHP：开启严格类型
来源：http://oy.huixinmuqiang.cn

declare(strict_types=1);
来源：http://gz.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://ec.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jd.wgjwhj.cn

[U46] PHP：可空类型
来源：http://vw.lnxyls.cn

?string $name = null
来源：http://sw.huanxung.cn

[U47] PHP：联合类型
来源：http://fm.yuntaijiaju.cn

int|string $id
来源：http://ye.colortex.cn

[U48] PHP：纯枚举
来源：http://dm.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sv.shxzukj.cn

[U49] PHP：只读属性
来源：http://ij.gzmigu.cn

public readonly string $name
来源：http://lx.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://tw.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://pp.colortex.cn

[U51] PHP：数组解构
来源：http://kq.muxihuayi.cn

[$a, $b] = $arr;
来源：http://xz.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://ra.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://be.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://qf.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://rf.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://do.newstarts.cn

$obj?->method()
来源：http://da.521024.cn

[U55] PHP：match 表达式
来源：http://xw.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rj.hnjuh.cn

[U56] PHP：命名参数
来源：http://dg.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://bp.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://xz.521024.cn

"值: {$a}"
来源：http://pp.wgjwhj.cn

[U58] PHP：数组三件套
来源：http://go.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mr.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://mb.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zo.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://no.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sw.521024.cn

[U61] PHP：正则
来源：http://zv.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rt.wgjwhj.cn

[U62] PHP：日期对象
来源：http://gj.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ef.szxytkj.cn

[U63] PHP：文件读写
来源：http://yj.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ya.nszjky.cn

[U64] PHP：目录遍历
来源：http://hd.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://yx.huixiangedu.cn

[U65] PHP：会话
来源：http://iu.9csxet.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hl.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://sv.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xr.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://ox.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vr.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://hm.szxytkj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ai.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://ld.nicolike.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dg.hahajie.cn

[U70] PHP：PDO 事务
来源：http://yw.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cm.lnxyls.cn

[U71] PHP：抛出异常
来源：http://je.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://bw.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://xp.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://xv.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://td.muxihuayi.cn

parse_ini_file("config.ini", true)
来源：http://vo.szsharing.cn

[U74] PHP：读取环境变量
来源：http://xb.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://ma.lnxyls.cn

[U75] PHP：依赖注入
来源：http://bi.newstarts.cn

composer require psr/container
来源：http://eh.haigaiapp.cn

[U76] PHP：简单路由
来源：http://co.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vg.shxzukj.cn

[U77] PHP：模板渲染
来源：http://df.521024.cn

composer require twig/twig
来源：http://tl.chemitech.net.cn

[U78] PHP：单元测试
来源：http://lx.521024.cn

composer require --dev phpunit/phpunit
来源：http://rm.muxihuayi.cn

[U79] PHP：静态分析
来源：http://dr.colortex.cn

composer require --dev phpstan/phpstan
来源：http://ib.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://ku.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qz.huanxung.cn

[U81] JS：初始化项目
来源：http://id.muxihuayi.cn

npm init -y;  npm i express
来源：http://bg.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://gv.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tt.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://py.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://je.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://wd.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gq.hnjuh.cn

[U85] JS：可选链
来源：http://wu.huixiangedu.cn

a?.b?.c
来源：http://tc.szxytkj.cn

[U86] JS：空值合并
来源：http://jx.lnxyls.cn

a ?? b
来源：http://bh.shxzukj.cn

[U87] JS：解构默认值
来源：http://ap.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://wh.szxytkj.cn

[U88] JS：对象展开合并
来源：http://tz.muxihuayi.cn

{ ...a, ...b }
来源：http://lz.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://nl.lnxyls.cn

[...new Set(arr)]
来源：http://nr.asd995.cn

[U90] JS：数字数组排序
来源：http://zk.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://ru.szsharing.cn

[U91] JS：对象键值遍历
来源：http://tz.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ko.newstarts.cn

[U92] JS：深拷贝
来源：http://wp.lnxyls.cn

structuredClone(obj)
来源：http://wm.shxzukj.cn

[U93] JS：模板字符串
来源：http://hz.chemitech.net.cn

`共 ${n} 条`
来源：http://qk.chemitech.net.cn

[U94] JS：箭头函数
来源：http://qj.jctech888.com.cn

const double = x => x * 2;
来源：http://vl.gzmigu.cn

[U95] JS：Promise 包装
来源：http://ku.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://ia.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://hq.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zk.shxzukj.cn

[U97] JS：并发请求
来源：http://un.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pl.521024.cn

[U98] JS：fetch 带 JSON
来源：http://nm.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dk.szxytkj.cn

[U99] JS：事件监听
来源：http://kk.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://kp.huixiangedu.cn

[U100] JS：DOM 查询
来源：http://ar.panjiajie.cn

document.querySelector(".item")
来源：http://tb.9csxet.cn

[U101] JS：classList 操作
来源：http://sq.muxihuayi.cn

el.classList.toggle("active")
来源：http://ao.haigaiapp.cn

[U102] JS：本地存储
来源：http://hq.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sx.jctech888.com.cn

[U103] JS：定时器
来源：http://td.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ug.shtwfgs.cn

[U104] JS：防抖
来源：http://iw.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aj.colortex.cn

[U105] JS：节流
来源：http://zz.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dd.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://kk.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xv.bjjhwx.cn

[U107] JS：数字千分位
来源：http://sp.521024.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uk.jctech888.com.cn

[U108] JS：随机整数
来源：http://ee.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tn.hahajie.cn

[U109] JS：数组分组
来源：http://gg.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://sa.newstarts.cn

[U110] JS：数组分块
来源：http://mc.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ik.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://yu.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://qr.haigaiapp.cn

[U112] JS：字符串补位
来源：http://yy.gzmigu.cn

"7".padStart(3, "0")
来源：http://nm.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://vc.hahajie.cn

s.replaceAll("a", "b")
来源：http://rx.hahajie.cn

[U114] JS：JSON 深比较
来源：http://tp.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gj.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://vy.nszjky.cn

crypto.randomUUID()
来源：http://ow.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://fi.szxytkj.cn

/** @param {string} name */ function f(name) {}
来源：http://te.bookmarksfly.cn

[U117] JS：单元测试
来源：http://iw.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://qa.9csxet.cn

[U118] JS：开发服务器
来源：http://ym.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://mb.hahajie.cn

[U119] JS：生产构建
来源：http://uo.newstarts.cn

npx vite build
来源：http://bt.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://an.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://ro.yuexingan06.cn

================================================================================
来源：http://vm.9csxet.cn

统计汇总
来源：http://ri.huanxung.cn

================================================================================
来源：http://ce.521024.cn

按语言统计（条）：
来源：http://vi.haigaiapp.cn

Python ......... 252
来源：http://sk.jianghongdianzi.cn

PHP ............ 252
来源：http://ws.huixiangedu.cn

JavaScript ..... 252
来源：http://af.szsharing.cn

TypeScript ..... 212
来源：http://ym.huixiangedu.cn

Java ........... 212
来源：http://ol.gzmigu.cn

Go ............. 212
来源：http://vs.gzmigu.cn

Ruby ........... 212
来源：http://iy.szxytkj.cn

C# ............. 212
来源：http://zf.huixinmuqiang.cn

C .............. 30
来源：http://zq.yuntaijiaju.cn

C++ ............ 30
来源：http://vq.yuntaijiaju.cn

SQL ............ 90
来源：http://lw.huixinmuqiang.cn

Bash ........... 80
来源：http://yz.huixinmuqiang.cn

Kotlin ......... 15
来源：http://bh.panjiajie.cn

Swift .......... 15
来源：http://bv.yuexingan06.cn

Lua ............ 10
来源：http://nz.chemitech.net.cn

Perl ........... 10
来源：http://hg.szsharing.cn

Scala .......... 10
来源：http://uk.9csxet.cn

------------------------------------
来源：http://mk.szsharing.cn

合计 ........... 2106 条
来源：http://bi.asd995.cn

按章节统计：
来源：http://rk.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ty.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vr.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dv.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pz.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://za.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sl.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dp.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jn.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rs.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hs.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ec.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ys.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yh.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qs.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ay.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qx.nszjky.cn

Q SQL 专题                              90
来源：http://do.521024.cn

R Bash 专题                             80
来源：http://dj.huixiangedu.cn

S C / C++ 专题                          60
来源：http://zg.wgjwhj.cn

T 其他语言补充                          60
来源：http://xi.shxzskj.cn

U 高频实用片段                         120
来源：http://ig.bjjhwx.cn

------------------------------------
来源：http://zj.shxzskj.cn

合计                                  2106 条
来源：http://fc.nicolike.cn

--------------------------------------------------------------------------------
来源：http://je.huixinmuqiang.cn

使用提醒
来源：http://ty.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://qc.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tu.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vf.jianghongdianzi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://eq.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bn.haigaiapp.cn

—— 文件结束 ——
来源：http://tr.chemitech.net.cn

================================================================================
来源：http://du.huixinmuqiang.cn

程序语言常见例子速查手册（2024 版）
来源：http://lb.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://ay.huixinmuqiang.cn

================================================================================
来源：http://yv.bjjhwx.cn

【收录内容】
来源：http://vy.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sz.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xo.chemitech.net.cn

SQL · Bash · C · C++
来源：http://ls.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ha.bookmarksfly.cn

【使用说明】
来源：http://gc.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gf.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xb.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vk.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jg.bookmarksfly.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cy.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://or.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://un.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tw.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yp.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wn.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bf.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gy.jctech888.com.cn

【文件统计】
来源：http://xn.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qk.521024.cn

--------------------------------------------------------------------------------
来源：http://jd.bjjhwx.cn

目  录
来源：http://dv.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://or.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xg.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eb.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kb.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cw.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kn.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://or.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fq.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ym.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yj.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wp.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ii.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ac.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hy.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gq.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ty.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ig.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fy.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ji.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://un.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jx.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wb.9csxet.cn

================================================================================
来源：http://gr.521024.cn

A. 基础语法与类型
来源：http://gs.lnxyls.cn

================================================================================
来源：http://ep.shxzukj.cn

[A01] Hello World
来源：http://tw.szxytkj.cn

Py:   print("Hello, World!")
来源：http://sj.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://hm.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://gy.nicolike.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jd.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://ye.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://xk.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://kx.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://js.haigaiapp.cn


<!-- 参考信息 -->