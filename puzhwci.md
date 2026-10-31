代发 wailian999

[U31] Py：单测
来源：http://sp.huanxung.cn

python -m pytest -q
来源：http://si.panjiajie.cn

[U32] Py：代码格式化
来源：http://ld.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://xv.szxytkj.cn

[U33] Py：打包发布
来源：http://io.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://tj.haigaiapp.cn

[U34] Py：判断编码
来源：http://ot.huixiangedu.cn

chardet.detect(raw)
来源：http://zf.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://al.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cu.huixiangedu.cn

[U36] Py：定时任务
来源：http://sh.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://zc.shxzukj.cn

[U37] Py：读写 Excel
来源：http://wv.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jk.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://ow.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://kw.lnxyls.cn

[U39] Py：判断是否在交互环境
来源：http://jt.muxihuayi.cn

sys.stdout.isatty()
来源：http://xg.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://cy.asd995.cn

print("err", file=sys.stderr)
来源：http://kt.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://jo.szsharing.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://px.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://cg.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rq.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://vx.hnjuh.cn

namespace App\Http;
来源：http://tm.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://yz.nicolike.cn

declare(strict_types=1);
来源：http://bm.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://wa.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://py.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://ra.huixiangedu.cn

?string $name = null
来源：http://ho.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://sv.gzmigu.cn

int|string $id
来源：http://rw.shxzskj.cn

[U48] PHP：纯枚举
来源：http://no.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rh.shxzukj.cn

[U49] PHP：只读属性
来源：http://fq.huixinmuqiang.cn

public readonly string $name
来源：http://im.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://bf.huanxung.cn

public function __construct(private int $id) {}
来源：http://ig.nszjky.cn

[U51] PHP：数组解构
来源：http://tv.shxzskj.cn

[$a, $b] = $arr;
来源：http://wc.huanxung.cn

[U52] PHP：箭头函数
来源：http://hp.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://sa.nszjky.cn

[U53] PHP：空合并运算符
来源：http://vp.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://mn.szsharing.cn

[U54] PHP：空安全调用
来源：http://pi.chemitech.net.cn

$obj?->method()
来源：http://ch.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://ur.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pb.haigaiapp.cn

[U56] PHP：命名参数
来源：http://tn.jianghongdianzi.cn

f(a: 1, b: 2)
来源：http://gn.9csxet.cn

[U57] PHP：字符串插值
来源：http://bp.nszjky.cn

"值: {$a}"
来源：http://tp.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://lr.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ci.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://sx.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bb.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://tk.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fw.shtwfgs.cn

[U61] PHP：正则
来源：http://wz.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://io.9csxet.cn

[U62] PHP：日期对象
来源：http://sh.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://js.muxihuayi.cn

[U63] PHP：文件读写
来源：http://ma.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xc.nicolike.cn

[U64] PHP：目录遍历
来源：http://di.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://qb.huanxung.cn

[U65] PHP：会话
来源：http://uq.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mg.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://fw.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ys.bookmarksfly.cn

[U67] PHP：处理文件上传
来源：http://kc.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yj.nicolike.cn

[U68] PHP：PDO 连接
来源：http://dc.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cs.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://qo.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sd.nszjky.cn

[U70] PHP：PDO 事务
来源：http://yd.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://re.jctech888.com.cn

[U71] PHP：抛出异常
来源：http://fr.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://lm.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://mg.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://sw.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://qh.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://cz.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://ss.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://at.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://ij.shtwfgs.cn

composer require psr/container
来源：http://zc.nszjky.cn

[U76] PHP：简单路由
来源：http://jn.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fn.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://dp.bjjhwx.cn

composer require twig/twig
来源：http://qy.shxzskj.cn

[U78] PHP：单元测试
来源：http://uo.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://cd.bjjhwx.cn

[U79] PHP：静态分析
来源：http://ux.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://ik.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://lw.shxzskj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bw.huixinmuqiang.cn

[U81] JS：初始化项目
来源：http://dl.asd995.cn

npm init -y;  npm i express
来源：http://ac.gzmigu.cn

[U82] JS：package.json 脚本
来源：http://lq.chemitech.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rd.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://to.chemitech.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tw.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://ry.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iz.gzmigu.cn

[U85] JS：可选链
来源：http://kb.jctech888.com.cn

a?.b?.c
来源：http://fg.9csxet.cn

[U86] JS：空值合并
来源：http://np.jctech888.com.cn

a ?? b
来源：http://in.gzmigu.cn

[U87] JS：解构默认值
来源：http://hy.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://gf.newstarts.cn

[U88] JS：对象展开合并
来源：http://td.newstarts.cn

{ ...a, ...b }
来源：http://wu.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://bj.shtwfgs.cn

[...new Set(arr)]
来源：http://ij.yuntaijiaju.cn

[U90] JS：数字数组排序
来源：http://nk.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://ko.newstarts.cn

[U91] JS：对象键值遍历
来源：http://qp.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://he.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://jr.jctech888.com.cn

structuredClone(obj)
来源：http://ql.muxihuayi.cn

[U93] JS：模板字符串
来源：http://ri.muxihuayi.cn

`共 ${n} 条`
来源：http://ry.shtwfgs.cn

[U94] JS：箭头函数
来源：http://cp.shtwfgs.cn

const double = x => x * 2;
来源：http://bb.panjiajie.cn

[U95] JS：Promise 包装
来源：http://sf.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://tk.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://nk.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gn.panjiajie.cn

[U97] JS：并发请求
来源：http://pg.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qb.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://zj.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qw.huixiangedu.cn

[U99] JS：事件监听
来源：http://so.huanxung.cn

el.addEventListener("click", e => {})
来源：http://ef.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://kl.szxytkj.cn

document.querySelector(".item")
来源：http://xy.gzmigu.cn

[U101] JS：classList 操作
来源：http://ed.bjjhwx.cn

el.classList.toggle("active")
来源：http://fu.521024.cn

[U102] JS：本地存储
来源：http://ak.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xr.chemitech.net.cn

[U103] JS：定时器
来源：http://dm.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ju.shtwfgs.cn

[U104] JS：防抖
来源：http://qb.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mp.nszjky.cn

[U105] JS：节流
来源：http://da.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vy.wgjwhj.cn

[U106] JS：日期格式化
来源：http://lv.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zz.nicolike.cn

[U107] JS：数字千分位
来源：http://ok.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ww.shxzskj.cn

[U108] JS：随机整数
来源：http://wt.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pl.521024.cn

[U109] JS：数组分组
来源：http://sh.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://cz.muxihuayi.cn

[U110] JS：数组分块
来源：http://uq.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cy.szxytkj.cn

[U111] JS：对象转 Map
来源：http://vj.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://hg.shtwfgs.cn

[U112] JS：字符串补位
来源：http://ln.9csxet.cn

"7".padStart(3, "0")
来源：http://hr.szxytkj.cn

[U113] JS：正则替换全部
来源：http://nm.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://ky.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://hj.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://os.wgjwhj.cn

[U115] JS：生成 UUID
来源：http://wq.szxytkj.cn

crypto.randomUUID()
来源：http://kh.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://aq.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://mq.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://cv.colortex.cn

npm i -D vitest;  npx vitest
来源：http://ye.bjjhwx.cn

[U118] JS：开发服务器
来源：http://gu.panjiajie.cn

npm i -D vite;  npx vite
来源：http://lb.haigaiapp.cn

[U119] JS：生产构建
来源：http://dl.szsharing.cn

npx vite build
来源：http://ni.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://ka.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://ue.haigaiapp.cn

================================================================================
来源：http://md.muxihuayi.cn

统计汇总
来源：http://dm.huanxung.cn

================================================================================
来源：http://wr.shtwfgs.cn

按语言统计（条）：
来源：http://rc.huixinmuqiang.cn

Python ......... 252
来源：http://hs.szsharing.cn

PHP ............ 252
来源：http://ui.lnxyls.cn

JavaScript ..... 252
来源：http://bo.huanxung.cn

TypeScript ..... 212
来源：http://ow.yuntaijiaju.cn

Java ........... 212
来源：http://jk.nicolike.cn

Go ............. 212
来源：http://tn.bookmarksfly.cn

Ruby ........... 212
来源：http://xr.colortex.cn

C# ............. 212
来源：http://pg.huixinmuqiang.cn

C .............. 30
来源：http://ke.shtwfgs.cn

C++ ............ 30
来源：http://ag.huixiangedu.cn

SQL ............ 90
来源：http://ag.huixiangedu.cn

Bash ........... 80
来源：http://ep.panjiajie.cn

Kotlin ......... 15
来源：http://nd.lnxyls.cn

Swift .......... 15
来源：http://ss.haigaiapp.cn

Lua ............ 10
来源：http://om.hahajie.cn

Perl ........... 10
来源：http://ns.huixinmuqiang.cn

Scala .......... 10
来源：http://qa.bjjhwx.cn

------------------------------------
来源：http://bk.newstarts.cn

合计 ........... 2106 条
来源：http://hy.huixinmuqiang.cn

按章节统计：
来源：http://mj.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://js.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vv.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hm.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://az.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ro.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hr.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oa.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://km.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://no.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wo.wgjwhj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pm.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kp.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oo.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rc.jctech888.com.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sg.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kn.shtwfgs.cn

Q SQL 专题                              90
来源：http://it.yuntaijiaju.cn

R Bash 专题                             80
来源：http://ud.newstarts.cn

S C / C++ 专题                          60
来源：http://vd.newstarts.cn

T 其他语言补充                          60
来源：http://rk.bookmarksfly.cn

U 高频实用片段                         120
来源：http://dg.szxytkj.cn

------------------------------------
来源：http://ql.hahajie.cn

合计                                  2106 条
来源：http://va.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://sz.jianghongdianzi.cn

使用提醒
来源：http://el.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://qr.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sm.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dy.chemitech.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://he.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://md.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://td.asd995.cn

—— 文件结束 ——
来源：http://bu.gzmigu.cn

================================================================================
来源：http://dr.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://rv.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://le.521024.cn

================================================================================
来源：http://oh.szxytkj.cn

【收录内容】
来源：http://ag.shxzukj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ry.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ab.wgjwhj.cn

SQL · Bash · C · C++
来源：http://ly.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xu.bjjhwx.cn

【使用说明】
来源：http://qo.panjiajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fa.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bq.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ps.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://im.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mo.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fy.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yi.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rg.wgjwhj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bs.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sc.shtwfgs.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://en.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nm.hahajie.cn

【文件统计】
来源：http://fn.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jt.nszjky.cn

--------------------------------------------------------------------------------
来源：http://kz.yuexingan06.cn

目  录
来源：http://pp.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://hf.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kx.shtwfgs.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pz.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wb.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ho.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://km.huixiangedu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pd.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jt.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ri.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uh.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ep.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rf.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kv.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mm.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jd.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zj.szxytkj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ok.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vk.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://br.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cv.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zl.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ek.bjjhwx.cn

================================================================================
来源：http://bc.jianghongdianzi.cn

A. 基础语法与类型
来源：http://hm.jianghongdianzi.cn

================================================================================
来源：http://wp.shtwfgs.cn

[A01] Hello World
来源：http://st.huanxung.cn

Py:   print("Hello, World!")
来源：http://jg.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://gc.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://lq.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ad.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://kz.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://po.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://gi.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qn.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://sk.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wt.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sy.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jf.panjiajie.cn


<!-- 参考信息 -->