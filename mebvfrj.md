代发 wailian999

[U09] Py：字典取最大值的键
来源：http://th.nicolike.cn

max(d, key=d.get)
来源：http://yj.szxytkj.cn

[U10] Py：按值排序字典
来源：http://ob.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sf.shxzskj.cn

[U11] Py：生成器表达式
来源：http://zj.lnxyls.cn

(x * 2 for x in arr)
来源：http://zr.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sn.hahajie.cn

Counter(arr).most_common(3)
来源：http://by.szsharing.cn

[U13] Py：固定长度队列
来源：http://tw.panjiajie.cn

deque(maxlen=10)
来源：http://qq.hahajie.cn

[U14] Py：分组收集到列表
来源：http://uy.gzmigu.cn

defaultdict(list)
来源：http://yb.haigaiapp.cn

[U15] Py：高精度计时
来源：http://nq.shtwfgs.cn

t = time.perf_counter()
来源：http://gj.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://ub.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ys.chemitech.net.cn

[U17] Py：初始化日志
来源：http://iu.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://jj.chemitech.net.cn

[U18] Py：预编译正则
来源：http://fv.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://yg.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://wz.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://on.huanxung.cn

[U20] Py：缓存函数结果
来源：http://kz.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://gt.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://fw.nicolike.cn

@contextlib.contextmanager
来源：http://xl.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://ki.shxzukj.cn

list(zip(*m))
来源：http://vb.szsharing.cn

[U23] Py：分块读取大文件
来源：http://op.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ih.asd995.cn

[U24] Py：路径操作
来源：http://zx.hnjuh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kz.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://id.shxzskj.cn

csv.DictReader(f)
来源：http://ox.shxzukj.cn

[U26] Py：并发下载
来源：http://zc.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sg.newstarts.cn

[U27] Py：异步 HTTP
来源：http://kn.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://ht.szsharing.cn

[U28] Py：类型别名
来源：http://kz.nszjky.cn

UserId = int
来源：http://rq.hahajie.cn

[U29] Py：属性校验
来源：http://wz.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://lz.521024.cn

[U30] Py：数据类
来源：http://jx.9csxet.cn

@dataclass(slots=True)
来源：http://hq.hnjuh.cn

[U31] Py：单测
来源：http://xi.huixiangedu.cn

python -m pytest -q
来源：http://sr.yuexingan06.cn

[U32] Py：代码格式化
来源：http://zz.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://xf.bookmarksfly.cn

[U33] Py：打包发布
来源：http://ij.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://im.bookmarksfly.cn

[U34] Py：判断编码
来源：http://wc.jctech888.com.cn

chardet.detect(raw)
来源：http://cy.shxzukj.cn

[U35] Py：发送邮件
来源：http://ij.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xg.chemitech.net.cn

[U36] Py：定时任务
来源：http://si.521024.cn

schedule.every(10).minutes.do(job)
来源：http://lx.9csxet.cn

[U37] Py：读写 Excel
来源：http://mq.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mx.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://jw.szsharing.cn

Path(__file__).resolve().parent
来源：http://cq.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://jd.szsharing.cn

sys.stdout.isatty()
来源：http://gm.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://zh.hahajie.cn

print("err", file=sys.stderr)
来源：http://ka.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://zv.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ui.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ib.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wj.jctech888.com.cn

[U43] PHP：声明命名空间
来源：http://id.bookmarksfly.cn

namespace App\Http;
来源：http://wq.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://xh.huanxung.cn

declare(strict_types=1);
来源：http://yd.yuexingan06.cn

[U45] PHP：类型声明与返回类型
来源：http://jr.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tf.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://tc.nszjky.cn

?string $name = null
来源：http://mo.newstarts.cn

[U47] PHP：联合类型
来源：http://ge.9csxet.cn

int|string $id
来源：http://mb.gzmigu.cn

[U48] PHP：纯枚举
来源：http://bz.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fa.panjiajie.cn

[U49] PHP：只读属性
来源：http://mk.nicolike.cn

public readonly string $name
来源：http://xc.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://yu.wgjwhj.cn

public function __construct(private int $id) {}
来源：http://ad.lnxyls.cn

[U51] PHP：数组解构
来源：http://dd.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://qy.hnjuh.cn

[U52] PHP：箭头函数
来源：http://wq.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://xn.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://po.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://tr.asd995.cn

[U54] PHP：空安全调用
来源：http://xp.huixinmuqiang.cn

$obj?->method()
来源：http://yn.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://tt.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vd.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://yj.gzmigu.cn

f(a: 1, b: 2)
来源：http://ci.9csxet.cn

[U57] PHP：字符串插值
来源：http://ns.szsharing.cn

"值: {$a}"
来源：http://fz.gzmigu.cn

[U58] PHP：数组三件套
来源：http://mg.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vt.gzmigu.cn

[U59] PHP：自定义排序
来源：http://yg.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xv.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://xb.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ca.nszjky.cn

[U61] PHP：正则
来源：http://xj.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ti.shtwfgs.cn

[U62] PHP：日期对象
来源：http://xs.huixiangedu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wo.lnxyls.cn

[U63] PHP：文件读写
来源：http://ad.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ud.hahajie.cn

[U64] PHP：目录遍历
来源：http://ha.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://iu.muxihuayi.cn

[U65] PHP：会话
来源：http://xx.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ee.haigaiapp.cn

[U66] PHP：设置 Cookie
来源：http://nx.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ri.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://zn.521024.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://id.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://js.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://co.colortex.cn

[U69] PHP：PDO 预处理
来源：http://mu.bjjhwx.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yu.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://fj.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pg.521024.cn

[U71] PHP：抛出异常
来源：http://se.yuntaijiaju.cn

throw new RuntimeException("失败", 500);
来源：http://um.yuntaijiaju.cn

[U72] PHP：写错误日志
来源：http://ek.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://zq.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://pb.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://vy.asd995.cn

[U74] PHP：读取环境变量
来源：http://fx.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://zd.asd995.cn

[U75] PHP：依赖注入
来源：http://br.huixinmuqiang.cn

composer require psr/container
来源：http://lw.panjiajie.cn

[U76] PHP：简单路由
来源：http://hr.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cj.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://cm.szsharing.cn

composer require twig/twig
来源：http://fh.shxzskj.cn

[U78] PHP：单元测试
来源：http://cq.muxihuayi.cn

composer require --dev phpunit/phpunit
来源：http://uw.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://dl.huanxung.cn

composer require --dev phpstan/phpstan
来源：http://kq.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://be.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rk.szsharing.cn

[U81] JS：初始化项目
来源：http://lg.wgjwhj.cn

npm init -y;  npm i express
来源：http://rl.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://np.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yt.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://eg.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://em.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://ni.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uu.jianghongdianzi.cn

[U85] JS：可选链
来源：http://nr.asd995.cn

a?.b?.c
来源：http://mx.haigaiapp.cn

[U86] JS：空值合并
来源：http://bk.huixinmuqiang.cn

a ?? b
来源：http://mt.shtwfgs.cn

[U87] JS：解构默认值
来源：http://ye.huixiangedu.cn

const { a = 1, b = 2 } = obj;
来源：http://bd.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://jq.hahajie.cn

{ ...a, ...b }
来源：http://lp.bjjhwx.cn

[U89] JS：数组去重
来源：http://aq.bookmarksfly.cn

[...new Set(arr)]
来源：http://vs.yuexingan06.cn

[U90] JS：数字数组排序
来源：http://mg.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://be.9csxet.cn

[U91] JS：对象键值遍历
来源：http://da.colortex.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cj.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://tx.bjjhwx.cn

structuredClone(obj)
来源：http://qe.colortex.cn

[U93] JS：模板字符串
来源：http://hc.shxzskj.cn

`共 ${n} 条`
来源：http://im.gzmigu.cn

[U94] JS：箭头函数
来源：http://ws.hnjuh.cn

const double = x => x * 2;
来源：http://so.jctech888.com.cn

[U95] JS：Promise 包装
来源：http://hp.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://hc.nicolike.cn

[U96] JS：async/await 与异常
来源：http://qi.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gc.panjiajie.cn

[U97] JS：并发请求
来源：http://mf.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tj.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://fw.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bp.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://zt.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://vv.shxzukj.cn

[U100] JS：DOM 查询
来源：http://ye.hnjuh.cn

document.querySelector(".item")
来源：http://oj.muxihuayi.cn

[U101] JS：classList 操作
来源：http://cr.shxzukj.cn

el.classList.toggle("active")
来源：http://jp.shtwfgs.cn

[U102] JS：本地存储
来源：http://mp.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lk.lnxyls.cn

[U103] JS：定时器
来源：http://np.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://du.szsharing.cn

[U104] JS：防抖
来源：http://qr.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hk.lnxyls.cn

[U105] JS：节流
来源：http://zv.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vv.haigaiapp.cn

[U106] JS：日期格式化
来源：http://mz.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ti.shtwfgs.cn

[U107] JS：数字千分位
来源：http://wd.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gr.gzmigu.cn

[U108] JS：随机整数
来源：http://yu.gzmigu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sx.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://ec.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://ew.huanxung.cn

[U110] JS：数组分块
来源：http://jq.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rs.lnxyls.cn

[U111] JS：对象转 Map
来源：http://ly.hahajie.cn

new Map(Object.entries(obj))
来源：http://mr.yuexingan06.cn

[U112] JS：字符串补位
来源：http://fw.colortex.cn

"7".padStart(3, "0")
来源：http://ni.gzmigu.cn

[U113] JS：正则替换全部
来源：http://jx.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://ka.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://kl.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pl.wgjwhj.cn

[U115] JS：生成 UUID
来源：http://vo.shxzukj.cn

crypto.randomUUID()
来源：http://yo.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://un.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://lw.chemitech.net.cn

[U117] JS：单元测试
来源：http://ik.colortex.cn

npm i -D vitest;  npx vitest
来源：http://uz.jctech888.com.cn

[U118] JS：开发服务器
来源：http://ti.asd995.cn

npm i -D vite;  npx vite
来源：http://ii.szxytkj.cn

[U119] JS：生产构建
来源：http://bn.lnxyls.cn

npx vite build
来源：http://gi.asd995.cn

[U120] JS：读取环境变量（Vite）
来源：http://iq.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://qe.nszjky.cn

================================================================================
来源：http://pc.nszjky.cn

统计汇总
来源：http://wd.chemitech.net.cn

================================================================================
来源：http://yq.shtwfgs.cn

按语言统计（条）：
来源：http://fk.haigaiapp.cn

Python ......... 252
来源：http://bx.shxzskj.cn

PHP ............ 252
来源：http://mk.nicolike.cn

JavaScript ..... 252
来源：http://py.yuntaijiaju.cn

TypeScript ..... 212
来源：http://we.9csxet.cn

Java ........... 212
来源：http://zc.521024.cn

Go ............. 212
来源：http://ap.chemitech.net.cn

Ruby ........... 212
来源：http://ms.muxihuayi.cn

C# ............. 212
来源：http://yc.szxytkj.cn

C .............. 30
来源：http://wi.bjjhwx.cn

C++ ............ 30
来源：http://ul.hahajie.cn

SQL ............ 90
来源：http://pa.shtwfgs.cn

Bash ........... 80
来源：http://gk.huixinmuqiang.cn

Kotlin ......... 15
来源：http://tb.huixinmuqiang.cn

Swift .......... 15
来源：http://cp.wgjwhj.cn

Lua ............ 10
来源：http://rv.haigaiapp.cn

Perl ........... 10
来源：http://lo.lnxyls.cn

Scala .......... 10
来源：http://yc.521024.cn

------------------------------------
来源：http://vv.szxytkj.cn

合计 ........... 2106 条
来源：http://wj.jctech888.com.cn

按章节统计：
来源：http://dg.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eh.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ln.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ao.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://by.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xo.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ta.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ex.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://if.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lp.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cp.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jb.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oy.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qo.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bq.huixiangedu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://md.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ys.huixiangedu.cn

Q SQL 专题                              90
来源：http://cl.hnjuh.cn

R Bash 专题                             80
来源：http://ah.haigaiapp.cn

S C / C++ 专题                          60
来源：http://yy.shtwfgs.cn

T 其他语言补充                          60
来源：http://hf.bjjhwx.cn

U 高频实用片段                         120
来源：http://cc.gzmigu.cn

------------------------------------
来源：http://rn.huanxung.cn

合计                                  2106 条
来源：http://te.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://zw.jianghongdianzi.cn

使用提醒
来源：http://dq.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://qo.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ty.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oi.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ls.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fs.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vu.hnjuh.cn

—— 文件结束 ——
来源：http://cb.asd995.cn

================================================================================
来源：http://ej.huixiangedu.cn

程序语言常见例子速查手册（2024 版）
来源：http://tj.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://bo.jianghongdianzi.cn

================================================================================
来源：http://yy.bookmarksfly.cn

【收录内容】
来源：http://fu.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bu.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ft.shxzukj.cn

SQL · Bash · C · C++
来源：http://mt.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dg.shtwfgs.cn

【使用说明】
来源：http://ff.asd995.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ko.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ca.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cd.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://af.shtwfgs.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yx.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://or.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oj.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qs.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yd.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qv.hahajie.cn


<!-- 参考信息 -->