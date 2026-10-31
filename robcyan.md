代发 wailian999

[U07] Py：反转字典键值
来源：http://ea.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://mj.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://nk.muxihuayi.cn

[y for x in nested for y in x]
来源：http://sz.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://fm.newstarts.cn

max(d, key=d.get)
来源：http://ap.szsharing.cn

[U10] Py：按值排序字典
来源：http://fk.yuntaijiaju.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://do.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://bp.shtwfgs.cn

(x * 2 for x in arr)
来源：http://ri.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pa.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://fe.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://gu.asd995.cn

deque(maxlen=10)
来源：http://ee.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://ml.chemitech.net.cn

defaultdict(list)
来源：http://ok.newstarts.cn

[U15] Py：高精度计时
来源：http://hr.asd995.cn

t = time.perf_counter()
来源：http://zy.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://ru.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yq.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://fx.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://dn.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://qs.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://mj.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://lo.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xm.colortex.cn

[U20] Py：缓存函数结果
来源：http://xu.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://qn.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://ka.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://ld.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://me.bjjhwx.cn

list(zip(*m))
来源：http://dd.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://zp.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sx.huixiangedu.cn

[U24] Py：路径操作
来源：http://kt.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rs.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://bl.9csxet.cn

csv.DictReader(f)
来源：http://ng.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://uj.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mf.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://yr.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://rq.colortex.cn

[U28] Py：类型别名
来源：http://mp.wgjwhj.cn

UserId = int
来源：http://hl.lnxyls.cn

[U29] Py：属性校验
来源：http://io.hnjuh.cn

@property 与 @x.setter 配合
来源：http://mp.panjiajie.cn

[U30] Py：数据类
来源：http://vu.nszjky.cn

@dataclass(slots=True)
来源：http://iw.shxzskj.cn

[U31] Py：单测
来源：http://na.huanxung.cn

python -m pytest -q
来源：http://oe.gzmigu.cn

[U32] Py：代码格式化
来源：http://kl.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://gj.asd995.cn

[U33] Py：打包发布
来源：http://mk.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://fv.huanxung.cn

[U34] Py：判断编码
来源：http://oo.lnxyls.cn

chardet.detect(raw)
来源：http://bt.huanxung.cn

[U35] Py：发送邮件
来源：http://dl.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bi.9csxet.cn

[U36] Py：定时任务
来源：http://mp.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://oo.shxzskj.cn

[U37] Py：读写 Excel
来源：http://vu.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pd.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://hd.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://cj.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://dl.asd995.cn

sys.stdout.isatty()
来源：http://ao.szsharing.cn

[U40] Py：打印到标准错误
来源：http://tl.szxytkj.cn

print("err", file=sys.stderr)
来源：http://wu.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://jr.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sh.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://mn.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uc.colortex.cn

[U43] PHP：声明命名空间
来源：http://ow.jctech888.com.cn

namespace App\Http;
来源：http://xc.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://qm.hnjuh.cn

declare(strict_types=1);
来源：http://pt.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://sb.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rg.shxzukj.cn

[U46] PHP：可空类型
来源：http://xq.gzmigu.cn

?string $name = null
来源：http://lk.szxytkj.cn

[U47] PHP：联合类型
来源：http://lv.bjjhwx.cn

int|string $id
来源：http://sk.gzmigu.cn

[U48] PHP：纯枚举
来源：http://cu.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iz.panjiajie.cn

[U49] PHP：只读属性
来源：http://zi.newstarts.cn

public readonly string $name
来源：http://rv.521024.cn

[U50] PHP：构造器属性提升
来源：http://hb.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://ze.muxihuayi.cn

[U51] PHP：数组解构
来源：http://tp.nszjky.cn

[$a, $b] = $arr;
来源：http://bp.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://de.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://ns.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://bb.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://cy.szsharing.cn

[U54] PHP：空安全调用
来源：http://rp.asd995.cn

$obj?->method()
来源：http://jm.gzmigu.cn

[U55] PHP：match 表达式
来源：http://bm.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wm.521024.cn

[U56] PHP：命名参数
来源：http://bw.szxytkj.cn

f(a: 1, b: 2)
来源：http://bb.colortex.cn

[U57] PHP：字符串插值
来源：http://es.hnjuh.cn

"值: {$a}"
来源：http://xs.hahajie.cn

[U58] PHP：数组三件套
来源：http://tp.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rp.nszjky.cn

[U59] PHP：自定义排序
来源：http://wq.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lf.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://nl.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tm.asd995.cn

[U61] PHP：正则
来源：http://cc.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jj.szsharing.cn

[U62] PHP：日期对象
来源：http://cx.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jn.szxytkj.cn

[U63] PHP：文件读写
来源：http://yc.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zr.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://bo.nszjky.cn

glob("dir/*.php");  scandir("dir");
来源：http://xu.bookmarksfly.cn

[U65] PHP：会话
来源：http://qf.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zm.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://cd.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wf.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://jf.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tt.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://cr.nszjky.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uh.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://wg.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://za.huanxung.cn

[U70] PHP：PDO 事务
来源：http://op.jctech888.com.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gm.huixiangedu.cn

[U71] PHP：抛出异常
来源：http://vp.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://xy.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://sf.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://zn.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://yf.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://jw.huanxung.cn

[U74] PHP：读取环境变量
来源：http://zm.muxihuayi.cn

getenv("APP_ENV") ?: "production"
来源：http://kr.521024.cn

[U75] PHP：依赖注入
来源：http://gp.jctech888.com.cn

composer require psr/container
来源：http://nc.asd995.cn

[U76] PHP：简单路由
来源：http://sb.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ak.szsharing.cn

[U77] PHP：模板渲染
来源：http://xt.bookmarksfly.cn

composer require twig/twig
来源：http://yl.newstarts.cn

[U78] PHP：单元测试
来源：http://ga.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://pe.shtwfgs.cn

[U79] PHP：静态分析
来源：http://ej.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://xk.huanxung.cn

[U80] PHP：代码规范修复
来源：http://ci.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://md.gzmigu.cn

[U81] JS：初始化项目
来源：http://et.hahajie.cn

npm init -y;  npm i express
来源：http://vr.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://zs.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gh.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://ck.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hr.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://ot.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ld.muxihuayi.cn

[U85] JS：可选链
来源：http://zk.haigaiapp.cn

a?.b?.c
来源：http://on.shxzukj.cn

[U86] JS：空值合并
来源：http://fp.muxihuayi.cn

a ?? b
来源：http://xn.nicolike.cn

[U87] JS：解构默认值
来源：http://fr.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://ml.panjiajie.cn

[U88] JS：对象展开合并
来源：http://vf.chemitech.net.cn

{ ...a, ...b }
来源：http://ui.szxytkj.cn

[U89] JS：数组去重
来源：http://va.newstarts.cn

[...new Set(arr)]
来源：http://zz.huanxung.cn

[U90] JS：数字数组排序
来源：http://ch.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://an.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://bl.nszjky.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ic.lnxyls.cn

[U92] JS：深拷贝
来源：http://pf.wgjwhj.cn

structuredClone(obj)
来源：http://xe.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://ff.gzmigu.cn

`共 ${n} 条`
来源：http://oy.shtwfgs.cn

[U94] JS：箭头函数
来源：http://xb.nicolike.cn

const double = x => x * 2;
来源：http://zs.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://ed.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://xz.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://wj.wgjwhj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://za.bookmarksfly.cn

[U97] JS：并发请求
来源：http://gn.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qi.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://dk.huixinmuqiang.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rr.newstarts.cn

[U99] JS：事件监听
来源：http://eg.huanxung.cn

el.addEventListener("click", e => {})
来源：http://sh.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://zt.yuexingan06.cn

document.querySelector(".item")
来源：http://gd.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://mn.lnxyls.cn

el.classList.toggle("active")
来源：http://jg.gzmigu.cn

[U102] JS：本地存储
来源：http://gk.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ah.chemitech.net.cn

[U103] JS：定时器
来源：http://zh.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://db.lnxyls.cn

[U104] JS：防抖
来源：http://ja.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kj.panjiajie.cn

[U105] JS：节流
来源：http://zk.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zz.chemitech.net.cn

[U106] JS：日期格式化
来源：http://so.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vr.newstarts.cn

[U107] JS：数字千分位
来源：http://yi.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hx.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://pf.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dm.bjjhwx.cn

[U109] JS：数组分组
来源：http://uk.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://bd.nicolike.cn

[U110] JS：数组分块
来源：http://yz.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://en.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://nz.521024.cn

new Map(Object.entries(obj))
来源：http://bu.nicolike.cn

[U112] JS：字符串补位
来源：http://zd.hnjuh.cn

"7".padStart(3, "0")
来源：http://ps.shxzukj.cn

[U113] JS：正则替换全部
来源：http://el.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://ki.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://xw.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ln.9csxet.cn

[U115] JS：生成 UUID
来源：http://bx.huixinmuqiang.cn

crypto.randomUUID()
来源：http://ls.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://mw.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://gh.lnxyls.cn

[U117] JS：单元测试
来源：http://xp.panjiajie.cn

npm i -D vitest;  npx vitest
来源：http://vp.shtwfgs.cn

[U118] JS：开发服务器
来源：http://wy.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://sq.shxzukj.cn

[U119] JS：生产构建
来源：http://bv.bookmarksfly.cn

npx vite build
来源：http://pf.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://vu.colortex.cn

import.meta.env.VITE_API_URL
来源：http://ml.nszjky.cn

================================================================================
来源：http://te.shtwfgs.cn

统计汇总
来源：http://aq.jctech888.com.cn

================================================================================
来源：http://lk.huixinmuqiang.cn

按语言统计（条）：
来源：http://qe.huixiangedu.cn

Python ......... 252
来源：http://fl.chemitech.net.cn

PHP ............ 252
来源：http://rd.shxzskj.cn

JavaScript ..... 252
来源：http://ll.huixinmuqiang.cn

TypeScript ..... 212
来源：http://ta.gzmigu.cn

Java ........... 212
来源：http://so.lnxyls.cn

Go ............. 212
来源：http://yg.szsharing.cn

Ruby ........... 212
来源：http://yk.huixiangedu.cn

C# ............. 212
来源：http://oi.haigaiapp.cn

C .............. 30
来源：http://di.nicolike.cn

C++ ............ 30
来源：http://qw.nicolike.cn

SQL ............ 90
来源：http://qg.yuntaijiaju.cn

Bash ........... 80
来源：http://jd.colortex.cn

Kotlin ......... 15
来源：http://dh.gzmigu.cn

Swift .......... 15
来源：http://kk.bookmarksfly.cn

Lua ............ 10
来源：http://aa.haigaiapp.cn

Perl ........... 10
来源：http://fw.muxihuayi.cn

Scala .......... 10
来源：http://um.bjjhwx.cn

------------------------------------
来源：http://em.huixiangedu.cn

合计 ........... 2106 条
来源：http://ae.521024.cn

按章节统计：
来源：http://zd.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ia.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uh.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fm.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ze.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aj.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dn.shtwfgs.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ji.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qx.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fl.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://et.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rz.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fc.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jm.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eo.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vc.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tx.haigaiapp.cn

Q SQL 专题                              90
来源：http://qz.nicolike.cn

R Bash 专题                             80
来源：http://wt.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://ea.gzmigu.cn

T 其他语言补充                          60
来源：http://we.nicolike.cn

U 高频实用片段                         120
来源：http://mc.yuexingan06.cn

------------------------------------
来源：http://mw.huixinmuqiang.cn

合计                                  2106 条
来源：http://ly.nszjky.cn

--------------------------------------------------------------------------------
来源：http://tc.nicolike.cn

使用提醒
来源：http://qb.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://mc.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oq.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kb.shxzskj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ap.huanxung.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xe.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ij.shxzukj.cn

—— 文件结束 ——
来源：http://se.521024.cn

================================================================================
来源：http://dg.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://fu.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://vi.muxihuayi.cn

================================================================================
来源：http://ii.nicolike.cn

【收录内容】
来源：http://rs.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zh.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://se.shtwfgs.cn

SQL · Bash · C · C++
来源：http://ai.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qq.colortex.cn

【使用说明】
来源：http://uf.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lc.asd995.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yq.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lh.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jh.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pr.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hu.gzmigu.cn


<!-- 参考信息 -->