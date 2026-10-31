代发 wailian999

[U05] Py：列表去重且保序
来源：http://ol.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://ua.newstarts.cn

[U06] Py：合并两个字典
来源：http://si.jianghongdianzi.cn

{**a, **b}
来源：http://po.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://yv.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://in.newstarts.cn

[U08] Py：展平二维列表
来源：http://qm.jctech888.com.cn

[y for x in nested for y in x]
来源：http://hq.shtwfgs.cn

[U09] Py：字典取最大值的键
来源：http://ch.bookmarksfly.cn

max(d, key=d.get)
来源：http://dk.hahajie.cn

[U10] Py：按值排序字典
来源：http://we.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pp.nszjky.cn

[U11] Py：生成器表达式
来源：http://yw.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://po.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oi.newstarts.cn

Counter(arr).most_common(3)
来源：http://ae.hahajie.cn

[U13] Py：固定长度队列
来源：http://wt.yuntaijiaju.cn

deque(maxlen=10)
来源：http://ye.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://kd.huixiangedu.cn

defaultdict(list)
来源：http://rz.szxytkj.cn

[U15] Py：高精度计时
来源：http://zx.huixinmuqiang.cn

t = time.perf_counter()
来源：http://qu.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://hk.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://to.shtwfgs.cn

[U17] Py：初始化日志
来源：http://bu.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://ih.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://tr.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://jm.huanxung.cn

[U19] Py：正则替换带回调
来源：http://xv.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ts.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://fy.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://ce.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://sk.hnjuh.cn

@contextlib.contextmanager
来源：http://sw.huanxung.cn

[U22] Py：矩阵转置
来源：http://zb.shtwfgs.cn

list(zip(*m))
来源：http://hk.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://cz.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://or.9csxet.cn

[U24] Py：路径操作
来源：http://nf.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dx.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://ar.hnjuh.cn

csv.DictReader(f)
来源：http://kv.bookmarksfly.cn

[U26] Py：并发下载
来源：http://ky.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tn.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://ql.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://pw.szsharing.cn

[U28] Py：类型别名
来源：http://uk.lnxyls.cn

UserId = int
来源：http://ku.nicolike.cn

[U29] Py：属性校验
来源：http://az.shxzukj.cn

@property 与 @x.setter 配合
来源：http://rg.9csxet.cn

[U30] Py：数据类
来源：http://io.nszjky.cn

@dataclass(slots=True)
来源：http://ae.jianghongdianzi.cn

[U31] Py：单测
来源：http://tj.bjjhwx.cn

python -m pytest -q
来源：http://dt.shtwfgs.cn

[U32] Py：代码格式化
来源：http://kr.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://zn.bjjhwx.cn

[U33] Py：打包发布
来源：http://qt.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://sk.panjiajie.cn

[U34] Py：判断编码
来源：http://rb.huixiangedu.cn

chardet.detect(raw)
来源：http://kt.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://ou.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eo.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://mz.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://ne.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://oc.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gd.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://md.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://cx.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://lx.nszjky.cn

sys.stdout.isatty()
来源：http://wk.nicolike.cn

[U40] Py：打印到标准错误
来源：http://ou.9csxet.cn

print("err", file=sys.stderr)
来源：http://qf.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://zg.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://up.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://oy.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ct.szsharing.cn

[U43] PHP：声明命名空间
来源：http://qt.shtwfgs.cn

namespace App\Http;
来源：http://gs.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://zz.jianghongdianzi.cn

declare(strict_types=1);
来源：http://ec.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://fw.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rr.colortex.cn

[U46] PHP：可空类型
来源：http://el.yuntaijiaju.cn

?string $name = null
来源：http://ff.huixiangedu.cn

[U47] PHP：联合类型
来源：http://vg.nicolike.cn

int|string $id
来源：http://az.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://cd.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://do.wgjwhj.cn

[U49] PHP：只读属性
来源：http://nd.hahajie.cn

public readonly string $name
来源：http://go.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://yk.shxzukj.cn

public function __construct(private int $id) {}
来源：http://is.haigaiapp.cn

[U51] PHP：数组解构
来源：http://iq.muxihuayi.cn

[$a, $b] = $arr;
来源：http://rz.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://cx.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://iq.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://ye.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://jx.gzmigu.cn

[U54] PHP：空安全调用
来源：http://iz.jianghongdianzi.cn

$obj?->method()
来源：http://qr.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://hp.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hc.hnjuh.cn

[U56] PHP：命名参数
来源：http://dp.panjiajie.cn

f(a: 1, b: 2)
来源：http://nj.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://ix.shxzskj.cn

"值: {$a}"
来源：http://kc.asd995.cn

[U58] PHP：数组三件套
来源：http://zn.lnxyls.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://as.hahajie.cn

[U59] PHP：自定义排序
来源：http://pv.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pq.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://ti.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rt.shxzskj.cn

[U61] PHP：正则
来源：http://la.panjiajie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cp.shtwfgs.cn

[U62] PHP：日期对象
来源：http://er.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qy.asd995.cn

[U63] PHP：文件读写
来源：http://cu.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rr.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://kc.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://nt.colortex.cn

[U65] PHP：会话
来源：http://tw.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mp.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://jv.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ug.haigaiapp.cn

[U67] PHP：处理文件上传
来源：http://zz.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rj.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://ps.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zw.hahajie.cn

[U69] PHP：PDO 预处理
来源：http://op.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ky.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://lt.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ro.hahajie.cn

[U71] PHP：抛出异常
来源：http://ry.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://tn.shxzskj.cn

[U72] PHP：写错误日志
来源：http://qn.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://gj.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://yo.asd995.cn

parse_ini_file("config.ini", true)
来源：http://kf.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://ns.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://ug.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://eo.colortex.cn

composer require psr/container
来源：http://bn.9csxet.cn

[U76] PHP：简单路由
来源：http://fb.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qo.gzmigu.cn

[U77] PHP：模板渲染
来源：http://ek.huixinmuqiang.cn

composer require twig/twig
来源：http://mn.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://um.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://fo.chemitech.net.cn

[U79] PHP：静态分析
来源：http://bt.gzmigu.cn

composer require --dev phpstan/phpstan
来源：http://st.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://ib.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sn.muxihuayi.cn

[U81] JS：初始化项目
来源：http://ol.huixiangedu.cn

npm init -y;  npm i express
来源：http://ti.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://il.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ym.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://cc.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iz.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://bx.muxihuayi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://km.newstarts.cn

[U85] JS：可选链
来源：http://wt.szxytkj.cn

a?.b?.c
来源：http://ui.wgjwhj.cn

[U86] JS：空值合并
来源：http://my.huixinmuqiang.cn

a ?? b
来源：http://qk.muxihuayi.cn

[U87] JS：解构默认值
来源：http://yn.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://tz.lnxyls.cn

[U88] JS：对象展开合并
来源：http://ls.chemitech.net.cn

{ ...a, ...b }
来源：http://tq.asd995.cn

[U89] JS：数组去重
来源：http://px.lnxyls.cn

[...new Set(arr)]
来源：http://ej.panjiajie.cn

[U90] JS：数字数组排序
来源：http://tg.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://zo.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://xs.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jz.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://lp.lnxyls.cn

structuredClone(obj)
来源：http://td.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://ls.szxytkj.cn

`共 ${n} 条`
来源：http://wg.asd995.cn

[U94] JS：箭头函数
来源：http://ca.hnjuh.cn

const double = x => x * 2;
来源：http://ie.nicolike.cn

[U95] JS：Promise 包装
来源：http://tx.shxzukj.cn

new Promise((resolve, reject) => {})
来源：http://et.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://vu.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pc.jctech888.com.cn

[U97] JS：并发请求
来源：http://rq.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cr.haigaiapp.cn

[U98] JS：fetch 带 JSON
来源：http://bt.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vi.shtwfgs.cn

[U99] JS：事件监听
来源：http://lm.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://wq.521024.cn

[U100] JS：DOM 查询
来源：http://bm.newstarts.cn

document.querySelector(".item")
来源：http://tg.hnjuh.cn

[U101] JS：classList 操作
来源：http://dh.bjjhwx.cn

el.classList.toggle("active")
来源：http://nf.bjjhwx.cn

[U102] JS：本地存储
来源：http://oh.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ub.szsharing.cn

[U103] JS：定时器
来源：http://fh.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hj.szsharing.cn

[U104] JS：防抖
来源：http://ee.shxzskj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yo.huixiangedu.cn

[U105] JS：节流
来源：http://yf.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yf.nszjky.cn

[U106] JS：日期格式化
来源：http://cx.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cw.szsharing.cn

[U107] JS：数字千分位
来源：http://hs.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ps.szsharing.cn

[U108] JS：随机整数
来源：http://qa.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ue.haigaiapp.cn

[U109] JS：数组分组
来源：http://zp.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://vn.shxzskj.cn

[U110] JS：数组分块
来源：http://wp.hnjuh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qu.9csxet.cn

[U111] JS：对象转 Map
来源：http://in.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://qd.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://tr.hnjuh.cn

"7".padStart(3, "0")
来源：http://xv.gzmigu.cn

[U113] JS：正则替换全部
来源：http://vz.shxzukj.cn

s.replaceAll("a", "b")
来源：http://zi.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://bf.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yt.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://my.shxzskj.cn

crypto.randomUUID()
来源：http://hi.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://gk.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://yc.haigaiapp.cn

[U117] JS：单元测试
来源：http://us.huixinmuqiang.cn

npm i -D vitest;  npx vitest
来源：http://vd.nszjky.cn

[U118] JS：开发服务器
来源：http://av.nszjky.cn

npm i -D vite;  npx vite
来源：http://dl.gzmigu.cn

[U119] JS：生产构建
来源：http://nb.huanxung.cn

npx vite build
来源：http://zd.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ov.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://bt.szxytkj.cn

================================================================================
来源：http://pf.shxzukj.cn

统计汇总
来源：http://iv.yuexingan06.cn

================================================================================
来源：http://fo.hnjuh.cn

按语言统计（条）：
来源：http://se.bookmarksfly.cn

Python ......... 252
来源：http://is.szxytkj.cn

PHP ............ 252
来源：http://vj.asd995.cn

JavaScript ..... 252
来源：http://vn.huanxung.cn

TypeScript ..... 212
来源：http://zk.bjjhwx.cn

Java ........... 212
来源：http://lw.muxihuayi.cn

Go ............. 212
来源：http://bk.haigaiapp.cn

Ruby ........... 212
来源：http://vq.9csxet.cn

C# ............. 212
来源：http://sg.lnxyls.cn

C .............. 30
来源：http://fz.panjiajie.cn

C++ ............ 30
来源：http://ri.haigaiapp.cn

SQL ............ 90
来源：http://ok.panjiajie.cn

Bash ........... 80
来源：http://il.asd995.cn

Kotlin ......... 15
来源：http://ai.bjjhwx.cn

Swift .......... 15
来源：http://it.huanxung.cn

Lua ............ 10
来源：http://re.huixinmuqiang.cn

Perl ........... 10
来源：http://mx.bookmarksfly.cn

Scala .......... 10
来源：http://np.newstarts.cn

------------------------------------
来源：http://ju.huixiangedu.cn

合计 ........... 2106 条
来源：http://nk.szxytkj.cn

按章节统计：
来源：http://hp.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://es.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zc.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mm.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rm.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mm.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wn.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pt.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gz.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://at.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dd.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gk.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zl.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bv.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://px.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://in.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yz.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://dp.hahajie.cn

R Bash 专题                             80
来源：http://ro.muxihuayi.cn

S C / C++ 专题                          60
来源：http://ht.shxzskj.cn

T 其他语言补充                          60
来源：http://zh.shxzskj.cn

U 高频实用片段                         120
来源：http://kk.shxzskj.cn

------------------------------------
来源：http://pu.huanxung.cn

合计                                  2106 条
来源：http://zu.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://dt.jianghongdianzi.cn

使用提醒
来源：http://bk.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://qs.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://be.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xy.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ux.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yt.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ll.newstarts.cn

—— 文件结束 ——
来源：http://di.szsharing.cn

================================================================================
来源：http://qe.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://xz.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://bm.shtwfgs.cn

================================================================================
来源：http://pp.newstarts.cn

【收录内容】
来源：http://zn.panjiajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lm.9csxet.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nr.gzmigu.cn

SQL · Bash · C · C++
来源：http://yq.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dl.hnjuh.cn

【使用说明】
来源：http://wv.shtwfgs.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nc.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cn.gzmigu.cn


<!-- 参考信息 -->