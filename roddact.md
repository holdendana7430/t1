代发 wailian999

[U25] Py：CSV 按字典读
来源：http://ye.huixiangedu.cn

csv.DictReader(f)
来源：http://kv.yuexingan06.cn

[U26] Py：并发下载
来源：http://uk.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lz.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://kz.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://ne.huanxung.cn

[U28] Py：类型别名
来源：http://ei.bookmarksfly.cn

UserId = int
来源：http://mu.colortex.cn

[U29] Py：属性校验
来源：http://ss.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://cy.bjjhwx.cn

[U30] Py：数据类
来源：http://gs.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://ft.shxzskj.cn

[U31] Py：单测
来源：http://op.shxzukj.cn

python -m pytest -q
来源：http://dj.panjiajie.cn

[U32] Py：代码格式化
来源：http://lf.szsharing.cn

ruff format . && ruff check --fix .
来源：http://vo.panjiajie.cn

[U33] Py：打包发布
来源：http://qt.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://im.nszjky.cn

[U34] Py：判断编码
来源：http://ns.hahajie.cn

chardet.detect(raw)
来源：http://vp.shxzskj.cn

[U35] Py：发送邮件
来源：http://pm.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ny.szxytkj.cn

[U36] Py：定时任务
来源：http://jj.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://ci.gzmigu.cn

[U37] Py：读写 Excel
来源：http://ey.muxihuayi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lj.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://ij.hnjuh.cn

Path(__file__).resolve().parent
来源：http://ap.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://ae.gzmigu.cn

sys.stdout.isatty()
来源：http://ay.asd995.cn

[U40] Py：打印到标准错误
来源：http://lv.panjiajie.cn

print("err", file=sys.stderr)
来源：http://dt.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://ti.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fy.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://uq.yuntaijiaju.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xx.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://sy.yuexingan06.cn

namespace App\Http;
来源：http://vg.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://be.newstarts.cn

declare(strict_types=1);
来源：http://ez.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://qf.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ej.bjjhwx.cn

[U46] PHP：可空类型
来源：http://rz.bjjhwx.cn

?string $name = null
来源：http://cb.szxytkj.cn

[U47] PHP：联合类型
来源：http://ug.szsharing.cn

int|string $id
来源：http://yw.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://ju.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ay.colortex.cn

[U49] PHP：只读属性
来源：http://hg.bookmarksfly.cn

public readonly string $name
来源：http://ow.521024.cn

[U50] PHP：构造器属性提升
来源：http://rc.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://fj.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://fs.huanxung.cn

[$a, $b] = $arr;
来源：http://yn.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://rf.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://ax.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://kd.haigaiapp.cn

$v = $a ?? $b ?? "default";
来源：http://ce.521024.cn

[U54] PHP：空安全调用
来源：http://vx.jctech888.com.cn

$obj?->method()
来源：http://ck.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://pt.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xa.jctech888.com.cn

[U56] PHP：命名参数
来源：http://na.9csxet.cn

f(a: 1, b: 2)
来源：http://cu.szxytkj.cn

[U57] PHP：字符串插值
来源：http://om.nszjky.cn

"值: {$a}"
来源：http://ll.shxzukj.cn

[U58] PHP：数组三件套
来源：http://pg.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sh.huanxung.cn

[U59] PHP：自定义排序
来源：http://pn.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jj.shxzskj.cn

[U60] PHP：JSON 编解码
来源：http://ca.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://me.yuntaijiaju.cn

[U61] PHP：正则
来源：http://km.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ux.muxihuayi.cn

[U62] PHP：日期对象
来源：http://if.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iq.panjiajie.cn

[U63] PHP：文件读写
来源：http://ma.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://au.hahajie.cn

[U64] PHP：目录遍历
来源：http://bb.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://ki.nszjky.cn

[U65] PHP：会话
来源：http://jc.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gx.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://tj.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://of.colortex.cn

[U67] PHP：处理文件上传
来源：http://tu.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ym.huanxung.cn

[U68] PHP：PDO 连接
来源：http://np.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qu.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://rp.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xy.colortex.cn

[U70] PHP：PDO 事务
来源：http://cw.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ib.szxytkj.cn

[U71] PHP：抛出异常
来源：http://us.521024.cn

throw new RuntimeException("失败", 500);
来源：http://sm.9csxet.cn

[U72] PHP：写错误日志
来源：http://pm.hnjuh.cn

error_log("失败: " . $e->getMessage());
来源：http://mc.lnxyls.cn

[U73] PHP：读取 ini 配置
来源：http://fw.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://dh.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://jq.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://ky.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://om.szsharing.cn

composer require psr/container
来源：http://ag.panjiajie.cn

[U76] PHP：简单路由
来源：http://mm.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://po.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://yd.newstarts.cn

composer require twig/twig
来源：http://ng.newstarts.cn

[U78] PHP：单元测试
来源：http://cs.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://df.bjjhwx.cn

[U79] PHP：静态分析
来源：http://yo.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://hi.shxzskj.cn

[U80] PHP：代码规范修复
来源：http://zy.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mn.nicolike.cn

[U81] JS：初始化项目
来源：http://zf.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://nm.panjiajie.cn

[U82] JS：package.json 脚本
来源：http://od.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gn.huixinmuqiang.cn

[U83] JS：ES Module 导入导出
来源：http://yb.muxihuayi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mh.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://me.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ye.shtwfgs.cn

[U85] JS：可选链
来源：http://nq.szxytkj.cn

a?.b?.c
来源：http://hq.nszjky.cn

[U86] JS：空值合并
来源：http://ce.gzmigu.cn

a ?? b
来源：http://dy.muxihuayi.cn

[U87] JS：解构默认值
来源：http://dt.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://pz.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://em.gzmigu.cn

{ ...a, ...b }
来源：http://bw.lnxyls.cn

[U89] JS：数组去重
来源：http://oo.muxihuayi.cn

[...new Set(arr)]
来源：http://yr.szxytkj.cn

[U90] JS：数字数组排序
来源：http://vl.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://ii.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://js.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uy.huixiangedu.cn

[U92] JS：深拷贝
来源：http://bv.hahajie.cn

structuredClone(obj)
来源：http://dn.panjiajie.cn

[U93] JS：模板字符串
来源：http://do.shtwfgs.cn

`共 ${n} 条`
来源：http://bz.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://ba.muxihuayi.cn

const double = x => x * 2;
来源：http://oj.newstarts.cn

[U95] JS：Promise 包装
来源：http://st.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://cb.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://dm.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ic.szxytkj.cn

[U97] JS：并发请求
来源：http://sr.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nb.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://py.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hl.muxihuayi.cn

[U99] JS：事件监听
来源：http://is.521024.cn

el.addEventListener("click", e => {})
来源：http://uo.521024.cn

[U100] JS：DOM 查询
来源：http://ew.lnxyls.cn

document.querySelector(".item")
来源：http://hx.bjjhwx.cn

[U101] JS：classList 操作
来源：http://kp.bookmarksfly.cn

el.classList.toggle("active")
来源：http://os.bookmarksfly.cn

[U102] JS：本地存储
来源：http://fx.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gg.nszjky.cn

[U103] JS：定时器
来源：http://xp.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pq.huixiangedu.cn

[U104] JS：防抖
来源：http://ay.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jd.newstarts.cn

[U105] JS：节流
来源：http://jb.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rn.szsharing.cn

[U106] JS：日期格式化
来源：http://eu.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gp.huixiangedu.cn

[U107] JS：数字千分位
来源：http://hn.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vj.newstarts.cn

[U108] JS：随机整数
来源：http://mf.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xf.521024.cn

[U109] JS：数组分组
来源：http://xc.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://cv.wgjwhj.cn

[U110] JS：数组分块
来源：http://tq.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qp.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://ln.szxytkj.cn

new Map(Object.entries(obj))
来源：http://fq.colortex.cn

[U112] JS：字符串补位
来源：http://da.muxihuayi.cn

"7".padStart(3, "0")
来源：http://xm.szxytkj.cn

[U113] JS：正则替换全部
来源：http://jt.colortex.cn

s.replaceAll("a", "b")
来源：http://an.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://un.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gr.szxytkj.cn

[U115] JS：生成 UUID
来源：http://ze.huixiangedu.cn

crypto.randomUUID()
来源：http://qx.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://hr.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://dz.nicolike.cn

[U117] JS：单元测试
来源：http://kq.521024.cn

npm i -D vitest;  npx vitest
来源：http://za.nicolike.cn

[U118] JS：开发服务器
来源：http://gm.szxytkj.cn

npm i -D vite;  npx vite
来源：http://ha.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://xc.9csxet.cn

npx vite build
来源：http://nv.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://fc.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://zu.nszjky.cn

================================================================================
来源：http://cd.muxihuayi.cn

统计汇总
来源：http://qn.wgjwhj.cn

================================================================================
来源：http://jv.panjiajie.cn

按语言统计（条）：
来源：http://tg.nicolike.cn

Python ......... 252
来源：http://zn.muxihuayi.cn

PHP ............ 252
来源：http://zj.lnxyls.cn

JavaScript ..... 252
来源：http://or.lnxyls.cn

TypeScript ..... 212
来源：http://mm.jianghongdianzi.cn

Java ........... 212
来源：http://bt.szsharing.cn

Go ............. 212
来源：http://ti.bookmarksfly.cn

Ruby ........... 212
来源：http://pu.yuexingan06.cn

C# ............. 212
来源：http://sl.hnjuh.cn

C .............. 30
来源：http://cn.chemitech.net.cn

C++ ............ 30
来源：http://ym.huanxung.cn

SQL ............ 90
来源：http://th.jctech888.com.cn

Bash ........... 80
来源：http://ez.hahajie.cn

Kotlin ......... 15
来源：http://gj.panjiajie.cn

Swift .......... 15
来源：http://tq.panjiajie.cn

Lua ............ 10
来源：http://xw.chemitech.net.cn

Perl ........... 10
来源：http://ex.shtwfgs.cn

Scala .......... 10
来源：http://le.bjjhwx.cn

------------------------------------
来源：http://xf.bookmarksfly.cn

合计 ........... 2106 条
来源：http://ys.asd995.cn

按章节统计：
来源：http://ru.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yg.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pq.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eh.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gk.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ir.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wg.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://er.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sg.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ld.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://is.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kr.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qw.asd995.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://le.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fp.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nq.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rk.colortex.cn

Q SQL 专题                              90
来源：http://yy.lnxyls.cn

R Bash 专题                             80
来源：http://qk.521024.cn

S C / C++ 专题                          60
来源：http://ld.wgjwhj.cn

T 其他语言补充                          60
来源：http://zy.shxzukj.cn

U 高频实用片段                         120
来源：http://sb.yuntaijiaju.cn

------------------------------------
来源：http://tv.521024.cn

合计                                  2106 条
来源：http://wo.nicolike.cn

--------------------------------------------------------------------------------
来源：http://uu.shxzukj.cn

使用提醒
来源：http://ld.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://qk.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dj.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lf.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bu.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ap.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yn.jianghongdianzi.cn

—— 文件结束 ——
来源：http://pp.newstarts.cn

================================================================================
来源：http://wj.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://qz.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://zd.asd995.cn

================================================================================
来源：http://ma.nicolike.cn

【收录内容】
来源：http://wg.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sc.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mc.nicolike.cn

SQL · Bash · C · C++
来源：http://ji.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mj.yuexingan06.cn

【使用说明】
来源：http://aw.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cr.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wz.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bu.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ok.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ez.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bv.bjjhwx.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cr.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zy.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zo.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ho.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sj.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://do.yuexingan06.cn

【文件统计】
来源：http://dg.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ll.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://dr.shtwfgs.cn

目  录
来源：http://va.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://ex.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jd.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mr.szsharing.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kv.asd995.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oy.9csxet.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uo.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bv.shxzskj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rq.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sq.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rd.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hl.lnxyls.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mp.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vo.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dt.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lx.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tt.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hh.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bz.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jy.jctech888.com.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yb.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mm.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ri.newstarts.cn

================================================================================
来源：http://yz.haigaiapp.cn

A. 基础语法与类型
来源：http://kh.chemitech.net.cn

================================================================================
来源：http://wh.shtwfgs.cn

[A01] Hello World
来源：http://gy.jctech888.com.cn


<!-- 参考信息 -->