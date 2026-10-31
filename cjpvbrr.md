代发 wailian999

[U19] Py：正则替换带回调
来源：http://zv.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://of.nicolike.cn

[U20] Py：缓存函数结果
来源：http://cn.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://rg.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://xu.bjjhwx.cn

@contextlib.contextmanager
来源：http://do.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://nr.huixinmuqiang.cn

list(zip(*m))
来源：http://we.hahajie.cn

[U23] Py：分块读取大文件
来源：http://vj.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hp.nicolike.cn

[U24] Py：路径操作
来源：http://br.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://td.huixiangedu.cn

[U25] Py：CSV 按字典读
来源：http://yd.bookmarksfly.cn

csv.DictReader(f)
来源：http://jc.asd995.cn

[U26] Py：并发下载
来源：http://xf.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qp.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://fy.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://iu.szsharing.cn

[U28] Py：类型别名
来源：http://jv.asd995.cn

UserId = int
来源：http://ed.nszjky.cn

[U29] Py：属性校验
来源：http://nm.panjiajie.cn

@property 与 @x.setter 配合
来源：http://vx.haigaiapp.cn

[U30] Py：数据类
来源：http://ss.hahajie.cn

@dataclass(slots=True)
来源：http://pk.jianghongdianzi.cn

[U31] Py：单测
来源：http://ed.hnjuh.cn

python -m pytest -q
来源：http://vd.colortex.cn

[U32] Py：代码格式化
来源：http://ga.521024.cn

ruff format . && ruff check --fix .
来源：http://qy.asd995.cn

[U33] Py：打包发布
来源：http://xv.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://ey.hnjuh.cn

[U34] Py：判断编码
来源：http://ky.gzmigu.cn

chardet.detect(raw)
来源：http://ia.szsharing.cn

[U35] Py：发送邮件
来源：http://fc.lnxyls.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wu.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://ar.jianghongdianzi.cn

schedule.every(10).minutes.do(job)
来源：http://se.lnxyls.cn

[U37] Py：读写 Excel
来源：http://bi.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://le.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://we.szsharing.cn

Path(__file__).resolve().parent
来源：http://gb.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://my.szxytkj.cn

sys.stdout.isatty()
来源：http://ki.nicolike.cn

[U40] Py：打印到标准错误
来源：http://ao.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://ve.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://ua.jianghongdianzi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rs.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://fr.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ft.szsharing.cn

[U43] PHP：声明命名空间
来源：http://hv.bookmarksfly.cn

namespace App\Http;
来源：http://cc.colortex.cn

[U44] PHP：开启严格类型
来源：http://yf.haigaiapp.cn

declare(strict_types=1);
来源：http://vg.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://wg.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pq.szxytkj.cn

[U46] PHP：可空类型
来源：http://gv.huixiangedu.cn

?string $name = null
来源：http://ig.colortex.cn

[U47] PHP：联合类型
来源：http://is.huixinmuqiang.cn

int|string $id
来源：http://ec.nszjky.cn

[U48] PHP：纯枚举
来源：http://oj.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fl.yuexingan06.cn

[U49] PHP：只读属性
来源：http://hn.shxzskj.cn

public readonly string $name
来源：http://wg.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://cw.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://yl.yuexingan06.cn

[U51] PHP：数组解构
来源：http://wo.gzmigu.cn

[$a, $b] = $arr;
来源：http://hb.huixiangedu.cn

[U52] PHP：箭头函数
来源：http://qd.haigaiapp.cn

$double = fn($x) => $x * 2;
来源：http://nx.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://nb.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://iv.shxzukj.cn

[U54] PHP：空安全调用
来源：http://ke.bookmarksfly.cn

$obj?->method()
来源：http://wg.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://pb.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ct.nicolike.cn

[U56] PHP：命名参数
来源：http://sy.9csxet.cn

f(a: 1, b: 2)
来源：http://qp.hahajie.cn

[U57] PHP：字符串插值
来源：http://jn.chemitech.net.cn

"值: {$a}"
来源：http://ii.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://rd.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sw.panjiajie.cn

[U59] PHP：自定义排序
来源：http://wy.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sa.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://gu.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://th.yuntaijiaju.cn

[U61] PHP：正则
来源：http://zt.521024.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rz.hahajie.cn

[U62] PHP：日期对象
来源：http://ot.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vt.colortex.cn

[U63] PHP：文件读写
来源：http://up.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mk.asd995.cn

[U64] PHP：目录遍历
来源：http://fg.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://hb.newstarts.cn

[U65] PHP：会话
来源：http://ho.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fd.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://jq.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pk.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://lb.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gw.nszjky.cn

[U68] PHP：PDO 连接
来源：http://pn.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nl.shtwfgs.cn

[U69] PHP：PDO 预处理
来源：http://eq.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vt.huanxung.cn

[U70] PHP：PDO 事务
来源：http://pp.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://su.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://ns.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://rt.521024.cn

[U72] PHP：写错误日志
来源：http://xs.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://pf.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://rd.521024.cn

parse_ini_file("config.ini", true)
来源：http://sf.colortex.cn

[U74] PHP：读取环境变量
来源：http://um.yuexingan06.cn

getenv("APP_ENV") ?: "production"
来源：http://pr.gzmigu.cn

[U75] PHP：依赖注入
来源：http://zq.panjiajie.cn

composer require psr/container
来源：http://vm.wgjwhj.cn

[U76] PHP：简单路由
来源：http://nq.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fy.lnxyls.cn

[U77] PHP：模板渲染
来源：http://iv.huixinmuqiang.cn

composer require twig/twig
来源：http://nz.nszjky.cn

[U78] PHP：单元测试
来源：http://hn.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://lp.szxytkj.cn

[U79] PHP：静态分析
来源：http://od.lnxyls.cn

composer require --dev phpstan/phpstan
来源：http://fw.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://hs.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ex.521024.cn

[U81] JS：初始化项目
来源：http://te.panjiajie.cn

npm init -y;  npm i express
来源：http://po.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://eb.huixinmuqiang.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fz.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://ml.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bq.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://oa.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ju.shxzskj.cn

[U85] JS：可选链
来源：http://cr.nicolike.cn

a?.b?.c
来源：http://wc.shxzukj.cn

[U86] JS：空值合并
来源：http://ny.bookmarksfly.cn

a ?? b
来源：http://ml.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://jz.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://zq.9csxet.cn

[U88] JS：对象展开合并
来源：http://kn.muxihuayi.cn

{ ...a, ...b }
来源：http://gd.shxzukj.cn

[U89] JS：数组去重
来源：http://du.asd995.cn

[...new Set(arr)]
来源：http://cq.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://af.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://nn.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://jp.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://go.yuexingan06.cn

[U92] JS：深拷贝
来源：http://al.szxytkj.cn

structuredClone(obj)
来源：http://sb.gzmigu.cn

[U93] JS：模板字符串
来源：http://qh.wgjwhj.cn

`共 ${n} 条`
来源：http://wv.shxzskj.cn

[U94] JS：箭头函数
来源：http://wd.hahajie.cn

const double = x => x * 2;
来源：http://tv.9csxet.cn

[U95] JS：Promise 包装
来源：http://ci.chemitech.net.cn

new Promise((resolve, reject) => {})
来源：http://qg.szsharing.cn

[U96] JS：async/await 与异常
来源：http://wn.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://is.szsharing.cn

[U97] JS：并发请求
来源：http://ft.wgjwhj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ql.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://eu.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qf.bjjhwx.cn

[U99] JS：事件监听
来源：http://vy.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://gs.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://pj.shxzskj.cn

document.querySelector(".item")
来源：http://hq.jctech888.com.cn

[U101] JS：classList 操作
来源：http://ra.shtwfgs.cn

el.classList.toggle("active")
来源：http://cz.bookmarksfly.cn

[U102] JS：本地存储
来源：http://ah.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://om.bjjhwx.cn

[U103] JS：定时器
来源：http://oj.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lb.lnxyls.cn

[U104] JS：防抖
来源：http://eb.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fm.haigaiapp.cn

[U105] JS：节流
来源：http://na.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xe.hahajie.cn

[U106] JS：日期格式化
来源：http://td.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ch.szsharing.cn

[U107] JS：数字千分位
来源：http://qr.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wm.shxzskj.cn

[U108] JS：随机整数
来源：http://zy.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xo.newstarts.cn

[U109] JS：数组分组
来源：http://cx.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://yd.yuexingan06.cn

[U110] JS：数组分块
来源：http://wm.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zy.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://ke.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://rx.szxytkj.cn

[U112] JS：字符串补位
来源：http://uf.lnxyls.cn

"7".padStart(3, "0")
来源：http://pg.szxytkj.cn

[U113] JS：正则替换全部
来源：http://zd.521024.cn

s.replaceAll("a", "b")
来源：http://vj.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://pc.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hj.chemitech.net.cn

[U115] JS：生成 UUID
来源：http://zp.hnjuh.cn

crypto.randomUUID()
来源：http://qo.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://jn.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://et.huixiangedu.cn

[U117] JS：单元测试
来源：http://se.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://oi.521024.cn

[U118] JS：开发服务器
来源：http://gp.521024.cn

npm i -D vite;  npx vite
来源：http://ho.shtwfgs.cn

[U119] JS：生产构建
来源：http://bd.9csxet.cn

npx vite build
来源：http://ca.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://gd.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://oa.yuexingan06.cn

================================================================================
来源：http://bv.huixinmuqiang.cn

统计汇总
来源：http://vz.jctech888.com.cn

================================================================================
来源：http://ww.nszjky.cn

按语言统计（条）：
来源：http://tk.asd995.cn

Python ......... 252
来源：http://pu.chemitech.net.cn

PHP ............ 252
来源：http://nu.bookmarksfly.cn

JavaScript ..... 252
来源：http://tq.muxihuayi.cn

TypeScript ..... 212
来源：http://tx.wgjwhj.cn

Java ........... 212
来源：http://dt.nszjky.cn

Go ............. 212
来源：http://cs.haigaiapp.cn

Ruby ........... 212
来源：http://jb.bjjhwx.cn

C# ............. 212
来源：http://wa.newstarts.cn

C .............. 30
来源：http://pd.shxzukj.cn

C++ ............ 30
来源：http://xj.nicolike.cn

SQL ............ 90
来源：http://pm.wgjwhj.cn

Bash ........... 80
来源：http://tj.jctech888.com.cn

Kotlin ......... 15
来源：http://hr.panjiajie.cn

Swift .......... 15
来源：http://co.lnxyls.cn

Lua ............ 10
来源：http://bs.huanxung.cn

Perl ........... 10
来源：http://vd.jctech888.com.cn

Scala .......... 10
来源：http://cr.huixiangedu.cn

------------------------------------
来源：http://xp.yuexingan06.cn

合计 ........... 2106 条
来源：http://ls.asd995.cn

按章节统计：
来源：http://vv.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://um.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ti.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ke.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zn.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://or.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dx.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sn.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lk.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bu.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ti.jianghongdianzi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lm.jianghongdianzi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xw.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wo.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eh.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pp.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rq.asd995.cn

Q SQL 专题                              90
来源：http://sn.yuexingan06.cn

R Bash 专题                             80
来源：http://du.nicolike.cn

S C / C++ 专题                          60
来源：http://dg.chemitech.net.cn

T 其他语言补充                          60
来源：http://zh.chemitech.net.cn

U 高频实用片段                         120
来源：http://lt.chemitech.net.cn

------------------------------------
来源：http://iw.hahajie.cn

合计                                  2106 条
来源：http://ly.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://yi.shtwfgs.cn

使用提醒
来源：http://cq.huanxung.cn

--------------------------------------------------------------------------------
来源：http://kn.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zt.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://go.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fx.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lr.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://od.shxzskj.cn

—— 文件结束 ——
来源：http://zu.hahajie.cn

================================================================================
来源：http://rs.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://jv.521024.cn

Common Programming Examples Cheat Book
来源：http://ue.yuexingan06.cn

================================================================================
来源：http://hh.colortex.cn

【收录内容】
来源：http://ur.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ao.panjiajie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jz.shtwfgs.cn

SQL · Bash · C · C++
来源：http://bl.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dp.newstarts.cn

【使用说明】
来源：http://pe.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ay.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lr.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uc.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ko.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rs.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zs.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lx.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fu.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://va.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aw.nszjky.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://te.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wc.wgjwhj.cn

【文件统计】
来源：http://hc.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pn.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://wa.bjjhwx.cn

目  录
来源：http://ss.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://ge.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ky.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pt.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gi.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uw.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kq.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cy.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ca.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ga.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hg.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qe.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ym.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ut.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gi.nszjky.cn


<!-- 参考信息 -->