代发 wailian999

[U19] Py：正则替换带回调
来源：http://si.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zc.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://zw.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://ix.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://pd.521024.cn

@contextlib.contextmanager
来源：http://sy.nicolike.cn

[U22] Py：矩阵转置
来源：http://br.yuexingan06.cn

list(zip(*m))
来源：http://ht.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://mf.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://to.shxzukj.cn

[U24] Py：路径操作
来源：http://nf.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lf.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://qb.panjiajie.cn

csv.DictReader(f)
来源：http://as.huanxung.cn

[U26] Py：并发下载
来源：http://it.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tj.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://io.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://so.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://fs.wgjwhj.cn

UserId = int
来源：http://ki.nicolike.cn

[U29] Py：属性校验
来源：http://hw.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://mp.yuexingan06.cn

[U30] Py：数据类
来源：http://se.yuexingan06.cn

@dataclass(slots=True)
来源：http://os.jctech888.com.cn

[U31] Py：单测
来源：http://wc.9csxet.cn

python -m pytest -q
来源：http://rx.shxzskj.cn

[U32] Py：代码格式化
来源：http://us.nicolike.cn

ruff format . && ruff check --fix .
来源：http://in.wgjwhj.cn

[U33] Py：打包发布
来源：http://ml.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://id.jctech888.com.cn

[U34] Py：判断编码
来源：http://ul.hahajie.cn

chardet.detect(raw)
来源：http://eo.521024.cn

[U35] Py：发送邮件
来源：http://yw.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wz.newstarts.cn

[U36] Py：定时任务
来源：http://ld.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://me.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://ae.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ab.shtwfgs.cn

[U38] Py：获取脚本所在目录
来源：http://qf.shxzskj.cn

Path(__file__).resolve().parent
来源：http://ns.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://ip.jctech888.com.cn

sys.stdout.isatty()
来源：http://zc.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://bq.jctech888.com.cn

print("err", file=sys.stderr)
来源：http://sx.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://vi.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vf.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://wn.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nj.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://rt.yuntaijiaju.cn

namespace App\Http;
来源：http://qh.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://tl.521024.cn

declare(strict_types=1);
来源：http://xf.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://rx.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vc.521024.cn

[U46] PHP：可空类型
来源：http://ph.shtwfgs.cn

?string $name = null
来源：http://vc.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://mg.panjiajie.cn

int|string $id
来源：http://jl.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://su.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ks.yuexingan06.cn

[U49] PHP：只读属性
来源：http://cp.huixinmuqiang.cn

public readonly string $name
来源：http://dr.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://fl.9csxet.cn

public function __construct(private int $id) {}
来源：http://ci.hahajie.cn

[U51] PHP：数组解构
来源：http://uq.huixiangedu.cn

[$a, $b] = $arr;
来源：http://nu.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://jw.yuexingan06.cn

$double = fn($x) => $x * 2;
来源：http://iw.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://fa.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://ul.9csxet.cn

[U54] PHP：空安全调用
来源：http://lu.newstarts.cn

$obj?->method()
来源：http://cx.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://od.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vg.nszjky.cn

[U56] PHP：命名参数
来源：http://gq.asd995.cn

f(a: 1, b: 2)
来源：http://em.9csxet.cn

[U57] PHP：字符串插值
来源：http://tu.jianghongdianzi.cn

"值: {$a}"
来源：http://at.gzmigu.cn

[U58] PHP：数组三件套
来源：http://eu.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ja.asd995.cn

[U59] PHP：自定义排序
来源：http://iv.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jb.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://ut.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zt.newstarts.cn

[U61] PHP：正则
来源：http://kj.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ck.szsharing.cn

[U62] PHP：日期对象
来源：http://ee.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sz.jctech888.com.cn

[U63] PHP：文件读写
来源：http://rf.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zs.panjiajie.cn

[U64] PHP：目录遍历
来源：http://yu.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://nd.jianghongdianzi.cn

[U65] PHP：会话
来源：http://na.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qo.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://dj.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zy.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://jb.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ae.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://kd.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://md.bookmarksfly.cn

[U69] PHP：PDO 预处理
来源：http://fh.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dr.hahajie.cn

[U70] PHP：PDO 事务
来源：http://xi.szsharing.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://of.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://xd.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://us.nszjky.cn

[U72] PHP：写错误日志
来源：http://sx.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://jl.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://pv.newstarts.cn

parse_ini_file("config.ini", true)
来源：http://vb.nicolike.cn

[U74] PHP：读取环境变量
来源：http://xa.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://ub.shxzukj.cn

[U75] PHP：依赖注入
来源：http://fr.huixiangedu.cn

composer require psr/container
来源：http://ol.newstarts.cn

[U76] PHP：简单路由
来源：http://sy.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oi.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://fe.huixiangedu.cn

composer require twig/twig
来源：http://de.nszjky.cn

[U78] PHP：单元测试
来源：http://go.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://zh.muxihuayi.cn

[U79] PHP：静态分析
来源：http://dl.huixinmuqiang.cn

composer require --dev phpstan/phpstan
来源：http://xe.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://bj.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tk.shxzukj.cn

[U81] JS：初始化项目
来源：http://og.hnjuh.cn

npm init -y;  npm i express
来源：http://es.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://de.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bx.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://oe.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://io.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://fy.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vx.nszjky.cn

[U85] JS：可选链
来源：http://wd.muxihuayi.cn

a?.b?.c
来源：http://wh.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://xw.521024.cn

a ?? b
来源：http://tu.521024.cn

[U87] JS：解构默认值
来源：http://bm.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://ca.nicolike.cn

[U88] JS：对象展开合并
来源：http://yv.huixiangedu.cn

{ ...a, ...b }
来源：http://hz.bookmarksfly.cn

[U89] JS：数组去重
来源：http://ph.szxytkj.cn

[...new Set(arr)]
来源：http://tr.nicolike.cn

[U90] JS：数字数组排序
来源：http://bg.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://lw.hahajie.cn

[U91] JS：对象键值遍历
来源：http://rd.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ai.newstarts.cn

[U92] JS：深拷贝
来源：http://ft.9csxet.cn

structuredClone(obj)
来源：http://nx.chemitech.net.cn

[U93] JS：模板字符串
来源：http://tl.bookmarksfly.cn

`共 ${n} 条`
来源：http://ph.newstarts.cn

[U94] JS：箭头函数
来源：http://jh.huanxung.cn

const double = x => x * 2;
来源：http://pa.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://kb.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://td.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://tt.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://em.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://cv.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zl.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://aa.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://he.panjiajie.cn

[U99] JS：事件监听
来源：http://ah.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://vg.asd995.cn

[U100] JS：DOM 查询
来源：http://ik.bookmarksfly.cn

document.querySelector(".item")
来源：http://hq.newstarts.cn

[U101] JS：classList 操作
来源：http://ko.szsharing.cn

el.classList.toggle("active")
来源：http://kb.shxzukj.cn

[U102] JS：本地存储
来源：http://bg.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://me.wgjwhj.cn

[U103] JS：定时器
来源：http://ex.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ue.newstarts.cn

[U104] JS：防抖
来源：http://ij.shtwfgs.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ik.shxzukj.cn

[U105] JS：节流
来源：http://ud.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sz.9csxet.cn

[U106] JS：日期格式化
来源：http://hr.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kz.colortex.cn

[U107] JS：数字千分位
来源：http://jv.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ke.huanxung.cn

[U108] JS：随机整数
来源：http://sz.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vf.9csxet.cn

[U109] JS：数组分组
来源：http://hj.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://rg.huanxung.cn

[U110] JS：数组分块
来源：http://cx.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mu.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://yp.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://up.huanxung.cn

[U112] JS：字符串补位
来源：http://ih.nszjky.cn

"7".padStart(3, "0")
来源：http://yi.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://mi.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://ho.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://zs.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qc.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://aq.huanxung.cn

crypto.randomUUID()
来源：http://ho.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://qq.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://af.shtwfgs.cn

[U117] JS：单元测试
来源：http://fx.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://id.gzmigu.cn

[U118] JS：开发服务器
来源：http://oz.colortex.cn

npm i -D vite;  npx vite
来源：http://jr.gzmigu.cn

[U119] JS：生产构建
来源：http://al.521024.cn

npx vite build
来源：http://uu.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://ub.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://sh.hahajie.cn

================================================================================
来源：http://co.szxytkj.cn

统计汇总
来源：http://ua.shxzskj.cn

================================================================================
来源：http://ur.chemitech.net.cn

按语言统计（条）：
来源：http://sn.huixiangedu.cn

Python ......... 252
来源：http://rg.asd995.cn

PHP ............ 252
来源：http://je.hnjuh.cn

JavaScript ..... 252
来源：http://ti.haigaiapp.cn

TypeScript ..... 212
来源：http://bm.huixinmuqiang.cn

Java ........... 212
来源：http://jx.shxzukj.cn

Go ............. 212
来源：http://tq.huixinmuqiang.cn

Ruby ........... 212
来源：http://ud.bjjhwx.cn

C# ............. 212
来源：http://dk.haigaiapp.cn

C .............. 30
来源：http://eq.shxzukj.cn

C++ ............ 30
来源：http://ky.9csxet.cn

SQL ............ 90
来源：http://ro.hahajie.cn

Bash ........... 80
来源：http://br.wgjwhj.cn

Kotlin ......... 15
来源：http://km.huanxung.cn

Swift .......... 15
来源：http://wu.colortex.cn

Lua ............ 10
来源：http://md.newstarts.cn

Perl ........... 10
来源：http://ch.bjjhwx.cn

Scala .......... 10
来源：http://fu.chemitech.net.cn

------------------------------------
来源：http://jh.shtwfgs.cn

合计 ........... 2106 条
来源：http://wd.521024.cn

按章节统计：
来源：http://nw.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kl.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fr.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jl.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ku.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pf.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tl.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://or.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qj.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fo.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zg.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wn.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mz.wgjwhj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fa.muxihuayi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yw.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kr.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ak.muxihuayi.cn

Q SQL 专题                              90
来源：http://jf.asd995.cn

R Bash 专题                             80
来源：http://oc.colortex.cn

S C / C++ 专题                          60
来源：http://sm.chemitech.net.cn

T 其他语言补充                          60
来源：http://vk.bookmarksfly.cn

U 高频实用片段                         120
来源：http://ey.muxihuayi.cn

------------------------------------
来源：http://ee.hahajie.cn

合计                                  2106 条
来源：http://ev.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://wp.nszjky.cn

使用提醒
来源：http://vs.9csxet.cn

--------------------------------------------------------------------------------
来源：http://wz.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tl.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://br.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://db.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gp.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ze.colortex.cn

—— 文件结束 ——
来源：http://fg.nicolike.cn

================================================================================
来源：http://wh.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://ho.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://lf.yuexingan06.cn

================================================================================
来源：http://ig.shxzukj.cn

【收录内容】
来源：http://ay.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fr.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nu.shxzskj.cn

SQL · Bash · C · C++
来源：http://co.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vo.chemitech.net.cn

【使用说明】
来源：http://pr.nicolike.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kb.bookmarksfly.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hr.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wo.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vx.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://oz.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vq.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gi.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yw.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qs.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xt.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gv.asd995.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qm.bookmarksfly.cn

【文件统计】
来源：http://bv.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gx.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://rc.shxzukj.cn

目  录
来源：http://cj.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://iz.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qm.hnjuh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dq.haigaiapp.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pm.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kg.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xu.shxzukj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hb.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jb.colortex.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://be.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vq.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fv.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hq.szxytkj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ow.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dk.haigaiapp.cn


<!-- 参考信息 -->